# Comparing `tmp/alibabacloud_cc5g20220314_py2-1.0.8.tar.gz` & `tmp/alibabacloud_cc5g20220314_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cc5g20220314_py2-1.0.8.tar", last modified: Fri Sep 30 03:32:47 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cc5g20220314_py2-1.0.9.tar", last modified: Thu Oct 13 12:02:58 2022, max compression
```

## Comparing `alibabacloud_cc5g20220314_py2-1.0.8.tar` & `alibabacloud_cc5g20220314_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      140 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57594 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/client.py
--rw-r--r--   0 root         (0) root         (0)   220208 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2022-09-30 03:32:47.000000 alibabacloud_cc5g20220314_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      175 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59449 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/client.py
+-rw-r--r--   0 root         (0) root         (0)   237210 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2022-10-13 12:02:58.000000 alibabacloud_cc5g20220314_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/LICENSE` & `alibabacloud_cc5g20220314_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/PKG-INFO` & `alibabacloud_cc5g20220314_py2-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cc5g20220314_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud CC5G (20220314) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/README-CN.md` & `alibabacloud_cc5g20220314_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/README.md` & `alibabacloud_cc5g20220314_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/client.py` & `alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,14 +652,40 @@
             self.call_api(params, req, runtime)
         )
 
     def grant_net_link(self, request):
         runtime = util_models.RuntimeOptions()
         return self.grant_net_link_with_options(request, runtime)
 
