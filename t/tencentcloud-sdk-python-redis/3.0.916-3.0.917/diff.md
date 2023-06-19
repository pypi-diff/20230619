# Comparing `tmp/tencentcloud-sdk-python-redis-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-redis-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.916.tar", last modified: Fri Jun 16 00:39:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-redis-3.0.917.tar", last modified: Mon Jun 19 00:31:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-redis-3.0.916.tar` & `tencentcloud-sdk-python-redis-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87184 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)   297548 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-16 00:39:22.000000 tencentcloud-sdk-python-redis-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87184 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)   298078 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-19 00:31:03.000000 tencentcloud-sdk-python-redis-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-redis-3.0.916/tencentcloud_sdk_python_redis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.917/tencentcloud_sdk_python_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-redis-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/redis_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2047,15 +2047,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpgradeInstanceVersion(self, request):
-        """将原本实例升级到高版本实例，或者将主从版实例升级到集群版实例
+        """将当前实例升级到更高版本，或者将当前标准架构升级至集群架构。
 
         :param request: Request instance for UpgradeInstanceVersion.
         :type request: :class:`tencentcloud.redis.v20180412.models.UpgradeInstanceVersionRequest`
         :rtype: :class:`tencentcloud.redis.v20180412.models.UpgradeInstanceVersionResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8233,19 +8233,26 @@
 class UpgradeInstanceVersionRequest(AbstractModel):
     """UpgradeInstanceVersion请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TargetInstanceType: 目标实例类型，同 [CreateInstances](https://cloud.tencent.com/document/api/239/20026) 的Type，即实例要变更的目标类型
+        :param TargetInstanceType: 目标实例类型，同 [CreateInstances](https://cloud.tencent.com/document/api/239/20026) 的**TypeId**，即实例要变更的目标类型。
+- Redis 4.0 及以上的版本，支持相同版本的实例从标准架构升级至集群架构，例如，支持 Redis 4.0 标准架构升级至 Redis 4.0 集群架构。
+- 不支持跨版本架构升级，例如，Redis 4.0 标准架构升级至 Redis 5.0 集群架构。
+- 不支持 Redis 2.8 版本升级架构。
+- 不支持从集群架构降级至标准架构。
+
         :type TargetInstanceType: str
-        :param SwitchOption: 切换模式：1-维护时间窗切换，2-立即切换
+        :param SwitchOption: 切换时间。
+- 1：维护时间窗切换。
+- 2：立即切换。
         :type SwitchOption: int
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定实例 ID。例如：crs-xjhsdj****，请登录[Redis控制台](https://console.cloud.tencent.com/redis#/)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.TargetInstanceType = None
         self.SwitchOption = None
         self.InstanceId = None
```

### Comparing `tencentcloud-sdk-python-redis-3.0.916/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-redis-3.0.917/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.916/README.rst` & `tencentcloud-sdk-python-redis-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-redis-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-redis-3.0.917/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-redis
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Redis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-redis-3.0.916/setup.py` & `tencentcloud-sdk-python-redis-3.0.917/setup.py`

 * *Files identical despite different names*

