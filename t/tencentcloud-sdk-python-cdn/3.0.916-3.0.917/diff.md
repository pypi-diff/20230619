# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.916.tar", last modified: Fri Jun 16 00:29:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.917.tar", last modified: Mon Jun 19 00:20:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.916.tar` & `tencentcloud-sdk-python-cdn-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   573678 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)    21972 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:29:12.000000 tencentcloud-sdk-python-cdn-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   573678 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)    80792 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)    21972 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:20:12.000000 tencentcloud-sdk-python-cdn-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.916'
+__version__ = '3.0.917'
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateVerifyRecord(self, request):
         """CreateVerifyRecord 用于生成一条子域名解析，提示客户添加到域名解析上，用于泛域名及域名取回校验归属权。
         生成的解析记录可通过 [VerifyDomainRecord](https://cloud.tencent.com/document/product/228/48117) 完成归属权校验。
+        注意：生成的解析记录有效期为24小时，超过24小时后，需重新生成。
         具体流程可参考：[使用API接口进行域名归属校验](https://cloud.tencent.com/document/product/228/61702#.E6.96.B9.E6.B3.95.E4.B8.89.EF.BC.9Aapi-.E6.8E.A5.E5.8F.A3.E6.93.8D.E4.BD.9C)
 
         :param request: Request instance for CreateVerifyRecord.
         :type request: :class:`tencentcloud.cdn.v20180606.models.CreateVerifyRecordRequest`
         :rtype: :class:`tencentcloud.cdn.v20180606.models.CreateVerifyRecordResponse`
 
         """
@@ -1897,15 +1898,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def VerifyDomainRecord(self, request):
         """VerifyDomainRecord 用于验证域名解析值。
-        验证域名解析记录值前，您需要通过 [CreateVerifyRecord](https://cloud.tencent.com/document/product/228/48118) 生成校验解析值。
+        验证域名解析记录值前，您需要通过 [CreateVerifyRecord](https://cloud.tencent.com/document/product/228/48118) 生成校验解析值，验证通过后，24小时有效。
         具体流程可参考：[使用API接口进行域名归属校验](https://cloud.tencent.com/document/product/228/61702#.E6.96.B9.E6.B3.95.E4.B8.89.EF.BC.9Aapi-.E6.8E.A5.E5.8F.A3.E6.93.8D.E4.BD.9C)
 
         :param request: Request instance for VerifyDomainRecord.
         :type request: :class:`tencentcloud.cdn.v20180606.models.VerifyDomainRecordRequest`
         :rtype: :class:`tencentcloud.cdn.v20180606.models.VerifyDomainRecordResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.917/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/README.rst` & `tencentcloud-sdk-python-cdn-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.917/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.917/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.916/setup.py` & `tencentcloud-sdk-python-cdn-3.0.917/setup.py`

 * *Files identical despite different names*