+    def list_apns_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListAPNs',
+            version='2022-03-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cc5g20220314_models.ListAPNsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_apns(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_apns_with_options(request, runtime)
+
     def list_authorization_rules_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -874,14 +900,40 @@
             self.call_api(params, req, runtime)
         )
 
     def list_regions(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_regions_with_options(request, runtime)
 
+    def list_wireless_cloud_connectors_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListWirelessCloudConnectors',
+            version='2022-03-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cc5g20220314_models.ListWirelessCloudConnectorsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_wireless_cloud_connectors(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_wireless_cloud_connectors_with_options(request, runtime)
+
     def list_zones_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314/models.py` & `alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2407,14 +2407,193 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GrantNetLinkResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListAPNsRequest(TeaModel):
+    def __init__(self, apn=None, isp=None, max_results=None, next_token=None, region_id=None):
+        self.apn = apn  # type: str
+        self.isp = isp  # type: str
+        self.max_results = max_results  # type: long
+        self.next_token = next_token  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListAPNsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.apn is not None:
+            result['APN'] = self.apn
+        if self.isp is not None:
+            result['ISP'] = self.isp
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('APN') is not None:
+            self.apn = m.get('APN')
+        if m.get('ISP') is not None:
+            self.isp = m.get('ISP')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListAPNsResponseBodyAPNs(TeaModel):
+    def __init__(self, apn=None, description=None, isp=None, name=None, zones=None):
+        self.apn = apn  # type: str
+        self.description = description  # type: str
+        self.isp = isp  # type: str
+        self.name = name  # type: str
+        self.zones = zones  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListAPNsResponseBodyAPNs, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.apn is not None:
+            result['APN'] = self.apn
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.isp is not None:
+            result['ISP'] = self.isp
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.zones is not None:
+            result['Zones'] = self.zones
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('APN') is not None:
+            self.apn = m.get('APN')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ISP') is not None:
+            self.isp = m.get('ISP')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Zones') is not None:
+            self.zones = m.get('Zones')
+        return self
+
+
+class ListAPNsResponseBody(TeaModel):
+    def __init__(self, apns=None, max_results=None, next_token=None, request_id=None, total_count=None):
+        self.apns = apns  # type: list[ListAPNsResponseBodyAPNs]
+        self.max_results = max_results  # type: str
+        self.next_token = next_token  # type: str
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: str
+
+    def validate(self):
+        if self.apns:
+            for k in self.apns:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListAPNsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['APNs'] = []
+        if self.apns is not None:
+            for k in self.apns:
+                result['APNs'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.apns = []
+        if m.get('APNs') is not None:
+            for k in m.get('APNs'):
+                temp_model = ListAPNsResponseBodyAPNs()
+                self.apns.append(temp_model.from_map(k))
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListAPNsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListAPNsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListAPNsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListAPNsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListAuthorizationRulesRequest(TeaModel):
     def __init__(self, authorization_rule_ids=None, destination=None, destination_port=None, destination_type=None,
                  dns=None, max_results=None, names=None, next_token=None, policy=None, protocol=None, statuses=None,
                  type=None, wireless_cloud_connector_id=None):
         self.authorization_rule_ids = authorization_rule_ids  # type: list[str]
         self.destination = destination  # type: str
         self.destination_port = destination_port  # type: str
@@ -4183,14 +4362,257 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListWirelessCloudConnectorsRequest(TeaModel):
+    def __init__(self, business_type=None, is_in_group=None, max_results=None, names=None, next_token=None,
+                 region_id=None, statuses=None, wireless_cloud_connector_group_id=None, wireless_cloud_connector_ids=None):
+        self.business_type = business_type  # type: str
+        self.is_in_group = is_in_group  # type: str
+        self.max_results = max_results  # type: long
+        self.names = names  # type: list[str]
+        self.next_token = next_token  # type: str
+        self.region_id = region_id  # type: str
+        self.statuses = statuses  # type: list[str]
+        self.wireless_cloud_connector_group_id = wireless_cloud_connector_group_id  # type: str
+        self.wireless_cloud_connector_ids = wireless_cloud_connector_ids  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListWirelessCloudConnectorsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.business_type is not None:
+            result['BusinessType'] = self.business_type
+        if self.is_in_group is not None:
+            result['IsInGroup'] = self.is_in_group
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.names is not None:
+            result['Names'] = self.names
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.statuses is not None:
+            result['Statuses'] = self.statuses
+        if self.wireless_cloud_connector_group_id is not None:
+            result['WirelessCloudConnectorGroupId'] = self.wireless_cloud_connector_group_id
+        if self.wireless_cloud_connector_ids is not None:
+            result['WirelessCloudConnectorIds'] = self.wireless_cloud_connector_ids
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BusinessType') is not None:
+            self.business_type = m.get('BusinessType')
+        if m.get('IsInGroup') is not None:
+            self.is_in_group = m.get('IsInGroup')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('Names') is not None:
+            self.names = m.get('Names')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Statuses') is not None:
+            self.statuses = m.get('Statuses')
+        if m.get('WirelessCloudConnectorGroupId') is not None:
+            self.wireless_cloud_connector_group_id = m.get('WirelessCloudConnectorGroupId')
+        if m.get('WirelessCloudConnectorIds') is not None:
+            self.wireless_cloud_connector_ids = m.get('WirelessCloudConnectorIds')
+        return self
+
+
+class ListWirelessCloudConnectorsResponseBodyWirelessCloudConnectors(TeaModel):
+    def __init__(self, business_type=None, card_count=None, create_time=None, data_package_id=None,
+                 data_package_type=None, description=None, name=None, region_id=None, service_type=None, status=None, use_case=None,
+                 wireless_cloud_connector_group_id=None, wireless_cloud_connector_id=None):
+        self.business_type = business_type  # type: str
+        self.card_count = card_count  # type: str
+        self.create_time = create_time  # type: str
+        self.data_package_id = data_package_id  # type: str
+        self.data_package_type = data_package_type  # type: str
+        self.description = description  # type: str
+        self.name = name  # type: str
+        self.region_id = region_id  # type: str
+        self.service_type = service_type  # type: str
+        self.status = status  # type: str
+        self.use_case = use_case  # type: str
+        self.wireless_cloud_connector_group_id = wireless_cloud_connector_group_id  # type: str
+        self.wireless_cloud_connector_id = wireless_cloud_connector_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListWirelessCloudConnectorsResponseBodyWirelessCloudConnectors, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.business_type is not None:
+            result['BusinessType'] = self.business_type
+        if self.card_count is not None:
+            result['CardCount'] = self.card_count
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.data_package_id is not None:
+            result['DataPackageId'] = self.data_package_id
+        if self.data_package_type is not None:
+            result['DataPackageType'] = self.data_package_type
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.use_case is not None:
+            result['UseCase'] = self.use_case
+        if self.wireless_cloud_connector_group_id is not None:
+            result['WirelessCloudConnectorGroupId'] = self.wireless_cloud_connector_group_id
+        if self.wireless_cloud_connector_id is not None:
+            result['WirelessCloudConnectorId'] = self.wireless_cloud_connector_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BusinessType') is not None:
+            self.business_type = m.get('BusinessType')
+        if m.get('CardCount') is not None:
+            self.card_count = m.get('CardCount')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('DataPackageId') is not None:
+            self.data_package_id = m.get('DataPackageId')
+        if m.get('DataPackageType') is not None:
+            self.data_package_type = m.get('DataPackageType')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UseCase') is not None:
+            self.use_case = m.get('UseCase')
+        if m.get('WirelessCloudConnectorGroupId') is not None:
+            self.wireless_cloud_connector_group_id = m.get('WirelessCloudConnectorGroupId')
+        if m.get('WirelessCloudConnectorId') is not None:
+            self.wireless_cloud_connector_id = m.get('WirelessCloudConnectorId')
+        return self
+
+
+class ListWirelessCloudConnectorsResponseBody(TeaModel):
+    def __init__(self, max_results=None, next_token=None, request_id=None, total_count=None,
+                 wireless_cloud_connectors=None):
+        self.max_results = max_results  # type: str
+        self.next_token = next_token  # type: str
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: str
+        self.wireless_cloud_connectors = wireless_cloud_connectors  # type: list[ListWirelessCloudConnectorsResponseBodyWirelessCloudConnectors]
+
+    def validate(self):
+        if self.wireless_cloud_connectors:
+            for k in self.wireless_cloud_connectors:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListWirelessCloudConnectorsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        result['WirelessCloudConnectors'] = []
+        if self.wireless_cloud_connectors is not None:
+            for k in self.wireless_cloud_connectors:
+                result['WirelessCloudConnectors'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        self.wireless_cloud_connectors = []
+        if m.get('WirelessCloudConnectors') is not None:
+            for k in m.get('WirelessCloudConnectors'):
+                temp_model = ListWirelessCloudConnectorsResponseBodyWirelessCloudConnectors()
+                self.wireless_cloud_connectors.append(temp_model.from_map(k))
+        return self
+
+
+class ListWirelessCloudConnectorsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListWirelessCloudConnectorsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListWirelessCloudConnectorsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListWirelessCloudConnectorsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListZonesRequest(TeaModel):
     def __init__(self, region_id=None):
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/alibabacloud_cc5g20220314_py2.egg-info/PKG-INFO` & `alibabacloud_cc5g20220314_py2-1.0.9/alibabacloud_cc5g20220314_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cc5g20220314-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud CC5G (20220314) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cc5g20220314_py2-1.0.8/setup.py` & `alibabacloud_cc5g20220314_py2-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cc5g20220314_py2.
 
-Created on 30/09/2022
+Created on 13/10/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cc5g20220314"
 NAME = "alibabacloud_cc5g20220314_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CC5G (20220314) SDK Library for Python2"
```

