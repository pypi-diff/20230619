# Comparing `tmp/alibabacloud_cc5g20220314-2.0.8.tar.gz` & `tmp/alibabacloud_cc5g20220314-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cc5g20220314-2.0.8.tar", last modified: Tue Feb 21 06:43:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cc5g20220314-2.0.9.tar", last modified: Tue Apr  4 10:29:16 2023, max compression
```

## Comparing `alibabacloud_cc5g20220314-2.0.8.tar` & `alibabacloud_cc5g20220314-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      315 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/__init__.py
--rw-r--r--   0 root         (0) root         (0)   193651 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/client.py
--rw-r--r--   0 root         (0) root         (0)   312237 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-21 06:43:32.000000 alibabacloud_cc5g20220314-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-02-21 06:43:31.000000 alibabacloud_cc5g20220314-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   196713 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/client.py
+-rw-r--r--   0 root         (0) root         (0)   315526 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-04 10:29:16.000000 alibabacloud_cc5g20220314-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-04 10:29:15.000000 alibabacloud_cc5g20220314-2.0.9/setup.py
```

### Comparing `alibabacloud_cc5g20220314-2.0.8/LICENSE` & `alibabacloud_cc5g20220314-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314-2.0.8/PKG-INFO` & `alibabacloud_cc5g20220314-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cc5g20220314
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud CC5G (20220314) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cc5g20220314-2.0.8/README-CN.md` & `alibabacloud_cc5g20220314-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314-2.0.8/README.md` & `alibabacloud_cc5g20220314-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/client.py` & `alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3267,14 +3267,96 @@
     async def open_cc_5g_service_async(
         self,
         request: cc5g20220314_models.OpenCc5gServiceRequest,
     ) -> cc5g20220314_models.OpenCc5gServiceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.open_cc_5g_service_with_options_async(request, runtime)
 
+    def rebind_cards_with_options(
+        self,
+        request: cc5g20220314_models.RebindCardsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cc5g20220314_models.RebindCardsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.iccids):
+            query['Iccids'] = request.iccids
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RebindCards',
+            version='2022-03-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cc5g20220314_models.RebindCardsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def rebind_cards_with_options_async(
+        self,
+        request: cc5g20220314_models.RebindCardsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cc5g20220314_models.RebindCardsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.iccids):
+            query['Iccids'] = request.iccids
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RebindCards',
+            version='2022-03-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cc5g20220314_models.RebindCardsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def rebind_cards(
+        self,
+        request: cc5g20220314_models.RebindCardsRequest,
+    ) -> cc5g20220314_models.RebindCardsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.rebind_cards_with_options(request, runtime)
+
+    async def rebind_cards_async(
+        self,
+        request: cc5g20220314_models.RebindCardsRequest,
+    ) -> cc5g20220314_models.RebindCardsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.rebind_cards_with_options_async(request, runtime)
+
     def remove_wireless_cloud_connector_from_group_with_options(
         self,
         request: cc5g20220314_models.RemoveWirelessCloudConnectorFromGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cc5g20220314_models.RemoveWirelessCloudConnectorFromGroupResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314/models.py` & `alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15580,3936 +15580,4142 @@
 0003cdb0: 3d20 4f70 656e 4363 3567 5365 7276 6963  = OpenCc5gServic
 0003cdc0: 6552 6573 706f 6e73 6542 6f64 7928 290a  eResponseBody().
 0003cdd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 0003cde0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
 0003cdf0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
 0003ce00: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
 0003ce10: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0003ce20: 7373 2052 656d 6f76 6557 6972 656c 6573  ss RemoveWireles
-0003ce30: 7343 6c6f 7564 436f 6e6e 6563 746f 7246  sCloudConnectorF
-0003ce40: 726f 6d47 726f 7570 5265 7175 6573 7428  romGroupRequest(
-0003ce50: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0003ce60: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0003ce70: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0003ce80: 2020 2063 6c69 656e 745f 746f 6b65 6e3a     client_token:
-0003ce90: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0003cea0: 2020 2020 2064 7279 5f72 756e 3a20 626f       dry_run: bo
-0003ceb0: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
-0003cec0: 2020 2072 6567 696f 6e5f 6964 3a20 7374     region_id: st
-0003ced0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0003cee0: 2020 7769 7265 6c65 7373 5f63 6c6f 7564    wireless_cloud
-0003cef0: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
-0003cf00: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-0003cf10: 0a20 2020 2020 2020 2077 6972 656c 6573  .        wireles
-0003cf20: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-0003cf30: 725f 6964 733a 204c 6973 745b 7374 725d  r_ids: List[str]
-0003cf40: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0003cf50: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-0003cf60: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
-0003cf70: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
-0003cf80: 2073 656c 662e 6472 795f 7275 6e20 3d20   self.dry_run = 
-0003cf90: 6472 795f 7275 6e0a 2020 2020 2020 2020  dry_run.        
-0003cfa0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-0003cfb0: 2072 6567 696f 6e5f 6964 0a20 2020 2020   region_id.     
-0003cfc0: 2020 2073 656c 662e 7769 7265 6c65 7373     self.wireless
-0003cfd0: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-0003cfe0: 5f67 726f 7570 5f69 6420 3d20 7769 7265  _group_id = wire
-0003cff0: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-0003d000: 6374 6f72 5f67 726f 7570 5f69 640a 2020  ctor_group_id.  
-0003d010: 2020 2020 2020 7365 6c66 2e77 6972 656c        self.wirel
-0003d020: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-0003d030: 746f 725f 6964 7320 3d20 7769 7265 6c65  tor_ids = wirele
-0003d040: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-0003d050: 6f72 5f69 6473 0a0a 2020 2020 6465 6620  or_ids..    def 
-0003d060: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003d070: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0003d080: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0003d090: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0003d0a0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0003d0b0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0003d0c0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0003d0d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0003d0e0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0003d0f0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0003d100: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0003d110: 662e 636c 6965 6e74 5f74 6f6b 656e 2069  f.client_token i
-0003d120: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003d130: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003d140: 436c 6965 6e74 546f 6b65 6e27 5d20 3d20  ClientToken'] = 
-0003d150: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-0003d160: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0003d170: 662e 6472 795f 7275 6e20 6973 206e 6f74  f.dry_run is not
-0003d180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003d190: 2020 2072 6573 756c 745b 2744 7279 5275     result['DryRu
-0003d1a0: 6e27 5d20 3d20 7365 6c66 2e64 7279 5f72  n'] = self.dry_r
-0003d1b0: 756e 0a20 2020 2020 2020 2069 6620 7365  un.        if se
-0003d1c0: 6c66 2e72 6567 696f 6e5f 6964 2069 7320  lf.region_id is 
-0003d1d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003d1e0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-0003d1f0: 6769 6f6e 4964 275d 203d 2073 656c 662e  gionId'] = self.
-0003d200: 7265 6769 6f6e 5f69 640a 2020 2020 2020  region_id.      
-0003d210: 2020 6966 2073 656c 662e 7769 7265 6c65    if self.wirele
-0003d220: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-0003d230: 6f72 5f67 726f 7570 5f69 6420 6973 206e  or_group_id is n
-0003d240: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003d250: 2020 2020 2072 6573 756c 745b 2757 6972       result['Wir
-0003d260: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
-0003d270: 746f 7247 726f 7570 4964 275d 203d 2073  torGroupId'] = s
-0003d280: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
-0003d290: 7564 5f63 6f6e 6e65 6374 6f72 5f67 726f  ud_connector_gro
-0003d2a0: 7570 5f69 640a 2020 2020 2020 2020 6966  up_id.        if
-0003d2b0: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
-0003d2c0: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
-0003d2d0: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
-0003d2e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003d2f0: 6c74 5b27 5769 7265 6c65 7373 436c 6f75  lt['WirelessClou
-0003d300: 6443 6f6e 6e65 6374 6f72 4964 7327 5d20  dConnectorIds'] 
-0003d310: 3d20 7365 6c66 2e77 6972 656c 6573 735f  = self.wireless_
-0003d320: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-0003d330: 6964 730a 2020 2020 2020 2020 7265 7475  ids.        retu
-0003d340: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0003d350: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0003d360: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0003d370: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0003d380: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0003d390: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
-0003d3a0: 656e 7454 6f6b 656e 2729 2069 7320 6e6f  entToken') is no
-0003d3b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003d3c0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-0003d3d0: 746f 6b65 6e20 3d20 6d2e 6765 7428 2743  token = m.get('C
-0003d3e0: 6c69 656e 7454 6f6b 656e 2729 0a20 2020  lientToken').   
-0003d3f0: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
-0003d400: 7279 5275 6e27 2920 6973 206e 6f74 204e  ryRun') is not N
-0003d410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003d420: 2073 656c 662e 6472 795f 7275 6e20 3d20   self.dry_run = 
-0003d430: 6d2e 6765 7428 2744 7279 5275 6e27 290a  m.get('DryRun').
-0003d440: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003d450: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
-0003d460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003d470: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-0003d480: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
-0003d490: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
-0003d4a0: 2069 6620 6d2e 6765 7428 2757 6972 656c   if m.get('Wirel
-0003d4b0: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-0003d4c0: 7247 726f 7570 4964 2729 2069 7320 6e6f  rGroupId') is no
-0003d4d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003d4e0: 2020 2020 7365 6c66 2e77 6972 656c 6573      self.wireles
-0003d4f0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-0003d500: 725f 6772 6f75 705f 6964 203d 206d 2e67  r_group_id = m.g
-0003d510: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
-0003d520: 6443 6f6e 6e65 6374 6f72 4772 6f75 7049  dConnectorGroupI
-0003d530: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0003d540: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-0003d550: 6f75 6443 6f6e 6e65 6374 6f72 4964 7327  oudConnectorIds'
-0003d560: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003d570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003d580: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
-0003d590: 6f6e 6e65 6374 6f72 5f69 6473 203d 206d  onnector_ids = m
-0003d5a0: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-0003d5b0: 6f75 6443 6f6e 6e65 6374 6f72 4964 7327  oudConnectorIds'
-0003d5c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0003d5d0: 2073 656c 660a 0a0a 636c 6173 7320 5265   self...class Re
-0003d5e0: 6d6f 7665 5769 7265 6c65 7373 436c 6f75  moveWirelessClou
-0003d5f0: 6443 6f6e 6e65 6374 6f72 4672 6f6d 4772  dConnectorFromGr
-0003d600: 6f75 7052 6573 706f 6e73 6542 6f64 7928  oupResponseBody(
-0003d610: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0003d620: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0003d630: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0003d640: 2020 2072 6571 7565 7374 5f69 643a 2073     request_id: s
-0003d650: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-0003d660: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
-0003d670: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-0003d680: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
-0003d690: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0003d6a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0003d6b0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0003d6c0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0003d6d0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0003d6e0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0003d6f0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0003d700: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0003d710: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0003d720: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0003d730: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0003d740: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-0003d750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003d760: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-0003d770: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-0003d780: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-0003d790: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0003d7a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0003d7b0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0003d7c0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0003d7d0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0003d7e0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0003d7f0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-0003d800: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003d810: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0003d820: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-0003d830: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-0003d840: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0003d850: 6c66 0a0a 0a63 6c61 7373 2052 656d 6f76  lf...class Remov
-0003d860: 6557 6972 656c 6573 7343 6c6f 7564 436f  eWirelessCloudCo
-0003d870: 6e6e 6563 746f 7246 726f 6d47 726f 7570  nnectorFromGroup
-0003d880: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-0003d890: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0003d8a0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0003d8b0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-0003d8c0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-0003d8d0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0003d8e0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-0003d8f0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0003d900: 2020 2020 2062 6f64 793a 2052 656d 6f76       body: Remov
-0003d910: 6557 6972 656c 6573 7343 6c6f 7564 436f  eWirelessCloudCo
-0003d920: 6e6e 6563 746f 7246 726f 6d47 726f 7570  nnectorFromGroup
-0003d930: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
-0003d940: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-0003d950: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-0003d960: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-0003d970: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0003d980: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-0003d990: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-0003d9a0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-0003d9b0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0003d9c0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0003d9d0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0003d9e0: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-0003d9f0: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-0003da00: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0003da10: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0003da20: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-0003da30: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-0003da40: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0003da50: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0003da60: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-0003da70: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0003da80: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-0003da90: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-0003daa0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0003dab0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0003dac0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0003dad0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0003dae0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0003daf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003db00: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0003db10: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0003db20: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0003db30: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-0003db40: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0003db50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003db60: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-0003db70: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-0003db80: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-0003db90: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-0003dba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003dbb0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-0003dbc0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-0003dbd0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-0003dbe0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-0003dbf0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003dc00: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-0003dc10: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-0003dc20: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-0003dc30: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0003dc40: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0003dc50: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-0003dc60: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-0003dc70: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0003dc80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0003dc90: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-0003dca0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003dcb0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0003dcc0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-0003dcd0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-0003dce0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-0003dcf0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-0003dd00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0003dd10: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0003dd20: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-0003dd30: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-0003dd40: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-0003dd50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003dd60: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-0003dd70: 656c 203d 2052 656d 6f76 6557 6972 656c  el = RemoveWirel
-0003dd80: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-0003dd90: 7246 726f 6d47 726f 7570 5265 7370 6f6e  rFromGroupRespon
-0003dda0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-0003ddb0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0003ddc0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-0003ddd0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-0003dde0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0003ddf0: 656c 660a 0a0a 636c 6173 7320 5265 7375  elf...class Resu
-0003de00: 6d65 4361 7264 7352 6571 7565 7374 2854  meCardsRequest(T
-0003de10: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0003de20: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0003de30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0003de40: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
-0003de50: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0003de60: 2020 2020 6472 795f 7275 6e3a 2062 6f6f      dry_run: boo
-0003de70: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
-0003de80: 2020 6963 6369 6473 3a20 4c69 7374 5b73    iccids: List[s
-0003de90: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0003dea0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
-0003deb0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-0003dec0: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-0003ded0: 6c69 656e 745f 746f 6b65 6e20 3d20 636c  lient_token = cl
-0003dee0: 6965 6e74 5f74 6f6b 656e 0a20 2020 2020  ient_token.     
-0003def0: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
-0003df00: 3d20 6472 795f 7275 6e0a 2020 2020 2020  = dry_run.      
-0003df10: 2020 7365 6c66 2e69 6363 6964 7320 3d20    self.iccids = 
-0003df20: 6963 6369 6473 0a20 2020 2020 2020 2073  iccids.        s
-0003df30: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-0003df40: 7265 6769 6f6e 5f69 640a 0a20 2020 2064  region_id..    d
-0003df50: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0003df60: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0003df70: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0003df80: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0003df90: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0003dfa0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0003dfb0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0003dfc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003dfd0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0003dfe0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0003dff0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0003e000: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-0003e010: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-0003e020: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0003e030: 745b 2743 6c69 656e 7454 6f6b 656e 275d  t['ClientToken']
-0003e040: 203d 2073 656c 662e 636c 6965 6e74 5f74   = self.client_t
-0003e050: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
-0003e060: 7365 6c66 2e64 7279 5f72 756e 2069 7320  self.dry_run is 
-0003e070: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003e080: 2020 2020 2020 7265 7375 6c74 5b27 4472        result['Dr
-0003e090: 7952 756e 275d 203d 2073 656c 662e 6472  yRun'] = self.dr
-0003e0a0: 795f 7275 6e0a 2020 2020 2020 2020 6966  y_run.        if
-0003e0b0: 2073 656c 662e 6963 6369 6473 2069 7320   self.iccids is 
-0003e0c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003e0d0: 2020 2020 2020 7265 7375 6c74 5b27 4963        result['Ic
-0003e0e0: 6369 6473 275d 203d 2073 656c 662e 6963  cids'] = self.ic
-0003e0f0: 6369 6473 0a20 2020 2020 2020 2069 6620  cids.        if 
-0003e100: 7365 6c66 2e72 6567 696f 6e5f 6964 2069  self.region_id i
-0003e110: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003e120: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003e130: 5265 6769 6f6e 4964 275d 203d 2073 656c  RegionId'] = sel
-0003e140: 662e 7265 6769 6f6e 5f69 640a 2020 2020  f.region_id.    
-0003e150: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0003e160: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0003e170: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0003e180: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0003e190: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0003e1a0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0003e1b0: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
-0003e1c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0003e1d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003e1e0: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
-0003e1f0: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
-0003e200: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
-0003e210: 6d2e 6765 7428 2744 7279 5275 6e27 2920  m.get('DryRun') 
-0003e220: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003e230: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
-0003e240: 795f 7275 6e20 3d20 6d2e 6765 7428 2744  y_run = m.get('D
-0003e250: 7279 5275 6e27 290a 2020 2020 2020 2020  ryRun').        
-0003e260: 6966 206d 2e67 6574 2827 4963 6369 6473  if m.get('Iccids
-0003e270: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0003e280: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0003e290: 2e69 6363 6964 7320 3d20 6d2e 6765 7428  .iccids = m.get(
-0003e2a0: 2749 6363 6964 7327 290a 2020 2020 2020  'Iccids').      
-0003e2b0: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
-0003e2c0: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
-0003e2d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003e2e0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-0003e2f0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-0003e300: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0003e310: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2052  n self...class R
-0003e320: 6573 756d 6543 6172 6473 5265 7370 6f6e  esumeCardsRespon
-0003e330: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-0003e340: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0003e350: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0003e360: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-0003e370: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-0003e380: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0003e390: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0003e3a0: 203d 2072 6571 7565 7374 5f69 640a 0a20   = request_id.. 
-0003e3b0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0003e3c0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0003e3d0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-0003e3e0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0003e3f0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0003e400: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0003e410: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0003e420: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003e430: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0003e440: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0003e450: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0003e460: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-0003e470: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0003e480: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003e490: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-0003e4a0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-0003e4b0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0003e4c0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0003e4d0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0003e4e0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0003e4f0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0003e500: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0003e510: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-0003e520: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-0003e530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003e540: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0003e550: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-0003e560: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
-0003e570: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-0003e580: 7320 5265 7375 6d65 4361 7264 7352 6573  s ResumeCardsRes
-0003e590: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-0003e5a0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0003e5b0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0003e5c0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-0003e5d0: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-0003e5e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0003e5f0: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-0003e600: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0003e610: 2020 626f 6479 3a20 5265 7375 6d65 4361    body: ResumeCa
-0003e620: 7264 7352 6573 706f 6e73 6542 6f64 7920  rdsResponseBody 
-0003e630: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0003e640: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0003e650: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0003e660: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0003e670: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0003e680: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0003e690: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0003e6a0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0003e6b0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0003e6c0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0003e6d0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-0003e6e0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-0003e6f0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0003e700: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0003e710: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-0003e720: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-0003e730: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0003e740: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0003e750: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-0003e760: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0003e770: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0003e780: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0003e790: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0003e7a0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0003e7b0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0003e7c0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0003e7d0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0003e7e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003e7f0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0003e800: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0003e810: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0003e820: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-0003e830: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-0003e840: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003e850: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-0003e860: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-0003e870: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0003e880: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-0003e890: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003e8a0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-0003e8b0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-0003e8c0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-0003e8d0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0003e8e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003e8f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0003e900: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0003e910: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0003e920: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0003e930: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0003e940: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0003e950: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0003e960: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0003e970: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0003e980: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0003e990: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003e9a0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0003e9b0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-0003e9c0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0003e9d0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-0003e9e0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-0003e9f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003ea00: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0003ea10: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-0003ea20: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-0003ea30: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0003ea40: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003ea50: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0003ea60: 6d6f 6465 6c20 3d20 5265 7375 6d65 4361  model = ResumeCa
-0003ea70: 7264 7352 6573 706f 6e73 6542 6f64 7928  rdsResponseBody(
+0003ce20: 7373 2052 6562 696e 6443 6172 6473 5265  ss RebindCardsRe
+0003ce30: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+0003ce40: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0003ce50: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0003ce60: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
+0003ce70: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
+0003ce80: 652c 0a20 2020 2020 2020 2064 7279 5f72  e,.        dry_r
+0003ce90: 756e 3a20 626f 6f6c 203d 204e 6f6e 652c  un: bool = None,
+0003cea0: 0a20 2020 2020 2020 2069 6363 6964 733a  .        iccids:
+0003ceb0: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
+0003cec0: 652c 0a20 2020 2020 2020 2072 6567 696f  e,.        regio
+0003ced0: 6e5f 6964 3a20 7374 7220 3d20 4e6f 6e65  n_id: str = None
+0003cee0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0003cef0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+0003cf00: 656e 203d 2063 6c69 656e 745f 746f 6b65  en = client_toke
+0003cf10: 6e0a 2020 2020 2020 2020 7365 6c66 2e64  n.        self.d
+0003cf20: 7279 5f72 756e 203d 2064 7279 5f72 756e  ry_run = dry_run
+0003cf30: 0a20 2020 2020 2020 2073 656c 662e 6963  .        self.ic
+0003cf40: 6369 6473 203d 2069 6363 6964 730a 2020  cids = iccids.  
+0003cf50: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+0003cf60: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
+0003cf70: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0003cf80: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0003cf90: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+0003cfa0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0003cfb0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0003cfc0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+0003cfd0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0003cfe0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003cff0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0003d000: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0003d010: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0003d020: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
+0003d030: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
+0003d040: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003d050: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
+0003d060: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
+0003d070: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
+0003d080: 2020 2020 6966 2073 656c 662e 6472 795f      if self.dry_
+0003d090: 7275 6e20 6973 206e 6f74 204e 6f6e 653a  run is not None:
+0003d0a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0003d0b0: 756c 745b 2744 7279 5275 6e27 5d20 3d20  ult['DryRun'] = 
+0003d0c0: 7365 6c66 2e64 7279 5f72 756e 0a20 2020  self.dry_run.   
+0003d0d0: 2020 2020 2069 6620 7365 6c66 2e69 6363       if self.icc
+0003d0e0: 6964 7320 6973 206e 6f74 204e 6f6e 653a  ids is not None:
+0003d0f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0003d100: 756c 745b 2749 6363 6964 7327 5d20 3d20  ult['Iccids'] = 
+0003d110: 7365 6c66 2e69 6363 6964 730a 2020 2020  self.iccids.    
+0003d120: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+0003d130: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+0003d140: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003d150: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+0003d160: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+0003d170: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0003d180: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0003d190: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0003d1a0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0003d1b0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0003d1c0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0003d1d0: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+0003d1e0: 6e74 546f 6b65 6e27 2920 6973 206e 6f74  ntToken') is not
+0003d1f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003d200: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+0003d210: 6f6b 656e 203d 206d 2e67 6574 2827 436c  oken = m.get('Cl
+0003d220: 6965 6e74 546f 6b65 6e27 290a 2020 2020  ientToken').    
+0003d230: 2020 2020 6966 206d 2e67 6574 2827 4472      if m.get('Dr
+0003d240: 7952 756e 2729 2069 7320 6e6f 7420 4e6f  yRun') is not No
+0003d250: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003d260: 7365 6c66 2e64 7279 5f72 756e 203d 206d  self.dry_run = m
+0003d270: 2e67 6574 2827 4472 7952 756e 2729 0a20  .get('DryRun'). 
+0003d280: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003d290: 2749 6363 6964 7327 2920 6973 206e 6f74  'Iccids') is not
+0003d2a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003d2b0: 2020 2073 656c 662e 6963 6369 6473 203d     self.iccids =
+0003d2c0: 206d 2e67 6574 2827 4963 6369 6473 2729   m.get('Iccids')
+0003d2d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003d2e0: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
+0003d2f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003d300: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+0003d310: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
+0003d320: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
+0003d330: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0003d340: 636c 6173 7320 5265 6269 6e64 4361 7264  class RebindCard
+0003d350: 7352 6573 706f 6e73 6542 6f64 7928 5465  sResponseBody(Te
+0003d360: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0003d370: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0003d380: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0003d390: 2072 6571 7565 7374 5f69 643a 2073 7472   request_id: str
+0003d3a0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0003d3b0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+0003d3c0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
+0003d3d0: 745f 6964 0a0a 2020 2020 6465 6620 7661  t_id..    def va
+0003d3e0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003d3f0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0003d400: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0003d410: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0003d420: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0003d430: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0003d440: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0003d450: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0003d460: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0003d470: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0003d480: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0003d490: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+0003d4a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003d4b0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+0003d4c0: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+0003d4d0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+0003d4e0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0003d4f0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0003d500: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0003d510: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0003d520: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0003d530: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003d540: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+0003d550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003d560: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+0003d570: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+0003d580: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+0003d590: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0003d5a0: 0a0a 0a63 6c61 7373 2052 6562 696e 6443  ...class RebindC
+0003d5b0: 6172 6473 5265 7370 6f6e 7365 2854 6561  ardsResponse(Tea
+0003d5c0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0003d5d0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0003d5e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0003d5f0: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+0003d600: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+0003d610: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+0003d620: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+0003d630: 0a20 2020 2020 2020 2062 6f64 793a 2052  .        body: R
+0003d640: 6562 696e 6443 6172 6473 5265 7370 6f6e  ebindCardsRespon
+0003d650: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
+0003d660: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0003d670: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+0003d680: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+0003d690: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+0003d6a0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0003d6b0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+0003d6c0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+0003d6d0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0003d6e0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0003d6f0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0003d700: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
+0003d710: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
+0003d720: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+0003d730: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
+0003d740: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
+0003d750: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
+0003d760: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+0003d770: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
+0003d780: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
+0003d790: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+0003d7a0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0003d7b0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+0003d7c0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0003d7d0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0003d7e0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+0003d7f0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0003d800: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0003d810: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003d820: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0003d830: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0003d840: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0003d850: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+0003d860: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003d870: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+0003d880: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+0003d890: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+0003d8a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0003d8b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0003d8c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0003d8d0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+0003d8e0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+0003d8f0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+0003d900: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+0003d910: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003d920: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+0003d930: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+0003d940: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+0003d950: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0003d960: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0003d970: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0003d980: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0003d990: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0003d9a0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+0003d9b0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+0003d9c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003d9d0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+0003d9e0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0003d9f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003da00: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+0003da10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003da20: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+0003da30: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+0003da40: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+0003da50: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003da60: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+0003da70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003da80: 2020 7465 6d70 5f6d 6f64 656c 203d 2052    temp_model = R
+0003da90: 6562 696e 6443 6172 6473 5265 7370 6f6e  ebindCardsRespon
+0003daa0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0003dab0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0003dac0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0003dad0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0003dae0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0003daf0: 656c 660a 0a0a 636c 6173 7320 5265 6d6f  elf...class Remo
+0003db00: 7665 5769 7265 6c65 7373 436c 6f75 6443  veWirelessCloudC
+0003db10: 6f6e 6e65 6374 6f72 4672 6f6d 4772 6f75  onnectorFromGrou
+0003db20: 7052 6571 7565 7374 2854 6561 4d6f 6465  pRequest(TeaMode
+0003db30: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+0003db40: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0003db50: 6c66 2c0a 2020 2020 2020 2020 636c 6965  lf,.        clie
+0003db60: 6e74 5f74 6f6b 656e 3a20 7374 7220 3d20  nt_token: str = 
+0003db70: 4e6f 6e65 2c0a 2020 2020 2020 2020 6472  None,.        dr
+0003db80: 795f 7275 6e3a 2062 6f6f 6c20 3d20 4e6f  y_run: bool = No
+0003db90: 6e65 2c0a 2020 2020 2020 2020 7265 6769  ne,.        regi
+0003dba0: 6f6e 5f69 643a 2073 7472 203d 204e 6f6e  on_id: str = Non
+0003dbb0: 652c 0a20 2020 2020 2020 2077 6972 656c  e,.        wirel
+0003dbc0: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
+0003dbd0: 746f 725f 6772 6f75 705f 6964 3a20 7374  tor_group_id: st
+0003dbe0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0003dbf0: 2020 7769 7265 6c65 7373 5f63 6c6f 7564    wireless_cloud
+0003dc00: 5f63 6f6e 6e65 6374 6f72 5f69 6473 3a20  _connector_ids: 
+0003dc10: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+0003dc20: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0003dc30: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+0003dc40: 656e 203d 2063 6c69 656e 745f 746f 6b65  en = client_toke
+0003dc50: 6e0a 2020 2020 2020 2020 7365 6c66 2e64  n.        self.d
+0003dc60: 7279 5f72 756e 203d 2064 7279 5f72 756e  ry_run = dry_run
+0003dc70: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0003dc80: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+0003dc90: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0003dca0: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+0003dcb0: 636f 6e6e 6563 746f 725f 6772 6f75 705f  connector_group_
+0003dcc0: 6964 203d 2077 6972 656c 6573 735f 636c  id = wireless_cl
+0003dcd0: 6f75 645f 636f 6e6e 6563 746f 725f 6772  oud_connector_gr
+0003dce0: 6f75 705f 6964 0a20 2020 2020 2020 2073  oup_id.        s
+0003dcf0: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
+0003dd00: 7564 5f63 6f6e 6e65 6374 6f72 5f69 6473  ud_connector_ids
+0003dd10: 203d 2077 6972 656c 6573 735f 636c 6f75   = wireless_clou
+0003dd20: 645f 636f 6e6e 6563 746f 725f 6964 730a  d_connector_ids.
+0003dd30: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0003dd40: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0003dd50: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0003dd60: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0003dd70: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0003dd80: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0003dd90: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0003dda0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003ddb0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0003ddc0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0003ddd0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0003dde0: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
+0003ddf0: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
+0003de00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003de10: 2072 6573 756c 745b 2743 6c69 656e 7454   result['ClientT
+0003de20: 6f6b 656e 275d 203d 2073 656c 662e 636c  oken'] = self.cl
+0003de30: 6965 6e74 5f74 6f6b 656e 0a20 2020 2020  ient_token.     
+0003de40: 2020 2069 6620 7365 6c66 2e64 7279 5f72     if self.dry_r
+0003de50: 756e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  un is not None:.
+0003de60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0003de70: 6c74 5b27 4472 7952 756e 275d 203d 2073  lt['DryRun'] = s
+0003de80: 656c 662e 6472 795f 7275 6e0a 2020 2020  elf.dry_run.    
+0003de90: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+0003dea0: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+0003deb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003dec0: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+0003ded0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+0003dee0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0003def0: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
+0003df00: 645f 636f 6e6e 6563 746f 725f 6772 6f75  d_connector_grou
+0003df10: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
+0003df20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003df30: 7375 6c74 5b27 5769 7265 6c65 7373 436c  sult['WirelessCl
+0003df40: 6f75 6443 6f6e 6e65 6374 6f72 4772 6f75  oudConnectorGrou
+0003df50: 7049 6427 5d20 3d20 7365 6c66 2e77 6972  pId'] = self.wir
+0003df60: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
+0003df70: 6563 746f 725f 6772 6f75 705f 6964 0a20  ector_group_id. 
+0003df80: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
+0003df90: 6972 656c 6573 735f 636c 6f75 645f 636f  ireless_cloud_co
+0003dfa0: 6e6e 6563 746f 725f 6964 7320 6973 206e  nnector_ids is n
+0003dfb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003dfc0: 2020 2020 2072 6573 756c 745b 2757 6972       result['Wir
+0003dfd0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+0003dfe0: 746f 7249 6473 275d 203d 2073 656c 662e  torIds'] = self.
+0003dff0: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+0003e000: 6f6e 6e65 6374 6f72 5f69 6473 0a20 2020  onnector_ids.   
+0003e010: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0003e020: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+0003e030: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+0003e040: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+0003e050: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0003e060: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0003e070: 2e67 6574 2827 436c 6965 6e74 546f 6b65  .get('ClientToke
+0003e080: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+0003e090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003e0a0: 662e 636c 6965 6e74 5f74 6f6b 656e 203d  f.client_token =
+0003e0b0: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
+0003e0c0: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+0003e0d0: 206d 2e67 6574 2827 4472 7952 756e 2729   m.get('DryRun')
+0003e0e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e0f0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0003e100: 7279 5f72 756e 203d 206d 2e67 6574 2827  ry_run = m.get('
+0003e110: 4472 7952 756e 2729 0a20 2020 2020 2020  DryRun').       
+0003e120: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
+0003e130: 6e49 6427 2920 6973 206e 6f74 204e 6f6e  nId') is not Non
+0003e140: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0003e150: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+0003e160: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
+0003e170: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003e180: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
+0003e190: 6443 6f6e 6e65 6374 6f72 4772 6f75 7049  dConnectorGroupI
+0003e1a0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0003e1b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003e1c0: 662e 7769 7265 6c65 7373 5f63 6c6f 7564  f.wireless_cloud
+0003e1d0: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
+0003e1e0: 5f69 6420 3d20 6d2e 6765 7428 2757 6972  _id = m.get('Wir
+0003e1f0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+0003e200: 746f 7247 726f 7570 4964 2729 0a20 2020  torGroupId').   
+0003e210: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+0003e220: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+0003e230: 6563 746f 7249 6473 2729 2069 7320 6e6f  ectorIds') is no
+0003e240: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003e250: 2020 2020 7365 6c66 2e77 6972 656c 6573      self.wireles
+0003e260: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
+0003e270: 725f 6964 7320 3d20 6d2e 6765 7428 2757  r_ids = m.get('W
+0003e280: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+0003e290: 6563 746f 7249 6473 2729 0a20 2020 2020  ectorIds').     
+0003e2a0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0003e2b0: 0a63 6c61 7373 2052 656d 6f76 6557 6972  .class RemoveWir
+0003e2c0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+0003e2d0: 746f 7246 726f 6d47 726f 7570 5265 7370  torFromGroupResp
+0003e2e0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+0003e2f0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+0003e300: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+0003e310: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
+0003e320: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
+0003e330: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003e340: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+0003e350: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+0003e360: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0003e370: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0003e380: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0003e390: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0003e3a0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0003e3b0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0003e3c0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0003e3d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003e3e0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0003e3f0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0003e400: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0003e410: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+0003e420: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+0003e430: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003e440: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+0003e450: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+0003e460: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
+0003e470: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0003e480: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0003e490: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0003e4a0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0003e4b0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0003e4c0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0003e4d0: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+0003e4e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003e4f0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+0003e500: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+0003e510: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+0003e520: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0003e530: 6173 7320 5265 6d6f 7665 5769 7265 6c65  ass RemoveWirele
+0003e540: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+0003e550: 4672 6f6d 4772 6f75 7052 6573 706f 6e73  FromGroupRespons
+0003e560: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+0003e570: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0003e580: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0003e590: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+0003e5a0: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+0003e5b0: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+0003e5c0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+0003e5d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+0003e5e0: 6479 3a20 5265 6d6f 7665 5769 7265 6c65  dy: RemoveWirele
+0003e5f0: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+0003e600: 4672 6f6d 4772 6f75 7052 6573 706f 6e73  FromGroupRespons
+0003e610: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+0003e620: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0003e630: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+0003e640: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+0003e650: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+0003e660: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+0003e670: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0003e680: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+0003e690: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0003e6a0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0003e6b0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0003e6c0: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+0003e6d0: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+0003e6e0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0003e6f0: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+0003e700: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+0003e710: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+0003e720: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0003e730: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+0003e740: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+0003e750: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+0003e760: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+0003e770: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+0003e780: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0003e790: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0003e7a0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+0003e7b0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0003e7c0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0003e7d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003e7e0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0003e7f0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0003e800: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0003e810: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+0003e820: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003e830: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+0003e840: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+0003e850: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+0003e860: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0003e870: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003e880: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003e890: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+0003e8a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0003e8b0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0003e8c0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+0003e8d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003e8e0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+0003e8f0: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+0003e900: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+0003e910: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0003e920: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0003e930: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0003e940: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0003e950: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0003e960: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+0003e970: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+0003e980: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003e990: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+0003e9a0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+0003e9b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0003e9c0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+0003e9d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0003e9e0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0003e9f0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+0003ea00: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+0003ea10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0003ea20: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+0003ea30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003ea40: 2074 656d 705f 6d6f 6465 6c20 3d20 5265   temp_model = Re
+0003ea50: 6d6f 7665 5769 7265 6c65 7373 436c 6f75  moveWirelessClou
+0003ea60: 6443 6f6e 6e65 6374 6f72 4672 6f6d 4772  dConnectorFromGr
+0003ea70: 6f75 7052 6573 706f 6e73 6542 6f64 7928  oupResponseBody(
 0003ea80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
 0003ea90: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
 0003eaa0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
 0003eab0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
 0003eac0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0003ead0: 6c61 7373 2052 6576 6f6b 654e 6574 4c69  lass RevokeNetLi
-0003eae0: 6e6b 5265 7175 6573 7428 5465 614d 6f64  nkRequest(TeaMod
-0003eaf0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0003eb00: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0003eb10: 656c 662c 0a20 2020 2020 2020 2063 6c69  elf,.        cli
-0003eb20: 656e 745f 746f 6b65 6e3a 2073 7472 203d  ent_token: str =
-0003eb30: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
-0003eb40: 7279 5f72 756e 3a20 626f 6f6c 203d 204e  ry_run: bool = N
-0003eb50: 6f6e 652c 0a20 2020 2020 2020 206e 6574  one,.        net
-0003eb60: 5f6c 696e 6b5f 6964 3a20 7374 7220 3d20  _link_id: str = 
-0003eb70: 4e6f 6e65 2c0a 2020 2020 2020 2020 7769  None,.        wi
-0003eb80: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
-0003eb90: 6e65 6374 6f72 5f69 643a 2073 7472 203d  nector_id: str =
-0003eba0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0003ebb0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-0003ebc0: 745f 746f 6b65 6e20 3d20 636c 6965 6e74  t_token = client
-0003ebd0: 5f74 6f6b 656e 0a20 2020 2020 2020 2073  _token.        s
-0003ebe0: 656c 662e 6472 795f 7275 6e20 3d20 6472  elf.dry_run = dr
-0003ebf0: 795f 7275 6e0a 2020 2020 2020 2020 7365  y_run.        se
-0003ec00: 6c66 2e6e 6574 5f6c 696e 6b5f 6964 203d  lf.net_link_id =
-0003ec10: 206e 6574 5f6c 696e 6b5f 6964 0a20 2020   net_link_id.   
-0003ec20: 2020 2020 2073 656c 662e 7769 7265 6c65       self.wirele
-0003ec30: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-0003ec40: 6f72 5f69 6420 3d20 7769 7265 6c65 7373  or_id = wireless
-0003ec50: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-0003ec60: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-0003ec70: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0003ec80: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0003ec90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0003eca0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0003ecb0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0003ecc0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0003ecd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003ece0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0003ecf0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0003ed00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0003ed10: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0003ed20: 6c69 656e 745f 746f 6b65 6e20 6973 206e  lient_token is n
-0003ed30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003ed40: 2020 2020 2072 6573 756c 745b 2743 6c69       result['Cli
-0003ed50: 656e 7454 6f6b 656e 275d 203d 2073 656c  entToken'] = sel
-0003ed60: 662e 636c 6965 6e74 5f74 6f6b 656e 0a20  f.client_token. 
-0003ed70: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0003ed80: 7279 5f72 756e 2069 7320 6e6f 7420 4e6f  ry_run is not No
-0003ed90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003eda0: 7265 7375 6c74 5b27 4472 7952 756e 275d  result['DryRun']
-0003edb0: 203d 2073 656c 662e 6472 795f 7275 6e0a   = self.dry_run.
-0003edc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0003edd0: 6e65 745f 6c69 6e6b 5f69 6420 6973 206e  net_link_id is n
-0003ede0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0003edf0: 2020 2020 2072 6573 756c 745b 274e 6574       result['Net
-0003ee00: 4c69 6e6b 4964 275d 203d 2073 656c 662e  LinkId'] = self.
-0003ee10: 6e65 745f 6c69 6e6b 5f69 640a 2020 2020  net_link_id.    
-0003ee20: 2020 2020 6966 2073 656c 662e 7769 7265      if self.wire
-0003ee30: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-0003ee40: 6374 6f72 5f69 6420 6973 206e 6f74 204e  ctor_id is not N
-0003ee50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0003ee60: 2072 6573 756c 745b 2757 6972 656c 6573   result['Wireles
-0003ee70: 7343 6c6f 7564 436f 6e6e 6563 746f 7249  sCloudConnectorI
-0003ee80: 6427 5d20 3d20 7365 6c66 2e77 6972 656c  d'] = self.wirel
-0003ee90: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-0003eea0: 746f 725f 6964 0a20 2020 2020 2020 2072  tor_id.        r
-0003eeb0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0003eec0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0003eed0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-0003eee0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0003eef0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0003ef00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0003ef10: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
-0003ef20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003ef30: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-0003ef40: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
-0003ef50: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
-0003ef60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003ef70: 2827 4472 7952 756e 2729 2069 7320 6e6f  ('DryRun') is no
-0003ef80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0003ef90: 2020 2020 7365 6c66 2e64 7279 5f72 756e      self.dry_run
-0003efa0: 203d 206d 2e67 6574 2827 4472 7952 756e   = m.get('DryRun
-0003efb0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0003efc0: 6765 7428 274e 6574 4c69 6e6b 4964 2729  get('NetLinkId')
-0003efd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0003efe0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0003eff0: 6574 5f6c 696e 6b5f 6964 203d 206d 2e67  et_link_id = m.g
-0003f000: 6574 2827 4e65 744c 696e 6b49 6427 290a  et('NetLinkId').
-0003f010: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0003f020: 2827 5769 7265 6c65 7373 436c 6f75 6443  ('WirelessCloudC
-0003f030: 6f6e 6e65 6374 6f72 4964 2729 2069 7320  onnectorId') is 
-0003f040: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003f050: 2020 2020 2020 7365 6c66 2e77 6972 656c        self.wirel
-0003f060: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-0003f070: 746f 725f 6964 203d 206d 2e67 6574 2827  tor_id = m.get('
-0003f080: 5769 7265 6c65 7373 436c 6f75 6443 6f6e  WirelessCloudCon
-0003f090: 6e65 6374 6f72 4964 2729 0a20 2020 2020  nectorId').     
-0003f0a0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003f0b0: 0a63 6c61 7373 2052 6576 6f6b 654e 6574  .class RevokeNet
-0003f0c0: 4c69 6e6b 5265 7370 6f6e 7365 426f 6479  LinkResponseBody
-0003f0d0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0003f0e0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0003f0f0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0003f100: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-0003f110: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0003f120: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0003f130: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-0003f140: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
-0003f150: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0003f160: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0003f170: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0003f180: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0003f190: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0003f1a0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0003f1b0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0003f1c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0003f1d0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0003f1e0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0003f1f0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0003f200: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0003f210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003f220: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0003f230: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0003f240: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0003f250: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0003f260: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0003f270: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0003f280: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0003f290: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0003f2a0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0003f2b0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0003f2c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0003f2d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0003f2e0: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-0003f2f0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-0003f300: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0003f310: 656c 660a 0a0a 636c 6173 7320 5265 766f  elf...class Revo
-0003f320: 6b65 4e65 744c 696e 6b52 6573 706f 6e73  keNetLinkRespons
-0003f330: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-0003f340: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0003f350: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0003f360: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-0003f370: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-0003f380: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
-0003f390: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
-0003f3a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-0003f3b0: 6479 3a20 5265 766f 6b65 4e65 744c 696e  dy: RevokeNetLin
-0003f3c0: 6b52 6573 706f 6e73 6542 6f64 7920 3d20  kResponseBody = 
-0003f3d0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0003f3e0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0003f3f0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-0003f400: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0003f410: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-0003f420: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-0003f430: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-0003f440: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0003f450: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-0003f460: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0003f470: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-0003f480: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-0003f490: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0003f4a0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0003f4b0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-0003f4c0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-0003f4d0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0003f4e0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0003f4f0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-0003f500: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0003f510: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0003f520: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0003f530: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0003f540: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0003f550: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0003f560: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0003f570: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0003f580: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003f590: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0003f5a0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0003f5b0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0003f5c0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-0003f5d0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-0003f5e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0003f5f0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-0003f600: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-0003f610: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0003f620: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-0003f630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003f640: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-0003f650: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-0003f660: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0003f670: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-0003f680: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003f690: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0003f6a0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-0003f6b0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-0003f6c0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0003f6d0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0003f6e0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0003f6f0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0003f700: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0003f710: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0003f720: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-0003f730: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0003f740: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0003f750: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-0003f760: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0003f770: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-0003f780: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-0003f790: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003f7a0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0003f7b0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-0003f7c0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-0003f7d0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0003f7e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003f7f0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0003f800: 6465 6c20 3d20 5265 766f 6b65 4e65 744c  del = RevokeNetL
-0003f810: 696e 6b52 6573 706f 6e73 6542 6f64 7928  inkResponseBody(
-0003f820: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0003f830: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0003f840: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0003f850: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0003f860: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0003f870: 6c61 7373 2053 746f 7043 6172 6473 5265  lass StopCardsRe
-0003f880: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-0003f890: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0003f8a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0003f8b0: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
-0003f8c0: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
-0003f8d0: 652c 0a20 2020 2020 2020 2064 7279 5f72  e,.        dry_r
-0003f8e0: 756e 3a20 626f 6f6c 203d 204e 6f6e 652c  un: bool = None,
-0003f8f0: 0a20 2020 2020 2020 2069 6363 6964 733a  .        iccids:
-0003f900: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
-0003f910: 652c 0a20 2020 2020 2020 2072 6567 696f  e,.        regio
-0003f920: 6e5f 6964 3a20 7374 7220 3d20 4e6f 6e65  n_id: str = None
-0003f930: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0003f940: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-0003f950: 656e 203d 2063 6c69 656e 745f 746f 6b65  en = client_toke
-0003f960: 6e0a 2020 2020 2020 2020 7365 6c66 2e64  n.        self.d
-0003f970: 7279 5f72 756e 203d 2064 7279 5f72 756e  ry_run = dry_run
-0003f980: 0a20 2020 2020 2020 2073 656c 662e 6963  .        self.ic
-0003f990: 6369 6473 203d 2069 6363 6964 730a 2020  cids = iccids.  
-0003f9a0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-0003f9b0: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
-0003f9c0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0003f9d0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0003f9e0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0003f9f0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0003fa00: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0003fa10: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0003fa20: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0003fa30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003fa40: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0003fa50: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0003fa60: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0003fa70: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-0003fa80: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
-0003fa90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003faa0: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-0003fab0: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
-0003fac0: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
-0003fad0: 2020 2020 6966 2073 656c 662e 6472 795f      if self.dry_
-0003fae0: 7275 6e20 6973 206e 6f74 204e 6f6e 653a  run is not None:
-0003faf0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003fb00: 756c 745b 2744 7279 5275 6e27 5d20 3d20  ult['DryRun'] = 
-0003fb10: 7365 6c66 2e64 7279 5f72 756e 0a20 2020  self.dry_run.   
-0003fb20: 2020 2020 2069 6620 7365 6c66 2e69 6363       if self.icc
-0003fb30: 6964 7320 6973 206e 6f74 204e 6f6e 653a  ids is not None:
-0003fb40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0003fb50: 756c 745b 2749 6363 6964 7327 5d20 3d20  ult['Iccids'] = 
-0003fb60: 7365 6c66 2e69 6363 6964 730a 2020 2020  self.iccids.    
-0003fb70: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
-0003fb80: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
-0003fb90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0003fba0: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
-0003fbb0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
-0003fbc0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0003fbd0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0003fbe0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0003fbf0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0003fc00: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0003fc10: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0003fc20: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
-0003fc30: 6e74 546f 6b65 6e27 2920 6973 206e 6f74  ntToken') is not
-0003fc40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003fc50: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
-0003fc60: 6f6b 656e 203d 206d 2e67 6574 2827 436c  oken = m.get('Cl
-0003fc70: 6965 6e74 546f 6b65 6e27 290a 2020 2020  ientToken').    
-0003fc80: 2020 2020 6966 206d 2e67 6574 2827 4472      if m.get('Dr
-0003fc90: 7952 756e 2729 2069 7320 6e6f 7420 4e6f  yRun') is not No
-0003fca0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0003fcb0: 7365 6c66 2e64 7279 5f72 756e 203d 206d  self.dry_run = m
-0003fcc0: 2e67 6574 2827 4472 7952 756e 2729 0a20  .get('DryRun'). 
-0003fcd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003fce0: 2749 6363 6964 7327 2920 6973 206e 6f74  'Iccids') is not
-0003fcf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0003fd00: 2020 2073 656c 662e 6963 6369 6473 203d     self.iccids =
-0003fd10: 206d 2e67 6574 2827 4963 6369 6473 2729   m.get('Iccids')
-0003fd20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0003fd30: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
-0003fd40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0003fd50: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
-0003fd60: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
-0003fd70: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
-0003fd80: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0003fd90: 636c 6173 7320 5374 6f70 4361 7264 7352  class StopCardsR
-0003fda0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0003fdb0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0003fdc0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0003fdd0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0003fde0: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-0003fdf0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0003fe00: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0003fe10: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-0003fe20: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
-0003fe30: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0003fe40: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-0003fe50: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0003fe60: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0003fe70: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-0003fe80: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0003fe90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0003fea0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0003feb0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0003fec0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0003fed0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0003fee0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-0003fef0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0003ff00: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-0003ff10: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-0003ff20: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-0003ff30: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0003ff40: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0003ff50: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0003ff60: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0003ff70: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0003ff80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0003ff90: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0003ffa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0003ffb0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0003ffc0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0003ffd0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0003ffe0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0003fff0: 0a63 6c61 7373 2053 746f 7043 6172 6473  .class StopCards
-00040000: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00040010: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00040020: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00040030: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-00040040: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-00040050: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00040060: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00040070: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00040080: 2020 2020 2062 6f64 793a 2053 746f 7043       body: StopC
-00040090: 6172 6473 5265 7370 6f6e 7365 426f 6479  ardsResponseBody
-000400a0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000400b0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000400c0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000400d0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000400e0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000400f0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-00040100: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-00040110: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00040120: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00040130: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-00040140: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
-00040150: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
-00040160: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00040170: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-00040180: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
-00040190: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
-000401a0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-000401b0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-000401c0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
-000401d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000401e0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-000401f0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00040200: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00040210: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00040220: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00040230: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00040240: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00040250: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00040260: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00040270: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00040280: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00040290: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-000402a0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-000402b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000402c0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000402d0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-000402e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000402f0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-00040300: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00040310: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00040320: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00040330: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00040340: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00040350: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00040360: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00040370: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00040380: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-00040390: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000403a0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000403b0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000403c0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000403d0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000403e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000403f0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00040400: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00040410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00040420: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00040430: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00040440: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00040450: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00040460: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00040470: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00040480: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00040490: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-000404a0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-000404b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000404c0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000404d0: 5f6d 6f64 656c 203d 2053 746f 7043 6172  _model = StopCar
-000404e0: 6473 5265 7370 6f6e 7365 426f 6479 2829  dsResponseBody()
-000404f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00040500: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-00040510: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-00040520: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-00040530: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00040540: 6173 7320 5375 626d 6974 4469 6167 6e6f  ass SubmitDiagno
-00040550: 7365 5461 736b 466f 7253 696e 676c 6543  seTaskForSingleC
-00040560: 6172 6452 6571 7565 7374 2854 6561 4d6f  ardRequest(TeaMo
-00040570: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00040580: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00040590: 7365 6c66 2c0a 2020 2020 2020 2020 6265  self,.        be
-000405a0: 6769 6e5f 7469 6d65 3a20 696e 7420 3d20  gin_time: int = 
-000405b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6465  None,.        de
-000405c0: 7374 696e 6174 696f 6e3a 2073 7472 203d  stination: str =
-000405d0: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-000405e0: 6e64 5f74 696d 653a 2069 6e74 203d 204e  nd_time: int = N
-000405f0: 6f6e 652c 0a20 2020 2020 2020 2072 6567  one,.        reg
-00040600: 696f 6e5f 6e6f 3a20 7374 7220 3d20 4e6f  ion_no: str = No
-00040610: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
-00040620: 7572 6365 5f75 6964 3a20 696e 7420 3d20  urce_uid: int = 
-00040630: 4e6f 6e65 2c0a 2020 2020 2020 2020 736f  None,.        so
-00040640: 7572 6365 3a20 7374 7220 3d20 4e6f 6e65  urce: str = None
-00040650: 2c0a 2020 2020 2020 2020 7769 7265 6c65  ,.        wirele
-00040660: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-00040670: 6f72 5f69 643a 2073 7472 203d 204e 6f6e  or_id: str = Non
-00040680: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00040690: 2020 7365 6c66 2e62 6567 696e 5f74 696d    self.begin_tim
-000406a0: 6520 3d20 6265 6769 6e5f 7469 6d65 0a20  e = begin_time. 
-000406b0: 2020 2020 2020 2073 656c 662e 6465 7374         self.dest
-000406c0: 696e 6174 696f 6e20 3d20 6465 7374 696e  ination = destin
-000406d0: 6174 696f 6e0a 2020 2020 2020 2020 7365  ation.        se
-000406e0: 6c66 2e65 6e64 5f74 696d 6520 3d20 656e  lf.end_time = en
-000406f0: 645f 7469 6d65 0a20 2020 2020 2020 2073  d_time.        s
-00040700: 656c 662e 7265 6769 6f6e 5f6e 6f20 3d20  elf.region_no = 
-00040710: 7265 6769 6f6e 5f6e 6f0a 2020 2020 2020  region_no.      
-00040720: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-00040730: 7569 6420 3d20 7265 736f 7572 6365 5f75  uid = resource_u
-00040740: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-00040750: 736f 7572 6365 203d 2073 6f75 7263 650a  source = source.
-00040760: 2020 2020 2020 2020 7365 6c66 2e77 6972          self.wir
-00040770: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
-00040780: 6563 746f 725f 6964 203d 2077 6972 656c  ector_id = wirel
-00040790: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-000407a0: 746f 725f 6964 0a0a 2020 2020 6465 6620  tor_id..    def 
-000407b0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000407c0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000407d0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000407e0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000407f0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00040800: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00040810: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00040820: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00040830: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00040840: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00040850: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00040860: 662e 6265 6769 6e5f 7469 6d65 2069 7320  f.begin_time is 
-00040870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00040880: 2020 2020 2020 7265 7375 6c74 5b27 4265        result['Be
-00040890: 6769 6e54 696d 6527 5d20 3d20 7365 6c66  ginTime'] = self
-000408a0: 2e62 6567 696e 5f74 696d 650a 2020 2020  .begin_time.    
-000408b0: 2020 2020 6966 2073 656c 662e 6465 7374      if self.dest
-000408c0: 696e 6174 696f 6e20 6973 206e 6f74 204e  ination is not N
-000408d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000408e0: 2072 6573 756c 745b 2744 6573 7469 6e61   result['Destina
-000408f0: 7469 6f6e 275d 203d 2073 656c 662e 6465  tion'] = self.de
-00040900: 7374 696e 6174 696f 6e0a 2020 2020 2020  stination.      
-00040910: 2020 6966 2073 656c 662e 656e 645f 7469    if self.end_ti
-00040920: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00040930: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00040940: 6c74 5b27 456e 6454 696d 6527 5d20 3d20  lt['EndTime'] = 
-00040950: 7365 6c66 2e65 6e64 5f74 696d 650a 2020  self.end_time.  
-00040960: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00040970: 6769 6f6e 5f6e 6f20 6973 206e 6f74 204e  gion_no is not N
-00040980: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00040990: 2072 6573 756c 745b 2752 6567 696f 6e4e   result['RegionN
-000409a0: 6f27 5d20 3d20 7365 6c66 2e72 6567 696f  o'] = self.regio
-000409b0: 6e5f 6e6f 0a20 2020 2020 2020 2069 6620  n_no.        if 
-000409c0: 7365 6c66 2e72 6573 6f75 7263 655f 7569  self.resource_ui
-000409d0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000409e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000409f0: 745b 2752 6573 6f75 7263 6555 6964 275d  t['ResourceUid']
-00040a00: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
-00040a10: 5f75 6964 0a20 2020 2020 2020 2069 6620  _uid.        if 
-00040a20: 7365 6c66 2e73 6f75 7263 6520 6973 206e  self.source is n
-00040a30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00040a40: 2020 2020 2072 6573 756c 745b 2753 6f75       result['Sou
-00040a50: 7263 6527 5d20 3d20 7365 6c66 2e73 6f75  rce'] = self.sou
-00040a60: 7263 650a 2020 2020 2020 2020 6966 2073  rce.        if s
-00040a70: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
-00040a80: 7564 5f63 6f6e 6e65 6374 6f72 5f69 6420  ud_connector_id 
-00040a90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00040aa0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00040ab0: 2757 6972 656c 6573 7343 6c6f 7564 436f  'WirelessCloudCo
-00040ac0: 6e6e 6563 746f 7249 6427 5d20 3d20 7365  nnectorId'] = se
-00040ad0: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
-00040ae0: 645f 636f 6e6e 6563 746f 725f 6964 0a20  d_connector_id. 
-00040af0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00040b00: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00040b10: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00040b20: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00040b30: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00040b40: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00040b50: 206d 2e67 6574 2827 4265 6769 6e54 696d   m.get('BeginTim
-00040b60: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00040b70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00040b80: 662e 6265 6769 6e5f 7469 6d65 203d 206d  f.begin_time = m
-00040b90: 2e67 6574 2827 4265 6769 6e54 696d 6527  .get('BeginTime'
-00040ba0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00040bb0: 6574 2827 4465 7374 696e 6174 696f 6e27  et('Destination'
-00040bc0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00040bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00040be0: 6465 7374 696e 6174 696f 6e20 3d20 6d2e  destination = m.
-00040bf0: 6765 7428 2744 6573 7469 6e61 7469 6f6e  get('Destination
-00040c00: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00040c10: 6765 7428 2745 6e64 5469 6d65 2729 2069  get('EndTime') i
-00040c20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00040c30: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
-00040c40: 5f74 696d 6520 3d20 6d2e 6765 7428 2745  _time = m.get('E
-00040c50: 6e64 5469 6d65 2729 0a20 2020 2020 2020  ndTime').       
-00040c60: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
-00040c70: 6e4e 6f27 2920 6973 206e 6f74 204e 6f6e  nNo') is not Non
+0003ead0: 6c61 7373 2052 6573 756d 6543 6172 6473  lass ResumeCards
+0003eae0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+0003eaf0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0003eb00: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0003eb10: 662c 0a20 2020 2020 2020 2063 6c69 656e  f,.        clien
+0003eb20: 745f 746f 6b65 6e3a 2073 7472 203d 204e  t_token: str = N
+0003eb30: 6f6e 652c 0a20 2020 2020 2020 2064 7279  one,.        dry
+0003eb40: 5f72 756e 3a20 626f 6f6c 203d 204e 6f6e  _run: bool = Non
+0003eb50: 652c 0a20 2020 2020 2020 2069 6363 6964  e,.        iccid
+0003eb60: 733a 204c 6973 745b 7374 725d 203d 204e  s: List[str] = N
+0003eb70: 6f6e 652c 0a20 2020 2020 2020 2072 6567  one,.        reg
+0003eb80: 696f 6e5f 6964 3a20 7374 7220 3d20 4e6f  ion_id: str = No
+0003eb90: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0003eba0: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+0003ebb0: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
+0003ebc0: 6b65 6e0a 2020 2020 2020 2020 7365 6c66  ken.        self
+0003ebd0: 2e64 7279 5f72 756e 203d 2064 7279 5f72  .dry_run = dry_r
+0003ebe0: 756e 0a20 2020 2020 2020 2073 656c 662e  un.        self.
+0003ebf0: 6963 6369 6473 203d 2069 6363 6964 730a  iccids = iccids.
+0003ec00: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+0003ec10: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
+0003ec20: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
+0003ec30: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0003ec40: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+0003ec50: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0003ec60: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0003ec70: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+0003ec80: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0003ec90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003eca0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0003ecb0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0003ecc0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0003ecd0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+0003ece0: 6965 6e74 5f74 6f6b 656e 2069 7320 6e6f  ient_token is no
+0003ecf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003ed00: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+0003ed10: 6e74 546f 6b65 6e27 5d20 3d20 7365 6c66  ntToken'] = self
+0003ed20: 2e63 6c69 656e 745f 746f 6b65 6e0a 2020  .client_token.  
+0003ed30: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
+0003ed40: 795f 7275 6e20 6973 206e 6f74 204e 6f6e  y_run is not Non
+0003ed50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003ed60: 6573 756c 745b 2744 7279 5275 6e27 5d20  esult['DryRun'] 
+0003ed70: 3d20 7365 6c66 2e64 7279 5f72 756e 0a20  = self.dry_run. 
+0003ed80: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+0003ed90: 6363 6964 7320 6973 206e 6f74 204e 6f6e  ccids is not Non
+0003eda0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0003edb0: 6573 756c 745b 2749 6363 6964 7327 5d20  esult['Iccids'] 
+0003edc0: 3d20 7365 6c66 2e69 6363 6964 730a 2020  = self.iccids.  
+0003edd0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+0003ede0: 6769 6f6e 5f69 6420 6973 206e 6f74 204e  gion_id is not N
+0003edf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003ee00: 2072 6573 756c 745b 2752 6567 696f 6e49   result['RegionI
+0003ee10: 6427 5d20 3d20 7365 6c66 2e72 6567 696f  d'] = self.regio
+0003ee20: 6e5f 6964 0a20 2020 2020 2020 2072 6574  n_id.        ret
+0003ee30: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0003ee40: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0003ee50: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0003ee60: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0003ee70: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0003ee80: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+0003ee90: 6965 6e74 546f 6b65 6e27 2920 6973 206e  ientToken') is n
+0003eea0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003eeb0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+0003eec0: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
+0003eed0: 436c 6965 6e74 546f 6b65 6e27 290a 2020  ClientToken').  
+0003eee0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003eef0: 4472 7952 756e 2729 2069 7320 6e6f 7420  DryRun') is not 
+0003ef00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0003ef10: 2020 7365 6c66 2e64 7279 5f72 756e 203d    self.dry_run =
+0003ef20: 206d 2e67 6574 2827 4472 7952 756e 2729   m.get('DryRun')
+0003ef30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0003ef40: 7428 2749 6363 6964 7327 2920 6973 206e  t('Iccids') is n
+0003ef50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0003ef60: 2020 2020 2073 656c 662e 6963 6369 6473       self.iccids
+0003ef70: 203d 206d 2e67 6574 2827 4963 6369 6473   = m.get('Iccids
+0003ef80: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003ef90: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
+0003efa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003efb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0003efc0: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
+0003efd0: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
+0003efe0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0003eff0: 0a0a 636c 6173 7320 5265 7375 6d65 4361  ..class ResumeCa
+0003f000: 7264 7352 6573 706f 6e73 6542 6f64 7928  rdsResponseBody(
+0003f010: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0003f020: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0003f030: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0003f040: 2020 2072 6571 7565 7374 5f69 643a 2073     request_id: s
+0003f050: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+0003f060: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
+0003f070: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
+0003f080: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
+0003f090: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0003f0a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0003f0b0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0003f0c0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0003f0d0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+0003f0e0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0003f0f0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0003f100: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0003f110: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0003f120: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0003f130: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0003f140: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
+0003f150: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0003f160: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+0003f170: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
+0003f180: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
+0003f190: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0003f1a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0003f1b0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+0003f1c0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+0003f1d0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0003f1e0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0003f1f0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+0003f200: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003f210: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0003f220: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+0003f230: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+0003f240: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0003f250: 6c66 0a0a 0a63 6c61 7373 2052 6573 756d  lf...class Resum
+0003f260: 6543 6172 6473 5265 7370 6f6e 7365 2854  eCardsResponse(T
+0003f270: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0003f280: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0003f290: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0003f2a0: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+0003f2b0: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+0003f2c0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+0003f2d0: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+0003f2e0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0003f2f0: 2052 6573 756d 6543 6172 6473 5265 7370   ResumeCardsResp
+0003f300: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
+0003f310: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0003f320: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+0003f330: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+0003f340: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0003f350: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
+0003f360: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0003f370: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+0003f380: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0003f390: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0003f3a0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0003f3b0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
+0003f3c0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+0003f3d0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0003f3e0: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
+0003f3f0: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
+0003f400: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
+0003f410: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0003f420: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
+0003f430: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
+0003f440: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0003f450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0003f460: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0003f470: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0003f480: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0003f490: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0003f4a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0003f4b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0003f4c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0003f4d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0003f4e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0003f4f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0003f500: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+0003f510: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003f520: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+0003f530: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+0003f540: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0003f550: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+0003f560: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+0003f570: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0003f580: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+0003f590: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+0003f5a0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+0003f5b0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+0003f5c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f5d0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+0003f5e0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+0003f5f0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+0003f600: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+0003f610: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+0003f620: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+0003f630: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0003f640: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0003f650: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0003f660: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+0003f670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f680: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0003f690: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+0003f6a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0003f6b0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003f6c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0003f6d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0003f6e0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+0003f6f0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0003f700: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0003f710: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+0003f720: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003f730: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+0003f740: 2052 6573 756d 6543 6172 6473 5265 7370   ResumeCardsResp
+0003f750: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0003f760: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0003f770: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0003f780: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0003f790: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0003f7a0: 2073 656c 660a 0a0a 636c 6173 7320 5265   self...class Re
+0003f7b0: 766f 6b65 4e65 744c 696e 6b52 6571 7565  vokeNetLinkReque
+0003f7c0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+0003f7d0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0003f7e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0003f7f0: 2020 2020 2020 636c 6965 6e74 5f74 6f6b        client_tok
+0003f800: 656e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  en: str = None,.
+0003f810: 2020 2020 2020 2020 6472 795f 7275 6e3a          dry_run:
+0003f820: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+0003f830: 2020 2020 2020 6e65 745f 6c69 6e6b 5f69        net_link_i
+0003f840: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0003f850: 2020 2020 2020 2077 6972 656c 6573 735f         wireless_
+0003f860: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
+0003f870: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0003f880: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0003f890: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
+0003f8a0: 203d 2063 6c69 656e 745f 746f 6b65 6e0a   = client_token.
+0003f8b0: 2020 2020 2020 2020 7365 6c66 2e64 7279          self.dry
+0003f8c0: 5f72 756e 203d 2064 7279 5f72 756e 0a20  _run = dry_run. 
+0003f8d0: 2020 2020 2020 2073 656c 662e 6e65 745f         self.net_
+0003f8e0: 6c69 6e6b 5f69 6420 3d20 6e65 745f 6c69  link_id = net_li
+0003f8f0: 6e6b 5f69 640a 2020 2020 2020 2020 7365  nk_id.        se
+0003f900: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
+0003f910: 645f 636f 6e6e 6563 746f 725f 6964 203d  d_connector_id =
+0003f920: 2077 6972 656c 6573 735f 636c 6f75 645f   wireless_cloud_
+0003f930: 636f 6e6e 6563 746f 725f 6964 0a0a 2020  connector_id..  
+0003f940: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0003f950: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0003f960: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0003f970: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0003f980: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0003f990: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0003f9a0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0003f9b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003f9c0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0003f9d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0003f9e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0003f9f0: 6966 2073 656c 662e 636c 6965 6e74 5f74  if self.client_t
+0003fa00: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
+0003fa10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003fa20: 7375 6c74 5b27 436c 6965 6e74 546f 6b65  sult['ClientToke
+0003fa30: 6e27 5d20 3d20 7365 6c66 2e63 6c69 656e  n'] = self.clien
+0003fa40: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
+0003fa50: 6966 2073 656c 662e 6472 795f 7275 6e20  if self.dry_run 
+0003fa60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0003fa70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0003fa80: 2744 7279 5275 6e27 5d20 3d20 7365 6c66  'DryRun'] = self
+0003fa90: 2e64 7279 5f72 756e 0a20 2020 2020 2020  .dry_run.       
+0003faa0: 2069 6620 7365 6c66 2e6e 6574 5f6c 696e   if self.net_lin
+0003fab0: 6b5f 6964 2069 7320 6e6f 7420 4e6f 6e65  k_id is not None
+0003fac0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0003fad0: 7375 6c74 5b27 4e65 744c 696e 6b49 6427  sult['NetLinkId'
+0003fae0: 5d20 3d20 7365 6c66 2e6e 6574 5f6c 696e  ] = self.net_lin
+0003faf0: 6b5f 6964 0a20 2020 2020 2020 2069 6620  k_id.        if 
+0003fb00: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
+0003fb10: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+0003fb20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0003fb30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0003fb40: 5b27 5769 7265 6c65 7373 436c 6f75 6443  ['WirelessCloudC
+0003fb50: 6f6e 6e65 6374 6f72 4964 275d 203d 2073  onnectorId'] = s
+0003fb60: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
+0003fb70: 7564 5f63 6f6e 6e65 6374 6f72 5f69 640a  ud_connector_id.
+0003fb80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0003fb90: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0003fba0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0003fbb0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0003fbc0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0003fbd0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0003fbe0: 6620 6d2e 6765 7428 2743 6c69 656e 7454  f m.get('ClientT
+0003fbf0: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
+0003fc00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003fc10: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+0003fc20: 6e20 3d20 6d2e 6765 7428 2743 6c69 656e  n = m.get('Clien
+0003fc30: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
+0003fc40: 2069 6620 6d2e 6765 7428 2744 7279 5275   if m.get('DryRu
+0003fc50: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+0003fc60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0003fc70: 662e 6472 795f 7275 6e20 3d20 6d2e 6765  f.dry_run = m.ge
+0003fc80: 7428 2744 7279 5275 6e27 290a 2020 2020  t('DryRun').    
+0003fc90: 2020 2020 6966 206d 2e67 6574 2827 4e65      if m.get('Ne
+0003fca0: 744c 696e 6b49 6427 2920 6973 206e 6f74  tLinkId') is not
+0003fcb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0003fcc0: 2020 2073 656c 662e 6e65 745f 6c69 6e6b     self.net_link
+0003fcd0: 5f69 6420 3d20 6d2e 6765 7428 274e 6574  _id = m.get('Net
+0003fce0: 4c69 6e6b 4964 2729 0a20 2020 2020 2020  LinkId').       
+0003fcf0: 2069 6620 6d2e 6765 7428 2757 6972 656c   if m.get('Wirel
+0003fd00: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
+0003fd10: 7249 6427 2920 6973 206e 6f74 204e 6f6e  rId') is not Non
+0003fd20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0003fd30: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
+0003fd40: 7564 5f63 6f6e 6e65 6374 6f72 5f69 6420  ud_connector_id 
+0003fd50: 3d20 6d2e 6765 7428 2757 6972 656c 6573  = m.get('Wireles
+0003fd60: 7343 6c6f 7564 436f 6e6e 6563 746f 7249  sCloudConnectorI
+0003fd70: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+0003fd80: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+0003fd90: 5265 766f 6b65 4e65 744c 696e 6b52 6573  RevokeNetLinkRes
+0003fda0: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+0003fdb0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0003fdc0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+0003fdd0: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
+0003fde0: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
+0003fdf0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+0003fe00: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+0003fe10: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+0003fe20: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0003fe30: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0003fe40: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+0003fe50: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0003fe60: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0003fe70: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+0003fe80: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0003fe90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0003fea0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0003feb0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0003fec0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0003fed0: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+0003fee0: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+0003fef0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0003ff00: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+0003ff10: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+0003ff20: 7374 5f69 640a 2020 2020 2020 2020 7265  st_id.        re
+0003ff30: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0003ff40: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0003ff50: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+0003ff60: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0003ff70: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0003ff80: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+0003ff90: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+0003ffa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0003ffb0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+0003ffc0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+0003ffd0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+0003ffe0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0003fff0: 6c61 7373 2052 6576 6f6b 654e 6574 4c69  lass RevokeNetLi
+00040000: 6e6b 5265 7370 6f6e 7365 2854 6561 4d6f  nkResponse(TeaMo
+00040010: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00040020: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00040030: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+00040040: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00040050: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00040060: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00040070: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00040080: 2020 2020 2020 2062 6f64 793a 2052 6576         body: Rev
+00040090: 6f6b 654e 6574 4c69 6e6b 5265 7370 6f6e  okeNetLinkRespon
+000400a0: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
+000400b0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+000400c0: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+000400d0: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+000400e0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+000400f0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00040100: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00040110: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+00040120: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00040130: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+00040140: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+00040150: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
+00040160: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
+00040170: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+00040180: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
+00040190: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
+000401a0: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
+000401b0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+000401c0: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
+000401d0: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
+000401e0: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+000401f0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00040200: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00040210: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00040220: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00040230: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00040240: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00040250: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00040260: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00040270: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00040280: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00040290: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000402a0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000402b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000402c0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000402d0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000402e0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000402f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00040300: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00040310: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00040320: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+00040330: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+00040340: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00040350: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+00040360: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00040370: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00040380: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00040390: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+000403a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000403b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000403c0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000403d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000403e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000403f0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00040400: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00040410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00040420: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00040430: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00040440: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00040450: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00040460: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00040470: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00040480: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00040490: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000404a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000404b0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+000404c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000404d0: 2020 7465 6d70 5f6d 6f64 656c 203d 2052    temp_model = R
+000404e0: 6576 6f6b 654e 6574 4c69 6e6b 5265 7370  evokeNetLinkResp
+000404f0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00040500: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00040510: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00040520: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00040530: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00040540: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
+00040550: 6f70 4361 7264 7352 6571 7565 7374 2854  opCardsRequest(T
+00040560: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00040570: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00040580: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00040590: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
+000405a0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000405b0: 2020 2020 6472 795f 7275 6e3a 2062 6f6f      dry_run: boo
+000405c0: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+000405d0: 2020 6963 6369 6473 3a20 4c69 7374 5b73    iccids: List[s
+000405e0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000405f0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
+00040600: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+00040610: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
+00040620: 6c69 656e 745f 746f 6b65 6e20 3d20 636c  lient_token = cl
+00040630: 6965 6e74 5f74 6f6b 656e 0a20 2020 2020  ient_token.     
+00040640: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
+00040650: 3d20 6472 795f 7275 6e0a 2020 2020 2020  = dry_run.      
+00040660: 2020 7365 6c66 2e69 6363 6964 7320 3d20    self.iccids = 
+00040670: 6963 6369 6473 0a20 2020 2020 2020 2073  iccids.        s
+00040680: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00040690: 7265 6769 6f6e 5f69 640a 0a20 2020 2064  region_id..    d
+000406a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000406b0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000406c0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000406d0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000406e0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000406f0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00040700: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00040710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00040720: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00040730: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00040740: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00040750: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00040760: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00040770: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00040780: 745b 2743 6c69 656e 7454 6f6b 656e 275d  t['ClientToken']
+00040790: 203d 2073 656c 662e 636c 6965 6e74 5f74   = self.client_t
+000407a0: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+000407b0: 7365 6c66 2e64 7279 5f72 756e 2069 7320  self.dry_run is 
+000407c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000407d0: 2020 2020 2020 7265 7375 6c74 5b27 4472        result['Dr
+000407e0: 7952 756e 275d 203d 2073 656c 662e 6472  yRun'] = self.dr
+000407f0: 795f 7275 6e0a 2020 2020 2020 2020 6966  y_run.        if
+00040800: 2073 656c 662e 6963 6369 6473 2069 7320   self.iccids is 
+00040810: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00040820: 2020 2020 2020 7265 7375 6c74 5b27 4963        result['Ic
+00040830: 6369 6473 275d 203d 2073 656c 662e 6963  cids'] = self.ic
+00040840: 6369 6473 0a20 2020 2020 2020 2069 6620  cids.        if 
+00040850: 7365 6c66 2e72 6567 696f 6e5f 6964 2069  self.region_id i
+00040860: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00040870: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00040880: 5265 6769 6f6e 4964 275d 203d 2073 656c  RegionId'] = sel
+00040890: 662e 7265 6769 6f6e 5f69 640a 2020 2020  f.region_id.    
+000408a0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000408b0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000408c0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000408d0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000408e0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000408f0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00040900: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
+00040910: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00040920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00040930: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
+00040940: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
+00040950: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
+00040960: 6d2e 6765 7428 2744 7279 5275 6e27 2920  m.get('DryRun') 
+00040970: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00040980: 2020 2020 2020 2020 2073 656c 662e 6472           self.dr
+00040990: 795f 7275 6e20 3d20 6d2e 6765 7428 2744  y_run = m.get('D
+000409a0: 7279 5275 6e27 290a 2020 2020 2020 2020  ryRun').        
+000409b0: 6966 206d 2e67 6574 2827 4963 6369 6473  if m.get('Iccids
+000409c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000409d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000409e0: 2e69 6363 6964 7320 3d20 6d2e 6765 7428  .iccids = m.get(
+000409f0: 2749 6363 6964 7327 290a 2020 2020 2020  'Iccids').      
+00040a00: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
+00040a10: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
+00040a20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00040a30: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00040a40: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+00040a50: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00040a60: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+00040a70: 746f 7043 6172 6473 5265 7370 6f6e 7365  topCardsResponse
+00040a80: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+00040a90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00040aa0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00040ab0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+00040ac0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00040ad0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00040ae0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+00040af0: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
+00040b00: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00040b10: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00040b20: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00040b30: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00040b40: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00040b50: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00040b60: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00040b70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040b80: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00040b90: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00040ba0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00040bb0: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
+00040bc0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00040bd0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00040be0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
+00040bf0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00040c00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00040c10: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00040c20: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00040c30: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00040c40: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00040c50: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00040c60: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+00040c70: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
 00040c80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00040c90: 656c 662e 7265 6769 6f6e 5f6e 6f20 3d20  elf.region_no = 
-00040ca0: 6d2e 6765 7428 2752 6567 696f 6e4e 6f27  m.get('RegionNo'
-00040cb0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00040cc0: 6574 2827 5265 736f 7572 6365 5569 6427  et('ResourceUid'
-00040cd0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00040ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00040cf0: 7265 736f 7572 6365 5f75 6964 203d 206d  resource_uid = m
-00040d00: 2e67 6574 2827 5265 736f 7572 6365 5569  .get('ResourceUi
-00040d10: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00040d20: 2e67 6574 2827 536f 7572 6365 2729 2069  .get('Source') i
-00040d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00040d40: 2020 2020 2020 2020 7365 6c66 2e73 6f75          self.sou
-00040d50: 7263 6520 3d20 6d2e 6765 7428 2753 6f75  rce = m.get('Sou
-00040d60: 7263 6527 290a 2020 2020 2020 2020 6966  rce').        if
-00040d70: 206d 2e67 6574 2827 5769 7265 6c65 7373   m.get('Wireless
-00040d80: 436c 6f75 6443 6f6e 6e65 6374 6f72 4964  CloudConnectorId
-00040d90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00040da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00040db0: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
-00040dc0: 636f 6e6e 6563 746f 725f 6964 203d 206d  connector_id = m
-00040dd0: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-00040de0: 6f75 6443 6f6e 6e65 6374 6f72 4964 2729  oudConnectorId')
-00040df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00040e00: 7365 6c66 0a0a 0a63 6c61 7373 2053 7562  self...class Sub
-00040e10: 6d69 7444 6961 676e 6f73 6554 6173 6b46  mitDiagnoseTaskF
-00040e20: 6f72 5369 6e67 6c65 4361 7264 5265 7370  orSingleCardResp
-00040e30: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-00040e40: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00040e50: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00040e60: 6c66 2c0a 2020 2020 2020 2020 6469 6167  lf,.        diag
-00040e70: 6e6f 7365 5f74 6173 6b5f 6964 3a20 7374  nose_task_id: st
-00040e80: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00040e90: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
-00040ea0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-00040eb0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
-00040ec0: 6167 6e6f 7365 5f74 6173 6b5f 6964 203d  agnose_task_id =
-00040ed0: 2064 6961 676e 6f73 655f 7461 736b 5f69   diagnose_task_i
-00040ee0: 640a 2020 2020 2020 2020 7365 6c66 2e72  d.        self.r
-00040ef0: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-00040f00: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
-00040f10: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00040f20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00040f30: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00040f40: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00040f50: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00040f60: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00040f70: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00040f80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00040f90: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00040fa0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00040fb0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00040fc0: 662e 6469 6167 6e6f 7365 5f74 6173 6b5f  f.diagnose_task_
-00040fd0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00040fe0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00040ff0: 6c74 5b27 4469 6167 6e6f 7365 5461 736b  lt['DiagnoseTask
-00041000: 4964 275d 203d 2073 656c 662e 6469 6167  Id'] = self.diag
-00041010: 6e6f 7365 5f74 6173 6b5f 6964 0a20 2020  nose_task_id.   
-00041020: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
-00041030: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
-00041040: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00041050: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
-00041060: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
-00041070: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
-00041080: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00041090: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000410a0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000410b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000410c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000410d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000410e0: 4469 6167 6e6f 7365 5461 736b 4964 2729  DiagnoseTaskId')
-000410f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00041100: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00041110: 6961 676e 6f73 655f 7461 736b 5f69 6420  iagnose_task_id 
-00041120: 3d20 6d2e 6765 7428 2744 6961 676e 6f73  = m.get('Diagnos
-00041130: 6554 6173 6b49 6427 290a 2020 2020 2020  eTaskId').      
-00041140: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-00041150: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-00041160: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00041170: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00041180: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-00041190: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
-000411a0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000411b0: 7320 5375 626d 6974 4469 6167 6e6f 7365  s SubmitDiagnose
-000411c0: 5461 736b 466f 7253 696e 676c 6543 6172  TaskForSingleCar
-000411d0: 6452 6573 706f 6e73 6528 5465 614d 6f64  dResponse(TeaMod
-000411e0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000411f0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00041200: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-00041210: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-00041220: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00041230: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-00041240: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00041250: 2020 2020 2020 626f 6479 3a20 5375 626d        body: Subm
-00041260: 6974 4469 6167 6e6f 7365 5461 736b 466f  itDiagnoseTaskFo
-00041270: 7253 696e 676c 6543 6172 6452 6573 706f  rSingleCardRespo
-00041280: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-00041290: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000412a0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000412b0: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-000412c0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000412d0: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-000412e0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-000412f0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-00041300: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00041310: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00041320: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00041330: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-00041340: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-00041350: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00041360: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-00041370: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-00041380: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-00041390: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-000413a0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-000413b0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-000413c0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-000413d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000413e0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-000413f0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00041400: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00041410: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00041420: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00041430: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00041440: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00041450: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00041460: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00041470: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00041480: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-00041490: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000414a0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-000414b0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-000414c0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-000414d0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-000414e0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-000414f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00041500: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-00041510: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00041520: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-00041530: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-00041540: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00041550: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-00041560: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-00041570: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-00041580: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00041590: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000415a0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-000415b0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-000415c0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-000415d0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-000415e0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-000415f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00041600: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00041610: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00041620: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00041630: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-00041640: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00041650: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00041660: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-00041670: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-00041680: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00041690: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-000416a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000416b0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-000416c0: 5375 626d 6974 4469 6167 6e6f 7365 5461  SubmitDiagnoseTa
-000416d0: 736b 466f 7253 696e 676c 6543 6172 6452  skForSingleCardR
-000416e0: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-000416f0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00041700: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00041710: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00041720: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00041730: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00041740: 2053 7769 7463 6857 6972 656c 6573 7343   SwitchWirelessC
-00041750: 6c6f 7564 436f 6e6e 6563 746f 7254 6f42  loudConnectorToB
-00041760: 7573 696e 6573 7352 6571 7565 7374 2854  usinessRequest(T
-00041770: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00041780: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00041790: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000417a0: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
-000417b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000417c0: 2020 2020 6472 795f 7275 6e3a 2062 6f6f      dry_run: boo
-000417d0: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
-000417e0: 2020 7769 7265 6c65 7373 5f63 6c6f 7564    wireless_cloud
-000417f0: 5f63 6f6e 6e65 6374 6f72 5f69 643a 2073  _connector_id: s
-00041800: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-00041810: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-00041820: 6c69 656e 745f 746f 6b65 6e20 3d20 636c  lient_token = cl
-00041830: 6965 6e74 5f74 6f6b 656e 0a20 2020 2020  ient_token.     
-00041840: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
-00041850: 3d20 6472 795f 7275 6e0a 2020 2020 2020  = dry_run.      
-00041860: 2020 7365 6c66 2e77 6972 656c 6573 735f    self.wireless_
-00041870: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-00041880: 6964 203d 2077 6972 656c 6573 735f 636c  id = wireless_cl
-00041890: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
-000418a0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000418b0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000418c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-000418d0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000418e0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000418f0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00041900: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00041910: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00041920: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00041930: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00041940: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00041950: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00041960: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
-00041970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00041980: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00041990: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
-000419a0: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
-000419b0: 2020 2020 6966 2073 656c 662e 6472 795f      if self.dry_
-000419c0: 7275 6e20 6973 206e 6f74 204e 6f6e 653a  run is not None:
-000419d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000419e0: 756c 745b 2744 7279 5275 6e27 5d20 3d20  ult['DryRun'] = 
-000419f0: 7365 6c66 2e64 7279 5f72 756e 0a20 2020  self.dry_run.   
-00041a00: 2020 2020 2069 6620 7365 6c66 2e77 6972       if self.wir
-00041a10: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
-00041a20: 6563 746f 725f 6964 2069 7320 6e6f 7420  ector_id is not 
-00041a30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00041a40: 2020 7265 7375 6c74 5b27 5769 7265 6c65    result['Wirele
-00041a50: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
-00041a60: 4964 275d 203d 2073 656c 662e 7769 7265  Id'] = self.wire
-00041a70: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-00041a80: 6374 6f72 5f69 640a 2020 2020 2020 2020  ctor_id.        
-00041a90: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00041aa0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00041ab0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00041ac0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00041ad0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00041ae0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00041af0: 2743 6c69 656e 7454 6f6b 656e 2729 2069  'ClientToken') i
-00041b00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00041b10: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00041b20: 656e 745f 746f 6b65 6e20 3d20 6d2e 6765  ent_token = m.ge
-00041b30: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
-00041b40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00041b50: 7428 2744 7279 5275 6e27 2920 6973 206e  t('DryRun') is n
-00041b60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00041b70: 2020 2020 2073 656c 662e 6472 795f 7275       self.dry_ru
-00041b80: 6e20 3d20 6d2e 6765 7428 2744 7279 5275  n = m.get('DryRu
-00041b90: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
-00041ba0: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-00041bb0: 6f75 6443 6f6e 6e65 6374 6f72 4964 2729  oudConnectorId')
-00041bc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00041bd0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-00041be0: 6972 656c 6573 735f 636c 6f75 645f 636f  ireless_cloud_co
-00041bf0: 6e6e 6563 746f 725f 6964 203d 206d 2e67  nnector_id = m.g
-00041c00: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
-00041c10: 6443 6f6e 6e65 6374 6f72 4964 2729 0a20  dConnectorId'). 
-00041c20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00041c30: 6c66 0a0a 0a63 6c61 7373 2053 7769 7463  lf...class Switc
-00041c40: 6857 6972 656c 6573 7343 6c6f 7564 436f  hWirelessCloudCo
-00041c50: 6e6e 6563 746f 7254 6f42 7573 696e 6573  nnectorToBusines
-00041c60: 7352 6573 706f 6e73 6542 6f64 7928 5465  sResponseBody(Te
-00041c70: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00041c80: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00041c90: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00041ca0: 2072 6571 7565 7374 5f69 643a 2073 7472   request_id: str
-00041cb0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00041cc0: 2020 2020 2020 2020 2320 4964 206f 6620          # Id of 
-00041cd0: 7468 6520 7265 7175 6573 740a 2020 2020  the request.    
-00041ce0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00041cf0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-00041d00: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00041d10: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00041d20: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00041d30: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00041d40: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00041d50: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00041d60: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00041d70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00041d80: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00041d90: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00041da0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00041db0: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
-00041dc0: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
-00041dd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00041de0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
-00041df0: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
-00041e00: 7374 5f69 640a 2020 2020 2020 2020 7265  st_id.        re
-00041e10: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00041e20: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00041e30: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00041e40: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00041e50: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00041e60: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00041e70: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-00041e80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00041e90: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00041ea0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-00041eb0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-00041ec0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00041ed0: 6c61 7373 2053 7769 7463 6857 6972 656c  lass SwitchWirel
-00041ee0: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-00041ef0: 7254 6f42 7573 696e 6573 7352 6573 706f  rToBusinessRespo
-00041f00: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-00041f10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00041f20: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00041f30: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-00041f40: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-00041f50: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00041f60: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-00041f70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00041f80: 626f 6479 3a20 5377 6974 6368 5769 7265  body: SwitchWire
-00041f90: 6c65 7373 436c 6f75 6443 6f6e 6e65 6374  lessCloudConnect
-00041fa0: 6f72 546f 4275 7369 6e65 7373 5265 7370  orToBusinessResp
-00041fb0: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
-00041fc0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00041fd0: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-00041fe0: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
-00041ff0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00042000: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-00042010: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-00042020: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-00042030: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00042040: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00042050: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-00042060: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
-00042070: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00042080: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-00042090: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
-000420a0: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
-000420b0: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
-000420c0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-000420d0: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
-000420e0: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
-000420f0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-00042100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00042110: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-00042120: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00042130: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00042140: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00042150: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00042160: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00042170: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042180: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00042190: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000421a0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000421b0: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000421c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000421d0: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000421e0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000421f0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00042200: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-00042210: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-00042220: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00042230: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-00042240: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-00042250: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-00042260: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00042270: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00042280: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-00042290: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-000422a0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-000422b0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000422c0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000422d0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000422e0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000422f0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00042300: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00042310: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00040c90: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+00040ca0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+00040cb0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+00040cc0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00040cd0: 5374 6f70 4361 7264 7352 6573 706f 6e73  StopCardsRespons
+00040ce0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00040cf0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00040d00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00040d10: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+00040d20: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+00040d30: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+00040d40: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+00040d50: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+00040d60: 6479 3a20 5374 6f70 4361 7264 7352 6573  dy: StopCardsRes
+00040d70: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+00040d80: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00040d90: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00040da0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00040db0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00040dc0: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+00040dd0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00040de0: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+00040df0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00040e00: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00040e10: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00040e20: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
+00040e30: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+00040e40: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+00040e50: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
+00040e60: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
+00040e70: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
+00040e80: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+00040e90: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
+00040ea0: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
+00040eb0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00040ec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00040ed0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+00040ee0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00040ef0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00040f00: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00040f10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00040f20: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00040f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00040f40: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00040f50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00040f60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00040f70: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00040f80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00040f90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00040fa0: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+00040fb0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+00040fc0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+00040fd0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+00040fe0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00040ff0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+00041000: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+00041010: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+00041020: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00041030: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00041040: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00041050: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00041060: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00041070: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00041080: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00041090: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+000410a0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000410b0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000410c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000410d0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000410e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000410f0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00041100: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+00041110: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+00041120: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00041130: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00041140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00041150: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00041160: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00041170: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00041180: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00041190: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000411a0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+000411b0: 3d20 5374 6f70 4361 7264 7352 6573 706f  = StopCardsRespo
+000411c0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+000411d0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000411e0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+000411f0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00041200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00041210: 7365 6c66 0a0a 0a63 6c61 7373 2053 7562  self...class Sub
+00041220: 6d69 7444 6961 676e 6f73 6554 6173 6b46  mitDiagnoseTaskF
+00041230: 6f72 5369 6e67 6c65 4361 7264 5265 7175  orSingleCardRequ
+00041240: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00041250: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00041260: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00041270: 2020 2020 2020 2062 6567 696e 5f74 696d         begin_tim
+00041280: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00041290: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+000412a0: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+000412b0: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
+000412c0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+000412d0: 2020 2020 2020 7265 6769 6f6e 5f6e 6f3a        region_no:
+000412e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000412f0: 2020 2020 2072 6573 6f75 7263 655f 7569       resource_ui
+00041300: 643a 2069 6e74 203d 204e 6f6e 652c 0a20  d: int = None,. 
+00041310: 2020 2020 2020 2073 6f75 7263 653a 2073         source: s
+00041320: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00041330: 2020 2077 6972 656c 6573 735f 636c 6f75     wireless_clou
+00041340: 645f 636f 6e6e 6563 746f 725f 6964 3a20  d_connector_id: 
+00041350: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00041360: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00041370: 6265 6769 6e5f 7469 6d65 203d 2062 6567  begin_time = beg
+00041380: 696e 5f74 696d 650a 2020 2020 2020 2020  in_time.        
+00041390: 7365 6c66 2e64 6573 7469 6e61 7469 6f6e  self.destination
+000413a0: 203d 2064 6573 7469 6e61 7469 6f6e 0a20   = destination. 
+000413b0: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
+000413c0: 7469 6d65 203d 2065 6e64 5f74 696d 650a  time = end_time.
+000413d0: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+000413e0: 696f 6e5f 6e6f 203d 2072 6567 696f 6e5f  ion_no = region_
+000413f0: 6e6f 0a20 2020 2020 2020 2073 656c 662e  no.        self.
+00041400: 7265 736f 7572 6365 5f75 6964 203d 2072  resource_uid = r
+00041410: 6573 6f75 7263 655f 7569 640a 2020 2020  esource_uid.    
+00041420: 2020 2020 7365 6c66 2e73 6f75 7263 6520      self.source 
+00041430: 3d20 736f 7572 6365 0a20 2020 2020 2020  = source.       
+00041440: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
+00041450: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
+00041460: 6420 3d20 7769 7265 6c65 7373 5f63 6c6f  d = wireless_clo
+00041470: 7564 5f63 6f6e 6e65 6374 6f72 5f69 640a  ud_connector_id.
+00041480: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00041490: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000414a0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000414b0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000414c0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000414d0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+000414e0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000414f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00041500: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00041510: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00041520: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00041530: 2020 2069 6620 7365 6c66 2e62 6567 696e     if self.begin
+00041540: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
+00041550: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00041560: 6573 756c 745b 2742 6567 696e 5469 6d65  esult['BeginTime
+00041570: 275d 203d 2073 656c 662e 6265 6769 6e5f  '] = self.begin_
+00041580: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
+00041590: 7365 6c66 2e64 6573 7469 6e61 7469 6f6e  self.destination
+000415a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000415b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000415c0: 5b27 4465 7374 696e 6174 696f 6e27 5d20  ['Destination'] 
+000415d0: 3d20 7365 6c66 2e64 6573 7469 6e61 7469  = self.destinati
+000415e0: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
+000415f0: 6c66 2e65 6e64 5f74 696d 6520 6973 206e  lf.end_time is n
+00041600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00041610: 2020 2020 2072 6573 756c 745b 2745 6e64       result['End
+00041620: 5469 6d65 275d 203d 2073 656c 662e 656e  Time'] = self.en
+00041630: 645f 7469 6d65 0a20 2020 2020 2020 2069  d_time.        i
+00041640: 6620 7365 6c66 2e72 6567 696f 6e5f 6e6f  f self.region_no
+00041650: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00041660: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00041670: 5b27 5265 6769 6f6e 4e6f 275d 203d 2073  ['RegionNo'] = s
+00041680: 656c 662e 7265 6769 6f6e 5f6e 6f0a 2020  elf.region_no.  
+00041690: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+000416a0: 736f 7572 6365 5f75 6964 2069 7320 6e6f  source_uid is no
+000416b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000416c0: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
+000416d0: 7572 6365 5569 6427 5d20 3d20 7365 6c66  urceUid'] = self
+000416e0: 2e72 6573 6f75 7263 655f 7569 640a 2020  .resource_uid.  
+000416f0: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
+00041700: 7572 6365 2069 7320 6e6f 7420 4e6f 6e65  urce is not None
+00041710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00041720: 7375 6c74 5b27 536f 7572 6365 275d 203d  sult['Source'] =
+00041730: 2073 656c 662e 736f 7572 6365 0a20 2020   self.source.   
+00041740: 2020 2020 2069 6620 7365 6c66 2e77 6972       if self.wir
+00041750: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
+00041760: 6563 746f 725f 6964 2069 7320 6e6f 7420  ector_id is not 
+00041770: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00041780: 2020 7265 7375 6c74 5b27 5769 7265 6c65    result['Wirele
+00041790: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+000417a0: 4964 275d 203d 2073 656c 662e 7769 7265  Id'] = self.wire
+000417b0: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
+000417c0: 6374 6f72 5f69 640a 2020 2020 2020 2020  ctor_id.        
+000417d0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+000417e0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+000417f0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00041800: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00041810: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00041820: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00041830: 2742 6567 696e 5469 6d65 2729 2069 7320  'BeginTime') is 
+00041840: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00041850: 2020 2020 2020 7365 6c66 2e62 6567 696e        self.begin
+00041860: 5f74 696d 6520 3d20 6d2e 6765 7428 2742  _time = m.get('B
+00041870: 6567 696e 5469 6d65 2729 0a20 2020 2020  eginTime').     
+00041880: 2020 2069 6620 6d2e 6765 7428 2744 6573     if m.get('Des
+00041890: 7469 6e61 7469 6f6e 2729 2069 7320 6e6f  tination') is no
+000418a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000418b0: 2020 2020 7365 6c66 2e64 6573 7469 6e61      self.destina
+000418c0: 7469 6f6e 203d 206d 2e67 6574 2827 4465  tion = m.get('De
+000418d0: 7374 696e 6174 696f 6e27 290a 2020 2020  stination').    
+000418e0: 2020 2020 6966 206d 2e67 6574 2827 456e      if m.get('En
+000418f0: 6454 696d 6527 2920 6973 206e 6f74 204e  dTime') is not N
+00041900: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00041910: 2073 656c 662e 656e 645f 7469 6d65 203d   self.end_time =
+00041920: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
+00041930: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00041940: 6574 2827 5265 6769 6f6e 4e6f 2729 2069  et('RegionNo') i
+00041950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00041960: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+00041970: 696f 6e5f 6e6f 203d 206d 2e67 6574 2827  ion_no = m.get('
+00041980: 5265 6769 6f6e 4e6f 2729 0a20 2020 2020  RegionNo').     
+00041990: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
+000419a0: 6f75 7263 6555 6964 2729 2069 7320 6e6f  ourceUid') is no
+000419b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000419c0: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+000419d0: 655f 7569 6420 3d20 6d2e 6765 7428 2752  e_uid = m.get('R
+000419e0: 6573 6f75 7263 6555 6964 2729 0a20 2020  esourceUid').   
+000419f0: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
+00041a00: 6f75 7263 6527 2920 6973 206e 6f74 204e  ource') is not N
+00041a10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00041a20: 2073 656c 662e 736f 7572 6365 203d 206d   self.source = m
+00041a30: 2e67 6574 2827 536f 7572 6365 2729 0a20  .get('Source'). 
+00041a40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00041a50: 2757 6972 656c 6573 7343 6c6f 7564 436f  'WirelessCloudCo
+00041a60: 6e6e 6563 746f 7249 6427 2920 6973 206e  nnectorId') is n
+00041a70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00041a80: 2020 2020 2073 656c 662e 7769 7265 6c65       self.wirele
+00041a90: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
+00041aa0: 6f72 5f69 6420 3d20 6d2e 6765 7428 2757  or_id = m.get('W
+00041ab0: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+00041ac0: 6563 746f 7249 6427 290a 2020 2020 2020  ectorId').      
+00041ad0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00041ae0: 636c 6173 7320 5375 626d 6974 4469 6167  class SubmitDiag
+00041af0: 6e6f 7365 5461 736b 466f 7253 696e 676c  noseTaskForSingl
+00041b00: 6543 6172 6452 6573 706f 6e73 6542 6f64  eCardResponseBod
+00041b10: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+00041b20: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00041b30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00041b40: 2020 2020 2064 6961 676e 6f73 655f 7461       diagnose_ta
+00041b50: 736b 5f69 643a 2073 7472 203d 204e 6f6e  sk_id: str = Non
+00041b60: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
+00041b70: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+00041b80: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00041b90: 2020 7365 6c66 2e64 6961 676e 6f73 655f    self.diagnose_
+00041ba0: 7461 736b 5f69 6420 3d20 6469 6167 6e6f  task_id = diagno
+00041bb0: 7365 5f74 6173 6b5f 6964 0a20 2020 2020  se_task_id.     
+00041bc0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00041bd0: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+00041be0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00041bf0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00041c00: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00041c10: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00041c20: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00041c30: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00041c40: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00041c50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00041c60: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00041c70: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00041c80: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00041c90: 2020 2069 6620 7365 6c66 2e64 6961 676e     if self.diagn
+00041ca0: 6f73 655f 7461 736b 5f69 6420 6973 206e  ose_task_id is n
+00041cb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00041cc0: 2020 2020 2072 6573 756c 745b 2744 6961       result['Dia
+00041cd0: 676e 6f73 6554 6173 6b49 6427 5d20 3d20  gnoseTaskId'] = 
+00041ce0: 7365 6c66 2e64 6961 676e 6f73 655f 7461  self.diagnose_ta
+00041cf0: 736b 5f69 640a 2020 2020 2020 2020 6966  sk_id.        if
+00041d00: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00041d10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00041d20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00041d30: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+00041d40: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+00041d50: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00041d60: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00041d70: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00041d80: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00041d90: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00041da0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00041db0: 6620 6d2e 6765 7428 2744 6961 676e 6f73  f m.get('Diagnos
+00041dc0: 6554 6173 6b49 6427 2920 6973 206e 6f74  eTaskId') is not
+00041dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00041de0: 2020 2073 656c 662e 6469 6167 6e6f 7365     self.diagnose
+00041df0: 5f74 6173 6b5f 6964 203d 206d 2e67 6574  _task_id = m.get
+00041e00: 2827 4469 6167 6e6f 7365 5461 736b 4964  ('DiagnoseTaskId
+00041e10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00041e20: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00041e30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00041e40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00041e50: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+00041e60: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+00041e70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00041e80: 6c66 0a0a 0a63 6c61 7373 2053 7562 6d69  lf...class Submi
+00041e90: 7444 6961 676e 6f73 6554 6173 6b46 6f72  tDiagnoseTaskFor
+00041ea0: 5369 6e67 6c65 4361 7264 5265 7370 6f6e  SingleCardRespon
+00041eb0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00041ec0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00041ed0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00041ee0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+00041ef0: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00041f00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00041f10: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+00041f20: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+00041f30: 6f64 793a 2053 7562 6d69 7444 6961 676e  ody: SubmitDiagn
+00041f40: 6f73 6554 6173 6b46 6f72 5369 6e67 6c65  oseTaskForSingle
+00041f50: 4361 7264 5265 7370 6f6e 7365 426f 6479  CardResponseBody
+00041f60: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00041f70: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00041f80: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+00041f90: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00041fa0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+00041fb0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+00041fc0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+00041fd0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00041fe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00041ff0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00042000: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+00042010: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+00042020: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00042030: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00042040: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+00042050: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+00042060: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00042070: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00042080: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+00042090: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000420a0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+000420b0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+000420c0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+000420d0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000420e0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000420f0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+00042100: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00042110: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042120: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00042130: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00042140: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+00042150: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+00042160: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+00042170: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00042180: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+00042190: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+000421a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000421b0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+000421c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000421d0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+000421e0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+000421f0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+00042200: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00042210: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+00042220: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00042230: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+00042240: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+00042250: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00042260: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00042270: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00042280: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00042290: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000422a0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000422b0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000422c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000422d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000422e0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+000422f0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+00042300: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+00042310: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
 00042320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00042330: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00042340: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-00042350: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00042360: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-00042370: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00042380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00042390: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-000423a0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000423b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000423c0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-000423d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000423e0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-000423f0: 2053 7769 7463 6857 6972 656c 6573 7343   SwitchWirelessC
-00042400: 6c6f 7564 436f 6e6e 6563 746f 7254 6f42  loudConnectorToB
-00042410: 7573 696e 6573 7352 6573 706f 6e73 6542  usinessResponseB
-00042420: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
-00042430: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-00042440: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00042450: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-00042460: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00042470: 0a0a 0a63 6c61 7373 2055 6e6c 6f63 6b43  ...class UnlockC
-00042480: 6172 6473 5265 7175 6573 7428 5465 614d  ardsRequest(TeaM
-00042490: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000424a0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000424b0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-000424c0: 6c69 656e 745f 746f 6b65 6e3a 2073 7472  lient_token: str
-000424d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000424e0: 2064 7279 5f72 756e 3a20 626f 6f6c 203d   dry_run: bool =
-000424f0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-00042500: 6363 6964 733a 204c 6973 745b 7374 725d  ccids: List[str]
-00042510: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00042520: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
-00042530: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00042540: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00042550: 6e74 5f74 6f6b 656e 203d 2063 6c69 656e  nt_token = clien
-00042560: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-00042570: 7365 6c66 2e64 7279 5f72 756e 203d 2064  self.dry_run = d
-00042580: 7279 5f72 756e 0a20 2020 2020 2020 2073  ry_run.        s
-00042590: 656c 662e 6963 6369 6473 203d 2069 6363  elf.iccids = icc
-000425a0: 6964 730a 2020 2020 2020 2020 7365 6c66  ids.        self
-000425b0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
-000425c0: 696f 6e5f 6964 0a0a 2020 2020 6465 6620  ion_id..    def 
-000425d0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000425e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000425f0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00042600: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00042610: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00042620: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00042630: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00042640: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00042650: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00042660: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00042670: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00042680: 662e 636c 6965 6e74 5f74 6f6b 656e 2069  f.client_token i
-00042690: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000426a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000426b0: 436c 6965 6e74 546f 6b65 6e27 5d20 3d20  ClientToken'] = 
-000426c0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-000426d0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-000426e0: 662e 6472 795f 7275 6e20 6973 206e 6f74  f.dry_run is not
-000426f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00042700: 2020 2072 6573 756c 745b 2744 7279 5275     result['DryRu
-00042710: 6e27 5d20 3d20 7365 6c66 2e64 7279 5f72  n'] = self.dry_r
-00042720: 756e 0a20 2020 2020 2020 2069 6620 7365  un.        if se
-00042730: 6c66 2e69 6363 6964 7320 6973 206e 6f74  lf.iccids is not
-00042740: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00042750: 2020 2072 6573 756c 745b 2749 6363 6964     result['Iccid
-00042760: 7327 5d20 3d20 7365 6c66 2e69 6363 6964  s'] = self.iccid
-00042770: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-00042780: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
-00042790: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000427a0: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
-000427b0: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
-000427c0: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
-000427d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000427e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000427f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00042800: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00042810: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00042820: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00042830: 2827 436c 6965 6e74 546f 6b65 6e27 2920  ('ClientToken') 
-00042840: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00042850: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00042860: 6965 6e74 5f74 6f6b 656e 203d 206d 2e67  ient_token = m.g
-00042870: 6574 2827 436c 6965 6e74 546f 6b65 6e27  et('ClientToken'
-00042880: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00042890: 6574 2827 4472 7952 756e 2729 2069 7320  et('DryRun') is 
-000428a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000428b0: 2020 2020 2020 7365 6c66 2e64 7279 5f72        self.dry_r
-000428c0: 756e 203d 206d 2e67 6574 2827 4472 7952  un = m.get('DryR
-000428d0: 756e 2729 0a20 2020 2020 2020 2069 6620  un').        if 
-000428e0: 6d2e 6765 7428 2749 6363 6964 7327 2920  m.get('Iccids') 
-000428f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00042900: 2020 2020 2020 2020 2073 656c 662e 6963           self.ic
-00042910: 6369 6473 203d 206d 2e67 6574 2827 4963  cids = m.get('Ic
-00042920: 6369 6473 2729 0a20 2020 2020 2020 2069  cids').        i
-00042930: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
-00042940: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00042950: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00042960: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
-00042970: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
-00042980: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00042990: 656c 660a 0a0a 636c 6173 7320 556e 6c6f  elf...class Unlo
-000429a0: 636b 4361 7264 7352 6573 706f 6e73 6542  ckCardsResponseB
-000429b0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-000429c0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000429d0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000429e0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-000429f0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00042a00: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00042a10: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00042a20: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
-00042a30: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00042a40: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00042a50: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00042a60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00042a70: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-00042a80: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00042a90: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00042aa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042ab0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00042ac0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00042ad0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00042ae0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00042af0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00042b00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00042b10: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
-00042b20: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
-00042b30: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00042b40: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00042b50: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00042b60: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00042b70: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00042b80: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00042b90: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-00042ba0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00042bb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00042bc0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00042bd0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00042be0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00042bf0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00042c00: 6e6c 6f63 6b43 6172 6473 5265 7370 6f6e  nlockCardsRespon
-00042c10: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00042c20: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00042c30: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00042c40: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-00042c50: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-00042c60: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00042c70: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-00042c80: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-00042c90: 6f64 793a 2055 6e6c 6f63 6b43 6172 6473  ody: UnlockCards
-00042ca0: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
-00042cb0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00042cc0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00042cd0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-00042ce0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00042cf0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00042d00: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-00042d10: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-00042d20: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00042d30: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00042d40: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-00042d50: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-00042d60: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-00042d70: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-00042d80: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-00042d90: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-00042da0: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-00042db0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-00042dc0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-00042dd0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-00042de0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00042df0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-00042e00: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-00042e10: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00042e20: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00042e30: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00042e40: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00042e50: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00042e60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00042e70: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00042e80: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00042e90: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00042ea0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-00042eb0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00042ec0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00042ed0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-00042ee0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-00042ef0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00042f00: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00042f10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00042f20: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00042f30: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00042f40: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00042f50: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00042f60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00042f70: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00042f80: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-00042f90: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-00042fa0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00042fb0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00042fc0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-00042fd0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-00042fe0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00042ff0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00043000: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00043010: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00043020: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00043030: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00043040: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00043050: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00043060: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00043070: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00043080: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00043090: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-000430a0: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-000430b0: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000430c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000430d0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000430e0: 656c 203d 2055 6e6c 6f63 6b43 6172 6473  el = UnlockCards
+00042330: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+00042340: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+00042350: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+00042360: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+00042370: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00042380: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00042390: 5f6d 6f64 656c 203d 2053 7562 6d69 7444  _model = SubmitD
+000423a0: 6961 676e 6f73 6554 6173 6b46 6f72 5369  iagnoseTaskForSi
+000423b0: 6e67 6c65 4361 7264 5265 7370 6f6e 7365  ngleCardResponse
+000423c0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+000423d0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+000423e0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+000423f0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+00042400: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00042410: 660a 0a0a 636c 6173 7320 5377 6974 6368  f...class Switch
+00042420: 5769 7265 6c65 7373 436c 6f75 6443 6f6e  WirelessCloudCon
+00042430: 6e65 6374 6f72 546f 4275 7369 6e65 7373  nectorToBusiness
+00042440: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00042450: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00042460: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00042470: 662c 0a20 2020 2020 2020 2063 6c69 656e  f,.        clien
+00042480: 745f 746f 6b65 6e3a 2073 7472 203d 204e  t_token: str = N
+00042490: 6f6e 652c 0a20 2020 2020 2020 2064 7279  one,.        dry
+000424a0: 5f72 756e 3a20 626f 6f6c 203d 204e 6f6e  _run: bool = Non
+000424b0: 652c 0a20 2020 2020 2020 2077 6972 656c  e,.        wirel
+000424c0: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
+000424d0: 746f 725f 6964 3a20 7374 7220 3d20 4e6f  tor_id: str = No
+000424e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000424f0: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+00042500: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
+00042510: 6b65 6e0a 2020 2020 2020 2020 7365 6c66  ken.        self
+00042520: 2e64 7279 5f72 756e 203d 2064 7279 5f72  .dry_run = dry_r
+00042530: 756e 0a20 2020 2020 2020 2073 656c 662e  un.        self.
+00042540: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+00042550: 6f6e 6e65 6374 6f72 5f69 6420 3d20 7769  onnector_id = wi
+00042560: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
+00042570: 6e65 6374 6f72 5f69 640a 0a20 2020 2064  nector_id..    d
+00042580: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00042590: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000425a0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000425b0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000425c0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000425d0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000425e0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000425f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00042600: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00042610: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00042620: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00042630: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00042640: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00042650: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00042660: 745b 2743 6c69 656e 7454 6f6b 656e 275d  t['ClientToken']
+00042670: 203d 2073 656c 662e 636c 6965 6e74 5f74   = self.client_t
+00042680: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+00042690: 7365 6c66 2e64 7279 5f72 756e 2069 7320  self.dry_run is 
+000426a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000426b0: 2020 2020 2020 7265 7375 6c74 5b27 4472        result['Dr
+000426c0: 7952 756e 275d 203d 2073 656c 662e 6472  yRun'] = self.dr
+000426d0: 795f 7275 6e0a 2020 2020 2020 2020 6966  y_run.        if
+000426e0: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
+000426f0: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
+00042700: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00042710: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00042720: 745b 2757 6972 656c 6573 7343 6c6f 7564  t['WirelessCloud
+00042730: 436f 6e6e 6563 746f 7249 6427 5d20 3d20  ConnectorId'] = 
+00042740: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
+00042750: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+00042760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00042770: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00042780: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00042790: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000427a0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000427b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000427c0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+000427d0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+000427e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000427f0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+00042800: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
+00042810: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
+00042820: 2020 6966 206d 2e67 6574 2827 4472 7952    if m.get('DryR
+00042830: 756e 2729 2069 7320 6e6f 7420 4e6f 6e65  un') is not None
+00042840: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00042850: 6c66 2e64 7279 5f72 756e 203d 206d 2e67  lf.dry_run = m.g
+00042860: 6574 2827 4472 7952 756e 2729 0a20 2020  et('DryRun').   
+00042870: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+00042880: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+00042890: 6563 746f 7249 6427 2920 6973 206e 6f74  ectorId') is not
+000428a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000428b0: 2020 2073 656c 662e 7769 7265 6c65 7373     self.wireless
+000428c0: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
+000428d0: 5f69 6420 3d20 6d2e 6765 7428 2757 6972  _id = m.get('Wir
+000428e0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+000428f0: 746f 7249 6427 290a 2020 2020 2020 2020  torId').        
+00042900: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00042910: 6173 7320 5377 6974 6368 5769 7265 6c65  ass SwitchWirele
+00042920: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+00042930: 546f 4275 7369 6e65 7373 5265 7370 6f6e  ToBusinessRespon
+00042940: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+00042950: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00042960: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00042970: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
+00042980: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
+00042990: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000429a0: 2023 2049 6420 6f66 2074 6865 2072 6571   # Id of the req
+000429b0: 7565 7374 0a20 2020 2020 2020 2073 656c  uest.        sel
+000429c0: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+000429d0: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
+000429e0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000429f0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00042a00: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00042a10: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00042a20: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00042a30: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00042a40: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00042a50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00042a60: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00042a70: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00042a80: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00042a90: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00042aa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00042ab0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00042ac0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00042ad0: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00042ae0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00042af0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00042b00: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00042b10: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00042b20: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00042b30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00042b40: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+00042b50: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00042b60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00042b70: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+00042b80: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00042b90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00042ba0: 2073 656c 660a 0a0a 636c 6173 7320 5377   self...class Sw
+00042bb0: 6974 6368 5769 7265 6c65 7373 436c 6f75  itchWirelessClou
+00042bc0: 6443 6f6e 6e65 6374 6f72 546f 4275 7369  dConnectorToBusi
+00042bd0: 6e65 7373 5265 7370 6f6e 7365 2854 6561  nessResponse(Tea
+00042be0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00042bf0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00042c00: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00042c10: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+00042c20: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+00042c30: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+00042c40: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+00042c50: 0a20 2020 2020 2020 2062 6f64 793a 2053  .        body: S
+00042c60: 7769 7463 6857 6972 656c 6573 7343 6c6f  witchWirelessClo
+00042c70: 7564 436f 6e6e 6563 746f 7254 6f42 7573  udConnectorToBus
+00042c80: 696e 6573 7352 6573 706f 6e73 6542 6f64  inessResponseBod
+00042c90: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+00042ca0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+00042cb0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+00042cc0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00042cd0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+00042ce0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+00042cf0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+00042d00: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00042d10: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00042d20: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+00042d30: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+00042d40: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+00042d50: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00042d60: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00042d70: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00042d80: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+00042d90: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00042da0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00042db0: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+00042dc0: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+00042dd0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+00042de0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+00042df0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+00042e00: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00042e10: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00042e20: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00042e30: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00042e40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00042e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00042e60: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00042e70: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00042e80: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00042e90: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00042ea0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00042eb0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+00042ec0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+00042ed0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00042ee0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+00042ef0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00042f00: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+00042f10: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+00042f20: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+00042f30: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00042f40: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00042f50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00042f60: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00042f70: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00042f80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00042f90: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00042fa0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00042fb0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00042fc0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00042fd0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00042fe0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+00042ff0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00043000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00043010: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+00043020: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+00043030: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+00043040: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+00043050: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00043060: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00043070: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+00043080: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+00043090: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+000430a0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+000430b0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+000430c0: 705f 6d6f 6465 6c20 3d20 5377 6974 6368  p_model = Switch
+000430d0: 5769 7265 6c65 7373 436c 6f75 6443 6f6e  WirelessCloudCon
+000430e0: 6e65 6374 6f72 546f 4275 7369 6e65 7373  nectorToBusiness
 000430f0: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
 00043100: 2020 2020 2020 2020 2020 2073 656c 662e             self.
 00043110: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
 00043120: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
 00043130: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
 00043140: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00043150: 7320 5570 6461 7465 4175 7468 6f72 697a  s UpdateAuthoriz
-00043160: 6174 696f 6e52 756c 6552 6571 7565 7374  ationRuleRequest
-00043170: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00043180: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-00043190: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000431a0: 2020 2020 6175 7468 6f72 697a 6174 696f      authorizatio
-000431b0: 6e5f 7275 6c65 5f69 643a 2073 7472 203d  n_rule_id: str =
-000431c0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-000431d0: 6c69 656e 745f 746f 6b65 6e3a 2073 7472  lient_token: str
-000431e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000431f0: 2064 6573 6372 6970 7469 6f6e 3a20 7374   description: st
-00043200: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00043210: 2020 6465 7374 696e 6174 696f 6e3a 2073    destination: s
-00043220: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00043230: 2020 2064 6573 7469 6e61 7469 6f6e 5f70     destination_p
-00043240: 6f72 743a 2073 7472 203d 204e 6f6e 652c  ort: str = None,
-00043250: 0a20 2020 2020 2020 2064 7279 5f72 756e  .        dry_run
-00043260: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
-00043270: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
-00043280: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00043290: 2070 6f6c 6963 793a 2073 7472 203d 204e   policy: str = N
-000432a0: 6f6e 652c 0a20 2020 2020 2020 2070 726f  one,.        pro
-000432b0: 746f 636f 6c3a 2073 7472 203d 204e 6f6e  tocol: str = Non
-000432c0: 652c 0a20 2020 2020 2020 2073 6f75 7263  e,.        sourc
-000432d0: 655f 6369 6472 3a20 7374 7220 3d20 4e6f  e_cidr: str = No
-000432e0: 6e65 2c0a 2020 2020 2020 2020 7769 7265  ne,.        wire
-000432f0: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-00043300: 6374 6f72 5f69 643a 2073 7472 203d 204e  ctor_id: str = N
-00043310: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00043320: 2020 2020 7365 6c66 2e61 7574 686f 7269      self.authori
-00043330: 7a61 7469 6f6e 5f72 756c 655f 6964 203d  zation_rule_id =
-00043340: 2061 7574 686f 7269 7a61 7469 6f6e 5f72   authorization_r
-00043350: 756c 655f 6964 0a20 2020 2020 2020 2073  ule_id.        s
-00043360: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-00043370: 203d 2063 6c69 656e 745f 746f 6b65 6e0a   = client_token.
-00043380: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-00043390: 6372 6970 7469 6f6e 203d 2064 6573 6372  cription = descr
-000433a0: 6970 7469 6f6e 0a20 2020 2020 2020 2073  iption.        s
-000433b0: 656c 662e 6465 7374 696e 6174 696f 6e20  elf.destination 
-000433c0: 3d20 6465 7374 696e 6174 696f 6e0a 2020  = destination.  
-000433d0: 2020 2020 2020 7365 6c66 2e64 6573 7469        self.desti
-000433e0: 6e61 7469 6f6e 5f70 6f72 7420 3d20 6465  nation_port = de
-000433f0: 7374 696e 6174 696f 6e5f 706f 7274 0a20  stination_port. 
-00043400: 2020 2020 2020 2073 656c 662e 6472 795f         self.dry_
-00043410: 7275 6e20 3d20 6472 795f 7275 6e0a 2020  run = dry_run.  
-00043420: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00043430: 3d20 6e61 6d65 0a20 2020 2020 2020 2073  = name.        s
-00043440: 656c 662e 706f 6c69 6379 203d 2070 6f6c  elf.policy = pol
-00043450: 6963 790a 2020 2020 2020 2020 7365 6c66  icy.        self
-00043460: 2e70 726f 746f 636f 6c20 3d20 7072 6f74  .protocol = prot
-00043470: 6f63 6f6c 0a20 2020 2020 2020 2073 656c  ocol.        sel
-00043480: 662e 736f 7572 6365 5f63 6964 7220 3d20  f.source_cidr = 
-00043490: 736f 7572 6365 5f63 6964 720a 2020 2020  source_cidr.    
-000434a0: 2020 2020 7365 6c66 2e77 6972 656c 6573      self.wireles
-000434b0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-000434c0: 725f 6964 203d 2077 6972 656c 6573 735f  r_id = wireless_
-000434d0: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-000434e0: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
-000434f0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00043500: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00043510: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00043520: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00043530: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00043540: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00043550: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00043560: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00043570: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00043580: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00043590: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
-000435a0: 7468 6f72 697a 6174 696f 6e5f 7275 6c65  thorization_rule
-000435b0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000435c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000435d0: 756c 745b 2741 7574 686f 7269 7a61 7469  ult['Authorizati
-000435e0: 6f6e 5275 6c65 4964 275d 203d 2073 656c  onRuleId'] = sel
-000435f0: 662e 6175 7468 6f72 697a 6174 696f 6e5f  f.authorization_
-00043600: 7275 6c65 5f69 640a 2020 2020 2020 2020  rule_id.        
-00043610: 6966 2073 656c 662e 636c 6965 6e74 5f74  if self.client_t
-00043620: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
-00043630: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00043640: 7375 6c74 5b27 436c 6965 6e74 546f 6b65  sult['ClientToke
-00043650: 6e27 5d20 3d20 7365 6c66 2e63 6c69 656e  n'] = self.clien
-00043660: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-00043670: 6966 2073 656c 662e 6465 7363 7269 7074  if self.descript
-00043680: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00043690: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000436a0: 756c 745b 2744 6573 6372 6970 7469 6f6e  ult['Description
-000436b0: 275d 203d 2073 656c 662e 6465 7363 7269  '] = self.descri
-000436c0: 7074 696f 6e0a 2020 2020 2020 2020 6966  ption.        if
-000436d0: 2073 656c 662e 6465 7374 696e 6174 696f   self.destinatio
-000436e0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-000436f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00043700: 745b 2744 6573 7469 6e61 7469 6f6e 275d  t['Destination']
-00043710: 203d 2073 656c 662e 6465 7374 696e 6174   = self.destinat
-00043720: 696f 6e0a 2020 2020 2020 2020 6966 2073  ion.        if s
-00043730: 656c 662e 6465 7374 696e 6174 696f 6e5f  elf.destination_
-00043740: 706f 7274 2069 7320 6e6f 7420 4e6f 6e65  port is not None
-00043750: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00043760: 7375 6c74 5b27 4465 7374 696e 6174 696f  sult['Destinatio
-00043770: 6e50 6f72 7427 5d20 3d20 7365 6c66 2e64  nPort'] = self.d
-00043780: 6573 7469 6e61 7469 6f6e 5f70 6f72 740a  estination_port.
-00043790: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000437a0: 6472 795f 7275 6e20 6973 206e 6f74 204e  dry_run is not N
-000437b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000437c0: 2072 6573 756c 745b 2744 7279 5275 6e27   result['DryRun'
-000437d0: 5d20 3d20 7365 6c66 2e64 7279 5f72 756e  ] = self.dry_run
-000437e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000437f0: 2e6e 616d 6520 6973 206e 6f74 204e 6f6e  .name is not Non
-00043800: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00043810: 6573 756c 745b 274e 616d 6527 5d20 3d20  esult['Name'] = 
-00043820: 7365 6c66 2e6e 616d 650a 2020 2020 2020  self.name.      
-00043830: 2020 6966 2073 656c 662e 706f 6c69 6379    if self.policy
-00043840: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00043850: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00043860: 5b27 506f 6c69 6379 275d 203d 2073 656c  ['Policy'] = sel
-00043870: 662e 706f 6c69 6379 0a20 2020 2020 2020  f.policy.       
-00043880: 2069 6620 7365 6c66 2e70 726f 746f 636f   if self.protoco
-00043890: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-000438a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000438b0: 745b 2750 726f 746f 636f 6c27 5d20 3d20  t['Protocol'] = 
-000438c0: 7365 6c66 2e70 726f 746f 636f 6c0a 2020  self.protocol.  
-000438d0: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
-000438e0: 7572 6365 5f63 6964 7220 6973 206e 6f74  urce_cidr is not
-000438f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043900: 2020 2072 6573 756c 745b 2753 6f75 7263     result['Sourc
-00043910: 6543 6964 7227 5d20 3d20 7365 6c66 2e73  eCidr'] = self.s
-00043920: 6f75 7263 655f 6369 6472 0a20 2020 2020  ource_cidr.     
-00043930: 2020 2069 6620 7365 6c66 2e77 6972 656c     if self.wirel
-00043940: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-00043950: 746f 725f 6964 2069 7320 6e6f 7420 4e6f  tor_id is not No
-00043960: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00043970: 7265 7375 6c74 5b27 5769 7265 6c65 7373  result['Wireless
-00043980: 436c 6f75 6443 6f6e 6e65 6374 6f72 4964  CloudConnectorId
-00043990: 275d 203d 2073 656c 662e 7769 7265 6c65  '] = self.wirele
-000439a0: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-000439b0: 6f72 5f69 640a 2020 2020 2020 2020 7265  or_id.        re
-000439c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000439d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000439e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-000439f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00043a00: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00043a10: 2020 2020 2069 6620 6d2e 6765 7428 2741       if m.get('A
-00043a20: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
-00043a30: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00043a40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00043a50: 6c66 2e61 7574 686f 7269 7a61 7469 6f6e  lf.authorization
-00043a60: 5f72 756c 655f 6964 203d 206d 2e67 6574  _rule_id = m.get
-00043a70: 2827 4175 7468 6f72 697a 6174 696f 6e52  ('AuthorizationR
-00043a80: 756c 6549 6427 290a 2020 2020 2020 2020  uleId').        
-00043a90: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-00043aa0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
-00043ab0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00043ac0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-00043ad0: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
-00043ae0: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
-00043af0: 2020 6966 206d 2e67 6574 2827 4465 7363    if m.get('Desc
-00043b00: 7269 7074 696f 6e27 2920 6973 206e 6f74  ription') is not
-00043b10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043b20: 2020 2073 656c 662e 6465 7363 7269 7074     self.descript
-00043b30: 696f 6e20 3d20 6d2e 6765 7428 2744 6573  ion = m.get('Des
-00043b40: 6372 6970 7469 6f6e 2729 0a20 2020 2020  cription').     
-00043b50: 2020 2069 6620 6d2e 6765 7428 2744 6573     if m.get('Des
-00043b60: 7469 6e61 7469 6f6e 2729 2069 7320 6e6f  tination') is no
-00043b70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00043b80: 2020 2020 7365 6c66 2e64 6573 7469 6e61      self.destina
-00043b90: 7469 6f6e 203d 206d 2e67 6574 2827 4465  tion = m.get('De
-00043ba0: 7374 696e 6174 696f 6e27 290a 2020 2020  stination').    
-00043bb0: 2020 2020 6966 206d 2e67 6574 2827 4465      if m.get('De
-00043bc0: 7374 696e 6174 696f 6e50 6f72 7427 2920  stinationPort') 
-00043bd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00043be0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00043bf0: 7374 696e 6174 696f 6e5f 706f 7274 203d  stination_port =
-00043c00: 206d 2e67 6574 2827 4465 7374 696e 6174   m.get('Destinat
-00043c10: 696f 6e50 6f72 7427 290a 2020 2020 2020  ionPort').      
-00043c20: 2020 6966 206d 2e67 6574 2827 4472 7952    if m.get('DryR
-00043c30: 756e 2729 2069 7320 6e6f 7420 4e6f 6e65  un') is not None
-00043c40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00043c50: 6c66 2e64 7279 5f72 756e 203d 206d 2e67  lf.dry_run = m.g
-00043c60: 6574 2827 4472 7952 756e 2729 0a20 2020  et('DryRun').   
-00043c70: 2020 2020 2069 6620 6d2e 6765 7428 274e       if m.get('N
-00043c80: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00043c90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00043ca0: 656c 662e 6e61 6d65 203d 206d 2e67 6574  elf.name = m.get
-00043cb0: 2827 4e61 6d65 2729 0a20 2020 2020 2020  ('Name').       
-00043cc0: 2069 6620 6d2e 6765 7428 2750 6f6c 6963   if m.get('Polic
-00043cd0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-00043ce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00043cf0: 662e 706f 6c69 6379 203d 206d 2e67 6574  f.policy = m.get
-00043d00: 2827 506f 6c69 6379 2729 0a20 2020 2020  ('Policy').     
-00043d10: 2020 2069 6620 6d2e 6765 7428 2750 726f     if m.get('Pro
-00043d20: 746f 636f 6c27 2920 6973 206e 6f74 204e  tocol') is not N
-00043d30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00043d40: 2073 656c 662e 7072 6f74 6f63 6f6c 203d   self.protocol =
-00043d50: 206d 2e67 6574 2827 5072 6f74 6f63 6f6c   m.get('Protocol
-00043d60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00043d70: 6765 7428 2753 6f75 7263 6543 6964 7227  get('SourceCidr'
-00043d80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00043d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00043da0: 736f 7572 6365 5f63 6964 7220 3d20 6d2e  source_cidr = m.
-00043db0: 6765 7428 2753 6f75 7263 6543 6964 7227  get('SourceCidr'
-00043dc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00043dd0: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
-00043de0: 6443 6f6e 6e65 6374 6f72 4964 2729 2069  dConnectorId') i
-00043df0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00043e00: 2020 2020 2020 2020 7365 6c66 2e77 6972          self.wir
-00043e10: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
-00043e20: 6563 746f 725f 6964 203d 206d 2e67 6574  ector_id = m.get
-00043e30: 2827 5769 7265 6c65 7373 436c 6f75 6443  ('WirelessCloudC
-00043e40: 6f6e 6e65 6374 6f72 4964 2729 0a20 2020  onnectorId').   
-00043e50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00043e60: 0a0a 0a63 6c61 7373 2055 7064 6174 6541  ...class UpdateA
-00043e70: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
-00043e80: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-00043e90: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00043ea0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00043eb0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00043ec0: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
-00043ed0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00043ee0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-00043ef0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-00043f00: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-00043f10: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00043f20: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00043f30: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00043f40: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00043f50: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00043f60: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00043f70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00043f80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00043f90: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00043fa0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00043fb0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00043fc0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-00043fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00043fe0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-00043ff0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-00044000: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-00044010: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00044020: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00044030: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00044040: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00044050: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00044060: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00044070: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
-00044080: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00044090: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-000440a0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
-000440b0: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
-000440c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000440d0: 0a0a 636c 6173 7320 5570 6461 7465 4175  ..class UpdateAu
-000440e0: 7468 6f72 697a 6174 696f 6e52 756c 6552  thorizationRuleR
-000440f0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00044100: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00044110: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00044120: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-00044130: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-00044140: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00044150: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-00044160: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-00044170: 2020 2020 626f 6479 3a20 5570 6461 7465      body: Update
-00044180: 4175 7468 6f72 697a 6174 696f 6e52 756c  AuthorizationRul
-00044190: 6552 6573 706f 6e73 6542 6f64 7920 3d20  eResponseBody = 
-000441a0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000441b0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000441c0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-000441d0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000441e0: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-000441f0: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-00044200: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-00044210: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00044220: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00044230: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00044240: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00044250: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00044260: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00044270: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00044280: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-00044290: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-000442a0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-000442b0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000442c0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-000442d0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000442e0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000442f0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00044300: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00044310: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00044320: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00044330: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00044340: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00044350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00044360: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00044370: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00044380: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00044390: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-000443a0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-000443b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000443c0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-000443d0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000443e0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000443f0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-00044400: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00044410: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-00044420: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-00044430: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00044440: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00044450: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00044460: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00044470: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00044480: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00044490: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000444a0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000444b0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000444c0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000444d0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000444e0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000444f0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-00044500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00044510: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00044520: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00044530: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00044540: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00044550: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00044560: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00044570: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00044580: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00044590: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-000445a0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000445b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000445c0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000445d0: 6465 6c20 3d20 5570 6461 7465 4175 7468  del = UpdateAuth
-000445e0: 6f72 697a 6174 696f 6e52 756c 6552 6573  orizationRuleRes
-000445f0: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-00044600: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00044610: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-00044620: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-00044630: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00044640: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00044650: 7064 6174 6542 6174 6368 4f70 6572 6174  pdateBatchOperat
-00044660: 6543 6172 6473 5461 736b 5265 7175 6573  eCardsTaskReques
-00044670: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-00044680: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00044690: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000446a0: 2020 2020 2062 6174 6368 5f6f 7065 7261       batch_opera
-000446b0: 7465 5f63 6172 6473 5f74 6173 6b5f 6964  te_cards_task_id
-000446c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000446d0: 2020 2020 2020 636c 6965 6e74 5f74 6f6b        client_tok
-000446e0: 656e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  en: str = None,.
-000446f0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00044700: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
-00044710: 0a20 2020 2020 2020 2064 7279 5f72 756e  .        dry_run
-00044720: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
-00044730: 2020 2020 2020 2065 6666 6563 745f 7479         effect_ty
-00044740: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
-00044750: 2020 2020 2020 2020 6963 6369 6473 3a20          iccids: 
-00044760: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
-00044770: 2c0a 2020 2020 2020 2020 6963 6369 6473  ,.        iccids
-00044780: 5f6f 7373 5f66 696c 655f 7061 7468 3a20  _oss_file_path: 
-00044790: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000447a0: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
-000447b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f70  None,.        op
-000447c0: 6572 6174 655f 7479 7065 3a20 7374 7220  erate_type: str 
-000447d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000447e0: 7265 6769 6f6e 5f69 643a 2073 7472 203d  region_id: str =
-000447f0: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-00044800: 6872 6573 686f 6c64 3a20 696e 7420 3d20  hreshold: int = 
-00044810: 4e6f 6e65 2c0a 2020 2020 2020 2020 7769  None,.        wi
-00044820: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
-00044830: 6e65 6374 6f72 5f69 6473 3a20 4c69 7374  nector_ids: List
-00044840: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00044850: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00044860: 662e 6261 7463 685f 6f70 6572 6174 655f  f.batch_operate_
-00044870: 6361 7264 735f 7461 736b 5f69 6420 3d20  cards_task_id = 
-00044880: 6261 7463 685f 6f70 6572 6174 655f 6361  batch_operate_ca
-00044890: 7264 735f 7461 736b 5f69 640a 2020 2020  rds_task_id.    
-000448a0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-000448b0: 746f 6b65 6e20 3d20 636c 6965 6e74 5f74  token = client_t
-000448c0: 6f6b 656e 0a20 2020 2020 2020 2073 656c  oken.        sel
-000448d0: 662e 6465 7363 7269 7074 696f 6e20 3d20  f.description = 
-000448e0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
-000448f0: 2020 2020 7365 6c66 2e64 7279 5f72 756e      self.dry_run
-00044900: 203d 2064 7279 5f72 756e 0a20 2020 2020   = dry_run.     
-00044910: 2020 2073 656c 662e 6566 6665 6374 5f74     self.effect_t
-00044920: 7970 6520 3d20 6566 6665 6374 5f74 7970  ype = effect_typ
-00044930: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
-00044940: 6363 6964 7320 3d20 6963 6369 6473 0a20  ccids = iccids. 
-00044950: 2020 2020 2020 2073 656c 662e 6963 6369         self.icci
-00044960: 6473 5f6f 7373 5f66 696c 655f 7061 7468  ds_oss_file_path
-00044970: 203d 2069 6363 6964 735f 6f73 735f 6669   = iccids_oss_fi
-00044980: 6c65 5f70 6174 680a 2020 2020 2020 2020  le_path.        
-00044990: 7365 6c66 2e6e 616d 6520 3d20 6e61 6d65  self.name = name
-000449a0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-000449b0: 6572 6174 655f 7479 7065 203d 206f 7065  erate_type = ope
-000449c0: 7261 7465 5f74 7970 650a 2020 2020 2020  rate_type.      
-000449d0: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-000449e0: 203d 2072 6567 696f 6e5f 6964 0a20 2020   = region_id.   
-000449f0: 2020 2020 2073 656c 662e 7468 7265 7368       self.thresh
-00044a00: 6f6c 6420 3d20 7468 7265 7368 6f6c 640a  old = threshold.
-00044a10: 2020 2020 2020 2020 7365 6c66 2e77 6972          self.wir
-00044a20: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
-00044a30: 6563 746f 725f 6964 7320 3d20 7769 7265  ector_ids = wire
-00044a40: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-00044a50: 6374 6f72 5f69 6473 0a0a 2020 2020 6465  ctor_ids..    de
-00044a60: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00044a70: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00044a80: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00044a90: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00044aa0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00044ab0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00044ac0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00044ad0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00044ae0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00044af0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00044b00: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00044b10: 656c 662e 6261 7463 685f 6f70 6572 6174  elf.batch_operat
-00044b20: 655f 6361 7264 735f 7461 736b 5f69 6420  e_cards_task_id 
-00044b30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00044b40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00044b50: 2742 6174 6368 4f70 6572 6174 6543 6172  'BatchOperateCar
-00044b60: 6473 5461 736b 4964 275d 203d 2073 656c  dsTaskId'] = sel
-00044b70: 662e 6261 7463 685f 6f70 6572 6174 655f  f.batch_operate_
-00044b80: 6361 7264 735f 7461 736b 5f69 640a 2020  cards_task_id.  
-00044b90: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-00044ba0: 6965 6e74 5f74 6f6b 656e 2069 7320 6e6f  ient_token is no
-00044bb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00044bc0: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
-00044bd0: 6e74 546f 6b65 6e27 5d20 3d20 7365 6c66  ntToken'] = self
-00044be0: 2e63 6c69 656e 745f 746f 6b65 6e0a 2020  .client_token.  
-00044bf0: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
-00044c00: 7363 7269 7074 696f 6e20 6973 206e 6f74  scription is not
-00044c10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00044c20: 2020 2072 6573 756c 745b 2744 6573 6372     result['Descr
-00044c30: 6970 7469 6f6e 275d 203d 2073 656c 662e  iption'] = self.
-00044c40: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
-00044c50: 2020 2020 6966 2073 656c 662e 6472 795f      if self.dry_
-00044c60: 7275 6e20 6973 206e 6f74 204e 6f6e 653a  run is not None:
-00044c70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00044c80: 756c 745b 2744 7279 5275 6e27 5d20 3d20  ult['DryRun'] = 
-00044c90: 7365 6c66 2e64 7279 5f72 756e 0a20 2020  self.dry_run.   
-00044ca0: 2020 2020 2069 6620 7365 6c66 2e65 6666       if self.eff
-00044cb0: 6563 745f 7479 7065 2069 7320 6e6f 7420  ect_type is not 
-00044cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00044cd0: 2020 7265 7375 6c74 5b27 4566 6665 6374    result['Effect
-00044ce0: 5479 7065 275d 203d 2073 656c 662e 6566  Type'] = self.ef
-00044cf0: 6665 6374 5f74 7970 650a 2020 2020 2020  fect_type.      
-00044d00: 2020 6966 2073 656c 662e 6963 6369 6473    if self.iccids
-00044d10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00044d20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00044d30: 5b27 4963 6369 6473 275d 203d 2073 656c  ['Iccids'] = sel
-00044d40: 662e 6963 6369 6473 0a20 2020 2020 2020  f.iccids.       
-00044d50: 2069 6620 7365 6c66 2e69 6363 6964 735f   if self.iccids_
-00044d60: 6f73 735f 6669 6c65 5f70 6174 6820 6973  oss_file_path is
-00044d70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00044d80: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
-00044d90: 6363 6964 734f 7373 4669 6c65 5061 7468  ccidsOssFilePath
-00044da0: 275d 203d 2073 656c 662e 6963 6369 6473  '] = self.iccids
-00044db0: 5f6f 7373 5f66 696c 655f 7061 7468 0a20  _oss_file_path. 
-00044dc0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00044dd0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00044de0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00044df0: 756c 745b 274e 616d 6527 5d20 3d20 7365  ult['Name'] = se
-00044e00: 6c66 2e6e 616d 650a 2020 2020 2020 2020  lf.name.        
-00044e10: 6966 2073 656c 662e 6f70 6572 6174 655f  if self.operate_
-00044e20: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-00044e30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00044e40: 7375 6c74 5b27 4f70 6572 6174 6554 7970  sult['OperateTyp
-00044e50: 6527 5d20 3d20 7365 6c66 2e6f 7065 7261  e'] = self.opera
-00044e60: 7465 5f74 7970 650a 2020 2020 2020 2020  te_type.        
-00044e70: 6966 2073 656c 662e 7265 6769 6f6e 5f69  if self.region_i
-00044e80: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00044e90: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00044ea0: 745b 2752 6567 696f 6e49 6427 5d20 3d20  t['RegionId'] = 
-00044eb0: 7365 6c66 2e72 6567 696f 6e5f 6964 0a20  self.region_id. 
-00044ec0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00044ed0: 6872 6573 686f 6c64 2069 7320 6e6f 7420  hreshold is not 
-00044ee0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00044ef0: 2020 7265 7375 6c74 5b27 5468 7265 7368    result['Thresh
-00044f00: 6f6c 6427 5d20 3d20 7365 6c66 2e74 6872  old'] = self.thr
-00044f10: 6573 686f 6c64 0a20 2020 2020 2020 2069  eshold.        i
-00044f20: 6620 7365 6c66 2e77 6972 656c 6573 735f  f self.wireless_
-00044f30: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-00044f40: 6964 7320 6973 206e 6f74 204e 6f6e 653a  ids is not None:
-00044f50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00044f60: 756c 745b 2757 6972 656c 6573 7343 6c6f  ult['WirelessClo
-00044f70: 7564 436f 6e6e 6563 746f 7249 6473 275d  udConnectorIds']
-00044f80: 203d 2073 656c 662e 7769 7265 6c65 7373   = self.wireless
-00044f90: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-00044fa0: 5f69 6473 0a20 2020 2020 2020 2072 6574  _ids.        ret
-00044fb0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00044fc0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00044fd0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00044fe0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00044ff0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00045000: 2020 2020 6966 206d 2e67 6574 2827 4261      if m.get('Ba
-00045010: 7463 684f 7065 7261 7465 4361 7264 7354  tchOperateCardsT
-00045020: 6173 6b49 6427 2920 6973 206e 6f74 204e  askId') is not N
-00045030: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00045040: 2073 656c 662e 6261 7463 685f 6f70 6572   self.batch_oper
-00045050: 6174 655f 6361 7264 735f 7461 736b 5f69  ate_cards_task_i
-00045060: 6420 3d20 6d2e 6765 7428 2742 6174 6368  d = m.get('Batch
-00045070: 4f70 6572 6174 6543 6172 6473 5461 736b  OperateCardsTask
-00045080: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00045090: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
-000450a0: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
-000450b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000450c0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
-000450d0: 3d20 6d2e 6765 7428 2743 6c69 656e 7454  = m.get('ClientT
-000450e0: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
-000450f0: 6620 6d2e 6765 7428 2744 6573 6372 6970  f m.get('Descrip
-00045100: 7469 6f6e 2729 2069 7320 6e6f 7420 4e6f  tion') is not No
-00045110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00045120: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00045130: 203d 206d 2e67 6574 2827 4465 7363 7269   = m.get('Descri
-00045140: 7074 696f 6e27 290a 2020 2020 2020 2020  ption').        
-00045150: 6966 206d 2e67 6574 2827 4472 7952 756e  if m.get('DryRun
-00045160: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00045170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00045180: 2e64 7279 5f72 756e 203d 206d 2e67 6574  .dry_run = m.get
-00045190: 2827 4472 7952 756e 2729 0a20 2020 2020  ('DryRun').     
-000451a0: 2020 2069 6620 6d2e 6765 7428 2745 6666     if m.get('Eff
-000451b0: 6563 7454 7970 6527 2920 6973 206e 6f74  ectType') is not
-000451c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000451d0: 2020 2073 656c 662e 6566 6665 6374 5f74     self.effect_t
-000451e0: 7970 6520 3d20 6d2e 6765 7428 2745 6666  ype = m.get('Eff
-000451f0: 6563 7454 7970 6527 290a 2020 2020 2020  ectType').      
-00045200: 2020 6966 206d 2e67 6574 2827 4963 6369    if m.get('Icci
-00045210: 6473 2729 2069 7320 6e6f 7420 4e6f 6e65  ds') is not None
-00045220: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00045230: 6c66 2e69 6363 6964 7320 3d20 6d2e 6765  lf.iccids = m.ge
-00045240: 7428 2749 6363 6964 7327 290a 2020 2020  t('Iccids').    
-00045250: 2020 2020 6966 206d 2e67 6574 2827 4963      if m.get('Ic
-00045260: 6369 6473 4f73 7346 696c 6550 6174 6827  cidsOssFilePath'
-00045270: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00045280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00045290: 6963 6369 6473 5f6f 7373 5f66 696c 655f  iccids_oss_file_
-000452a0: 7061 7468 203d 206d 2e67 6574 2827 4963  path = m.get('Ic
-000452b0: 6369 6473 4f73 7346 696c 6550 6174 6827  cidsOssFilePath'
-000452c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000452d0: 6574 2827 4e61 6d65 2729 2069 7320 6e6f  et('Name') is no
-000452e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000452f0: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-00045300: 6d2e 6765 7428 274e 616d 6527 290a 2020  m.get('Name').  
-00045310: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00045320: 4f70 6572 6174 6554 7970 6527 2920 6973  OperateType') is
-00045330: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00045340: 2020 2020 2020 2073 656c 662e 6f70 6572         self.oper
-00045350: 6174 655f 7479 7065 203d 206d 2e67 6574  ate_type = m.get
-00045360: 2827 4f70 6572 6174 6554 7970 6527 290a  ('OperateType').
-00045370: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00045380: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
-00045390: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000453a0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-000453b0: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
-000453c0: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
-000453d0: 2069 6620 6d2e 6765 7428 2754 6872 6573   if m.get('Thres
-000453e0: 686f 6c64 2729 2069 7320 6e6f 7420 4e6f  hold') is not No
-000453f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00045400: 7365 6c66 2e74 6872 6573 686f 6c64 203d  self.threshold =
-00045410: 206d 2e67 6574 2827 5468 7265 7368 6f6c   m.get('Threshol
-00045420: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00045430: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-00045440: 6f75 6443 6f6e 6e65 6374 6f72 4964 7327  oudConnectorIds'
-00045450: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00045460: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00045470: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
-00045480: 6f6e 6e65 6374 6f72 5f69 6473 203d 206d  onnector_ids = m
-00045490: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
-000454a0: 6f75 6443 6f6e 6e65 6374 6f72 4964 7327  oudConnectorIds'
-000454b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000454c0: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-000454d0: 6461 7465 4261 7463 684f 7065 7261 7465  dateBatchOperate
-000454e0: 4361 7264 7354 6173 6b52 6573 706f 6e73  CardsTaskRespons
-000454f0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
-00045500: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00045510: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00045520: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00045530: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00045540: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00045550: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-00045560: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
-00045570: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00045580: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-00045590: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-000455a0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-000455b0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-000455c0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000455d0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-000455e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000455f0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00045600: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00045610: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00045620: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-00045630: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00045640: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00045650: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-00045660: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-00045670: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-00045680: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00045690: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000456a0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-000456b0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000456c0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000456d0: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
-000456e0: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
-000456f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00045700: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-00045710: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
-00045720: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
-00045730: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00045740: 2055 7064 6174 6542 6174 6368 4f70 6572   UpdateBatchOper
-00045750: 6174 6543 6172 6473 5461 736b 5265 7370  ateCardsTaskResp
-00045760: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-00045770: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00045780: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00045790: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-000457a0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-000457b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000457c0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-000457d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000457e0: 2062 6f64 793a 2055 7064 6174 6542 6174   body: UpdateBat
-000457f0: 6368 4f70 6572 6174 6543 6172 6473 5461  chOperateCardsTa
-00045800: 736b 5265 7370 6f6e 7365 426f 6479 203d  skResponseBody =
-00045810: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00045820: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00045830: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-00045840: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00045850: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00045860: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-00045870: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-00045880: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00045890: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-000458a0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-000458b0: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-000458c0: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-000458d0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-000458e0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-000458f0: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-00045900: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-00045910: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00045920: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00045930: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-00045940: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00045950: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-00045960: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-00045970: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00045980: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00045990: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000459a0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-000459b0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000459c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000459d0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000459e0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000459f0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00045a00: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-00045a10: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-00045a20: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00045a30: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-00045a40: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-00045a50: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00045a60: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-00045a70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00045a80: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-00045a90: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-00045aa0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00045ab0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-00045ac0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00045ad0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00045ae0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-00045af0: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-00045b00: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00045b10: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00045b20: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-00045b30: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-00045b40: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00045b50: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00045b60: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-00045b70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00045b80: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-00045b90: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-00045ba0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-00045bb0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-00045bc0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-00045bd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00045be0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00045bf0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-00045c00: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-00045c10: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-00045c20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00045c30: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-00045c40: 6f64 656c 203d 2055 7064 6174 6542 6174  odel = UpdateBat
-00045c50: 6368 4f70 6572 6174 6543 6172 6473 5461  chOperateCardsTa
-00045c60: 736b 5265 7370 6f6e 7365 426f 6479 2829  skResponseBody()
-00045c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00045c80: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-00045c90: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-00045ca0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-00045cb0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00045cc0: 6173 7320 5570 6461 7465 4361 7264 5265  ass UpdateCardRe
-00045cd0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00045ce0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00045cf0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00045d00: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
-00045d10: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
-00045d20: 652c 0a20 2020 2020 2020 2064 6573 6372  e,.        descr
-00045d30: 6970 7469 6f6e 3a20 7374 7220 3d20 4e6f  iption: str = No
-00045d40: 6e65 2c0a 2020 2020 2020 2020 6472 795f  ne,.        dry_
-00045d50: 7275 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65  run: bool = None
-00045d60: 2c0a 2020 2020 2020 2020 6963 6369 643a  ,.        iccid:
-00045d70: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00045d80: 2020 2020 206e 616d 653a 2073 7472 203d       name: str =
-00045d90: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
-00045da0: 6972 656c 6573 735f 636c 6f75 645f 636f  ireless_cloud_co
-00045db0: 6e6e 6563 746f 725f 6964 3a20 7374 7220  nnector_id: str 
-00045dc0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00045dd0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00045de0: 6e74 5f74 6f6b 656e 203d 2063 6c69 656e  nt_token = clien
-00045df0: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-00045e00: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00045e10: 203d 2064 6573 6372 6970 7469 6f6e 0a20   = description. 
-00045e20: 2020 2020 2020 2073 656c 662e 6472 795f         self.dry_
-00045e30: 7275 6e20 3d20 6472 795f 7275 6e0a 2020  run = dry_run.  
-00045e40: 2020 2020 2020 7365 6c66 2e69 6363 6964        self.iccid
-00045e50: 203d 2069 6363 6964 0a20 2020 2020 2020   = iccid.       
-00045e60: 2073 656c 662e 6e61 6d65 203d 206e 616d   self.name = nam
-00045e70: 650a 2020 2020 2020 2020 7365 6c66 2e77  e.        self.w
-00045e80: 6972 656c 6573 735f 636c 6f75 645f 636f  ireless_cloud_co
-00045e90: 6e6e 6563 746f 725f 6964 203d 2077 6972  nnector_id = wir
-00045ea0: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
-00045eb0: 6563 746f 725f 6964 0a0a 2020 2020 6465  ector_id..    de
-00045ec0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00045ed0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00045ee0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00045ef0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00045f00: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00045f10: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00045f20: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00045f30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00045f40: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00045f50: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00045f60: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00045f70: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-00045f80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00045f90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00045fa0: 5b27 436c 6965 6e74 546f 6b65 6e27 5d20  ['ClientToken'] 
-00045fb0: 3d20 7365 6c66 2e63 6c69 656e 745f 746f  = self.client_to
-00045fc0: 6b65 6e0a 2020 2020 2020 2020 6966 2073  ken.        if s
-00045fd0: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-00045fe0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00045ff0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00046000: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
-00046010: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
-00046020: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-00046030: 662e 6472 795f 7275 6e20 6973 206e 6f74  f.dry_run is not
-00046040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00046050: 2020 2072 6573 756c 745b 2744 7279 5275     result['DryRu
-00046060: 6e27 5d20 3d20 7365 6c66 2e64 7279 5f72  n'] = self.dry_r
-00046070: 756e 0a20 2020 2020 2020 2069 6620 7365  un.        if se
-00046080: 6c66 2e69 6363 6964 2069 7320 6e6f 7420  lf.iccid is not 
-00046090: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000460a0: 2020 7265 7375 6c74 5b27 4963 6369 6427    result['Iccid'
-000460b0: 5d20 3d20 7365 6c66 2e69 6363 6964 0a20  ] = self.iccid. 
-000460c0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000460d0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000460e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000460f0: 756c 745b 274e 616d 6527 5d20 3d20 7365  ult['Name'] = se
-00046100: 6c66 2e6e 616d 650a 2020 2020 2020 2020  lf.name.        
-00046110: 6966 2073 656c 662e 7769 7265 6c65 7373  if self.wireless
-00046120: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-00046130: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00046140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00046150: 756c 745b 2757 6972 656c 6573 7343 6c6f  ult['WirelessClo
-00046160: 7564 436f 6e6e 6563 746f 7249 6427 5d20  udConnectorId'] 
-00046170: 3d20 7365 6c66 2e77 6972 656c 6573 735f  = self.wireless_
-00046180: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-00046190: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-000461a0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000461b0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000461c0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000461d0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000461e0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000461f0: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
-00046200: 6e74 546f 6b65 6e27 2920 6973 206e 6f74  ntToken') is not
-00046210: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00046220: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
-00046230: 6f6b 656e 203d 206d 2e67 6574 2827 436c  oken = m.get('Cl
-00046240: 6965 6e74 546f 6b65 6e27 290a 2020 2020  ientToken').    
-00046250: 2020 2020 6966 206d 2e67 6574 2827 4465      if m.get('De
-00046260: 7363 7269 7074 696f 6e27 2920 6973 206e  scription') is n
-00046270: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00046280: 2020 2020 2073 656c 662e 6465 7363 7269       self.descri
-00046290: 7074 696f 6e20 3d20 6d2e 6765 7428 2744  ption = m.get('D
-000462a0: 6573 6372 6970 7469 6f6e 2729 0a20 2020  escription').   
-000462b0: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
-000462c0: 7279 5275 6e27 2920 6973 206e 6f74 204e  ryRun') is not N
-000462d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000462e0: 2073 656c 662e 6472 795f 7275 6e20 3d20   self.dry_run = 
-000462f0: 6d2e 6765 7428 2744 7279 5275 6e27 290a  m.get('DryRun').
-00046300: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00046310: 2827 4963 6369 6427 2920 6973 206e 6f74  ('Iccid') is not
-00046320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00046330: 2020 2073 656c 662e 6963 6369 6420 3d20     self.iccid = 
-00046340: 6d2e 6765 7428 2749 6363 6964 2729 0a20  m.get('Iccid'). 
-00046350: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00046360: 274e 616d 6527 2920 6973 206e 6f74 204e  'Name') is not N
-00046370: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00046380: 2073 656c 662e 6e61 6d65 203d 206d 2e67   self.name = m.g
-00046390: 6574 2827 4e61 6d65 2729 0a20 2020 2020  et('Name').     
-000463a0: 2020 2069 6620 6d2e 6765 7428 2757 6972     if m.get('Wir
-000463b0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
-000463c0: 746f 7249 6427 2920 6973 206e 6f74 204e  torId') is not N
-000463d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000463e0: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
-000463f0: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
-00046400: 6420 3d20 6d2e 6765 7428 2757 6972 656c  d = m.get('Wirel
-00046410: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-00046420: 7249 6427 290a 2020 2020 2020 2020 7265  rId').        re
-00046430: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00046440: 7320 5570 6461 7465 4361 7264 5265 7370  s UpdateCardResp
-00046450: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-00046460: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00046470: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00046480: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
-00046490: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
-000464a0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000464b0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-000464c0: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
-000464d0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-000464e0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000464f0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00046500: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00046510: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00046520: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00046530: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00046540: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00046550: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00046560: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00046570: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00046580: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
-00046590: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
-000465a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000465b0: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
-000465c0: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-000465d0: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
-000465e0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000465f0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00046600: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00046610: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00046620: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00046630: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00046640: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-00046650: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00046660: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00046670: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-00046680: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-00046690: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-000466a0: 6173 7320 5570 6461 7465 4361 7264 5265  ass UpdateCardRe
-000466b0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-000466c0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000466d0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000466e0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000466f0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-00046700: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00046710: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-00046720: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-00046730: 2020 2062 6f64 793a 2055 7064 6174 6543     body: UpdateC
-00046740: 6172 6452 6573 706f 6e73 6542 6f64 7920  ardResponseBody 
-00046750: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00046760: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00046770: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-00046780: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00046790: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-000467a0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-000467b0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-000467c0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000467d0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-000467e0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-000467f0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-00046800: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-00046810: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00046820: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00046830: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-00046840: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-00046850: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00046860: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00046870: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-00046880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00046890: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-000468a0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-000468b0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-000468c0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000468d0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000468e0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-000468f0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00046900: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00046910: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00046920: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00046930: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00046940: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-00046950: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-00046960: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00046970: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-00046980: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-00046990: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000469a0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-000469b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000469c0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-000469d0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-000469e0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-000469f0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00046a00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00046a10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00046a20: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-00046a30: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-00046a40: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00046a50: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-00046a60: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-00046a70: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-00046a80: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00046a90: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00046aa0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-00046ab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00046ac0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00046ad0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-00046ae0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00046af0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-00046b00: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-00046b10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00046b20: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00046b30: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-00046b40: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-00046b50: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-00046b60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00046b70: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00046b80: 6d6f 6465 6c20 3d20 5570 6461 7465 4361  model = UpdateCa
-00046b90: 7264 5265 7370 6f6e 7365 426f 6479 2829  rdResponseBody()
-00046ba0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00046bb0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-00046bc0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-00046bd0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-00046be0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00046bf0: 6173 7320 5570 6461 7465 444e 5341 7574  ass UpdateDNSAut
-00046c00: 686f 7269 7a61 7469 6f6e 5275 6c65 5265  horizationRuleRe
-00046c10: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00046c20: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00046c30: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00046c40: 0a20 2020 2020 2020 2061 7574 686f 7269  .        authori
-00046c50: 7a61 7469 6f6e 5f72 756c 655f 6964 3a20  zation_rule_id: 
-00046c60: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00046c70: 2020 2020 636c 6965 6e74 5f74 6f6b 656e      client_token
-00046c80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00046c90: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00046ca0: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-00046cb0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-00046cc0: 6f6e 5f69 703a 2073 7472 203d 204e 6f6e  on_ip: str = Non
-00046cd0: 652c 0a20 2020 2020 2020 2064 7279 5f72  e,.        dry_r
-00046ce0: 756e 3a20 626f 6f6c 203d 204e 6f6e 652c  un: bool = None,
-00046cf0: 0a20 2020 2020 2020 206e 616d 653a 2073  .        name: s
-00046d00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00046d10: 2020 2073 6f75 7263 655f 646e 7369 703a     source_dnsip:
-00046d20: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00046d30: 2020 2020 2077 6972 656c 6573 735f 636c       wireless_cl
-00046d40: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
-00046d50: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00046d60: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00046d70: 662e 6175 7468 6f72 697a 6174 696f 6e5f  f.authorization_
-00046d80: 7275 6c65 5f69 6420 3d20 6175 7468 6f72  rule_id = author
-00046d90: 697a 6174 696f 6e5f 7275 6c65 5f69 640a  ization_rule_id.
-00046da0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00046db0: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
-00046dc0: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
-00046dd0: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
-00046de0: 6e20 3d20 6465 7363 7269 7074 696f 6e0a  n = description.
-00046df0: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-00046e00: 7469 6e61 7469 6f6e 5f69 7020 3d20 6465  tination_ip = de
-00046e10: 7374 696e 6174 696f 6e5f 6970 0a20 2020  stination_ip.   
-00046e20: 2020 2020 2073 656c 662e 6472 795f 7275       self.dry_ru
-00046e30: 6e20 3d20 6472 795f 7275 6e0a 2020 2020  n = dry_run.    
-00046e40: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-00046e50: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
-00046e60: 662e 736f 7572 6365 5f64 6e73 6970 203d  f.source_dnsip =
-00046e70: 2073 6f75 7263 655f 646e 7369 700a 2020   source_dnsip.  
-00046e80: 2020 2020 2020 7365 6c66 2e77 6972 656c        self.wirel
-00046e90: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
-00046ea0: 746f 725f 6964 203d 2077 6972 656c 6573  tor_id = wireles
-00046eb0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-00046ec0: 725f 6964 0a0a 2020 2020 6465 6620 7661  r_id..    def va
-00046ed0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00046ee0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00046ef0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00046f00: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00046f10: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-00046f20: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00046f30: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00046f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00046f50: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00046f60: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00046f70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00046f80: 6175 7468 6f72 697a 6174 696f 6e5f 7275  authorization_ru
-00046f90: 6c65 5f69 6420 6973 206e 6f74 204e 6f6e  le_id is not Non
-00046fa0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00046fb0: 6573 756c 745b 2741 7574 686f 7269 7a61  esult['Authoriza
-00046fc0: 7469 6f6e 5275 6c65 4964 275d 203d 2073  tionRuleId'] = s
-00046fd0: 656c 662e 6175 7468 6f72 697a 6174 696f  elf.authorizatio
-00046fe0: 6e5f 7275 6c65 5f69 640a 2020 2020 2020  n_rule_id.      
-00046ff0: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
-00047000: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
-00047010: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00047020: 7265 7375 6c74 5b27 436c 6965 6e74 546f  result['ClientTo
-00047030: 6b65 6e27 5d20 3d20 7365 6c66 2e63 6c69  ken'] = self.cli
-00047040: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
-00047050: 2020 6966 2073 656c 662e 6465 7363 7269    if self.descri
-00047060: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
-00047070: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00047080: 6573 756c 745b 2744 6573 6372 6970 7469  esult['Descripti
-00047090: 6f6e 275d 203d 2073 656c 662e 6465 7363  on'] = self.desc
-000470a0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-000470b0: 6966 2073 656c 662e 6465 7374 696e 6174  if self.destinat
-000470c0: 696f 6e5f 6970 2069 7320 6e6f 7420 4e6f  ion_ip is not No
-000470d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000470e0: 7265 7375 6c74 5b27 4465 7374 696e 6174  result['Destinat
-000470f0: 696f 6e49 7027 5d20 3d20 7365 6c66 2e64  ionIp'] = self.d
-00047100: 6573 7469 6e61 7469 6f6e 5f69 700a 2020  estination_ip.  
-00047110: 2020 2020 2020 6966 2073 656c 662e 6472        if self.dr
-00047120: 795f 7275 6e20 6973 206e 6f74 204e 6f6e  y_run is not Non
-00047130: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00047140: 6573 756c 745b 2744 7279 5275 6e27 5d20  esult['DryRun'] 
-00047150: 3d20 7365 6c66 2e64 7279 5f72 756e 0a20  = self.dry_run. 
-00047160: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-00047170: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00047180: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00047190: 756c 745b 274e 616d 6527 5d20 3d20 7365  ult['Name'] = se
-000471a0: 6c66 2e6e 616d 650a 2020 2020 2020 2020  lf.name.        
-000471b0: 6966 2073 656c 662e 736f 7572 6365 5f64  if self.source_d
-000471c0: 6e73 6970 2069 7320 6e6f 7420 4e6f 6e65  nsip is not None
-000471d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000471e0: 7375 6c74 5b27 536f 7572 6365 444e 5349  sult['SourceDNSI
-000471f0: 7027 5d20 3d20 7365 6c66 2e73 6f75 7263  p'] = self.sourc
-00047200: 655f 646e 7369 700a 2020 2020 2020 2020  e_dnsip.        
-00047210: 6966 2073 656c 662e 7769 7265 6c65 7373  if self.wireless
-00047220: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-00047230: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00047240: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00047250: 756c 745b 2757 6972 656c 6573 7343 6c6f  ult['WirelessClo
-00047260: 7564 436f 6e6e 6563 746f 7249 6427 5d20  udConnectorId'] 
-00047270: 3d20 7365 6c66 2e77 6972 656c 6573 735f  = self.wireless_
-00047280: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-00047290: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-000472a0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000472b0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000472c0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000472d0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000472e0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000472f0: 2020 6966 206d 2e67 6574 2827 4175 7468    if m.get('Auth
-00047300: 6f72 697a 6174 696f 6e52 756c 6549 6427  orizationRuleId'
-00047310: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00047320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00047330: 6175 7468 6f72 697a 6174 696f 6e5f 7275  authorization_ru
-00047340: 6c65 5f69 6420 3d20 6d2e 6765 7428 2741  le_id = m.get('A
-00047350: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
-00047360: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00047370: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
-00047380: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
-00047390: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000473a0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
-000473b0: 3d20 6d2e 6765 7428 2743 6c69 656e 7454  = m.get('ClientT
-000473c0: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
-000473d0: 6620 6d2e 6765 7428 2744 6573 6372 6970  f m.get('Descrip
-000473e0: 7469 6f6e 2729 2069 7320 6e6f 7420 4e6f  tion') is not No
-000473f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00047400: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00047410: 203d 206d 2e67 6574 2827 4465 7363 7269   = m.get('Descri
-00047420: 7074 696f 6e27 290a 2020 2020 2020 2020  ption').        
-00047430: 6966 206d 2e67 6574 2827 4465 7374 696e  if m.get('Destin
-00047440: 6174 696f 6e49 7027 2920 6973 206e 6f74  ationIp') is not
-00047450: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00047460: 2020 2073 656c 662e 6465 7374 696e 6174     self.destinat
-00047470: 696f 6e5f 6970 203d 206d 2e67 6574 2827  ion_ip = m.get('
-00047480: 4465 7374 696e 6174 696f 6e49 7027 290a  DestinationIp').
-00047490: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000474a0: 2827 4472 7952 756e 2729 2069 7320 6e6f  ('DryRun') is no
-000474b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000474c0: 2020 2020 7365 6c66 2e64 7279 5f72 756e      self.dry_run
-000474d0: 203d 206d 2e67 6574 2827 4472 7952 756e   = m.get('DryRun
-000474e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000474f0: 6765 7428 274e 616d 6527 2920 6973 206e  get('Name') is n
-00047500: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00047510: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-00047520: 206d 2e67 6574 2827 4e61 6d65 2729 0a20   m.get('Name'). 
-00047530: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00047540: 2753 6f75 7263 6544 4e53 4970 2729 2069  'SourceDNSIp') i
-00047550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00047560: 2020 2020 2020 2020 7365 6c66 2e73 6f75          self.sou
-00047570: 7263 655f 646e 7369 7020 3d20 6d2e 6765  rce_dnsip = m.ge
-00047580: 7428 2753 6f75 7263 6544 4e53 4970 2729  t('SourceDNSIp')
-00047590: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000475a0: 7428 2757 6972 656c 6573 7343 6c6f 7564  t('WirelessCloud
-000475b0: 436f 6e6e 6563 746f 7249 6427 2920 6973  ConnectorId') is
-000475c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000475d0: 2020 2020 2020 2073 656c 662e 7769 7265         self.wire
-000475e0: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-000475f0: 6374 6f72 5f69 6420 3d20 6d2e 6765 7428  ctor_id = m.get(
-00047600: 2757 6972 656c 6573 7343 6c6f 7564 436f  'WirelessCloudCo
-00047610: 6e6e 6563 746f 7249 6427 290a 2020 2020  nnectorId').    
-00047620: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00047630: 0a0a 636c 6173 7320 5570 6461 7465 444e  ..class UpdateDN
-00047640: 5341 7574 686f 7269 7a61 7469 6f6e 5275  SAuthorizationRu
-00047650: 6c65 5265 7370 6f6e 7365 426f 6479 2854  leResponseBody(T
-00047660: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00047670: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00047680: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00047690: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
-000476a0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-000476b0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000476c0: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
-000476d0: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
-000476e0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000476f0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00047700: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00047710: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00047720: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-00047730: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00047740: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00047750: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00047760: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00047770: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00047780: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00047790: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
-000477a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000477b0: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
-000477c0: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
-000477d0: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-000477e0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000477f0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00047800: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-00047810: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-00047820: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00047830: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00047840: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-00047850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00047860: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00047870: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-00047880: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-00047890: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000478a0: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
-000478b0: 444e 5341 7574 686f 7269 7a61 7469 6f6e  DNSAuthorization
-000478c0: 5275 6c65 5265 7370 6f6e 7365 2854 6561  RuleResponse(Tea
-000478d0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000478e0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-000478f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00047900: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
-00047910: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
-00047920: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-00047930: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
-00047940: 0a20 2020 2020 2020 2062 6f64 793a 2055  .        body: U
-00047950: 7064 6174 6544 4e53 4175 7468 6f72 697a  pdateDNSAuthoriz
-00047960: 6174 696f 6e52 756c 6552 6573 706f 6e73  ationRuleRespons
-00047970: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-00047980: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00047990: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000479a0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000479b0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000479c0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-000479d0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-000479e0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-000479f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00047a00: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00047a10: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00047a20: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
-00047a30: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
-00047a40: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00047a50: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
-00047a60: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
-00047a70: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
-00047a80: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00047a90: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
-00047aa0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
-00047ab0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-00047ac0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00047ad0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-00047ae0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00047af0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00047b00: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00047b10: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00047b20: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00047b30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00047b40: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00047b50: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00047b60: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00047b70: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-00047b80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00047b90: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-00047ba0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-00047bb0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-00047bc0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00047bd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00047be0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00047bf0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-00047c00: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00047c10: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00047c20: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00047c30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00047c40: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-00047c50: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-00047c60: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-00047c70: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00047c80: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00047c90: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00047ca0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00047cb0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00047cc0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-00047cd0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-00047ce0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00047cf0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-00047d00: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-00047d10: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00047d20: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-00047d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00047d40: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00047d50: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00047d60: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00047d70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00047d80: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00047d90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00047da0: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
-00047db0: 6461 7465 444e 5341 7574 686f 7269 7a61  dateDNSAuthoriza
-00047dc0: 7469 6f6e 5275 6c65 5265 7370 6f6e 7365  tionRuleResponse
-00047dd0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-00047de0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00047df0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00047e00: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00047e10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00047e20: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
-00047e30: 4772 6f75 7041 7574 686f 7269 7a61 7469  GroupAuthorizati
-00047e40: 6f6e 5275 6c65 5265 7175 6573 7428 5465  onRuleRequest(Te
-00047e50: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00047e60: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00047e70: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00047e80: 2061 7574 686f 7269 7a61 7469 6f6e 5f72   authorization_r
-00047e90: 756c 655f 6964 3a20 7374 7220 3d20 4e6f  ule_id: str = No
-00047ea0: 6e65 2c0a 2020 2020 2020 2020 636c 6965  ne,.        clie
-00047eb0: 6e74 5f74 6f6b 656e 3a20 7374 7220 3d20  nt_token: str = 
-00047ec0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6465  None,.        de
-00047ed0: 7363 7269 7074 696f 6e3a 2073 7472 203d  scription: str =
-00047ee0: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
-00047ef0: 6573 7469 6e61 7469 6f6e 3a20 7374 7220  estination: str 
-00047f00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00047f10: 6465 7374 696e 6174 696f 6e5f 706f 7274  destination_port
-00047f20: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00047f30: 2020 2020 2020 6472 795f 7275 6e3a 2062        dry_run: b
-00047f40: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-00047f50: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
-00047f60: 4e6f 6e65 2c0a 2020 2020 2020 2020 706f  None,.        po
-00047f70: 6c69 6379 3a20 7374 7220 3d20 4e6f 6e65  licy: str = None
-00047f80: 2c0a 2020 2020 2020 2020 7072 6f74 6f63  ,.        protoc
-00047f90: 6f6c 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ol: str = None,.
-00047fa0: 2020 2020 2020 2020 736f 7572 6365 5f63          source_c
-00047fb0: 6964 723a 2073 7472 203d 204e 6f6e 652c  idr: str = None,
-00047fc0: 0a20 2020 2020 2020 2077 6972 656c 6573  .        wireles
-00047fd0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-00047fe0: 725f 6772 6f75 705f 6964 3a20 7374 7220  r_group_id: str 
-00047ff0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00048000: 2020 2020 2020 2073 656c 662e 6175 7468         self.auth
-00048010: 6f72 697a 6174 696f 6e5f 7275 6c65 5f69  orization_rule_i
-00048020: 6420 3d20 6175 7468 6f72 697a 6174 696f  d = authorizatio
-00048030: 6e5f 7275 6c65 5f69 640a 2020 2020 2020  n_rule_id.      
-00048040: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
-00048050: 6b65 6e20 3d20 636c 6965 6e74 5f74 6f6b  ken = client_tok
-00048060: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
-00048070: 6465 7363 7269 7074 696f 6e20 3d20 6465  description = de
-00048080: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
-00048090: 2020 7365 6c66 2e64 6573 7469 6e61 7469    self.destinati
-000480a0: 6f6e 203d 2064 6573 7469 6e61 7469 6f6e  on = destination
-000480b0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-000480c0: 7374 696e 6174 696f 6e5f 706f 7274 203d  stination_port =
-000480d0: 2064 6573 7469 6e61 7469 6f6e 5f70 6f72   destination_por
-000480e0: 740a 2020 2020 2020 2020 7365 6c66 2e64  t.        self.d
-000480f0: 7279 5f72 756e 203d 2064 7279 5f72 756e  ry_run = dry_run
-00048100: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-00048110: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
-00048120: 2020 7365 6c66 2e70 6f6c 6963 7920 3d20    self.policy = 
-00048130: 706f 6c69 6379 0a20 2020 2020 2020 2073  policy.        s
-00048140: 656c 662e 7072 6f74 6f63 6f6c 203d 2070  elf.protocol = p
-00048150: 726f 746f 636f 6c0a 2020 2020 2020 2020  rotocol.        
-00048160: 7365 6c66 2e73 6f75 7263 655f 6369 6472  self.source_cidr
-00048170: 203d 2073 6f75 7263 655f 6369 6472 0a20   = source_cidr. 
-00048180: 2020 2020 2020 2073 656c 662e 7769 7265         self.wire
-00048190: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-000481a0: 6374 6f72 5f67 726f 7570 5f69 6420 3d20  ctor_group_id = 
-000481b0: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
-000481c0: 6f6e 6e65 6374 6f72 5f67 726f 7570 5f69  onnector_group_i
-000481d0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-000481e0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000481f0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00048200: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00048210: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00048220: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00048230: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00048240: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00048250: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00048260: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00048270: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00048280: 2020 2020 2069 6620 7365 6c66 2e61 7574       if self.aut
-00048290: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
-000482a0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000482b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000482c0: 6c74 5b27 4175 7468 6f72 697a 6174 696f  lt['Authorizatio
-000482d0: 6e52 756c 6549 6427 5d20 3d20 7365 6c66  nRuleId'] = self
-000482e0: 2e61 7574 686f 7269 7a61 7469 6f6e 5f72  .authorization_r
-000482f0: 756c 655f 6964 0a20 2020 2020 2020 2069  ule_id.        i
-00048300: 6620 7365 6c66 2e63 6c69 656e 745f 746f  f self.client_to
-00048310: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
-00048320: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00048330: 756c 745b 2743 6c69 656e 7454 6f6b 656e  ult['ClientToken
-00048340: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-00048350: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
-00048360: 6620 7365 6c66 2e64 6573 6372 6970 7469  f self.descripti
-00048370: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00048380: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00048390: 6c74 5b27 4465 7363 7269 7074 696f 6e27  lt['Description'
-000483a0: 5d20 3d20 7365 6c66 2e64 6573 6372 6970  ] = self.descrip
-000483b0: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
-000483c0: 7365 6c66 2e64 6573 7469 6e61 7469 6f6e  self.destination
-000483d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000483e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000483f0: 5b27 4465 7374 696e 6174 696f 6e27 5d20  ['Destination'] 
-00048400: 3d20 7365 6c66 2e64 6573 7469 6e61 7469  = self.destinati
-00048410: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
-00048420: 6c66 2e64 6573 7469 6e61 7469 6f6e 5f70  lf.destination_p
-00048430: 6f72 7420 6973 206e 6f74 204e 6f6e 653a  ort is not None:
-00048440: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00048450: 756c 745b 2744 6573 7469 6e61 7469 6f6e  ult['Destination
-00048460: 506f 7274 275d 203d 2073 656c 662e 6465  Port'] = self.de
-00048470: 7374 696e 6174 696f 6e5f 706f 7274 0a20  stination_port. 
-00048480: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00048490: 7279 5f72 756e 2069 7320 6e6f 7420 4e6f  ry_run is not No
-000484a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000484b0: 7265 7375 6c74 5b27 4472 7952 756e 275d  result['DryRun']
-000484c0: 203d 2073 656c 662e 6472 795f 7275 6e0a   = self.dry_run.
-000484d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000484e0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-000484f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00048500: 7375 6c74 5b27 4e61 6d65 275d 203d 2073  sult['Name'] = s
-00048510: 656c 662e 6e61 6d65 0a20 2020 2020 2020  elf.name.       
-00048520: 2069 6620 7365 6c66 2e70 6f6c 6963 7920   if self.policy 
-00048530: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00048540: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00048550: 2750 6f6c 6963 7927 5d20 3d20 7365 6c66  'Policy'] = self
-00048560: 2e70 6f6c 6963 790a 2020 2020 2020 2020  .policy.        
-00048570: 6966 2073 656c 662e 7072 6f74 6f63 6f6c  if self.protocol
-00048580: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00048590: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000485a0: 5b27 5072 6f74 6f63 6f6c 275d 203d 2073  ['Protocol'] = s
-000485b0: 656c 662e 7072 6f74 6f63 6f6c 0a20 2020  elf.protocol.   
-000485c0: 2020 2020 2069 6620 7365 6c66 2e73 6f75       if self.sou
-000485d0: 7263 655f 6369 6472 2069 7320 6e6f 7420  rce_cidr is not 
-000485e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000485f0: 2020 7265 7375 6c74 5b27 536f 7572 6365    result['Source
-00048600: 4369 6472 275d 203d 2073 656c 662e 736f  Cidr'] = self.so
-00048610: 7572 6365 5f63 6964 720a 2020 2020 2020  urce_cidr.      
-00048620: 2020 6966 2073 656c 662e 7769 7265 6c65    if self.wirele
-00048630: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-00048640: 6f72 5f67 726f 7570 5f69 6420 6973 206e  or_group_id is n
-00048650: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00048660: 2020 2020 2072 6573 756c 745b 2757 6972       result['Wir
-00048670: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
-00048680: 746f 7247 726f 7570 4964 275d 203d 2073  torGroupId'] = s
-00048690: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
-000486a0: 7564 5f63 6f6e 6e65 6374 6f72 5f67 726f  ud_connector_gro
-000486b0: 7570 5f69 640a 2020 2020 2020 2020 7265  up_id.        re
-000486c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000486d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000486e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-000486f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00048700: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00048710: 2020 2020 2069 6620 6d2e 6765 7428 2741       if m.get('A
-00048720: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
-00048730: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00048740: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00048750: 6c66 2e61 7574 686f 7269 7a61 7469 6f6e  lf.authorization
-00048760: 5f72 756c 655f 6964 203d 206d 2e67 6574  _rule_id = m.get
-00048770: 2827 4175 7468 6f72 697a 6174 696f 6e52  ('AuthorizationR
-00048780: 756c 6549 6427 290a 2020 2020 2020 2020  uleId').        
-00048790: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-000487a0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
-000487b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000487c0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-000487d0: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
-000487e0: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
-000487f0: 2020 6966 206d 2e67 6574 2827 4465 7363    if m.get('Desc
-00048800: 7269 7074 696f 6e27 2920 6973 206e 6f74  ription') is not
-00048810: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00048820: 2020 2073 656c 662e 6465 7363 7269 7074     self.descript
-00048830: 696f 6e20 3d20 6d2e 6765 7428 2744 6573  ion = m.get('Des
-00048840: 6372 6970 7469 6f6e 2729 0a20 2020 2020  cription').     
-00048850: 2020 2069 6620 6d2e 6765 7428 2744 6573     if m.get('Des
-00048860: 7469 6e61 7469 6f6e 2729 2069 7320 6e6f  tination') is no
-00048870: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00048880: 2020 2020 7365 6c66 2e64 6573 7469 6e61      self.destina
-00048890: 7469 6f6e 203d 206d 2e67 6574 2827 4465  tion = m.get('De
-000488a0: 7374 696e 6174 696f 6e27 290a 2020 2020  stination').    
-000488b0: 2020 2020 6966 206d 2e67 6574 2827 4465      if m.get('De
-000488c0: 7374 696e 6174 696f 6e50 6f72 7427 2920  stinationPort') 
-000488d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000488e0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-000488f0: 7374 696e 6174 696f 6e5f 706f 7274 203d  stination_port =
-00048900: 206d 2e67 6574 2827 4465 7374 696e 6174   m.get('Destinat
-00048910: 696f 6e50 6f72 7427 290a 2020 2020 2020  ionPort').      
-00048920: 2020 6966 206d 2e67 6574 2827 4472 7952    if m.get('DryR
-00048930: 756e 2729 2069 7320 6e6f 7420 4e6f 6e65  un') is not None
-00048940: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00048950: 6c66 2e64 7279 5f72 756e 203d 206d 2e67  lf.dry_run = m.g
-00048960: 6574 2827 4472 7952 756e 2729 0a20 2020  et('DryRun').   
-00048970: 2020 2020 2069 6620 6d2e 6765 7428 274e       if m.get('N
-00048980: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00048990: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000489a0: 656c 662e 6e61 6d65 203d 206d 2e67 6574  elf.name = m.get
-000489b0: 2827 4e61 6d65 2729 0a20 2020 2020 2020  ('Name').       
-000489c0: 2069 6620 6d2e 6765 7428 2750 6f6c 6963   if m.get('Polic
-000489d0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-000489e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000489f0: 662e 706f 6c69 6379 203d 206d 2e67 6574  f.policy = m.get
-00048a00: 2827 506f 6c69 6379 2729 0a20 2020 2020  ('Policy').     
-00048a10: 2020 2069 6620 6d2e 6765 7428 2750 726f     if m.get('Pro
-00048a20: 746f 636f 6c27 2920 6973 206e 6f74 204e  tocol') is not N
-00048a30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00048a40: 2073 656c 662e 7072 6f74 6f63 6f6c 203d   self.protocol =
-00048a50: 206d 2e67 6574 2827 5072 6f74 6f63 6f6c   m.get('Protocol
-00048a60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00048a70: 6765 7428 2753 6f75 7263 6543 6964 7227  get('SourceCidr'
-00048a80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00048a90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00048aa0: 736f 7572 6365 5f63 6964 7220 3d20 6d2e  source_cidr = m.
-00048ab0: 6765 7428 2753 6f75 7263 6543 6964 7227  get('SourceCidr'
-00048ac0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00048ad0: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
-00048ae0: 6443 6f6e 6e65 6374 6f72 4772 6f75 7049  dConnectorGroupI
-00048af0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00048b00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00048b10: 662e 7769 7265 6c65 7373 5f63 6c6f 7564  f.wireless_cloud
-00048b20: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
-00048b30: 5f69 6420 3d20 6d2e 6765 7428 2757 6972  _id = m.get('Wir
-00048b40: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
-00048b50: 746f 7247 726f 7570 4964 2729 0a20 2020  torGroupId').   
-00048b60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00048b70: 0a0a 0a63 6c61 7373 2055 7064 6174 6547  ...class UpdateG
-00048b80: 726f 7570 4175 7468 6f72 697a 6174 696f  roupAuthorizatio
-00048b90: 6e52 756c 6552 6573 706f 6e73 6542 6f64  nRuleResponseBod
-00048ba0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-00048bb0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00048bc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00048bd0: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
-00048be0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00048bf0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00048c00: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
-00048c10: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
-00048c20: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00048c30: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00048c40: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00048c50: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00048c60: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00048c70: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00048c80: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00048c90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00048ca0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00048cb0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00048cc0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00048cd0: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
-00048ce0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00048cf0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00048d00: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
-00048d10: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
-00048d20: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00048d30: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-00048d40: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-00048d50: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-00048d60: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00048d70: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00048d80: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00048d90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00048da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00048db0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-00048dc0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00048dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00048de0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
-00048df0: 6174 6547 726f 7570 4175 7468 6f72 697a  ateGroupAuthoriz
-00048e00: 6174 696f 6e52 756c 6552 6573 706f 6e73  ationRuleRespons
-00048e10: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-00048e20: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00048e30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00048e40: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-00048e50: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-00048e60: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
-00048e70: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
-00048e80: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-00048e90: 6479 3a20 5570 6461 7465 4772 6f75 7041  dy: UpdateGroupA
-00048ea0: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
-00048eb0: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
-00048ec0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00048ed0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00048ee0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-00048ef0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00048f00: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-00048f10: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-00048f20: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-00048f30: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00048f40: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00048f50: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-00048f60: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-00048f70: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-00048f80: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-00048f90: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-00048fa0: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-00048fb0: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-00048fc0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-00048fd0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-00048fe0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-00048ff0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00049000: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-00049010: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-00049020: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00049030: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00049040: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00049050: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00049060: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00049070: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00049080: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00049090: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000490a0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000490b0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-000490c0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000490d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000490e0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-000490f0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-00049100: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00049110: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-00049120: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00049130: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-00049140: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-00049150: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00049160: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-00049170: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00049180: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-00049190: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-000491a0: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-000491b0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000491c0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000491d0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000491e0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000491f0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00049200: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00049210: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00049220: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00049230: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00049240: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00049250: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00049260: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00049270: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00049280: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00049290: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-000492a0: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-000492b0: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-000492c0: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-000492d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000492e0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-000492f0: 656c 203d 2055 7064 6174 6547 726f 7570  el = UpdateGroup
-00049300: 4175 7468 6f72 697a 6174 696f 6e52 756c  AuthorizationRul
-00049310: 6552 6573 706f 6e73 6542 6f64 7928 290a  eResponseBody().
-00049320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00049330: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-00049340: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-00049350: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-00049360: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00049370: 7373 2055 7064 6174 6547 726f 7570 446e  ss UpdateGroupDn
-00049380: 7341 7574 686f 7269 7a61 7469 6f6e 5275  sAuthorizationRu
-00049390: 6c65 5265 7175 6573 7428 5465 614d 6f64  leRequest(TeaMod
-000493a0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000493b0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000493c0: 656c 662c 0a20 2020 2020 2020 2061 7574  elf,.        aut
-000493d0: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
-000493e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-000493f0: 2020 2020 2020 2020 636c 6965 6e74 5f74          client_t
-00049400: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
-00049410: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
-00049420: 7074 696f 6e3a 2073 7472 203d 204e 6f6e  ption: str = Non
-00049430: 652c 0a20 2020 2020 2020 2064 6573 7469  e,.        desti
-00049440: 6e61 7469 6f6e 5f69 703a 2073 7472 203d  nation_ip: str =
-00049450: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
-00049460: 7279 5f72 756e 3a20 626f 6f6c 203d 204e  ry_run: bool = N
-00049470: 6f6e 652c 0a20 2020 2020 2020 206e 616d  one,.        nam
-00049480: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-00049490: 2020 2020 2020 2073 6f75 7263 655f 646e         source_dn
-000494a0: 7369 703a 2073 7472 203d 204e 6f6e 652c  sip: str = None,
-000494b0: 0a20 2020 2020 2020 2077 6972 656c 6573  .        wireles
-000494c0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-000494d0: 725f 6772 6f75 705f 6964 3a20 7374 7220  r_group_id: str 
-000494e0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-000494f0: 2020 2020 2020 2073 656c 662e 6175 7468         self.auth
-00049500: 6f72 697a 6174 696f 6e5f 7275 6c65 5f69  orization_rule_i
-00049510: 6420 3d20 6175 7468 6f72 697a 6174 696f  d = authorizatio
-00049520: 6e5f 7275 6c65 5f69 640a 2020 2020 2020  n_rule_id.      
-00049530: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
-00049540: 6b65 6e20 3d20 636c 6965 6e74 5f74 6f6b  ken = client_tok
-00049550: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
-00049560: 6465 7363 7269 7074 696f 6e20 3d20 6465  description = de
-00049570: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
-00049580: 2020 7365 6c66 2e64 6573 7469 6e61 7469    self.destinati
-00049590: 6f6e 5f69 7020 3d20 6465 7374 696e 6174  on_ip = destinat
-000495a0: 696f 6e5f 6970 0a20 2020 2020 2020 2073  ion_ip.        s
-000495b0: 656c 662e 6472 795f 7275 6e20 3d20 6472  elf.dry_run = dr
-000495c0: 795f 7275 6e0a 2020 2020 2020 2020 7365  y_run.        se
-000495d0: 6c66 2e6e 616d 6520 3d20 6e61 6d65 0a20  lf.name = name. 
-000495e0: 2020 2020 2020 2073 656c 662e 736f 7572         self.sour
-000495f0: 6365 5f64 6e73 6970 203d 2073 6f75 7263  ce_dnsip = sourc
-00049600: 655f 646e 7369 700a 2020 2020 2020 2020  e_dnsip.        
-00049610: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
-00049620: 6f75 645f 636f 6e6e 6563 746f 725f 6772  oud_connector_gr
-00049630: 6f75 705f 6964 203d 2077 6972 656c 6573  oup_id = wireles
-00049640: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-00049650: 725f 6772 6f75 705f 6964 0a0a 2020 2020  r_group_id..    
-00049660: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00049670: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00049680: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00049690: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000496a0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000496b0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000496c0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000496d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000496e0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000496f0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00049700: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00049710: 2073 656c 662e 6175 7468 6f72 697a 6174   self.authorizat
-00049720: 696f 6e5f 7275 6c65 5f69 6420 6973 206e  ion_rule_id is n
-00049730: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00049740: 2020 2020 2072 6573 756c 745b 2741 7574       result['Aut
-00049750: 686f 7269 7a61 7469 6f6e 5275 6c65 4964  horizationRuleId
-00049760: 275d 203d 2073 656c 662e 6175 7468 6f72  '] = self.author
-00049770: 697a 6174 696f 6e5f 7275 6c65 5f69 640a  ization_rule_id.
-00049780: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00049790: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
-000497a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000497b0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-000497c0: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
-000497d0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
-000497e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000497f0: 6465 7363 7269 7074 696f 6e20 6973 206e  description is n
-00049800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00049810: 2020 2020 2072 6573 756c 745b 2744 6573       result['Des
-00049820: 6372 6970 7469 6f6e 275d 203d 2073 656c  cription'] = sel
-00049830: 662e 6465 7363 7269 7074 696f 6e0a 2020  f.description.  
-00049840: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
-00049850: 7374 696e 6174 696f 6e5f 6970 2069 7320  stination_ip is 
-00049860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00049870: 2020 2020 2020 7265 7375 6c74 5b27 4465        result['De
-00049880: 7374 696e 6174 696f 6e49 7027 5d20 3d20  stinationIp'] = 
-00049890: 7365 6c66 2e64 6573 7469 6e61 7469 6f6e  self.destination
-000498a0: 5f69 700a 2020 2020 2020 2020 6966 2073  _ip.        if s
-000498b0: 656c 662e 6472 795f 7275 6e20 6973 206e  elf.dry_run is n
-000498c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000498d0: 2020 2020 2072 6573 756c 745b 2744 7279       result['Dry
-000498e0: 5275 6e27 5d20 3d20 7365 6c66 2e64 7279  Run'] = self.dry
-000498f0: 5f72 756e 0a20 2020 2020 2020 2069 6620  _run.        if 
-00049900: 7365 6c66 2e6e 616d 6520 6973 206e 6f74  self.name is not
-00049910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00049920: 2020 2072 6573 756c 745b 274e 616d 6527     result['Name'
-00049930: 5d20 3d20 7365 6c66 2e6e 616d 650a 2020  ] = self.name.  
-00049940: 2020 2020 2020 6966 2073 656c 662e 736f        if self.so
-00049950: 7572 6365 5f64 6e73 6970 2069 7320 6e6f  urce_dnsip is no
-00049960: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00049970: 2020 2020 7265 7375 6c74 5b27 536f 7572      result['Sour
-00049980: 6365 444e 5349 7027 5d20 3d20 7365 6c66  ceDNSIp'] = self
-00049990: 2e73 6f75 7263 655f 646e 7369 700a 2020  .source_dnsip.  
-000499a0: 2020 2020 2020 6966 2073 656c 662e 7769        if self.wi
-000499b0: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
-000499c0: 6e65 6374 6f72 5f67 726f 7570 5f69 6420  nector_group_id 
-000499d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000499e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000499f0: 2757 6972 656c 6573 7343 6c6f 7564 436f  'WirelessCloudCo
-00049a00: 6e6e 6563 746f 7247 726f 7570 4964 275d  nnectorGroupId']
-00049a10: 203d 2073 656c 662e 7769 7265 6c65 7373   = self.wireless
-00049a20: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-00049a30: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
-00049a40: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00049a50: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00049a60: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00049a70: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00049a80: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00049a90: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00049aa0: 7428 2741 7574 686f 7269 7a61 7469 6f6e  t('Authorization
-00049ab0: 5275 6c65 4964 2729 2069 7320 6e6f 7420  RuleId') is not 
-00049ac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00049ad0: 2020 7365 6c66 2e61 7574 686f 7269 7a61    self.authoriza
-00049ae0: 7469 6f6e 5f72 756c 655f 6964 203d 206d  tion_rule_id = m
-00049af0: 2e67 6574 2827 4175 7468 6f72 697a 6174  .get('Authorizat
-00049b00: 696f 6e52 756c 6549 6427 290a 2020 2020  ionRuleId').    
-00049b10: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-00049b20: 6965 6e74 546f 6b65 6e27 2920 6973 206e  ientToken') is n
-00049b30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00049b40: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00049b50: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-00049b60: 436c 6965 6e74 546f 6b65 6e27 290a 2020  ClientToken').  
-00049b70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00049b80: 4465 7363 7269 7074 696f 6e27 2920 6973  Description') is
-00049b90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00049ba0: 2020 2020 2020 2073 656c 662e 6465 7363         self.desc
-00049bb0: 7269 7074 696f 6e20 3d20 6d2e 6765 7428  ription = m.get(
-00049bc0: 2744 6573 6372 6970 7469 6f6e 2729 0a20  'Description'). 
-00049bd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00049be0: 2744 6573 7469 6e61 7469 6f6e 4970 2729  'DestinationIp')
-00049bf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00049c00: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00049c10: 6573 7469 6e61 7469 6f6e 5f69 7020 3d20  estination_ip = 
-00049c20: 6d2e 6765 7428 2744 6573 7469 6e61 7469  m.get('Destinati
-00049c30: 6f6e 4970 2729 0a20 2020 2020 2020 2069  onIp').        i
-00049c40: 6620 6d2e 6765 7428 2744 7279 5275 6e27  f m.get('DryRun'
-00049c50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00049c60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00049c70: 6472 795f 7275 6e20 3d20 6d2e 6765 7428  dry_run = m.get(
-00049c80: 2744 7279 5275 6e27 290a 2020 2020 2020  'DryRun').      
-00049c90: 2020 6966 206d 2e67 6574 2827 4e61 6d65    if m.get('Name
-00049ca0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00049cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00049cc0: 2e6e 616d 6520 3d20 6d2e 6765 7428 274e  .name = m.get('N
-00049cd0: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
-00049ce0: 206d 2e67 6574 2827 536f 7572 6365 444e   m.get('SourceDN
-00049cf0: 5349 7027 2920 6973 206e 6f74 204e 6f6e  SIp') is not Non
-00049d00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00049d10: 656c 662e 736f 7572 6365 5f64 6e73 6970  elf.source_dnsip
-00049d20: 203d 206d 2e67 6574 2827 536f 7572 6365   = m.get('Source
-00049d30: 444e 5349 7027 290a 2020 2020 2020 2020  DNSIp').        
-00049d40: 6966 206d 2e67 6574 2827 5769 7265 6c65  if m.get('Wirele
-00049d50: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
-00049d60: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
-00049d70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00049d80: 2020 2073 656c 662e 7769 7265 6c65 7373     self.wireless
-00049d90: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-00049da0: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
-00049db0: 7428 2757 6972 656c 6573 7343 6c6f 7564  t('WirelessCloud
-00049dc0: 436f 6e6e 6563 746f 7247 726f 7570 4964  ConnectorGroupId
-00049dd0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00049de0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-00049df0: 7064 6174 6547 726f 7570 446e 7341 7574  pdateGroupDnsAut
-00049e00: 686f 7269 7a61 7469 6f6e 5275 6c65 5265  horizationRuleRe
-00049e10: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-00049e20: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00049e30: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00049e40: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
-00049e50: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
-00049e60: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00049e70: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-00049e80: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-00049e90: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-00049ea0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00049eb0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00049ec0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00049ed0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00049ee0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00049ef0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00049f00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00049f10: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00049f20: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00049f30: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00049f40: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
-00049f50: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
-00049f60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00049f70: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
-00049f80: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
-00049f90: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
-00049fa0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-00049fb0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00049fc0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00049fd0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00049fe0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00049ff0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0004a000: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-0004a010: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0004a020: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0004a030: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-0004a040: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-0004a050: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0004a060: 636c 6173 7320 5570 6461 7465 4772 6f75  class UpdateGrou
-0004a070: 7044 6e73 4175 7468 6f72 697a 6174 696f  pDnsAuthorizatio
-0004a080: 6e52 756c 6552 6573 706f 6e73 6528 5465  nRuleResponse(Te
-0004a090: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0004a0a0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-0004a0b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0004a0c0: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-0004a0d0: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-0004a0e0: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-0004a0f0: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-0004a100: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-0004a110: 5570 6461 7465 4772 6f75 7044 6e73 4175  UpdateGroupDnsAu
-0004a120: 7468 6f72 697a 6174 696f 6e52 756c 6552  thorizationRuleR
-0004a130: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
-0004a140: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0004a150: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0004a160: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-0004a170: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0004a180: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-0004a190: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-0004a1a0: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-0004a1b0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0004a1c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0004a1d0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0004a1e0: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
-0004a1f0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0004a200: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0004a210: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
-0004a220: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
-0004a230: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
-0004a240: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0004a250: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
-0004a260: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
-0004a270: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0004a280: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0004a290: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0004a2a0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0004a2b0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0004a2c0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0004a2d0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0004a2e0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0004a2f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004a300: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0004a310: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0004a320: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0004a330: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0004a340: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004a350: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0004a360: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0004a370: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0004a380: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0004a390: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0004a3a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004a3b0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0004a3c0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0004a3d0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0004a3e0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0004a3f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004a400: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-0004a410: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0004a420: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0004a430: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0004a440: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0004a450: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0004a460: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0004a470: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0004a480: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0004a490: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-0004a4a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004a4b0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-0004a4c0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-0004a4d0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-0004a4e0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-0004a4f0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-0004a500: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0004a510: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0004a520: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-0004a530: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-0004a540: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-0004a550: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004a560: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-0004a570: 6c20 3d20 5570 6461 7465 4772 6f75 7044  l = UpdateGroupD
-0004a580: 6e73 4175 7468 6f72 697a 6174 696f 6e52  nsAuthorizationR
-0004a590: 756c 6552 6573 706f 6e73 6542 6f64 7928  uleResponseBody(
-0004a5a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0004a5b0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0004a5c0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0004a5d0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0004a5e0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0004a5f0: 6c61 7373 2055 7064 6174 6557 6972 656c  lass UpdateWirel
-0004a600: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-0004a610: 7252 6571 7565 7374 2854 6561 4d6f 6465  rRequest(TeaMode
-0004a620: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0004a630: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0004a640: 6c66 2c0a 2020 2020 2020 2020 636c 6965  lf,.        clie
-0004a650: 6e74 5f74 6f6b 656e 3a20 7374 7220 3d20  nt_token: str = 
-0004a660: 4e6f 6e65 2c0a 2020 2020 2020 2020 6465  None,.        de
-0004a670: 7363 7269 7074 696f 6e3a 2073 7472 203d  scription: str =
-0004a680: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
-0004a690: 7279 5f72 756e 3a20 626f 6f6c 203d 204e  ry_run: bool = N
-0004a6a0: 6f6e 652c 0a20 2020 2020 2020 206e 616d  one,.        nam
-0004a6b0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-0004a6c0: 2020 2020 2020 2077 6972 656c 6573 735f         wireless_
-0004a6d0: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
-0004a6e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0004a6f0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0004a700: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-0004a710: 203d 2063 6c69 656e 745f 746f 6b65 6e0a   = client_token.
-0004a720: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-0004a730: 6372 6970 7469 6f6e 203d 2064 6573 6372  cription = descr
-0004a740: 6970 7469 6f6e 0a20 2020 2020 2020 2073  iption.        s
-0004a750: 656c 662e 6472 795f 7275 6e20 3d20 6472  elf.dry_run = dr
-0004a760: 795f 7275 6e0a 2020 2020 2020 2020 7365  y_run.        se
-0004a770: 6c66 2e6e 616d 6520 3d20 6e61 6d65 0a20  lf.name = name. 
-0004a780: 2020 2020 2020 2073 656c 662e 7769 7265         self.wire
-0004a790: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
-0004a7a0: 6374 6f72 5f69 6420 3d20 7769 7265 6c65  ctor_id = wirele
-0004a7b0: 7373 5f63 6c6f 7564 5f63 6f6e 6e65 6374  ss_cloud_connect
-0004a7c0: 6f72 5f69 640a 0a20 2020 2064 6566 2076  or_id..    def v
-0004a7d0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0004a7e0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0004a7f0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0004a800: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0004a810: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-0004a820: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0004a830: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0004a840: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0004a850: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0004a860: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0004a870: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0004a880: 2e63 6c69 656e 745f 746f 6b65 6e20 6973  .client_token is
-0004a890: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004a8a0: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-0004a8b0: 6c69 656e 7454 6f6b 656e 275d 203d 2073  lientToken'] = s
-0004a8c0: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-0004a8d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0004a8e0: 2e64 6573 6372 6970 7469 6f6e 2069 7320  .description is 
-0004a8f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004a900: 2020 2020 2020 7265 7375 6c74 5b27 4465        result['De
-0004a910: 7363 7269 7074 696f 6e27 5d20 3d20 7365  scription'] = se
-0004a920: 6c66 2e64 6573 6372 6970 7469 6f6e 0a20  lf.description. 
-0004a930: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0004a940: 7279 5f72 756e 2069 7320 6e6f 7420 4e6f  ry_run is not No
-0004a950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004a960: 7265 7375 6c74 5b27 4472 7952 756e 275d  result['DryRun']
-0004a970: 203d 2073 656c 662e 6472 795f 7275 6e0a   = self.dry_run.
-0004a980: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0004a990: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0004a9a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004a9b0: 7375 6c74 5b27 4e61 6d65 275d 203d 2073  sult['Name'] = s
-0004a9c0: 656c 662e 6e61 6d65 0a20 2020 2020 2020  elf.name.       
-0004a9d0: 2069 6620 7365 6c66 2e77 6972 656c 6573   if self.wireles
-0004a9e0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-0004a9f0: 725f 6964 2069 7320 6e6f 7420 4e6f 6e65  r_id is not None
-0004aa00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004aa10: 7375 6c74 5b27 5769 7265 6c65 7373 436c  sult['WirelessCl
-0004aa20: 6f75 6443 6f6e 6e65 6374 6f72 4964 275d  oudConnectorId']
-0004aa30: 203d 2073 656c 662e 7769 7265 6c65 7373   = self.wireless
-0004aa40: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-0004aa50: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0004aa60: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0004aa70: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0004aa80: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0004aa90: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0004aaa0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0004aab0: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
-0004aac0: 656e 7454 6f6b 656e 2729 2069 7320 6e6f  entToken') is no
-0004aad0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004aae0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-0004aaf0: 746f 6b65 6e20 3d20 6d2e 6765 7428 2743  token = m.get('C
-0004ab00: 6c69 656e 7454 6f6b 656e 2729 0a20 2020  lientToken').   
-0004ab10: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
-0004ab20: 6573 6372 6970 7469 6f6e 2729 2069 7320  escription') is 
-0004ab30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004ab40: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
-0004ab50: 6970 7469 6f6e 203d 206d 2e67 6574 2827  iption = m.get('
-0004ab60: 4465 7363 7269 7074 696f 6e27 290a 2020  Description').  
-0004ab70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0004ab80: 4472 7952 756e 2729 2069 7320 6e6f 7420  DryRun') is not 
-0004ab90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004aba0: 2020 7365 6c66 2e64 7279 5f72 756e 203d    self.dry_run =
-0004abb0: 206d 2e67 6574 2827 4472 7952 756e 2729   m.get('DryRun')
-0004abc0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0004abd0: 7428 274e 616d 6527 2920 6973 206e 6f74  t('Name') is not
-0004abe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004abf0: 2020 2073 656c 662e 6e61 6d65 203d 206d     self.name = m
-0004ac00: 2e67 6574 2827 4e61 6d65 2729 0a20 2020  .get('Name').   
-0004ac10: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
-0004ac20: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
-0004ac30: 6563 746f 7249 6427 2920 6973 206e 6f74  ectorId') is not
-0004ac40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004ac50: 2020 2073 656c 662e 7769 7265 6c65 7373     self.wireless
-0004ac60: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
-0004ac70: 5f69 6420 3d20 6d2e 6765 7428 2757 6972  _id = m.get('Wir
-0004ac80: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
-0004ac90: 746f 7249 6427 290a 2020 2020 2020 2020  torId').        
-0004aca0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0004acb0: 6173 7320 5570 6461 7465 5769 7265 6c65  ass UpdateWirele
-0004acc0: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
-0004acd0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-0004ace0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0004acf0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0004ad00: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0004ad10: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
-0004ad20: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0004ad30: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-0004ad40: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-0004ad50: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-0004ad60: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0004ad70: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0004ad80: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0004ad90: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0004ada0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0004adb0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0004adc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004add0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0004ade0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0004adf0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0004ae00: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0004ae10: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-0004ae20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004ae30: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-0004ae40: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-0004ae50: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-0004ae60: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0004ae70: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0004ae80: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-0004ae90: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0004aea0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0004aeb0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0004aec0: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
-0004aed0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004aee0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-0004aef0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
-0004af00: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
-0004af10: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0004af20: 0a0a 636c 6173 7320 5570 6461 7465 5769  ..class UpdateWi
-0004af30: 7265 6c65 7373 436c 6f75 6443 6f6e 6e65  relessCloudConne
-0004af40: 6374 6f72 5265 7370 6f6e 7365 2854 6561  ctorResponse(Tea
-0004af50: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0004af60: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0004af70: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0004af80: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
-0004af90: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
-0004afa0: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-0004afb0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
-0004afc0: 0a20 2020 2020 2020 2062 6f64 793a 2055  .        body: U
-0004afd0: 7064 6174 6557 6972 656c 6573 7343 6c6f  pdateWirelessClo
-0004afe0: 7564 436f 6e6e 6563 746f 7252 6573 706f  udConnectorRespo
-0004aff0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-0004b000: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0004b010: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-0004b020: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-0004b030: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0004b040: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-0004b050: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0004b060: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-0004b070: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0004b080: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0004b090: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0004b0a0: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-0004b0b0: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-0004b0c0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0004b0d0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-0004b0e0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-0004b0f0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-0004b100: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0004b110: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-0004b120: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-0004b130: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-0004b140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0004b150: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0004b160: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0004b170: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0004b180: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0004b190: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0004b1a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0004b1b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004b1c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0004b1d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0004b1e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0004b1f0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-0004b200: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004b210: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-0004b220: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-0004b230: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-0004b240: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-0004b250: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-0004b260: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0004b270: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-0004b280: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-0004b290: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-0004b2a0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-0004b2b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004b2c0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-0004b2d0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-0004b2e0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-0004b2f0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0004b300: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0004b310: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0004b320: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0004b330: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0004b340: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-0004b350: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-0004b360: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004b370: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0004b380: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0004b390: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0004b3a0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0004b3b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004b3c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0004b3d0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-0004b3e0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0004b3f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0004b400: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-0004b410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004b420: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-0004b430: 5570 6461 7465 5769 7265 6c65 7373 436c  UpdateWirelessCl
-0004b440: 6f75 6443 6f6e 6e65 6374 6f72 5265 7370  oudConnectorResp
-0004b450: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
-0004b460: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0004b470: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-0004b480: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-0004b490: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0004b4a0: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-0004b4b0: 6461 7465 5769 7265 6c65 7373 436c 6f75  dateWirelessClou
-0004b4c0: 6443 6f6e 6e65 6374 6f72 4772 6f75 7052  dConnectorGroupR
-0004b4d0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-0004b4e0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0004b4f0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0004b500: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
-0004b510: 5f74 6f6b 656e 3a20 7374 7220 3d20 4e6f  _token: str = No
-0004b520: 6e65 2c0a 2020 2020 2020 2020 6465 7363  ne,.        desc
-0004b530: 7269 7074 696f 6e3a 2073 7472 203d 204e  ription: str = N
-0004b540: 6f6e 652c 0a20 2020 2020 2020 2064 7279  one,.        dry
-0004b550: 5f72 756e 3a20 626f 6f6c 203d 204e 6f6e  _run: bool = Non
-0004b560: 652c 0a20 2020 2020 2020 206e 616d 653a  e,.        name:
-0004b570: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0004b580: 2020 2020 2077 6972 656c 6573 735f 636c       wireless_cl
-0004b590: 6f75 645f 636f 6e6e 6563 746f 725f 6772  oud_connector_gr
-0004b5a0: 6f75 705f 6964 3a20 7374 7220 3d20 4e6f  oup_id: str = No
-0004b5b0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0004b5c0: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
-0004b5d0: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
-0004b5e0: 6b65 6e0a 2020 2020 2020 2020 7365 6c66  ken.        self
-0004b5f0: 2e64 6573 6372 6970 7469 6f6e 203d 2064  .description = d
-0004b600: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
-0004b610: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
-0004b620: 3d20 6472 795f 7275 6e0a 2020 2020 2020  = dry_run.      
-0004b630: 2020 7365 6c66 2e6e 616d 6520 3d20 6e61    self.name = na
-0004b640: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-0004b650: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
-0004b660: 6f6e 6e65 6374 6f72 5f67 726f 7570 5f69  onnector_group_i
-0004b670: 6420 3d20 7769 7265 6c65 7373 5f63 6c6f  d = wireless_clo
-0004b680: 7564 5f63 6f6e 6e65 6374 6f72 5f67 726f  ud_connector_gro
-0004b690: 7570 5f69 640a 0a20 2020 2064 6566 2076  up_id..    def v
-0004b6a0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0004b6b0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0004b6c0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0004b6d0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0004b6e0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-0004b6f0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0004b700: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0004b710: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0004b720: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0004b730: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0004b740: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0004b750: 2e63 6c69 656e 745f 746f 6b65 6e20 6973  .client_token is
-0004b760: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004b770: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-0004b780: 6c69 656e 7454 6f6b 656e 275d 203d 2073  lientToken'] = s
-0004b790: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-0004b7a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0004b7b0: 2e64 6573 6372 6970 7469 6f6e 2069 7320  .description is 
-0004b7c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004b7d0: 2020 2020 2020 7265 7375 6c74 5b27 4465        result['De
-0004b7e0: 7363 7269 7074 696f 6e27 5d20 3d20 7365  scription'] = se
-0004b7f0: 6c66 2e64 6573 6372 6970 7469 6f6e 0a20  lf.description. 
-0004b800: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-0004b810: 7279 5f72 756e 2069 7320 6e6f 7420 4e6f  ry_run is not No
-0004b820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004b830: 7265 7375 6c74 5b27 4472 7952 756e 275d  result['DryRun']
-0004b840: 203d 2073 656c 662e 6472 795f 7275 6e0a   = self.dry_run.
-0004b850: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0004b860: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0004b870: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0004b880: 7375 6c74 5b27 4e61 6d65 275d 203d 2073  sult['Name'] = s
-0004b890: 656c 662e 6e61 6d65 0a20 2020 2020 2020  elf.name.       
-0004b8a0: 2069 6620 7365 6c66 2e77 6972 656c 6573   if self.wireles
-0004b8b0: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
-0004b8c0: 725f 6772 6f75 705f 6964 2069 7320 6e6f  r_group_id is no
-0004b8d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004b8e0: 2020 2020 7265 7375 6c74 5b27 5769 7265      result['Wire
-0004b8f0: 6c65 7373 436c 6f75 6443 6f6e 6e65 6374  lessCloudConnect
-0004b900: 6f72 4772 6f75 7049 6427 5d20 3d20 7365  orGroupId'] = se
-0004b910: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
-0004b920: 645f 636f 6e6e 6563 746f 725f 6772 6f75  d_connector_grou
-0004b930: 705f 6964 0a20 2020 2020 2020 2072 6574  p_id.        ret
-0004b940: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0004b950: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0004b960: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0004b970: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0004b980: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0004b990: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-0004b9a0: 6965 6e74 546f 6b65 6e27 2920 6973 206e  ientToken') is n
-0004b9b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0004b9c0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-0004b9d0: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-0004b9e0: 436c 6965 6e74 546f 6b65 6e27 290a 2020  ClientToken').  
-0004b9f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0004ba00: 4465 7363 7269 7074 696f 6e27 2920 6973  Description') is
-0004ba10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0004ba20: 2020 2020 2020 2073 656c 662e 6465 7363         self.desc
-0004ba30: 7269 7074 696f 6e20 3d20 6d2e 6765 7428  ription = m.get(
-0004ba40: 2744 6573 6372 6970 7469 6f6e 2729 0a20  'Description'). 
-0004ba50: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0004ba60: 2744 7279 5275 6e27 2920 6973 206e 6f74  'DryRun') is not
-0004ba70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004ba80: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
-0004ba90: 3d20 6d2e 6765 7428 2744 7279 5275 6e27  = m.get('DryRun'
-0004baa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0004bab0: 6574 2827 4e61 6d65 2729 2069 7320 6e6f  et('Name') is no
-0004bac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0004bad0: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-0004bae0: 6d2e 6765 7428 274e 616d 6527 290a 2020  m.get('Name').  
-0004baf0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0004bb00: 5769 7265 6c65 7373 436c 6f75 6443 6f6e  WirelessCloudCon
-0004bb10: 6e65 6374 6f72 4772 6f75 7049 6427 2920  nectorGroupId') 
-0004bb20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0004bb30: 2020 2020 2020 2020 2073 656c 662e 7769           self.wi
-0004bb40: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
-0004bb50: 6e65 6374 6f72 5f67 726f 7570 5f69 6420  nector_group_id 
-0004bb60: 3d20 6d2e 6765 7428 2757 6972 656c 6573  = m.get('Wireles
-0004bb70: 7343 6c6f 7564 436f 6e6e 6563 746f 7247  sCloudConnectorG
-0004bb80: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
-0004bb90: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0004bba0: 6c61 7373 2055 7064 6174 6557 6972 656c  lass UpdateWirel
-0004bbb0: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
-0004bbc0: 7247 726f 7570 5265 7370 6f6e 7365 426f  rGroupResponseBo
-0004bbd0: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
-0004bbe0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-0004bbf0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0004bc00: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
-0004bc10: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0004bc20: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-0004bc30: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
-0004bc40: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
-0004bc50: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0004bc60: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0004bc70: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0004bc80: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0004bc90: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0004bca0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0004bcb0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0004bcc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004bcd0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0004bce0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0004bcf0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0004bd00: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0004bd10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0004bd20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0004bd30: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
-0004bd40: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
-0004bd50: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0004bd60: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0004bd70: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0004bd80: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0004bd90: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0004bda0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0004bdb0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0004bdc0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0004bdd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0004bde0: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-0004bdf0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0004be00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0004be10: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-0004be20: 6461 7465 5769 7265 6c65 7373 436c 6f75  dateWirelessClou
-0004be30: 6443 6f6e 6e65 6374 6f72 4772 6f75 7052  dConnectorGroupR
-0004be40: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-0004be50: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0004be60: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0004be70: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-0004be80: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-0004be90: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0004bea0: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-0004beb0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-0004bec0: 2020 2020 626f 6479 3a20 5570 6461 7465      body: Update
-0004bed0: 5769 7265 6c65 7373 436c 6f75 6443 6f6e  WirelessCloudCon
-0004bee0: 6e65 6374 6f72 4772 6f75 7052 6573 706f  nectorGroupRespo
-0004bef0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-0004bf00: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0004bf10: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-0004bf20: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-0004bf30: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0004bf40: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-0004bf50: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0004bf60: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-0004bf70: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0004bf80: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0004bf90: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0004bfa0: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-0004bfb0: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-0004bfc0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0004bfd0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-0004bfe0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-0004bff0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-0004c000: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0004c010: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-0004c020: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-0004c030: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+00043150: 7320 556e 6c6f 636b 4361 7264 7352 6571  s UnlockCardsReq
+00043160: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00043170: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00043180: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00043190: 2020 2020 2020 2020 636c 6965 6e74 5f74          client_t
+000431a0: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
+000431b0: 2c0a 2020 2020 2020 2020 6472 795f 7275  ,.        dry_ru
+000431c0: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
+000431d0: 2020 2020 2020 2020 6963 6369 6473 3a20          iccids: 
+000431e0: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
+000431f0: 2c0a 2020 2020 2020 2020 7265 6769 6f6e  ,.        region
+00043200: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00043210: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00043220: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00043230: 6e20 3d20 636c 6965 6e74 5f74 6f6b 656e  n = client_token
+00043240: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
+00043250: 795f 7275 6e20 3d20 6472 795f 7275 6e0a  y_run = dry_run.
+00043260: 2020 2020 2020 2020 7365 6c66 2e69 6363          self.icc
+00043270: 6964 7320 3d20 6963 6369 6473 0a20 2020  ids = iccids.   
+00043280: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
+00043290: 5f69 6420 3d20 7265 6769 6f6e 5f69 640a  _id = region_id.
+000432a0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000432b0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000432c0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000432d0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000432e0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000432f0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00043300: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00043310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00043320: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00043330: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00043340: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00043350: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
+00043360: 745f 746f 6b65 6e20 6973 206e 6f74 204e  t_token is not N
+00043370: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043380: 2072 6573 756c 745b 2743 6c69 656e 7454   result['ClientT
+00043390: 6f6b 656e 275d 203d 2073 656c 662e 636c  oken'] = self.cl
+000433a0: 6965 6e74 5f74 6f6b 656e 0a20 2020 2020  ient_token.     
+000433b0: 2020 2069 6620 7365 6c66 2e64 7279 5f72     if self.dry_r
+000433c0: 756e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  un is not None:.
+000433d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000433e0: 6c74 5b27 4472 7952 756e 275d 203d 2073  lt['DryRun'] = s
+000433f0: 656c 662e 6472 795f 7275 6e0a 2020 2020  elf.dry_run.    
+00043400: 2020 2020 6966 2073 656c 662e 6963 6369      if self.icci
+00043410: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
+00043420: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00043430: 6c74 5b27 4963 6369 6473 275d 203d 2073  lt['Iccids'] = s
+00043440: 656c 662e 6963 6369 6473 0a20 2020 2020  elf.iccids.     
+00043450: 2020 2069 6620 7365 6c66 2e72 6567 696f     if self.regio
+00043460: 6e5f 6964 2069 7320 6e6f 7420 4e6f 6e65  n_id is not None
+00043470: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00043480: 7375 6c74 5b27 5265 6769 6f6e 4964 275d  sult['RegionId']
+00043490: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
+000434a0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+000434b0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+000434c0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000434d0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+000434e0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000434f0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00043500: 2069 6620 6d2e 6765 7428 2743 6c69 656e   if m.get('Clien
+00043510: 7454 6f6b 656e 2729 2069 7320 6e6f 7420  tToken') is not 
+00043520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00043530: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
+00043540: 6b65 6e20 3d20 6d2e 6765 7428 2743 6c69  ken = m.get('Cli
+00043550: 656e 7454 6f6b 656e 2729 0a20 2020 2020  entToken').     
+00043560: 2020 2069 6620 6d2e 6765 7428 2744 7279     if m.get('Dry
+00043570: 5275 6e27 2920 6973 206e 6f74 204e 6f6e  Run') is not Non
+00043580: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00043590: 656c 662e 6472 795f 7275 6e20 3d20 6d2e  elf.dry_run = m.
+000435a0: 6765 7428 2744 7279 5275 6e27 290a 2020  get('DryRun').  
+000435b0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000435c0: 4963 6369 6473 2729 2069 7320 6e6f 7420  Iccids') is not 
+000435d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000435e0: 2020 7365 6c66 2e69 6363 6964 7320 3d20    self.iccids = 
+000435f0: 6d2e 6765 7428 2749 6363 6964 7327 290a  m.get('Iccids').
+00043600: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00043610: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
+00043620: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00043630: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+00043640: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
+00043650: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
+00043660: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00043670: 6c61 7373 2055 6e6c 6f63 6b43 6172 6473  lass UnlockCards
+00043680: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+00043690: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000436a0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000436b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000436c0: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
+000436d0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+000436e0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000436f0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
+00043700: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+00043710: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00043720: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00043730: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00043740: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00043750: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00043760: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00043770: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00043780: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00043790: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000437a0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+000437b0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000437c0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+000437d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000437e0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+000437f0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+00043800: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+00043810: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00043820: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00043830: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00043840: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00043850: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00043860: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00043870: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+00043880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00043890: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000438a0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+000438b0: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+000438c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000438d0: 0a0a 636c 6173 7320 556e 6c6f 636b 4361  ..class UnlockCa
+000438e0: 7264 7352 6573 706f 6e73 6528 5465 614d  rdsResponse(TeaM
+000438f0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00043900: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00043910: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
+00043920: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
+00043930: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
+00043940: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
+00043950: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
+00043960: 2020 2020 2020 2020 626f 6479 3a20 556e          body: Un
+00043970: 6c6f 636b 4361 7264 7352 6573 706f 6e73  lockCardsRespons
+00043980: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+00043990: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000439a0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000439b0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000439c0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000439d0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000439e0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000439f0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00043a00: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00043a10: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00043a20: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00043a30: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00043a40: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00043a50: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00043a60: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00043a70: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00043a80: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00043a90: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00043aa0: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00043ab0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00043ac0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+00043ad0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00043ae0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+00043af0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00043b00: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00043b10: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00043b20: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00043b30: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00043b40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00043b50: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00043b60: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00043b70: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00043b80: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00043b90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00043ba0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00043bb0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00043bc0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00043bd0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00043be0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00043bf0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00043c00: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00043c10: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00043c20: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00043c30: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00043c40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00043c50: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00043c60: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00043c70: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00043c80: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00043c90: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00043ca0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+00043cb0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00043cc0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00043cd0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+00043ce0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+00043cf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00043d00: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+00043d10: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+00043d20: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00043d30: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+00043d40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00043d50: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00043d60: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+00043d70: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+00043d80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00043d90: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00043da0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00043db0: 2074 656d 705f 6d6f 6465 6c20 3d20 556e   temp_model = Un
+00043dc0: 6c6f 636b 4361 7264 7352 6573 706f 6e73  lockCardsRespons
+00043dd0: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
+00043de0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00043df0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00043e00: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00043e10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00043e20: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+00043e30: 6541 7574 686f 7269 7a61 7469 6f6e 5275  eAuthorizationRu
+00043e40: 6c65 5265 7175 6573 7428 5465 614d 6f64  leRequest(TeaMod
+00043e50: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00043e60: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00043e70: 656c 662c 0a20 2020 2020 2020 2061 7574  elf,.        aut
+00043e80: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
+00043e90: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00043ea0: 2020 2020 2020 2020 636c 6965 6e74 5f74          client_t
+00043eb0: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
+00043ec0: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
+00043ed0: 7074 696f 6e3a 2073 7472 203d 204e 6f6e  ption: str = Non
+00043ee0: 652c 0a20 2020 2020 2020 2064 6573 7469  e,.        desti
+00043ef0: 6e61 7469 6f6e 3a20 7374 7220 3d20 4e6f  nation: str = No
+00043f00: 6e65 2c0a 2020 2020 2020 2020 6465 7374  ne,.        dest
+00043f10: 696e 6174 696f 6e5f 706f 7274 3a20 7374  ination_port: st
+00043f20: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00043f30: 2020 6472 795f 7275 6e3a 2062 6f6f 6c20    dry_run: bool 
+00043f40: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00043f50: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+00043f60: 2c0a 2020 2020 2020 2020 706f 6c69 6379  ,.        policy
+00043f70: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00043f80: 2020 2020 2020 7072 6f74 6f63 6f6c 3a20        protocol: 
+00043f90: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00043fa0: 2020 2020 736f 7572 6365 5f63 6964 723a      source_cidr:
+00043fb0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00043fc0: 2020 2020 2077 6972 656c 6573 735f 636c       wireless_cl
+00043fd0: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+00043fe0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00043ff0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00044000: 662e 6175 7468 6f72 697a 6174 696f 6e5f  f.authorization_
+00044010: 7275 6c65 5f69 6420 3d20 6175 7468 6f72  rule_id = author
+00044020: 697a 6174 696f 6e5f 7275 6c65 5f69 640a  ization_rule_id.
+00044030: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+00044040: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
+00044050: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+00044060: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+00044070: 6e20 3d20 6465 7363 7269 7074 696f 6e0a  n = description.
+00044080: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
+00044090: 7469 6e61 7469 6f6e 203d 2064 6573 7469  tination = desti
+000440a0: 6e61 7469 6f6e 0a20 2020 2020 2020 2073  nation.        s
+000440b0: 656c 662e 6465 7374 696e 6174 696f 6e5f  elf.destination_
+000440c0: 706f 7274 203d 2064 6573 7469 6e61 7469  port = destinati
+000440d0: 6f6e 5f70 6f72 740a 2020 2020 2020 2020  on_port.        
+000440e0: 7365 6c66 2e64 7279 5f72 756e 203d 2064  self.dry_run = d
+000440f0: 7279 5f72 756e 0a20 2020 2020 2020 2073  ry_run.        s
+00044100: 656c 662e 6e61 6d65 203d 206e 616d 650a  elf.name = name.
+00044110: 2020 2020 2020 2020 7365 6c66 2e70 6f6c          self.pol
+00044120: 6963 7920 3d20 706f 6c69 6379 0a20 2020  icy = policy.   
+00044130: 2020 2020 2073 656c 662e 7072 6f74 6f63       self.protoc
+00044140: 6f6c 203d 2070 726f 746f 636f 6c0a 2020  ol = protocol.  
+00044150: 2020 2020 2020 7365 6c66 2e73 6f75 7263        self.sourc
+00044160: 655f 6369 6472 203d 2073 6f75 7263 655f  e_cidr = source_
+00044170: 6369 6472 0a20 2020 2020 2020 2073 656c  cidr.        sel
+00044180: 662e 7769 7265 6c65 7373 5f63 6c6f 7564  f.wireless_cloud
+00044190: 5f63 6f6e 6e65 6374 6f72 5f69 6420 3d20  _connector_id = 
+000441a0: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+000441b0: 6f6e 6e65 6374 6f72 5f69 640a 0a20 2020  onnector_id..   
+000441c0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000441d0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000441e0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+000441f0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00044200: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00044210: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00044220: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00044230: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00044240: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00044250: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00044260: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00044270: 6620 7365 6c66 2e61 7574 686f 7269 7a61  f self.authoriza
+00044280: 7469 6f6e 5f72 756c 655f 6964 2069 7320  tion_rule_id is 
+00044290: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000442a0: 2020 2020 2020 7265 7375 6c74 5b27 4175        result['Au
+000442b0: 7468 6f72 697a 6174 696f 6e52 756c 6549  thorizationRuleI
+000442c0: 6427 5d20 3d20 7365 6c66 2e61 7574 686f  d'] = self.autho
+000442d0: 7269 7a61 7469 6f6e 5f72 756c 655f 6964  rization_rule_id
+000442e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000442f0: 2e63 6c69 656e 745f 746f 6b65 6e20 6973  .client_token is
+00044300: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044310: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
+00044320: 6c69 656e 7454 6f6b 656e 275d 203d 2073  lientToken'] = s
+00044330: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
+00044340: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00044350: 2e64 6573 6372 6970 7469 6f6e 2069 7320  .description is 
+00044360: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00044370: 2020 2020 2020 7265 7375 6c74 5b27 4465        result['De
+00044380: 7363 7269 7074 696f 6e27 5d20 3d20 7365  scription'] = se
+00044390: 6c66 2e64 6573 6372 6970 7469 6f6e 0a20  lf.description. 
+000443a0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+000443b0: 6573 7469 6e61 7469 6f6e 2069 7320 6e6f  estination is no
+000443c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000443d0: 2020 2020 7265 7375 6c74 5b27 4465 7374      result['Dest
+000443e0: 696e 6174 696f 6e27 5d20 3d20 7365 6c66  ination'] = self
+000443f0: 2e64 6573 7469 6e61 7469 6f6e 0a20 2020  .destination.   
+00044400: 2020 2020 2069 6620 7365 6c66 2e64 6573       if self.des
+00044410: 7469 6e61 7469 6f6e 5f70 6f72 7420 6973  tination_port is
+00044420: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044430: 2020 2020 2020 2072 6573 756c 745b 2744         result['D
+00044440: 6573 7469 6e61 7469 6f6e 506f 7274 275d  estinationPort']
+00044450: 203d 2073 656c 662e 6465 7374 696e 6174   = self.destinat
+00044460: 696f 6e5f 706f 7274 0a20 2020 2020 2020  ion_port.       
+00044470: 2069 6620 7365 6c66 2e64 7279 5f72 756e   if self.dry_run
+00044480: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044490: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000444a0: 5b27 4472 7952 756e 275d 203d 2073 656c  ['DryRun'] = sel
+000444b0: 662e 6472 795f 7275 6e0a 2020 2020 2020  f.dry_run.      
+000444c0: 2020 6966 2073 656c 662e 6e61 6d65 2069    if self.name i
+000444d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000444e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000444f0: 4e61 6d65 275d 203d 2073 656c 662e 6e61  Name'] = self.na
+00044500: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+00044510: 6c66 2e70 6f6c 6963 7920 6973 206e 6f74  lf.policy is not
+00044520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00044530: 2020 2072 6573 756c 745b 2750 6f6c 6963     result['Polic
+00044540: 7927 5d20 3d20 7365 6c66 2e70 6f6c 6963  y'] = self.polic
+00044550: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+00044560: 662e 7072 6f74 6f63 6f6c 2069 7320 6e6f  f.protocol is no
+00044570: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00044580: 2020 2020 7265 7375 6c74 5b27 5072 6f74      result['Prot
+00044590: 6f63 6f6c 275d 203d 2073 656c 662e 7072  ocol'] = self.pr
+000445a0: 6f74 6f63 6f6c 0a20 2020 2020 2020 2069  otocol.        i
+000445b0: 6620 7365 6c66 2e73 6f75 7263 655f 6369  f self.source_ci
+000445c0: 6472 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dr is not None:.
+000445d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000445e0: 6c74 5b27 536f 7572 6365 4369 6472 275d  lt['SourceCidr']
+000445f0: 203d 2073 656c 662e 736f 7572 6365 5f63   = self.source_c
+00044600: 6964 720a 2020 2020 2020 2020 6966 2073  idr.        if s
+00044610: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
+00044620: 7564 5f63 6f6e 6e65 6374 6f72 5f69 6420  ud_connector_id 
+00044630: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00044640: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00044650: 2757 6972 656c 6573 7343 6c6f 7564 436f  'WirelessCloudCo
+00044660: 6e6e 6563 746f 7249 6427 5d20 3d20 7365  nnectorId'] = se
+00044670: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
+00044680: 645f 636f 6e6e 6563 746f 725f 6964 0a20  d_connector_id. 
+00044690: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000446a0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000446b0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000446c0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000446d0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000446e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000446f0: 206d 2e67 6574 2827 4175 7468 6f72 697a   m.get('Authoriz
+00044700: 6174 696f 6e52 756c 6549 6427 2920 6973  ationRuleId') is
+00044710: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044720: 2020 2020 2020 2073 656c 662e 6175 7468         self.auth
+00044730: 6f72 697a 6174 696f 6e5f 7275 6c65 5f69  orization_rule_i
+00044740: 6420 3d20 6d2e 6765 7428 2741 7574 686f  d = m.get('Autho
+00044750: 7269 7a61 7469 6f6e 5275 6c65 4964 2729  rizationRuleId')
+00044760: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00044770: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
+00044780: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044790: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000447a0: 6c69 656e 745f 746f 6b65 6e20 3d20 6d2e  lient_token = m.
+000447b0: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
+000447c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000447d0: 6765 7428 2744 6573 6372 6970 7469 6f6e  get('Description
+000447e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000447f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00044800: 2e64 6573 6372 6970 7469 6f6e 203d 206d  .description = m
+00044810: 2e67 6574 2827 4465 7363 7269 7074 696f  .get('Descriptio
+00044820: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
+00044830: 2e67 6574 2827 4465 7374 696e 6174 696f  .get('Destinatio
+00044840: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+00044850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00044860: 662e 6465 7374 696e 6174 696f 6e20 3d20  f.destination = 
+00044870: 6d2e 6765 7428 2744 6573 7469 6e61 7469  m.get('Destinati
+00044880: 6f6e 2729 0a20 2020 2020 2020 2069 6620  on').        if 
+00044890: 6d2e 6765 7428 2744 6573 7469 6e61 7469  m.get('Destinati
+000448a0: 6f6e 506f 7274 2729 2069 7320 6e6f 7420  onPort') is not 
+000448b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000448c0: 2020 7365 6c66 2e64 6573 7469 6e61 7469    self.destinati
+000448d0: 6f6e 5f70 6f72 7420 3d20 6d2e 6765 7428  on_port = m.get(
+000448e0: 2744 6573 7469 6e61 7469 6f6e 506f 7274  'DestinationPort
+000448f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00044900: 6765 7428 2744 7279 5275 6e27 2920 6973  get('DryRun') is
+00044910: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00044920: 2020 2020 2020 2073 656c 662e 6472 795f         self.dry_
+00044930: 7275 6e20 3d20 6d2e 6765 7428 2744 7279  run = m.get('Dry
+00044940: 5275 6e27 290a 2020 2020 2020 2020 6966  Run').        if
+00044950: 206d 2e67 6574 2827 4e61 6d65 2729 2069   m.get('Name') i
+00044960: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00044970: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+00044980: 6520 3d20 6d2e 6765 7428 274e 616d 6527  e = m.get('Name'
+00044990: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000449a0: 6574 2827 506f 6c69 6379 2729 2069 7320  et('Policy') is 
+000449b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000449c0: 2020 2020 2020 7365 6c66 2e70 6f6c 6963        self.polic
+000449d0: 7920 3d20 6d2e 6765 7428 2750 6f6c 6963  y = m.get('Polic
+000449e0: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+000449f0: 2e67 6574 2827 5072 6f74 6f63 6f6c 2729  .get('Protocol')
+00044a00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00044a10: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00044a20: 726f 746f 636f 6c20 3d20 6d2e 6765 7428  rotocol = m.get(
+00044a30: 2750 726f 746f 636f 6c27 290a 2020 2020  'Protocol').    
+00044a40: 2020 2020 6966 206d 2e67 6574 2827 536f      if m.get('So
+00044a50: 7572 6365 4369 6472 2729 2069 7320 6e6f  urceCidr') is no
+00044a60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00044a70: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
+00044a80: 6369 6472 203d 206d 2e67 6574 2827 536f  cidr = m.get('So
+00044a90: 7572 6365 4369 6472 2729 0a20 2020 2020  urceCidr').     
+00044aa0: 2020 2069 6620 6d2e 6765 7428 2757 6972     if m.get('Wir
+00044ab0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+00044ac0: 746f 7249 6427 2920 6973 206e 6f74 204e  torId') is not N
+00044ad0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00044ae0: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
+00044af0: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
+00044b00: 6420 3d20 6d2e 6765 7428 2757 6972 656c  d = m.get('Wirel
+00044b10: 6573 7343 6c6f 7564 436f 6e6e 6563 746f  essCloudConnecto
+00044b20: 7249 6427 290a 2020 2020 2020 2020 7265  rId').        re
+00044b30: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00044b40: 7320 5570 6461 7465 4175 7468 6f72 697a  s UpdateAuthoriz
+00044b50: 6174 696f 6e52 756c 6552 6573 706f 6e73  ationRuleRespons
+00044b60: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+00044b70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00044b80: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00044b90: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00044ba0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00044bb0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00044bc0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00044bd0: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
+00044be0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00044bf0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00044c00: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00044c10: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00044c20: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00044c30: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00044c40: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00044c50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00044c60: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00044c70: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00044c80: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00044c90: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+00044ca0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00044cb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00044cc0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+00044cd0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+00044ce0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00044cf0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00044d00: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00044d10: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00044d20: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00044d30: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00044d40: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+00044d50: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+00044d60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00044d70: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00044d80: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+00044d90: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00044da0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00044db0: 2055 7064 6174 6541 7574 686f 7269 7a61   UpdateAuthoriza
+00044dc0: 7469 6f6e 5275 6c65 5265 7370 6f6e 7365  tionRuleResponse
+00044dd0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00044de0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00044df0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00044e00: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+00044e10: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+00044e20: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+00044e30: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+00044e40: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+00044e50: 793a 2055 7064 6174 6541 7574 686f 7269  y: UpdateAuthori
+00044e60: 7a61 7469 6f6e 5275 6c65 5265 7370 6f6e  zationRuleRespon
+00044e70: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
+00044e80: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00044e90: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+00044ea0: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+00044eb0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00044ec0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00044ed0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00044ee0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+00044ef0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00044f00: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+00044f10: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+00044f20: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
+00044f30: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
+00044f40: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+00044f50: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
+00044f60: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
+00044f70: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
+00044f80: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+00044f90: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
+00044fa0: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
+00044fb0: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00044fc0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00044fd0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00044fe0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00044ff0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00045000: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00045010: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00045020: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00045030: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00045040: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00045050: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00045060: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00045070: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+00045080: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00045090: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000450a0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000450b0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000450c0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000450d0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000450e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000450f0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+00045100: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+00045110: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+00045120: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+00045130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00045140: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00045150: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00045160: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00045170: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00045180: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00045190: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000451a0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000451b0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000451c0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000451d0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000451e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000451f0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00045200: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00045210: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00045220: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00045230: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00045240: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00045250: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00045260: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00045270: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00045280: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00045290: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000452a0: 2020 7465 6d70 5f6d 6f64 656c 203d 2055    temp_model = U
+000452b0: 7064 6174 6541 7574 686f 7269 7a61 7469  pdateAuthorizati
+000452c0: 6f6e 5275 6c65 5265 7370 6f6e 7365 426f  onRuleResponseBo
+000452d0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+000452e0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+000452f0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00045300: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00045310: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00045320: 0a0a 636c 6173 7320 5570 6461 7465 4261  ..class UpdateBa
+00045330: 7463 684f 7065 7261 7465 4361 7264 7354  tchOperateCardsT
+00045340: 6173 6b52 6571 7565 7374 2854 6561 4d6f  askRequest(TeaMo
+00045350: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00045360: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00045370: 7365 6c66 2c0a 2020 2020 2020 2020 6261  self,.        ba
+00045380: 7463 685f 6f70 6572 6174 655f 6361 7264  tch_operate_card
+00045390: 735f 7461 736b 5f69 643a 2073 7472 203d  s_task_id: str =
+000453a0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
+000453b0: 6c69 656e 745f 746f 6b65 6e3a 2073 7472  lient_token: str
+000453c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000453d0: 2064 6573 6372 6970 7469 6f6e 3a20 7374   description: st
+000453e0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000453f0: 2020 6472 795f 7275 6e3a 2062 6f6f 6c20    dry_run: bool 
+00045400: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00045410: 6566 6665 6374 5f74 7970 653a 2073 7472  effect_type: str
+00045420: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00045430: 2069 6363 6964 733a 204c 6973 745b 7374   iccids: List[st
+00045440: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00045450: 2020 2069 6363 6964 735f 6f73 735f 6669     iccids_oss_fi
+00045460: 6c65 5f70 6174 683a 2073 7472 203d 204e  le_path: str = N
+00045470: 6f6e 652c 0a20 2020 2020 2020 206e 616d  one,.        nam
+00045480: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00045490: 2020 2020 2020 206f 7065 7261 7465 5f74         operate_t
+000454a0: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
+000454b0: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
+000454c0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+000454d0: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
+000454e0: 643a 2069 6e74 203d 204e 6f6e 652c 0a20  d: int = None,. 
+000454f0: 2020 2020 2020 2077 6972 656c 6573 735f         wireless_
+00045500: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
+00045510: 6964 733a 204c 6973 745b 7374 725d 203d  ids: List[str] =
+00045520: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00045530: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
+00045540: 5f6f 7065 7261 7465 5f63 6172 6473 5f74  _operate_cards_t
+00045550: 6173 6b5f 6964 203d 2062 6174 6368 5f6f  ask_id = batch_o
+00045560: 7065 7261 7465 5f63 6172 6473 5f74 6173  perate_cards_tas
+00045570: 6b5f 6964 0a20 2020 2020 2020 2073 656c  k_id.        sel
+00045580: 662e 636c 6965 6e74 5f74 6f6b 656e 203d  f.client_token =
+00045590: 2063 6c69 656e 745f 746f 6b65 6e0a 2020   client_token.  
+000455a0: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
+000455b0: 6970 7469 6f6e 203d 2064 6573 6372 6970  iption = descrip
+000455c0: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
+000455d0: 662e 6472 795f 7275 6e20 3d20 6472 795f  f.dry_run = dry_
+000455e0: 7275 6e0a 2020 2020 2020 2020 7365 6c66  run.        self
+000455f0: 2e65 6666 6563 745f 7479 7065 203d 2065  .effect_type = e
+00045600: 6666 6563 745f 7479 7065 0a20 2020 2020  ffect_type.     
+00045610: 2020 2073 656c 662e 6963 6369 6473 203d     self.iccids =
+00045620: 2069 6363 6964 730a 2020 2020 2020 2020   iccids.        
+00045630: 7365 6c66 2e69 6363 6964 735f 6f73 735f  self.iccids_oss_
+00045640: 6669 6c65 5f70 6174 6820 3d20 6963 6369  file_path = icci
+00045650: 6473 5f6f 7373 5f66 696c 655f 7061 7468  ds_oss_file_path
+00045660: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
+00045670: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
+00045680: 2020 7365 6c66 2e6f 7065 7261 7465 5f74    self.operate_t
+00045690: 7970 6520 3d20 6f70 6572 6174 655f 7479  ype = operate_ty
+000456a0: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
+000456b0: 7265 6769 6f6e 5f69 6420 3d20 7265 6769  region_id = regi
+000456c0: 6f6e 5f69 640a 2020 2020 2020 2020 7365  on_id.        se
+000456d0: 6c66 2e74 6872 6573 686f 6c64 203d 2074  lf.threshold = t
+000456e0: 6872 6573 686f 6c64 0a20 2020 2020 2020  hreshold.       
+000456f0: 2073 656c 662e 7769 7265 6c65 7373 5f63   self.wireless_c
+00045700: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
+00045710: 6473 203d 2077 6972 656c 6573 735f 636c  ds = wireless_cl
+00045720: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+00045730: 730a 0a20 2020 2064 6566 2076 616c 6964  s..    def valid
+00045740: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00045750: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00045760: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00045770: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00045780: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00045790: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000457a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000457b0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000457c0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000457d0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000457e0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+000457f0: 6368 5f6f 7065 7261 7465 5f63 6172 6473  ch_operate_cards
+00045800: 5f74 6173 6b5f 6964 2069 7320 6e6f 7420  _task_id is not 
+00045810: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00045820: 2020 7265 7375 6c74 5b27 4261 7463 684f    result['BatchO
+00045830: 7065 7261 7465 4361 7264 7354 6173 6b49  perateCardsTaskI
+00045840: 6427 5d20 3d20 7365 6c66 2e62 6174 6368  d'] = self.batch
+00045850: 5f6f 7065 7261 7465 5f63 6172 6473 5f74  _operate_cards_t
+00045860: 6173 6b5f 6964 0a20 2020 2020 2020 2069  ask_id.        i
+00045870: 6620 7365 6c66 2e63 6c69 656e 745f 746f  f self.client_to
+00045880: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
+00045890: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000458a0: 756c 745b 2743 6c69 656e 7454 6f6b 656e  ult['ClientToken
+000458b0: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
+000458c0: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
+000458d0: 6620 7365 6c66 2e64 6573 6372 6970 7469  f self.descripti
+000458e0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+000458f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00045900: 6c74 5b27 4465 7363 7269 7074 696f 6e27  lt['Description'
+00045910: 5d20 3d20 7365 6c66 2e64 6573 6372 6970  ] = self.descrip
+00045920: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+00045930: 7365 6c66 2e64 7279 5f72 756e 2069 7320  self.dry_run is 
+00045940: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045950: 2020 2020 2020 7265 7375 6c74 5b27 4472        result['Dr
+00045960: 7952 756e 275d 203d 2073 656c 662e 6472  yRun'] = self.dr
+00045970: 795f 7275 6e0a 2020 2020 2020 2020 6966  y_run.        if
+00045980: 2073 656c 662e 6566 6665 6374 5f74 7970   self.effect_typ
+00045990: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000459a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000459b0: 745b 2745 6666 6563 7454 7970 6527 5d20  t['EffectType'] 
+000459c0: 3d20 7365 6c66 2e65 6666 6563 745f 7479  = self.effect_ty
+000459d0: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+000459e0: 6c66 2e69 6363 6964 7320 6973 206e 6f74  lf.iccids is not
+000459f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00045a00: 2020 2072 6573 756c 745b 2749 6363 6964     result['Iccid
+00045a10: 7327 5d20 3d20 7365 6c66 2e69 6363 6964  s'] = self.iccid
+00045a20: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00045a30: 662e 6963 6369 6473 5f6f 7373 5f66 696c  f.iccids_oss_fil
+00045a40: 655f 7061 7468 2069 7320 6e6f 7420 4e6f  e_path is not No
+00045a50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00045a60: 7265 7375 6c74 5b27 4963 6369 6473 4f73  result['IccidsOs
+00045a70: 7346 696c 6550 6174 6827 5d20 3d20 7365  sFilePath'] = se
+00045a80: 6c66 2e69 6363 6964 735f 6f73 735f 6669  lf.iccids_oss_fi
+00045a90: 6c65 5f70 6174 680a 2020 2020 2020 2020  le_path.        
+00045aa0: 6966 2073 656c 662e 6e61 6d65 2069 7320  if self.name is 
+00045ab0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045ac0: 2020 2020 2020 7265 7375 6c74 5b27 4e61        result['Na
+00045ad0: 6d65 275d 203d 2073 656c 662e 6e61 6d65  me'] = self.name
+00045ae0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00045af0: 2e6f 7065 7261 7465 5f74 7970 6520 6973  .operate_type is
+00045b00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00045b10: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
+00045b20: 7065 7261 7465 5479 7065 275d 203d 2073  perateType'] = s
+00045b30: 656c 662e 6f70 6572 6174 655f 7479 7065  elf.operate_type
+00045b40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00045b50: 2e72 6567 696f 6e5f 6964 2069 7320 6e6f  .region_id is no
+00045b60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00045b70: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
+00045b80: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
+00045b90: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+00045ba0: 6966 2073 656c 662e 7468 7265 7368 6f6c  if self.threshol
+00045bb0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00045bc0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00045bd0: 745b 2754 6872 6573 686f 6c64 275d 203d  t['Threshold'] =
+00045be0: 2073 656c 662e 7468 7265 7368 6f6c 640a   self.threshold.
+00045bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00045c00: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+00045c10: 6f6e 6e65 6374 6f72 5f69 6473 2069 7320  onnector_ids is 
+00045c20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00045c30: 2020 2020 2020 7265 7375 6c74 5b27 5769        result['Wi
+00045c40: 7265 6c65 7373 436c 6f75 6443 6f6e 6e65  relessCloudConne
+00045c50: 6374 6f72 4964 7327 5d20 3d20 7365 6c66  ctorIds'] = self
+00045c60: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+00045c70: 636f 6e6e 6563 746f 725f 6964 730a 2020  connector_ids.  
+00045c80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00045c90: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00045ca0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00045cb0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00045cc0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00045cd0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00045ce0: 6d2e 6765 7428 2742 6174 6368 4f70 6572  m.get('BatchOper
+00045cf0: 6174 6543 6172 6473 5461 736b 4964 2729  ateCardsTaskId')
+00045d00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00045d10: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00045d20: 6174 6368 5f6f 7065 7261 7465 5f63 6172  atch_operate_car
+00045d30: 6473 5f74 6173 6b5f 6964 203d 206d 2e67  ds_task_id = m.g
+00045d40: 6574 2827 4261 7463 684f 7065 7261 7465  et('BatchOperate
+00045d50: 4361 7264 7354 6173 6b49 6427 290a 2020  CardsTaskId').  
+00045d60: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00045d70: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
+00045d80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00045d90: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00045da0: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
+00045db0: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
+00045dc0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00045dd0: 2827 4465 7363 7269 7074 696f 6e27 2920  ('Description') 
+00045de0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00045df0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00045e00: 7363 7269 7074 696f 6e20 3d20 6d2e 6765  scription = m.ge
+00045e10: 7428 2744 6573 6372 6970 7469 6f6e 2729  t('Description')
+00045e20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00045e30: 7428 2744 7279 5275 6e27 2920 6973 206e  t('DryRun') is n
+00045e40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00045e50: 2020 2020 2073 656c 662e 6472 795f 7275       self.dry_ru
+00045e60: 6e20 3d20 6d2e 6765 7428 2744 7279 5275  n = m.get('DryRu
+00045e70: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
+00045e80: 2e67 6574 2827 4566 6665 6374 5479 7065  .get('EffectType
+00045e90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00045ea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00045eb0: 2e65 6666 6563 745f 7479 7065 203d 206d  .effect_type = m
+00045ec0: 2e67 6574 2827 4566 6665 6374 5479 7065  .get('EffectType
+00045ed0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00045ee0: 6765 7428 2749 6363 6964 7327 2920 6973  get('Iccids') is
+00045ef0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00045f00: 2020 2020 2020 2073 656c 662e 6963 6369         self.icci
+00045f10: 6473 203d 206d 2e67 6574 2827 4963 6369  ds = m.get('Icci
+00045f20: 6473 2729 0a20 2020 2020 2020 2069 6620  ds').        if 
+00045f30: 6d2e 6765 7428 2749 6363 6964 734f 7373  m.get('IccidsOss
+00045f40: 4669 6c65 5061 7468 2729 2069 7320 6e6f  FilePath') is no
+00045f50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00045f60: 2020 2020 7365 6c66 2e69 6363 6964 735f      self.iccids_
+00045f70: 6f73 735f 6669 6c65 5f70 6174 6820 3d20  oss_file_path = 
+00045f80: 6d2e 6765 7428 2749 6363 6964 734f 7373  m.get('IccidsOss
+00045f90: 4669 6c65 5061 7468 2729 0a20 2020 2020  FilePath').     
+00045fa0: 2020 2069 6620 6d2e 6765 7428 274e 616d     if m.get('Nam
+00045fb0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00045fc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00045fd0: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
+00045fe0: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+00045ff0: 6620 6d2e 6765 7428 274f 7065 7261 7465  f m.get('Operate
+00046000: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+00046010: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00046020: 7365 6c66 2e6f 7065 7261 7465 5f74 7970  self.operate_typ
+00046030: 6520 3d20 6d2e 6765 7428 274f 7065 7261  e = m.get('Opera
+00046040: 7465 5479 7065 2729 0a20 2020 2020 2020  teType').       
+00046050: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
+00046060: 6e49 6427 2920 6973 206e 6f74 204e 6f6e  nId') is not Non
+00046070: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00046080: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00046090: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
+000460a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000460b0: 6574 2827 5468 7265 7368 6f6c 6427 2920  et('Threshold') 
+000460c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000460d0: 2020 2020 2020 2020 2073 656c 662e 7468           self.th
+000460e0: 7265 7368 6f6c 6420 3d20 6d2e 6765 7428  reshold = m.get(
+000460f0: 2754 6872 6573 686f 6c64 2729 0a20 2020  'Threshold').   
+00046100: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+00046110: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+00046120: 6563 746f 7249 6473 2729 2069 7320 6e6f  ectorIds') is no
+00046130: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00046140: 2020 2020 7365 6c66 2e77 6972 656c 6573      self.wireles
+00046150: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
+00046160: 725f 6964 7320 3d20 6d2e 6765 7428 2757  r_ids = m.get('W
+00046170: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+00046180: 6563 746f 7249 6473 2729 0a20 2020 2020  ectorIds').     
+00046190: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+000461a0: 0a63 6c61 7373 2055 7064 6174 6542 6174  .class UpdateBat
+000461b0: 6368 4f70 6572 6174 6543 6172 6473 5461  chOperateCardsTa
+000461c0: 736b 5265 7370 6f6e 7365 426f 6479 2854  skResponseBody(T
+000461d0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000461e0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000461f0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00046200: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
+00046210: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+00046220: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00046230: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+00046240: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+00046250: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00046260: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00046270: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00046280: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00046290: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000462a0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000462b0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000462c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000462d0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000462e0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000462f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00046300: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
+00046310: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00046320: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
+00046330: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
+00046340: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+00046350: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00046360: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00046370: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00046380: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00046390: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000463a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000463b0: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+000463c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000463d0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+000463e0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+000463f0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+00046400: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00046410: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
+00046420: 4261 7463 684f 7065 7261 7465 4361 7264  BatchOperateCard
+00046430: 7354 6173 6b52 6573 706f 6e73 6528 5465  sTaskResponse(Te
+00046440: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00046450: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00046460: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00046470: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+00046480: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+00046490: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+000464a0: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+000464b0: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+000464c0: 5570 6461 7465 4261 7463 684f 7065 7261  UpdateBatchOpera
+000464d0: 7465 4361 7264 7354 6173 6b52 6573 706f  teCardsTaskRespo
+000464e0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
+000464f0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00046500: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00046510: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+00046520: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00046530: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+00046540: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00046550: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+00046560: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00046570: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00046580: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00046590: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
+000465a0: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
+000465b0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+000465c0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
+000465d0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
+000465e0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
+000465f0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+00046600: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
+00046610: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
+00046620: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+00046630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00046640: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+00046650: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00046660: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00046670: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00046680: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00046690: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000466a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000466b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000466c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000466d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000466e0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000466f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00046700: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+00046710: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+00046720: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+00046730: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+00046740: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+00046750: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00046760: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00046770: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00046780: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+00046790: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000467a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000467b0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000467c0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000467d0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000467e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000467f0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00046800: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00046810: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00046820: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00046830: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00046840: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00046850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00046860: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00046870: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00046880: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00046890: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000468a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000468b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000468c0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000468d0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000468e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000468f0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00046900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00046910: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00046920: 5570 6461 7465 4261 7463 684f 7065 7261  UpdateBatchOpera
+00046930: 7465 4361 7264 7354 6173 6b52 6573 706f  teCardsTaskRespo
+00046940: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00046950: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00046960: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00046970: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00046980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00046990: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+000469a0: 6174 6543 6172 6452 6571 7565 7374 2854  ateCardRequest(T
+000469b0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000469c0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000469d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000469e0: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
+000469f0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00046a00: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00046a10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00046a20: 2020 2020 2064 7279 5f72 756e 3a20 626f       dry_run: bo
+00046a30: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+00046a40: 2020 2069 6363 6964 3a20 7374 7220 3d20     iccid: str = 
+00046a50: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e61  None,.        na
+00046a60: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
+00046a70: 2020 2020 2020 2020 7769 7265 6c65 7373          wireless
+00046a80: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
+00046a90: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00046aa0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00046ab0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00046ac0: 6e20 3d20 636c 6965 6e74 5f74 6f6b 656e  n = client_token
+00046ad0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+00046ae0: 7363 7269 7074 696f 6e20 3d20 6465 7363  scription = desc
+00046af0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
+00046b00: 7365 6c66 2e64 7279 5f72 756e 203d 2064  self.dry_run = d
+00046b10: 7279 5f72 756e 0a20 2020 2020 2020 2073  ry_run.        s
+00046b20: 656c 662e 6963 6369 6420 3d20 6963 6369  elf.iccid = icci
+00046b30: 640a 2020 2020 2020 2020 7365 6c66 2e6e  d.        self.n
+00046b40: 616d 6520 3d20 6e61 6d65 0a20 2020 2020  ame = name.     
+00046b50: 2020 2073 656c 662e 7769 7265 6c65 7373     self.wireless
+00046b60: 5f63 6c6f 7564 5f63 6f6e 6e65 6374 6f72  _cloud_connector
+00046b70: 5f69 6420 3d20 7769 7265 6c65 7373 5f63  _id = wireless_c
+00046b80: 6c6f 7564 5f63 6f6e 6e65 6374 6f72 5f69  loud_connector_i
+00046b90: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+00046ba0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00046bb0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00046bc0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00046bd0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00046be0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00046bf0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00046c00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00046c10: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00046c20: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00046c30: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00046c40: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+00046c50: 656e 745f 746f 6b65 6e20 6973 206e 6f74  ent_token is not
+00046c60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00046c70: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+00046c80: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
+00046c90: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
+00046ca0: 2020 2020 2069 6620 7365 6c66 2e64 6573       if self.des
+00046cb0: 6372 6970 7469 6f6e 2069 7320 6e6f 7420  cription is not 
+00046cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00046cd0: 2020 7265 7375 6c74 5b27 4465 7363 7269    result['Descri
+00046ce0: 7074 696f 6e27 5d20 3d20 7365 6c66 2e64  ption'] = self.d
+00046cf0: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
+00046d00: 2020 2069 6620 7365 6c66 2e64 7279 5f72     if self.dry_r
+00046d10: 756e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  un is not None:.
+00046d20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00046d30: 6c74 5b27 4472 7952 756e 275d 203d 2073  lt['DryRun'] = s
+00046d40: 656c 662e 6472 795f 7275 6e0a 2020 2020  elf.dry_run.    
+00046d50: 2020 2020 6966 2073 656c 662e 6963 6369      if self.icci
+00046d60: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00046d70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00046d80: 745b 2749 6363 6964 275d 203d 2073 656c  t['Iccid'] = sel
+00046d90: 662e 6963 6369 640a 2020 2020 2020 2020  f.iccid.        
+00046da0: 6966 2073 656c 662e 6e61 6d65 2069 7320  if self.name is 
+00046db0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00046dc0: 2020 2020 2020 7265 7375 6c74 5b27 4e61        result['Na
+00046dd0: 6d65 275d 203d 2073 656c 662e 6e61 6d65  me'] = self.name
+00046de0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00046df0: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+00046e00: 636f 6e6e 6563 746f 725f 6964 2069 7320  connector_id is 
+00046e10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00046e20: 2020 2020 2020 7265 7375 6c74 5b27 5769        result['Wi
+00046e30: 7265 6c65 7373 436c 6f75 6443 6f6e 6e65  relessCloudConne
+00046e40: 6374 6f72 4964 275d 203d 2073 656c 662e  ctorId'] = self.
+00046e50: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+00046e60: 6f6e 6e65 6374 6f72 5f69 640a 2020 2020  onnector_id.    
+00046e70: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00046e80: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00046e90: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00046ea0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00046eb0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00046ec0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00046ed0: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
+00046ee0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00046ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00046f00: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
+00046f10: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
+00046f20: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
+00046f30: 6d2e 6765 7428 2744 6573 6372 6970 7469  m.get('Descripti
+00046f40: 6f6e 2729 2069 7320 6e6f 7420 4e6f 6e65  on') is not None
+00046f50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00046f60: 6c66 2e64 6573 6372 6970 7469 6f6e 203d  lf.description =
+00046f70: 206d 2e67 6574 2827 4465 7363 7269 7074   m.get('Descript
+00046f80: 696f 6e27 290a 2020 2020 2020 2020 6966  ion').        if
+00046f90: 206d 2e67 6574 2827 4472 7952 756e 2729   m.get('DryRun')
+00046fa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00046fb0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00046fc0: 7279 5f72 756e 203d 206d 2e67 6574 2827  ry_run = m.get('
+00046fd0: 4472 7952 756e 2729 0a20 2020 2020 2020  DryRun').       
+00046fe0: 2069 6620 6d2e 6765 7428 2749 6363 6964   if m.get('Iccid
+00046ff0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00047000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00047010: 2e69 6363 6964 203d 206d 2e67 6574 2827  .iccid = m.get('
+00047020: 4963 6369 6427 290a 2020 2020 2020 2020  Iccid').        
+00047030: 6966 206d 2e67 6574 2827 4e61 6d65 2729  if m.get('Name')
+00047040: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00047050: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00047060: 616d 6520 3d20 6d2e 6765 7428 274e 616d  ame = m.get('Nam
+00047070: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00047080: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
+00047090: 6f75 6443 6f6e 6e65 6374 6f72 4964 2729  oudConnectorId')
+000470a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000470b0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000470c0: 6972 656c 6573 735f 636c 6f75 645f 636f  ireless_cloud_co
+000470d0: 6e6e 6563 746f 725f 6964 203d 206d 2e67  nnector_id = m.g
+000470e0: 6574 2827 5769 7265 6c65 7373 436c 6f75  et('WirelessClou
+000470f0: 6443 6f6e 6e65 6374 6f72 4964 2729 0a20  dConnectorId'). 
+00047100: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00047110: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+00047120: 6543 6172 6452 6573 706f 6e73 6542 6f64  eCardResponseBod
+00047130: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+00047140: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00047150: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00047160: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+00047170: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00047180: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00047190: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+000471a0: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+000471b0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000471c0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000471d0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000471e0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000471f0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00047200: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00047210: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00047220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00047230: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00047240: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00047250: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00047260: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+00047270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00047280: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00047290: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+000472a0: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+000472b0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000472c0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000472d0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000472e0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000472f0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00047300: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00047310: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+00047320: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00047330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00047340: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+00047350: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00047360: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00047370: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+00047380: 6174 6543 6172 6452 6573 706f 6e73 6528  ateCardResponse(
+00047390: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000473a0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000473b0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000473c0: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+000473d0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+000473e0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+000473f0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+00047400: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+00047410: 3a20 5570 6461 7465 4361 7264 5265 7370  : UpdateCardResp
+00047420: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
+00047430: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00047440: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00047450: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+00047460: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00047470: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
+00047480: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00047490: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+000474a0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000474b0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+000474c0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+000474d0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
+000474e0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+000474f0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00047500: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
+00047510: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
+00047520: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
+00047530: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00047540: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
+00047550: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
+00047560: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+00047570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00047580: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+00047590: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000475a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000475b0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000475c0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000475d0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000475e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000475f0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00047600: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00047610: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00047620: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+00047630: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00047640: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+00047650: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+00047660: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+00047670: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+00047680: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+00047690: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000476a0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+000476b0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+000476c0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+000476d0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+000476e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000476f0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+00047700: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+00047710: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+00047720: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00047730: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00047740: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00047750: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00047760: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00047770: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00047780: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00047790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000477a0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+000477b0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+000477c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000477d0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000477e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000477f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00047800: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+00047810: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+00047820: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00047830: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+00047840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00047850: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00047860: 2055 7064 6174 6543 6172 6452 6573 706f   UpdateCardRespo
+00047870: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00047880: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00047890: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+000478a0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+000478b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000478c0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+000478d0: 6174 6544 4e53 4175 7468 6f72 697a 6174  ateDNSAuthorizat
+000478e0: 696f 6e52 756c 6552 6571 7565 7374 2854  ionRuleRequest(T
+000478f0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00047900: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00047910: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00047920: 2020 6175 7468 6f72 697a 6174 696f 6e5f    authorization_
+00047930: 7275 6c65 5f69 643a 2073 7472 203d 204e  rule_id: str = N
+00047940: 6f6e 652c 0a20 2020 2020 2020 2063 6c69  one,.        cli
+00047950: 656e 745f 746f 6b65 6e3a 2073 7472 203d  ent_token: str =
+00047960: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+00047970: 6573 6372 6970 7469 6f6e 3a20 7374 7220  escription: str 
+00047980: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00047990: 6465 7374 696e 6174 696f 6e5f 6970 3a20  destination_ip: 
+000479a0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000479b0: 2020 2020 6472 795f 7275 6e3a 2062 6f6f      dry_run: boo
+000479c0: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+000479d0: 2020 6e61 6d65 3a20 7374 7220 3d20 4e6f    name: str = No
+000479e0: 6e65 2c0a 2020 2020 2020 2020 736f 7572  ne,.        sour
+000479f0: 6365 5f64 6e73 6970 3a20 7374 7220 3d20  ce_dnsip: str = 
+00047a00: 4e6f 6e65 2c0a 2020 2020 2020 2020 7769  None,.        wi
+00047a10: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
+00047a20: 6e65 6374 6f72 5f69 643a 2073 7472 203d  nector_id: str =
+00047a30: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00047a40: 2020 2020 2020 7365 6c66 2e61 7574 686f        self.autho
+00047a50: 7269 7a61 7469 6f6e 5f72 756c 655f 6964  rization_rule_id
+00047a60: 203d 2061 7574 686f 7269 7a61 7469 6f6e   = authorization
+00047a70: 5f72 756c 655f 6964 0a20 2020 2020 2020  _rule_id.       
+00047a80: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+00047a90: 656e 203d 2063 6c69 656e 745f 746f 6b65  en = client_toke
+00047aa0: 6e0a 2020 2020 2020 2020 7365 6c66 2e64  n.        self.d
+00047ab0: 6573 6372 6970 7469 6f6e 203d 2064 6573  escription = des
+00047ac0: 6372 6970 7469 6f6e 0a20 2020 2020 2020  cription.       
+00047ad0: 2073 656c 662e 6465 7374 696e 6174 696f   self.destinatio
+00047ae0: 6e5f 6970 203d 2064 6573 7469 6e61 7469  n_ip = destinati
+00047af0: 6f6e 5f69 700a 2020 2020 2020 2020 7365  on_ip.        se
+00047b00: 6c66 2e64 7279 5f72 756e 203d 2064 7279  lf.dry_run = dry
+00047b10: 5f72 756e 0a20 2020 2020 2020 2073 656c  _run.        sel
+00047b20: 662e 6e61 6d65 203d 206e 616d 650a 2020  f.name = name.  
+00047b30: 2020 2020 2020 7365 6c66 2e73 6f75 7263        self.sourc
+00047b40: 655f 646e 7369 7020 3d20 736f 7572 6365  e_dnsip = source
+00047b50: 5f64 6e73 6970 0a20 2020 2020 2020 2073  _dnsip.        s
+00047b60: 656c 662e 7769 7265 6c65 7373 5f63 6c6f  elf.wireless_clo
+00047b70: 7564 5f63 6f6e 6e65 6374 6f72 5f69 6420  ud_connector_id 
+00047b80: 3d20 7769 7265 6c65 7373 5f63 6c6f 7564  = wireless_cloud
+00047b90: 5f63 6f6e 6e65 6374 6f72 5f69 640a 0a20  _connector_id.. 
+00047ba0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00047bb0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00047bc0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00047bd0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00047be0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00047bf0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00047c00: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00047c10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00047c20: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00047c30: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00047c40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00047c50: 2069 6620 7365 6c66 2e61 7574 686f 7269   if self.authori
+00047c60: 7a61 7469 6f6e 5f72 756c 655f 6964 2069  zation_rule_id i
+00047c70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00047c80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00047c90: 4175 7468 6f72 697a 6174 696f 6e52 756c  AuthorizationRul
+00047ca0: 6549 6427 5d20 3d20 7365 6c66 2e61 7574  eId'] = self.aut
+00047cb0: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
+00047cc0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+00047cd0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+00047ce0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00047cf0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00047d00: 2743 6c69 656e 7454 6f6b 656e 275d 203d  'ClientToken'] =
+00047d10: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+00047d20: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
+00047d30: 6c66 2e64 6573 6372 6970 7469 6f6e 2069  lf.description i
+00047d40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00047d50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00047d60: 4465 7363 7269 7074 696f 6e27 5d20 3d20  Description'] = 
+00047d70: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+00047d80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00047d90: 2e64 6573 7469 6e61 7469 6f6e 5f69 7020  .destination_ip 
+00047da0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00047db0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00047dc0: 2744 6573 7469 6e61 7469 6f6e 4970 275d  'DestinationIp']
+00047dd0: 203d 2073 656c 662e 6465 7374 696e 6174   = self.destinat
+00047de0: 696f 6e5f 6970 0a20 2020 2020 2020 2069  ion_ip.        i
+00047df0: 6620 7365 6c66 2e64 7279 5f72 756e 2069  f self.dry_run i
+00047e00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00047e10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00047e20: 4472 7952 756e 275d 203d 2073 656c 662e  DryRun'] = self.
+00047e30: 6472 795f 7275 6e0a 2020 2020 2020 2020  dry_run.        
+00047e40: 6966 2073 656c 662e 6e61 6d65 2069 7320  if self.name is 
+00047e50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00047e60: 2020 2020 2020 7265 7375 6c74 5b27 4e61        result['Na
+00047e70: 6d65 275d 203d 2073 656c 662e 6e61 6d65  me'] = self.name
+00047e80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00047e90: 2e73 6f75 7263 655f 646e 7369 7020 6973  .source_dnsip is
+00047ea0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00047eb0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+00047ec0: 6f75 7263 6544 4e53 4970 275d 203d 2073  ourceDNSIp'] = s
+00047ed0: 656c 662e 736f 7572 6365 5f64 6e73 6970  elf.source_dnsip
+00047ee0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00047ef0: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+00047f00: 636f 6e6e 6563 746f 725f 6964 2069 7320  connector_id is 
+00047f10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00047f20: 2020 2020 2020 7265 7375 6c74 5b27 5769        result['Wi
+00047f30: 7265 6c65 7373 436c 6f75 6443 6f6e 6e65  relessCloudConne
+00047f40: 6374 6f72 4964 275d 203d 2073 656c 662e  ctorId'] = self.
+00047f50: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+00047f60: 6f6e 6e65 6374 6f72 5f69 640a 2020 2020  onnector_id.    
+00047f70: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00047f80: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00047f90: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00047fa0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00047fb0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00047fc0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00047fd0: 6765 7428 2741 7574 686f 7269 7a61 7469  get('Authorizati
+00047fe0: 6f6e 5275 6c65 4964 2729 2069 7320 6e6f  onRuleId') is no
+00047ff0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00048000: 2020 2020 7365 6c66 2e61 7574 686f 7269      self.authori
+00048010: 7a61 7469 6f6e 5f72 756c 655f 6964 203d  zation_rule_id =
+00048020: 206d 2e67 6574 2827 4175 7468 6f72 697a   m.get('Authoriz
+00048030: 6174 696f 6e52 756c 6549 6427 290a 2020  ationRuleId').  
+00048040: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00048050: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
+00048060: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00048070: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00048080: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
+00048090: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
+000480a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000480b0: 2827 4465 7363 7269 7074 696f 6e27 2920  ('Description') 
+000480c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000480d0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+000480e0: 7363 7269 7074 696f 6e20 3d20 6d2e 6765  scription = m.ge
+000480f0: 7428 2744 6573 6372 6970 7469 6f6e 2729  t('Description')
+00048100: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00048110: 7428 2744 6573 7469 6e61 7469 6f6e 4970  t('DestinationIp
+00048120: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00048130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00048140: 2e64 6573 7469 6e61 7469 6f6e 5f69 7020  .destination_ip 
+00048150: 3d20 6d2e 6765 7428 2744 6573 7469 6e61  = m.get('Destina
+00048160: 7469 6f6e 4970 2729 0a20 2020 2020 2020  tionIp').       
+00048170: 2069 6620 6d2e 6765 7428 2744 7279 5275   if m.get('DryRu
+00048180: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+00048190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000481a0: 662e 6472 795f 7275 6e20 3d20 6d2e 6765  f.dry_run = m.ge
+000481b0: 7428 2744 7279 5275 6e27 290a 2020 2020  t('DryRun').    
+000481c0: 2020 2020 6966 206d 2e67 6574 2827 4e61      if m.get('Na
+000481d0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+000481e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000481f0: 6c66 2e6e 616d 6520 3d20 6d2e 6765 7428  lf.name = m.get(
+00048200: 274e 616d 6527 290a 2020 2020 2020 2020  'Name').        
+00048210: 6966 206d 2e67 6574 2827 536f 7572 6365  if m.get('Source
+00048220: 444e 5349 7027 2920 6973 206e 6f74 204e  DNSIp') is not N
+00048230: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00048240: 2073 656c 662e 736f 7572 6365 5f64 6e73   self.source_dns
+00048250: 6970 203d 206d 2e67 6574 2827 536f 7572  ip = m.get('Sour
+00048260: 6365 444e 5349 7027 290a 2020 2020 2020  ceDNSIp').      
+00048270: 2020 6966 206d 2e67 6574 2827 5769 7265    if m.get('Wire
+00048280: 6c65 7373 436c 6f75 6443 6f6e 6e65 6374  lessCloudConnect
+00048290: 6f72 4964 2729 2069 7320 6e6f 7420 4e6f  orId') is not No
+000482a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000482b0: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
+000482c0: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+000482d0: 203d 206d 2e67 6574 2827 5769 7265 6c65   = m.get('Wirele
+000482e0: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+000482f0: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00048300: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00048310: 2055 7064 6174 6544 4e53 4175 7468 6f72   UpdateDNSAuthor
+00048320: 697a 6174 696f 6e52 756c 6552 6573 706f  izationRuleRespo
+00048330: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+00048340: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00048350: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00048360: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+00048370: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+00048380: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00048390: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+000483a0: 6420 3d20 7265 7175 6573 745f 6964 0a0a  d = request_id..
+000483b0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000483c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000483d0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000483e0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000483f0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00048400: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00048410: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00048420: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00048430: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00048440: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00048450: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00048460: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+00048470: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00048480: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00048490: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+000484a0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+000484b0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+000484c0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+000484d0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000484e0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+000484f0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00048500: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00048510: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+00048520: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+00048530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00048540: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+00048550: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+00048560: 7374 4964 2729 0a20 2020 2020 2020 2072  stId').        r
+00048570: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00048580: 7373 2055 7064 6174 6544 4e53 4175 7468  ss UpdateDNSAuth
+00048590: 6f72 697a 6174 696f 6e52 756c 6552 6573  orizationRuleRes
+000485a0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+000485b0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000485c0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000485d0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+000485e0: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
+000485f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00048600: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
+00048610: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+00048620: 2020 626f 6479 3a20 5570 6461 7465 444e    body: UpdateDN
+00048630: 5341 7574 686f 7269 7a61 7469 6f6e 5275  SAuthorizationRu
+00048640: 6c65 5265 7370 6f6e 7365 426f 6479 203d  leResponseBody =
+00048650: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00048660: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00048670: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+00048680: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00048690: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000486a0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+000486b0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+000486c0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000486d0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+000486e0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+000486f0: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
+00048700: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
+00048710: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+00048720: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+00048730: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
+00048740: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
+00048750: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+00048760: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+00048770: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
+00048780: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00048790: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+000487a0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+000487b0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+000487c0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+000487d0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+000487e0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+000487f0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00048800: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00048810: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00048820: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00048830: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00048840: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+00048850: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+00048860: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00048870: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+00048880: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+00048890: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000488a0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+000488b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000488c0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+000488d0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+000488e0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000488f0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00048900: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00048910: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00048920: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00048930: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00048940: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00048950: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00048960: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00048970: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00048980: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00048990: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000489a0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+000489b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000489c0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000489d0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000489e0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000489f0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+00048a00: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+00048a10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00048a20: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00048a30: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00048a40: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00048a50: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00048a60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00048a70: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00048a80: 6f64 656c 203d 2055 7064 6174 6544 4e53  odel = UpdateDNS
+00048a90: 4175 7468 6f72 697a 6174 696f 6e52 756c  AuthorizationRul
+00048aa0: 6552 6573 706f 6e73 6542 6f64 7928 290a  eResponseBody().
+00048ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00048ac0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+00048ad0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+00048ae0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+00048af0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00048b00: 7373 2055 7064 6174 6547 726f 7570 4175  ss UpdateGroupAu
+00048b10: 7468 6f72 697a 6174 696f 6e52 756c 6552  thorizationRuleR
+00048b20: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00048b30: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00048b40: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00048b50: 2c0a 2020 2020 2020 2020 6175 7468 6f72  ,.        author
+00048b60: 697a 6174 696f 6e5f 7275 6c65 5f69 643a  ization_rule_id:
+00048b70: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00048b80: 2020 2020 2063 6c69 656e 745f 746f 6b65       client_toke
+00048b90: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+00048ba0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00048bb0: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+00048bc0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00048bd0: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
+00048be0: 0a20 2020 2020 2020 2064 6573 7469 6e61  .        destina
+00048bf0: 7469 6f6e 5f70 6f72 743a 2073 7472 203d  tion_port: str =
+00048c00: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
+00048c10: 7279 5f72 756e 3a20 626f 6f6c 203d 204e  ry_run: bool = N
+00048c20: 6f6e 652c 0a20 2020 2020 2020 206e 616d  one,.        nam
+00048c30: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00048c40: 2020 2020 2020 2070 6f6c 6963 793a 2073         policy: s
+00048c50: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00048c60: 2020 2070 726f 746f 636f 6c3a 2073 7472     protocol: str
+00048c70: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00048c80: 2073 6f75 7263 655f 6369 6472 3a20 7374   source_cidr: st
+00048c90: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00048ca0: 2020 7769 7265 6c65 7373 5f63 6c6f 7564    wireless_cloud
+00048cb0: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
+00048cc0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00048cd0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00048ce0: 7365 6c66 2e61 7574 686f 7269 7a61 7469  self.authorizati
+00048cf0: 6f6e 5f72 756c 655f 6964 203d 2061 7574  on_rule_id = aut
+00048d00: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
+00048d10: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+00048d20: 636c 6965 6e74 5f74 6f6b 656e 203d 2063  client_token = c
+00048d30: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
+00048d40: 2020 2020 7365 6c66 2e64 6573 6372 6970      self.descrip
+00048d50: 7469 6f6e 203d 2064 6573 6372 6970 7469  tion = descripti
+00048d60: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+00048d70: 6465 7374 696e 6174 696f 6e20 3d20 6465  destination = de
+00048d80: 7374 696e 6174 696f 6e0a 2020 2020 2020  stination.      
+00048d90: 2020 7365 6c66 2e64 6573 7469 6e61 7469    self.destinati
+00048da0: 6f6e 5f70 6f72 7420 3d20 6465 7374 696e  on_port = destin
+00048db0: 6174 696f 6e5f 706f 7274 0a20 2020 2020  ation_port.     
+00048dc0: 2020 2073 656c 662e 6472 795f 7275 6e20     self.dry_run 
+00048dd0: 3d20 6472 795f 7275 6e0a 2020 2020 2020  = dry_run.      
+00048de0: 2020 7365 6c66 2e6e 616d 6520 3d20 6e61    self.name = na
+00048df0: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+00048e00: 706f 6c69 6379 203d 2070 6f6c 6963 790a  policy = policy.
+00048e10: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00048e20: 746f 636f 6c20 3d20 7072 6f74 6f63 6f6c  tocol = protocol
+00048e30: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+00048e40: 7572 6365 5f63 6964 7220 3d20 736f 7572  urce_cidr = sour
+00048e50: 6365 5f63 6964 720a 2020 2020 2020 2020  ce_cidr.        
+00048e60: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
+00048e70: 6f75 645f 636f 6e6e 6563 746f 725f 6772  oud_connector_gr
+00048e80: 6f75 705f 6964 203d 2077 6972 656c 6573  oup_id = wireles
+00048e90: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
+00048ea0: 725f 6772 6f75 705f 6964 0a0a 2020 2020  r_group_id..    
+00048eb0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00048ec0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00048ed0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00048ee0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00048ef0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00048f00: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00048f10: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00048f20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00048f30: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00048f40: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00048f50: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00048f60: 2073 656c 662e 6175 7468 6f72 697a 6174   self.authorizat
+00048f70: 696f 6e5f 7275 6c65 5f69 6420 6973 206e  ion_rule_id is n
+00048f80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00048f90: 2020 2020 2072 6573 756c 745b 2741 7574       result['Aut
+00048fa0: 686f 7269 7a61 7469 6f6e 5275 6c65 4964  horizationRuleId
+00048fb0: 275d 203d 2073 656c 662e 6175 7468 6f72  '] = self.author
+00048fc0: 697a 6174 696f 6e5f 7275 6c65 5f69 640a  ization_rule_id.
+00048fd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00048fe0: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
+00048ff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00049000: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
+00049010: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
+00049020: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
+00049030: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00049040: 6465 7363 7269 7074 696f 6e20 6973 206e  description is n
+00049050: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00049060: 2020 2020 2072 6573 756c 745b 2744 6573       result['Des
+00049070: 6372 6970 7469 6f6e 275d 203d 2073 656c  cription'] = sel
+00049080: 662e 6465 7363 7269 7074 696f 6e0a 2020  f.description.  
+00049090: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
+000490a0: 7374 696e 6174 696f 6e20 6973 206e 6f74  stination is not
+000490b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000490c0: 2020 2072 6573 756c 745b 2744 6573 7469     result['Desti
+000490d0: 6e61 7469 6f6e 275d 203d 2073 656c 662e  nation'] = self.
+000490e0: 6465 7374 696e 6174 696f 6e0a 2020 2020  destination.    
+000490f0: 2020 2020 6966 2073 656c 662e 6465 7374      if self.dest
+00049100: 696e 6174 696f 6e5f 706f 7274 2069 7320  ination_port is 
+00049110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00049120: 2020 2020 2020 7265 7375 6c74 5b27 4465        result['De
+00049130: 7374 696e 6174 696f 6e50 6f72 7427 5d20  stinationPort'] 
+00049140: 3d20 7365 6c66 2e64 6573 7469 6e61 7469  = self.destinati
+00049150: 6f6e 5f70 6f72 740a 2020 2020 2020 2020  on_port.        
+00049160: 6966 2073 656c 662e 6472 795f 7275 6e20  if self.dry_run 
+00049170: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00049180: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00049190: 2744 7279 5275 6e27 5d20 3d20 7365 6c66  'DryRun'] = self
+000491a0: 2e64 7279 5f72 756e 0a20 2020 2020 2020  .dry_run.       
+000491b0: 2069 6620 7365 6c66 2e6e 616d 6520 6973   if self.name is
+000491c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000491d0: 2020 2020 2020 2072 6573 756c 745b 274e         result['N
+000491e0: 616d 6527 5d20 3d20 7365 6c66 2e6e 616d  ame'] = self.nam
+000491f0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00049200: 662e 706f 6c69 6379 2069 7320 6e6f 7420  f.policy is not 
+00049210: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00049220: 2020 7265 7375 6c74 5b27 506f 6c69 6379    result['Policy
+00049230: 275d 203d 2073 656c 662e 706f 6c69 6379  '] = self.policy
+00049240: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00049250: 2e70 726f 746f 636f 6c20 6973 206e 6f74  .protocol is not
+00049260: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00049270: 2020 2072 6573 756c 745b 2750 726f 746f     result['Proto
+00049280: 636f 6c27 5d20 3d20 7365 6c66 2e70 726f  col'] = self.pro
+00049290: 746f 636f 6c0a 2020 2020 2020 2020 6966  tocol.        if
+000492a0: 2073 656c 662e 736f 7572 6365 5f63 6964   self.source_cid
+000492b0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+000492c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000492d0: 745b 2753 6f75 7263 6543 6964 7227 5d20  t['SourceCidr'] 
+000492e0: 3d20 7365 6c66 2e73 6f75 7263 655f 6369  = self.source_ci
+000492f0: 6472 0a20 2020 2020 2020 2069 6620 7365  dr.        if se
+00049300: 6c66 2e77 6972 656c 6573 735f 636c 6f75  lf.wireless_clou
+00049310: 645f 636f 6e6e 6563 746f 725f 6772 6f75  d_connector_grou
+00049320: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
+00049330: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00049340: 7375 6c74 5b27 5769 7265 6c65 7373 436c  sult['WirelessCl
+00049350: 6f75 6443 6f6e 6e65 6374 6f72 4772 6f75  oudConnectorGrou
+00049360: 7049 6427 5d20 3d20 7365 6c66 2e77 6972  pId'] = self.wir
+00049370: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
+00049380: 6563 746f 725f 6772 6f75 705f 6964 0a20  ector_group_id. 
+00049390: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000493a0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000493b0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000493c0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000493d0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000493e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000493f0: 206d 2e67 6574 2827 4175 7468 6f72 697a   m.get('Authoriz
+00049400: 6174 696f 6e52 756c 6549 6427 2920 6973  ationRuleId') is
+00049410: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00049420: 2020 2020 2020 2073 656c 662e 6175 7468         self.auth
+00049430: 6f72 697a 6174 696f 6e5f 7275 6c65 5f69  orization_rule_i
+00049440: 6420 3d20 6d2e 6765 7428 2741 7574 686f  d = m.get('Autho
+00049450: 7269 7a61 7469 6f6e 5275 6c65 4964 2729  rizationRuleId')
+00049460: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00049470: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
+00049480: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00049490: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000494a0: 6c69 656e 745f 746f 6b65 6e20 3d20 6d2e  lient_token = m.
+000494b0: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
+000494c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000494d0: 6765 7428 2744 6573 6372 6970 7469 6f6e  get('Description
+000494e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000494f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00049500: 2e64 6573 6372 6970 7469 6f6e 203d 206d  .description = m
+00049510: 2e67 6574 2827 4465 7363 7269 7074 696f  .get('Descriptio
+00049520: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
+00049530: 2e67 6574 2827 4465 7374 696e 6174 696f  .get('Destinatio
+00049540: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+00049550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00049560: 662e 6465 7374 696e 6174 696f 6e20 3d20  f.destination = 
+00049570: 6d2e 6765 7428 2744 6573 7469 6e61 7469  m.get('Destinati
+00049580: 6f6e 2729 0a20 2020 2020 2020 2069 6620  on').        if 
+00049590: 6d2e 6765 7428 2744 6573 7469 6e61 7469  m.get('Destinati
+000495a0: 6f6e 506f 7274 2729 2069 7320 6e6f 7420  onPort') is not 
+000495b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000495c0: 2020 7365 6c66 2e64 6573 7469 6e61 7469    self.destinati
+000495d0: 6f6e 5f70 6f72 7420 3d20 6d2e 6765 7428  on_port = m.get(
+000495e0: 2744 6573 7469 6e61 7469 6f6e 506f 7274  'DestinationPort
+000495f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00049600: 6765 7428 2744 7279 5275 6e27 2920 6973  get('DryRun') is
+00049610: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00049620: 2020 2020 2020 2073 656c 662e 6472 795f         self.dry_
+00049630: 7275 6e20 3d20 6d2e 6765 7428 2744 7279  run = m.get('Dry
+00049640: 5275 6e27 290a 2020 2020 2020 2020 6966  Run').        if
+00049650: 206d 2e67 6574 2827 4e61 6d65 2729 2069   m.get('Name') i
+00049660: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00049670: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+00049680: 6520 3d20 6d2e 6765 7428 274e 616d 6527  e = m.get('Name'
+00049690: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000496a0: 6574 2827 506f 6c69 6379 2729 2069 7320  et('Policy') is 
+000496b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000496c0: 2020 2020 2020 7365 6c66 2e70 6f6c 6963        self.polic
+000496d0: 7920 3d20 6d2e 6765 7428 2750 6f6c 6963  y = m.get('Polic
+000496e0: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+000496f0: 2e67 6574 2827 5072 6f74 6f63 6f6c 2729  .get('Protocol')
+00049700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00049710: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00049720: 726f 746f 636f 6c20 3d20 6d2e 6765 7428  rotocol = m.get(
+00049730: 2750 726f 746f 636f 6c27 290a 2020 2020  'Protocol').    
+00049740: 2020 2020 6966 206d 2e67 6574 2827 536f      if m.get('So
+00049750: 7572 6365 4369 6472 2729 2069 7320 6e6f  urceCidr') is no
+00049760: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00049770: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
+00049780: 6369 6472 203d 206d 2e67 6574 2827 536f  cidr = m.get('So
+00049790: 7572 6365 4369 6472 2729 0a20 2020 2020  urceCidr').     
+000497a0: 2020 2069 6620 6d2e 6765 7428 2757 6972     if m.get('Wir
+000497b0: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+000497c0: 746f 7247 726f 7570 4964 2729 2069 7320  torGroupId') is 
+000497d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000497e0: 2020 2020 2020 7365 6c66 2e77 6972 656c        self.wirel
+000497f0: 6573 735f 636c 6f75 645f 636f 6e6e 6563  ess_cloud_connec
+00049800: 746f 725f 6772 6f75 705f 6964 203d 206d  tor_group_id = m
+00049810: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
+00049820: 6f75 6443 6f6e 6e65 6374 6f72 4772 6f75  oudConnectorGrou
+00049830: 7049 6427 290a 2020 2020 2020 2020 7265  pId').        re
+00049840: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00049850: 7320 5570 6461 7465 4772 6f75 7041 7574  s UpdateGroupAut
+00049860: 686f 7269 7a61 7469 6f6e 5275 6c65 5265  horizationRuleRe
+00049870: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+00049880: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00049890: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000498a0: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
+000498b0: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
+000498c0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000498d0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+000498e0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+000498f0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+00049900: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00049910: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00049920: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00049930: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00049940: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00049950: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00049960: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00049970: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00049980: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00049990: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000499a0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+000499b0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+000499c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000499d0: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
+000499e0: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
+000499f0: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
+00049a00: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00049a10: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00049a20: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00049a30: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00049a40: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00049a50: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00049a60: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+00049a70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00049a80: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00049a90: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+00049aa0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+00049ab0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00049ac0: 636c 6173 7320 5570 6461 7465 4772 6f75  class UpdateGrou
+00049ad0: 7041 7574 686f 7269 7a61 7469 6f6e 5275  pAuthorizationRu
+00049ae0: 6c65 5265 7370 6f6e 7365 2854 6561 4d6f  leResponse(TeaMo
+00049af0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00049b00: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00049b10: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+00049b20: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00049b30: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00049b40: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00049b50: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00049b60: 2020 2020 2020 2062 6f64 793a 2055 7064         body: Upd
+00049b70: 6174 6547 726f 7570 4175 7468 6f72 697a  ateGroupAuthoriz
+00049b80: 6174 696f 6e52 756c 6552 6573 706f 6e73  ationRuleRespons
+00049b90: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+00049ba0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00049bb0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00049bc0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00049bd0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00049be0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00049bf0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00049c00: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00049c10: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00049c20: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00049c30: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00049c40: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00049c50: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00049c60: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00049c70: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00049c80: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00049c90: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00049ca0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00049cb0: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00049cc0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00049cd0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+00049ce0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00049cf0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+00049d00: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00049d10: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00049d20: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00049d30: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00049d40: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00049d50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00049d60: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00049d70: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00049d80: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00049d90: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00049da0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00049db0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00049dc0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00049dd0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00049de0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00049df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00049e00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00049e10: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00049e20: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00049e30: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00049e40: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00049e50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00049e60: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00049e70: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00049e80: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00049e90: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00049ea0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00049eb0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+00049ec0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00049ed0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00049ee0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+00049ef0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+00049f00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00049f10: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+00049f20: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+00049f30: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00049f40: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+00049f50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00049f60: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00049f70: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+00049f80: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+00049f90: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00049fa0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00049fb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00049fc0: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
+00049fd0: 6461 7465 4772 6f75 7041 7574 686f 7269  dateGroupAuthori
+00049fe0: 7a61 7469 6f6e 5275 6c65 5265 7370 6f6e  zationRuleRespon
+00049ff0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0004a000: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0004a010: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0004a020: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0004a030: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0004a040: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+0004a050: 7465 4772 6f75 7044 6e73 4175 7468 6f72  teGroupDnsAuthor
+0004a060: 697a 6174 696f 6e52 756c 6552 6571 7565  izationRuleReque
+0004a070: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+0004a080: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0004a090: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0004a0a0: 2020 2020 2020 6175 7468 6f72 697a 6174        authorizat
+0004a0b0: 696f 6e5f 7275 6c65 5f69 643a 2073 7472  ion_rule_id: str
+0004a0c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004a0d0: 2063 6c69 656e 745f 746f 6b65 6e3a 2073   client_token: s
+0004a0e0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0004a0f0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+0004a100: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0004a110: 2020 2020 6465 7374 696e 6174 696f 6e5f      destination_
+0004a120: 6970 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ip: str = None,.
+0004a130: 2020 2020 2020 2020 6472 795f 7275 6e3a          dry_run:
+0004a140: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+0004a150: 2020 2020 2020 6e61 6d65 3a20 7374 7220        name: str 
+0004a160: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004a170: 736f 7572 6365 5f64 6e73 6970 3a20 7374  source_dnsip: st
+0004a180: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0004a190: 2020 7769 7265 6c65 7373 5f63 6c6f 7564    wireless_cloud
+0004a1a0: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
+0004a1b0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0004a1c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0004a1d0: 7365 6c66 2e61 7574 686f 7269 7a61 7469  self.authorizati
+0004a1e0: 6f6e 5f72 756c 655f 6964 203d 2061 7574  on_rule_id = aut
+0004a1f0: 686f 7269 7a61 7469 6f6e 5f72 756c 655f  horization_rule_
+0004a200: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+0004a210: 636c 6965 6e74 5f74 6f6b 656e 203d 2063  client_token = c
+0004a220: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
+0004a230: 2020 2020 7365 6c66 2e64 6573 6372 6970      self.descrip
+0004a240: 7469 6f6e 203d 2064 6573 6372 6970 7469  tion = descripti
+0004a250: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+0004a260: 6465 7374 696e 6174 696f 6e5f 6970 203d  destination_ip =
+0004a270: 2064 6573 7469 6e61 7469 6f6e 5f69 700a   destination_ip.
+0004a280: 2020 2020 2020 2020 7365 6c66 2e64 7279          self.dry
+0004a290: 5f72 756e 203d 2064 7279 5f72 756e 0a20  _run = dry_run. 
+0004a2a0: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+0004a2b0: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+0004a2c0: 7365 6c66 2e73 6f75 7263 655f 646e 7369  self.source_dnsi
+0004a2d0: 7020 3d20 736f 7572 6365 5f64 6e73 6970  p = source_dnsip
+0004a2e0: 0a20 2020 2020 2020 2073 656c 662e 7769  .        self.wi
+0004a2f0: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
+0004a300: 6e65 6374 6f72 5f67 726f 7570 5f69 6420  nector_group_id 
+0004a310: 3d20 7769 7265 6c65 7373 5f63 6c6f 7564  = wireless_cloud
+0004a320: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
+0004a330: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+0004a340: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0004a350: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0004a360: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0004a370: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0004a380: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0004a390: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0004a3a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0004a3b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0004a3c0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0004a3d0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0004a3e0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+0004a3f0: 7574 686f 7269 7a61 7469 6f6e 5f72 756c  uthorization_rul
+0004a400: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0004a410: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0004a420: 7375 6c74 5b27 4175 7468 6f72 697a 6174  sult['Authorizat
+0004a430: 696f 6e52 756c 6549 6427 5d20 3d20 7365  ionRuleId'] = se
+0004a440: 6c66 2e61 7574 686f 7269 7a61 7469 6f6e  lf.authorization
+0004a450: 5f72 756c 655f 6964 0a20 2020 2020 2020  _rule_id.       
+0004a460: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+0004a470: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+0004a480: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004a490: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
+0004a4a0: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
+0004a4b0: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+0004a4c0: 2069 6620 7365 6c66 2e64 6573 6372 6970   if self.descrip
+0004a4d0: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+0004a4e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0004a4f0: 7375 6c74 5b27 4465 7363 7269 7074 696f  sult['Descriptio
+0004a500: 6e27 5d20 3d20 7365 6c66 2e64 6573 6372  n'] = self.descr
+0004a510: 6970 7469 6f6e 0a20 2020 2020 2020 2069  iption.        i
+0004a520: 6620 7365 6c66 2e64 6573 7469 6e61 7469  f self.destinati
+0004a530: 6f6e 5f69 7020 6973 206e 6f74 204e 6f6e  on_ip is not Non
+0004a540: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004a550: 6573 756c 745b 2744 6573 7469 6e61 7469  esult['Destinati
+0004a560: 6f6e 4970 275d 203d 2073 656c 662e 6465  onIp'] = self.de
+0004a570: 7374 696e 6174 696f 6e5f 6970 0a20 2020  stination_ip.   
+0004a580: 2020 2020 2069 6620 7365 6c66 2e64 7279       if self.dry
+0004a590: 5f72 756e 2069 7320 6e6f 7420 4e6f 6e65  _run is not None
+0004a5a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0004a5b0: 7375 6c74 5b27 4472 7952 756e 275d 203d  sult['DryRun'] =
+0004a5c0: 2073 656c 662e 6472 795f 7275 6e0a 2020   self.dry_run.  
+0004a5d0: 2020 2020 2020 6966 2073 656c 662e 6e61        if self.na
+0004a5e0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+0004a5f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0004a600: 6c74 5b27 4e61 6d65 275d 203d 2073 656c  lt['Name'] = sel
+0004a610: 662e 6e61 6d65 0a20 2020 2020 2020 2069  f.name.        i
+0004a620: 6620 7365 6c66 2e73 6f75 7263 655f 646e  f self.source_dn
+0004a630: 7369 7020 6973 206e 6f74 204e 6f6e 653a  sip is not None:
+0004a640: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0004a650: 756c 745b 2753 6f75 7263 6544 4e53 4970  ult['SourceDNSIp
+0004a660: 275d 203d 2073 656c 662e 736f 7572 6365  '] = self.source
+0004a670: 5f64 6e73 6970 0a20 2020 2020 2020 2069  _dnsip.        i
+0004a680: 6620 7365 6c66 2e77 6972 656c 6573 735f  f self.wireless_
+0004a690: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
+0004a6a0: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
+0004a6b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004a6c0: 2020 7265 7375 6c74 5b27 5769 7265 6c65    result['Wirele
+0004a6d0: 7373 436c 6f75 6443 6f6e 6e65 6374 6f72  ssCloudConnector
+0004a6e0: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
+0004a6f0: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+0004a700: 636f 6e6e 6563 746f 725f 6772 6f75 705f  connector_group_
+0004a710: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0004a720: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0004a730: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0004a740: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0004a750: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0004a760: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0004a770: 2020 6966 206d 2e67 6574 2827 4175 7468    if m.get('Auth
+0004a780: 6f72 697a 6174 696f 6e52 756c 6549 6427  orizationRuleId'
+0004a790: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0004a7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0004a7b0: 6175 7468 6f72 697a 6174 696f 6e5f 7275  authorization_ru
+0004a7c0: 6c65 5f69 6420 3d20 6d2e 6765 7428 2741  le_id = m.get('A
+0004a7d0: 7574 686f 7269 7a61 7469 6f6e 5275 6c65  uthorizationRule
+0004a7e0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0004a7f0: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
+0004a800: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
+0004a810: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0004a820: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+0004a830: 3d20 6d2e 6765 7428 2743 6c69 656e 7454  = m.get('ClientT
+0004a840: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
+0004a850: 6620 6d2e 6765 7428 2744 6573 6372 6970  f m.get('Descrip
+0004a860: 7469 6f6e 2729 2069 7320 6e6f 7420 4e6f  tion') is not No
+0004a870: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004a880: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+0004a890: 203d 206d 2e67 6574 2827 4465 7363 7269   = m.get('Descri
+0004a8a0: 7074 696f 6e27 290a 2020 2020 2020 2020  ption').        
+0004a8b0: 6966 206d 2e67 6574 2827 4465 7374 696e  if m.get('Destin
+0004a8c0: 6174 696f 6e49 7027 2920 6973 206e 6f74  ationIp') is not
+0004a8d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0004a8e0: 2020 2073 656c 662e 6465 7374 696e 6174     self.destinat
+0004a8f0: 696f 6e5f 6970 203d 206d 2e67 6574 2827  ion_ip = m.get('
+0004a900: 4465 7374 696e 6174 696f 6e49 7027 290a  DestinationIp').
+0004a910: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0004a920: 2827 4472 7952 756e 2729 2069 7320 6e6f  ('DryRun') is no
+0004a930: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0004a940: 2020 2020 7365 6c66 2e64 7279 5f72 756e      self.dry_run
+0004a950: 203d 206d 2e67 6574 2827 4472 7952 756e   = m.get('DryRun
+0004a960: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0004a970: 6765 7428 274e 616d 6527 2920 6973 206e  get('Name') is n
+0004a980: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004a990: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
+0004a9a0: 206d 2e67 6574 2827 4e61 6d65 2729 0a20   m.get('Name'). 
+0004a9b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0004a9c0: 2753 6f75 7263 6544 4e53 4970 2729 2069  'SourceDNSIp') i
+0004a9d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0004a9e0: 2020 2020 2020 2020 7365 6c66 2e73 6f75          self.sou
+0004a9f0: 7263 655f 646e 7369 7020 3d20 6d2e 6765  rce_dnsip = m.ge
+0004aa00: 7428 2753 6f75 7263 6544 4e53 4970 2729  t('SourceDNSIp')
+0004aa10: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0004aa20: 7428 2757 6972 656c 6573 7343 6c6f 7564  t('WirelessCloud
+0004aa30: 436f 6e6e 6563 746f 7247 726f 7570 4964  ConnectorGroupId
+0004aa40: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004aa50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0004aa60: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+0004aa70: 636f 6e6e 6563 746f 725f 6772 6f75 705f  connector_group_
+0004aa80: 6964 203d 206d 2e67 6574 2827 5769 7265  id = m.get('Wire
+0004aa90: 6c65 7373 436c 6f75 6443 6f6e 6e65 6374  lessCloudConnect
+0004aaa0: 6f72 4772 6f75 7049 6427 290a 2020 2020  orGroupId').    
+0004aab0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0004aac0: 0a0a 636c 6173 7320 5570 6461 7465 4772  ..class UpdateGr
+0004aad0: 6f75 7044 6e73 4175 7468 6f72 697a 6174  oupDnsAuthorizat
+0004aae0: 696f 6e52 756c 6552 6573 706f 6e73 6542  ionRuleResponseB
+0004aaf0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+0004ab00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0004ab10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0004ab20: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
+0004ab30: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0004ab40: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0004ab50: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0004ab60: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
+0004ab70: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0004ab80: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0004ab90: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0004aba0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004abb0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0004abc0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0004abd0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0004abe0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0004abf0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0004ac00: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0004ac10: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004ac20: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0004ac30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0004ac40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0004ac50: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+0004ac60: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+0004ac70: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0004ac80: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0004ac90: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0004aca0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0004acb0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0004acc0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0004acd0: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+0004ace0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0004acf0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0004ad00: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0004ad10: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0004ad20: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0004ad30: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
+0004ad40: 7064 6174 6547 726f 7570 446e 7341 7574  pdateGroupDnsAut
+0004ad50: 686f 7269 7a61 7469 6f6e 5275 6c65 5265  horizationRuleRe
+0004ad60: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0004ad70: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0004ad80: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0004ad90: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0004ada0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+0004adb0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0004adc0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+0004add0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+0004ade0: 2020 2062 6f64 793a 2055 7064 6174 6547     body: UpdateG
+0004adf0: 726f 7570 446e 7341 7574 686f 7269 7a61  roupDnsAuthoriza
+0004ae00: 7469 6f6e 5275 6c65 5265 7370 6f6e 7365  tionRuleResponse
+0004ae10: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+0004ae20: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0004ae30: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+0004ae40: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+0004ae50: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+0004ae60: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+0004ae70: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+0004ae80: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+0004ae90: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0004aea0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0004aeb0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+0004aec0: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+0004aed0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+0004aee0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0004aef0: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+0004af00: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+0004af10: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0004af20: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0004af30: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+0004af40: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+0004af50: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0004af60: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0004af70: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0004af80: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0004af90: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0004afa0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+0004afb0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0004afc0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0004afd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0004afe0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0004aff0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0004b000: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0004b010: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+0004b020: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0004b030: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+0004b040: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+0004b050: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+0004b060: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0004b070: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004b080: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0004b090: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+0004b0a0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0004b0b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0004b0c0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+0004b0d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004b0e0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+0004b0f0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+0004b100: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0004b110: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0004b120: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0004b130: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0004b140: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0004b150: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0004b160: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+0004b170: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+0004b180: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0004b190: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+0004b1a0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+0004b1b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0004b1c0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+0004b1d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0004b1e0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0004b1f0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+0004b200: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+0004b210: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0004b220: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+0004b230: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004b240: 7465 6d70 5f6d 6f64 656c 203d 2055 7064  temp_model = Upd
+0004b250: 6174 6547 726f 7570 446e 7341 7574 686f  ateGroupDnsAutho
+0004b260: 7269 7a61 7469 6f6e 5275 6c65 5265 7370  rizationRuleResp
+0004b270: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0004b280: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0004b290: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0004b2a0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0004b2b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0004b2c0: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+0004b2d0: 6461 7465 5769 7265 6c65 7373 436c 6f75  dateWirelessClou
+0004b2e0: 6443 6f6e 6e65 6374 6f72 5265 7175 6573  dConnectorReques
+0004b2f0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+0004b300: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0004b310: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0004b320: 2020 2020 2063 6c69 656e 745f 746f 6b65       client_toke
+0004b330: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+0004b340: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+0004b350: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+0004b360: 2020 2020 2020 2020 6472 795f 7275 6e3a          dry_run:
+0004b370: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+0004b380: 2020 2020 2020 6e61 6d65 3a20 7374 7220        name: str 
+0004b390: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0004b3a0: 7769 7265 6c65 7373 5f63 6c6f 7564 5f63  wireless_cloud_c
+0004b3b0: 6f6e 6e65 6374 6f72 5f69 643a 2073 7472  onnector_id: str
+0004b3c0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0004b3d0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+0004b3e0: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
+0004b3f0: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+0004b400: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+0004b410: 6e20 3d20 6465 7363 7269 7074 696f 6e0a  n = description.
+0004b420: 2020 2020 2020 2020 7365 6c66 2e64 7279          self.dry
+0004b430: 5f72 756e 203d 2064 7279 5f72 756e 0a20  _run = dry_run. 
+0004b440: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+0004b450: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+0004b460: 7365 6c66 2e77 6972 656c 6573 735f 636c  self.wireless_cl
+0004b470: 6f75 645f 636f 6e6e 6563 746f 725f 6964  oud_connector_id
+0004b480: 203d 2077 6972 656c 6573 735f 636c 6f75   = wireless_clou
+0004b490: 645f 636f 6e6e 6563 746f 725f 6964 0a0a  d_connector_id..
+0004b4a0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0004b4b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004b4c0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0004b4d0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0004b4e0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0004b4f0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+0004b500: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0004b510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004b520: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0004b530: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0004b540: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0004b550: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
+0004b560: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
+0004b570: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004b580: 7265 7375 6c74 5b27 436c 6965 6e74 546f  result['ClientTo
+0004b590: 6b65 6e27 5d20 3d20 7365 6c66 2e63 6c69  ken'] = self.cli
+0004b5a0: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
+0004b5b0: 2020 6966 2073 656c 662e 6465 7363 7269    if self.descri
+0004b5c0: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
+0004b5d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004b5e0: 6573 756c 745b 2744 6573 6372 6970 7469  esult['Descripti
+0004b5f0: 6f6e 275d 203d 2073 656c 662e 6465 7363  on'] = self.desc
+0004b600: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
+0004b610: 6966 2073 656c 662e 6472 795f 7275 6e20  if self.dry_run 
+0004b620: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004b630: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0004b640: 2744 7279 5275 6e27 5d20 3d20 7365 6c66  'DryRun'] = self
+0004b650: 2e64 7279 5f72 756e 0a20 2020 2020 2020  .dry_run.       
+0004b660: 2069 6620 7365 6c66 2e6e 616d 6520 6973   if self.name is
+0004b670: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0004b680: 2020 2020 2020 2072 6573 756c 745b 274e         result['N
+0004b690: 616d 6527 5d20 3d20 7365 6c66 2e6e 616d  ame'] = self.nam
+0004b6a0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0004b6b0: 662e 7769 7265 6c65 7373 5f63 6c6f 7564  f.wireless_cloud
+0004b6c0: 5f63 6f6e 6e65 6374 6f72 5f69 6420 6973  _connector_id is
+0004b6d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0004b6e0: 2020 2020 2020 2072 6573 756c 745b 2757         result['W
+0004b6f0: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+0004b700: 6563 746f 7249 6427 5d20 3d20 7365 6c66  ectorId'] = self
+0004b710: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+0004b720: 636f 6e6e 6563 746f 725f 6964 0a20 2020  connector_id.   
+0004b730: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0004b740: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+0004b750: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+0004b760: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+0004b770: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0004b780: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0004b790: 2e67 6574 2827 436c 6965 6e74 546f 6b65  .get('ClientToke
+0004b7a0: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+0004b7b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0004b7c0: 662e 636c 6965 6e74 5f74 6f6b 656e 203d  f.client_token =
+0004b7d0: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
+0004b7e0: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+0004b7f0: 206d 2e67 6574 2827 4465 7363 7269 7074   m.get('Descript
+0004b800: 696f 6e27 2920 6973 206e 6f74 204e 6f6e  ion') is not Non
+0004b810: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0004b820: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+0004b830: 3d20 6d2e 6765 7428 2744 6573 6372 6970  = m.get('Descrip
+0004b840: 7469 6f6e 2729 0a20 2020 2020 2020 2069  tion').        i
+0004b850: 6620 6d2e 6765 7428 2744 7279 5275 6e27  f m.get('DryRun'
+0004b860: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0004b870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0004b880: 6472 795f 7275 6e20 3d20 6d2e 6765 7428  dry_run = m.get(
+0004b890: 2744 7279 5275 6e27 290a 2020 2020 2020  'DryRun').      
+0004b8a0: 2020 6966 206d 2e67 6574 2827 4e61 6d65    if m.get('Name
+0004b8b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004b8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0004b8d0: 2e6e 616d 6520 3d20 6d2e 6765 7428 274e  .name = m.get('N
+0004b8e0: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
+0004b8f0: 206d 2e67 6574 2827 5769 7265 6c65 7373   m.get('Wireless
+0004b900: 436c 6f75 6443 6f6e 6e65 6374 6f72 4964  CloudConnectorId
+0004b910: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004b920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0004b930: 2e77 6972 656c 6573 735f 636c 6f75 645f  .wireless_cloud_
+0004b940: 636f 6e6e 6563 746f 725f 6964 203d 206d  connector_id = m
+0004b950: 2e67 6574 2827 5769 7265 6c65 7373 436c  .get('WirelessCl
+0004b960: 6f75 6443 6f6e 6e65 6374 6f72 4964 2729  oudConnectorId')
+0004b970: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0004b980: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+0004b990: 6174 6557 6972 656c 6573 7343 6c6f 7564  ateWirelessCloud
+0004b9a0: 436f 6e6e 6563 746f 7252 6573 706f 6e73  ConnectorRespons
+0004b9b0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+0004b9c0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0004b9d0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0004b9e0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0004b9f0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0004ba00: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0004ba10: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0004ba20: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
+0004ba30: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0004ba40: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0004ba50: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0004ba60: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0004ba70: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0004ba80: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0004ba90: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0004baa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0004bab0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0004bac0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0004bad0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0004bae0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+0004baf0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0004bb00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0004bb10: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+0004bb20: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+0004bb30: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+0004bb40: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0004bb50: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0004bb60: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+0004bb70: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0004bb80: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0004bb90: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+0004bba0: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+0004bbb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004bbc0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0004bbd0: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+0004bbe0: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+0004bbf0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0004bc00: 2055 7064 6174 6557 6972 656c 6573 7343   UpdateWirelessC
+0004bc10: 6c6f 7564 436f 6e6e 6563 746f 7252 6573  loudConnectorRes
+0004bc20: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+0004bc30: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0004bc40: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0004bc50: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+0004bc60: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
+0004bc70: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0004bc80: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
+0004bc90: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+0004bca0: 2020 626f 6479 3a20 5570 6461 7465 5769    body: UpdateWi
+0004bcb0: 7265 6c65 7373 436c 6f75 6443 6f6e 6e65  relessCloudConne
+0004bcc0: 6374 6f72 5265 7370 6f6e 7365 426f 6479  ctorResponseBody
+0004bcd0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0004bce0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0004bcf0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+0004bd00: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0004bd10: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0004bd20: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+0004bd30: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+0004bd40: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0004bd50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004bd60: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0004bd70: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+0004bd80: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+0004bd90: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0004bda0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0004bdb0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+0004bdc0: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+0004bdd0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0004bde0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0004bdf0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+0004be00: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0004be10: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+0004be20: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+0004be30: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+0004be40: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0004be50: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0004be60: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+0004be70: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0004be80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004be90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0004bea0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0004beb0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0004bec0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+0004bed0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+0004bee0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004bef0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+0004bf00: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+0004bf10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0004bf20: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+0004bf30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004bf40: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+0004bf50: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+0004bf60: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+0004bf70: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0004bf80: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0004bf90: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0004bfa0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+0004bfb0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+0004bfc0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0004bfd0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0004bfe0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0004bff0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0004c000: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0004c010: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004c020: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0004c030: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
 0004c040: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0004c050: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0004c060: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0004c070: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0004c080: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0004c090: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0004c0a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0004c0b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0004c0c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0004c0d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0004c0e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0004c0f0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-0004c100: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0004c110: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-0004c120: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-0004c130: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-0004c140: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-0004c150: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-0004c160: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0004c170: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-0004c180: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-0004c190: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-0004c1a0: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-0004c1b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004c1c0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-0004c1d0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-0004c1e0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-0004c1f0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0004c200: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0004c210: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0004c220: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0004c230: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0004c240: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-0004c250: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-0004c260: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0004c270: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0004c280: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0004c290: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0004c2a0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0004c2b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0004c2c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0004c2d0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-0004c2e0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0004c2f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0004c300: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-0004c310: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0004c320: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-0004c330: 5570 6461 7465 5769 7265 6c65 7373 436c  UpdateWirelessCl
-0004c340: 6f75 6443 6f6e 6e65 6374 6f72 4772 6f75  oudConnectorGrou
-0004c350: 7052 6573 706f 6e73 6542 6f64 7928 290a  pResponseBody().
-0004c360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0004c370: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-0004c380: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-0004c390: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-0004c3a0: 6574 7572 6e20 7365 6c66 0a0a 0a         eturn self...
+0004c050: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+0004c060: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+0004c070: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+0004c080: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
+0004c090: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0004c0a0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+0004c0b0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+0004c0c0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+0004c0d0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+0004c0e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004c0f0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0004c100: 5f6d 6f64 656c 203d 2055 7064 6174 6557  _model = UpdateW
+0004c110: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+0004c120: 6563 746f 7252 6573 706f 6e73 6542 6f64  ectorResponseBod
+0004c130: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0004c140: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+0004c150: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+0004c160: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+0004c170: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0004c180: 0a63 6c61 7373 2055 7064 6174 6557 6972  .class UpdateWir
+0004c190: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+0004c1a0: 746f 7247 726f 7570 5265 7175 6573 7428  torGroupRequest(
+0004c1b0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0004c1c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0004c1d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0004c1e0: 2020 2063 6c69 656e 745f 746f 6b65 6e3a     client_token:
+0004c1f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0004c200: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+0004c210: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0004c220: 2020 2020 2020 6472 795f 7275 6e3a 2062        dry_run: b
+0004c230: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
+0004c240: 2020 2020 6e61 6d65 3a20 7374 7220 3d20      name: str = 
+0004c250: 4e6f 6e65 2c0a 2020 2020 2020 2020 7769  None,.        wi
+0004c260: 7265 6c65 7373 5f63 6c6f 7564 5f63 6f6e  reless_cloud_con
+0004c270: 6e65 6374 6f72 5f67 726f 7570 5f69 643a  nector_group_id:
+0004c280: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0004c290: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0004c2a0: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
+0004c2b0: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
+0004c2c0: 2020 2020 2073 656c 662e 6465 7363 7269       self.descri
+0004c2d0: 7074 696f 6e20 3d20 6465 7363 7269 7074  ption = descript
+0004c2e0: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
+0004c2f0: 2e64 7279 5f72 756e 203d 2064 7279 5f72  .dry_run = dry_r
+0004c300: 756e 0a20 2020 2020 2020 2073 656c 662e  un.        self.
+0004c310: 6e61 6d65 203d 206e 616d 650a 2020 2020  name = name.    
+0004c320: 2020 2020 7365 6c66 2e77 6972 656c 6573      self.wireles
+0004c330: 735f 636c 6f75 645f 636f 6e6e 6563 746f  s_cloud_connecto
+0004c340: 725f 6772 6f75 705f 6964 203d 2077 6972  r_group_id = wir
+0004c350: 656c 6573 735f 636c 6f75 645f 636f 6e6e  eless_cloud_conn
+0004c360: 6563 746f 725f 6772 6f75 705f 6964 0a0a  ector_group_id..
+0004c370: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0004c380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004c390: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0004c3a0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0004c3b0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0004c3c0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+0004c3d0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0004c3e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004c3f0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0004c400: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0004c410: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0004c420: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
+0004c430: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
+0004c440: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004c450: 7265 7375 6c74 5b27 436c 6965 6e74 546f  result['ClientTo
+0004c460: 6b65 6e27 5d20 3d20 7365 6c66 2e63 6c69  ken'] = self.cli
+0004c470: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
+0004c480: 2020 6966 2073 656c 662e 6465 7363 7269    if self.descri
+0004c490: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
+0004c4a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004c4b0: 6573 756c 745b 2744 6573 6372 6970 7469  esult['Descripti
+0004c4c0: 6f6e 275d 203d 2073 656c 662e 6465 7363  on'] = self.desc
+0004c4d0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
+0004c4e0: 6966 2073 656c 662e 6472 795f 7275 6e20  if self.dry_run 
+0004c4f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004c500: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0004c510: 2744 7279 5275 6e27 5d20 3d20 7365 6c66  'DryRun'] = self
+0004c520: 2e64 7279 5f72 756e 0a20 2020 2020 2020  .dry_run.       
+0004c530: 2069 6620 7365 6c66 2e6e 616d 6520 6973   if self.name is
+0004c540: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0004c550: 2020 2020 2020 2072 6573 756c 745b 274e         result['N
+0004c560: 616d 6527 5d20 3d20 7365 6c66 2e6e 616d  ame'] = self.nam
+0004c570: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0004c580: 662e 7769 7265 6c65 7373 5f63 6c6f 7564  f.wireless_cloud
+0004c590: 5f63 6f6e 6e65 6374 6f72 5f67 726f 7570  _connector_group
+0004c5a0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0004c5b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0004c5c0: 756c 745b 2757 6972 656c 6573 7343 6c6f  ult['WirelessClo
+0004c5d0: 7564 436f 6e6e 6563 746f 7247 726f 7570  udConnectorGroup
+0004c5e0: 4964 275d 203d 2073 656c 662e 7769 7265  Id'] = self.wire
+0004c5f0: 6c65 7373 5f63 6c6f 7564 5f63 6f6e 6e65  less_cloud_conne
+0004c600: 6374 6f72 5f67 726f 7570 5f69 640a 2020  ctor_group_id.  
+0004c610: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0004c620: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0004c630: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0004c640: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0004c650: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0004c660: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0004c670: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
+0004c680: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
+0004c690: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0004c6a0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+0004c6b0: 3d20 6d2e 6765 7428 2743 6c69 656e 7454  = m.get('ClientT
+0004c6c0: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
+0004c6d0: 6620 6d2e 6765 7428 2744 6573 6372 6970  f m.get('Descrip
+0004c6e0: 7469 6f6e 2729 2069 7320 6e6f 7420 4e6f  tion') is not No
+0004c6f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0004c700: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
+0004c710: 203d 206d 2e67 6574 2827 4465 7363 7269   = m.get('Descri
+0004c720: 7074 696f 6e27 290a 2020 2020 2020 2020  ption').        
+0004c730: 6966 206d 2e67 6574 2827 4472 7952 756e  if m.get('DryRun
+0004c740: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004c750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0004c760: 2e64 7279 5f72 756e 203d 206d 2e67 6574  .dry_run = m.get
+0004c770: 2827 4472 7952 756e 2729 0a20 2020 2020  ('DryRun').     
+0004c780: 2020 2069 6620 6d2e 6765 7428 274e 616d     if m.get('Nam
+0004c790: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0004c7a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0004c7b0: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
+0004c7c0: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+0004c7d0: 6620 6d2e 6765 7428 2757 6972 656c 6573  f m.get('Wireles
+0004c7e0: 7343 6c6f 7564 436f 6e6e 6563 746f 7247  sCloudConnectorG
+0004c7f0: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
+0004c800: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004c810: 2020 7365 6c66 2e77 6972 656c 6573 735f    self.wireless_
+0004c820: 636c 6f75 645f 636f 6e6e 6563 746f 725f  cloud_connector_
+0004c830: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+0004c840: 2827 5769 7265 6c65 7373 436c 6f75 6443  ('WirelessCloudC
+0004c850: 6f6e 6e65 6374 6f72 4772 6f75 7049 6427  onnectorGroupId'
+0004c860: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0004c870: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+0004c880: 6461 7465 5769 7265 6c65 7373 436c 6f75  dateWirelessClou
+0004c890: 6443 6f6e 6e65 6374 6f72 4772 6f75 7052  dConnectorGroupR
+0004c8a0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+0004c8b0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0004c8c0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0004c8d0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
+0004c8e0: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
+0004c8f0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0004c900: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0004c910: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0004c920: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
+0004c930: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0004c940: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+0004c950: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0004c960: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0004c970: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+0004c980: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0004c990: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004c9a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0004c9b0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0004c9c0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0004c9d0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+0004c9e0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
+0004c9f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0004ca00: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
+0004ca10: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
+0004ca20: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
+0004ca30: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0004ca40: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0004ca50: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0004ca60: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0004ca70: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0004ca80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0004ca90: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+0004caa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0004cab0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0004cac0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+0004cad0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+0004cae0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0004caf0: 0a63 6c61 7373 2055 7064 6174 6557 6972  .class UpdateWir
+0004cb00: 656c 6573 7343 6c6f 7564 436f 6e6e 6563  elessCloudConnec
+0004cb10: 746f 7247 726f 7570 5265 7370 6f6e 7365  torGroupResponse
+0004cb20: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0004cb30: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0004cb40: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0004cb50: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0004cb60: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0004cb70: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0004cb80: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0004cb90: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0004cba0: 793a 2055 7064 6174 6557 6972 656c 6573  y: UpdateWireles
+0004cbb0: 7343 6c6f 7564 436f 6e6e 6563 746f 7247  sCloudConnectorG
+0004cbc0: 726f 7570 5265 7370 6f6e 7365 426f 6479  roupResponseBody
+0004cbd0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0004cbe0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0004cbf0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+0004cc00: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0004cc10: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0004cc20: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+0004cc30: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+0004cc40: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0004cc50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0004cc60: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0004cc70: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+0004cc80: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+0004cc90: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0004cca0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0004ccb0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+0004ccc0: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+0004ccd0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0004cce0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0004ccf0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+0004cd00: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0004cd10: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+0004cd20: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+0004cd30: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+0004cd40: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0004cd50: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0004cd60: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+0004cd70: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0004cd80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0004cd90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0004cda0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0004cdb0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0004cdc0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+0004cdd0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+0004cde0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0004cdf0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+0004ce00: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+0004ce10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0004ce20: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+0004ce30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0004ce40: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+0004ce50: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+0004ce60: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+0004ce70: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0004ce80: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0004ce90: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0004cea0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+0004ceb0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+0004cec0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0004ced0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0004cee0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0004cef0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0004cf00: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0004cf10: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0004cf20: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0004cf30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0004cf40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0004cf50: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+0004cf60: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+0004cf70: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+0004cf80: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
+0004cf90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0004cfa0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+0004cfb0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+0004cfc0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+0004cfd0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+0004cfe0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0004cff0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0004d000: 5f6d 6f64 656c 203d 2055 7064 6174 6557  _model = UpdateW
+0004d010: 6972 656c 6573 7343 6c6f 7564 436f 6e6e  irelessCloudConn
+0004d020: 6563 746f 7247 726f 7570 5265 7370 6f6e  ectorGroupRespon
+0004d030: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0004d040: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0004d050: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0004d060: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0004d070: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0004d080: 656c 660a 0a0a                           elf...
```

### Comparing `alibabacloud_cc5g20220314-2.0.8/alibabacloud_cc5g20220314.egg-info/PKG-INFO` & `alibabacloud_cc5g20220314-2.0.9/alibabacloud_cc5g20220314.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cc5g20220314
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud CC5G (20220314) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cc5g20220314-2.0.8/setup.py` & `alibabacloud_cc5g20220314-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cc5g20220314.
 
-Created on 21/02/2023
+Created on 04/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cc5g20220314"
 NAME = "alibabacloud_cc5g20220314" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CC5G (20220314) SDK Library for Python"
```

