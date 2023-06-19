# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.916.tar", last modified: Fri Jun 16 00:38:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.917.tar", last modified: Mon Jun 19 00:30:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.916.tar` & `tencentcloud-sdk-python-oceanus-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23497 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)   113771 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-16 00:38:30.000000 tencentcloud-sdk-python-oceanus-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24382 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)   125223 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-19 00:30:12.000000 tencentcloud-sdk-python-oceanus-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,14 +505,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeWorkSpaces(self, request):
+        """授权工作空间列表
+
+        :param request: Request instance for DescribeWorkSpaces.
+        :type request: :class:`tencentcloud.oceanus.v20190422.models.DescribeWorkSpacesRequest`
+        :rtype: :class:`tencentcloud.oceanus.v20190422.models.DescribeWorkSpacesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeWorkSpaces", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeWorkSpacesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyJob(self, request):
         """更新作业属性，仅允许以下3种操作，不支持组合操作：
         (1)	更新作业名称
         (2)	更新作业备注
         (3)	更新作业最大并行度
         变更前提：WorkerCuNum<=MaxParallelism
         如果MaxParallelism变小，不重启作业，待下一次重启生效
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,14 +316,110 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ClusterGroupSetItem(AbstractModel):
+    """工作空间集群组信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: clusterGroup 的 SerialId
+        :type ClusterId: str
+        :param Name: 集群名称
+        :type Name: str
+        :param Region: 地域
+        :type Region: str
+        :param Zone: 区
+        :type Zone: str
+        :param AppId: 账号 APPID
+        :type AppId: int
+        :param OwnerUin: 主账号 UIN
+        :type OwnerUin: str
+        :param CreatorUin: 创建账号 UIN
+        :type CreatorUin: str
+        :param CuNum: CU 数量
+        :type CuNum: int
+        :param CuMem: CU 内存规格
+        :type CuMem: int
+        :param Status: 集群状态, 1 未初始化,，3 初始化中，2 运行中
+        :type Status: int
+        :param StatusDesc: 状态描述
+        :type StatusDesc: str
+        :param CreateTime: 集群创建时间
+        :type CreateTime: str
+        :param UpdateTime: 最后一次操作集群的时间
+        :type UpdateTime: str
+        :param Remark: 描述
+        :type Remark: str
+        :param NetEnvironmentType: 网络
+        :type NetEnvironmentType: int
+        :param FreeCuNum: 空闲 CU
+        :type FreeCuNum: int
+        :param FreeCu: 细粒度资源下的空闲CU
+        :type FreeCu: float
+        :param RunningCu: 运行中CU
+        :type RunningCu: float
+        :param PayMode: 付费模式
+        :type PayMode: int
+        """
+        self.ClusterId = None
+        self.Name = None
+        self.Region = None
+        self.Zone = None
+        self.AppId = None
+        self.OwnerUin = None
+        self.CreatorUin = None
+        self.CuNum = None
+        self.CuMem = None
+        self.Status = None
+        self.StatusDesc = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Remark = None
+        self.NetEnvironmentType = None
+        self.FreeCuNum = None
+        self.FreeCu = None
+        self.RunningCu = None
+        self.PayMode = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.Name = params.get("Name")
+        self.Region = params.get("Region")
+        self.Zone = params.get("Zone")
+        self.AppId = params.get("AppId")
+        self.OwnerUin = params.get("OwnerUin")
+        self.CreatorUin = params.get("CreatorUin")
+        self.CuNum = params.get("CuNum")
+        self.CuMem = params.get("CuMem")
+        self.Status = params.get("Status")
+        self.StatusDesc = params.get("StatusDesc")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Remark = params.get("Remark")
+        self.NetEnvironmentType = params.get("NetEnvironmentType")
+        self.FreeCuNum = params.get("FreeCuNum")
+        self.FreeCu = params.get("FreeCu")
+        self.RunningCu = params.get("RunningCu")
+        self.PayMode = params.get("PayMode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ClusterSession(AbstractModel):
     """session集群信息
 
     """
 
 
 class ClusterVersion(AbstractModel):
@@ -1937,14 +2033,86 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeWorkSpacesRequest(AbstractModel):
+    """DescribeWorkSpaces请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Offset: 偏移量，默认 0
+        :type Offset: int
+        :param OrderType: 1 按照创建时间降序排序(默认) 2.按照创建时间升序排序，3. 按照状态降序排序 4. 按照状态升序排序 默认为0
+        :type OrderType: int
+        :param Limit: 请求的集群数量，默认 20
+        :type Limit: int
+        :param Filters: 过滤规则
+        :type Filters: list of Filter
+        """
+        self.Offset = None
+        self.OrderType = None
+        self.Limit = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.Offset = params.get("Offset")
+        self.OrderType = params.get("OrderType")
+        self.Limit = params.get("Limit")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeWorkSpacesResponse(AbstractModel):
+    """DescribeWorkSpaces返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param WorkSpaceSetItem: 空间详情列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WorkSpaceSetItem: list of WorkSpaceSetItem
+        :param TotalCount: 空间总数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.WorkSpaceSetItem = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("WorkSpaceSetItem") is not None:
+            self.WorkSpaceSetItem = []
+            for item in params.get("WorkSpaceSetItem"):
+                obj = WorkSpaceSetItem()
+                obj._deserialize(item)
+                self.WorkSpaceSetItem.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class Filter(AbstractModel):
     """查询作业列表时的过滤器
 
     """
 
     def __init__(self):
         r"""
@@ -2752,14 +2920,85 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RoleAuth(AbstractModel):
+    """角色授权信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppId: 用户 AppID
+        :type AppId: int
+        :param WorkSpaceSerialId: 工作空间 SerialId
+        :type WorkSpaceSerialId: str
+        :param OwnerUin: 主账号 UIN
+        :type OwnerUin: str
+        :param CreatorUin: 创建者 UIN
+        :type CreatorUin: str
+        :param AuthSubAccountUin: 绑定授权的 UIN
+        :type AuthSubAccountUin: str
+        :param Permission: 对应 role表的id
+        :type Permission: int
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param UpdateTime: 最后一次操作时间
+        :type UpdateTime: str
+        :param Status: 2 启用 1 停用
+        :type Status: int
+        :param Id: id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: int
+        :param WorkSpaceId: 工作空间id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WorkSpaceId: int
+        :param RoleName: 权限名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RoleName: str
+        """
+        self.AppId = None
+        self.WorkSpaceSerialId = None
+        self.OwnerUin = None
+        self.CreatorUin = None
+        self.AuthSubAccountUin = None
+        self.Permission = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Status = None
+        self.Id = None
+        self.WorkSpaceId = None
+        self.RoleName = None
+
+
+    def _deserialize(self, params):
+        self.AppId = params.get("AppId")
+        self.WorkSpaceSerialId = params.get("WorkSpaceSerialId")
+        self.OwnerUin = params.get("OwnerUin")
+        self.CreatorUin = params.get("CreatorUin")
+        self.AuthSubAccountUin = params.get("AuthSubAccountUin")
+        self.Permission = params.get("Permission")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        self.WorkSpaceId = params.get("WorkSpaceId")
+        self.RoleName = params.get("RoleName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RunJobDescription(AbstractModel):
     """作业启动详情
 
     """
 
     def __init__(self):
         r"""
@@ -3268,8 +3507,99 @@
         self.ProjectIdStr = params.get("ProjectIdStr")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class WorkSpaceSetItem(AbstractModel):
+    """工作空间详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SerialId: 工作空间 SerialId
+        :type SerialId: str
+        :param AppId: 用户 APPID
+        :type AppId: int
+        :param OwnerUin: 主账号 UIN
+        :type OwnerUin: str
+        :param CreatorUin: 创建者 UIN
+        :type CreatorUin: str
+        :param WorkSpaceName: 工作空间名称
+        :type WorkSpaceName: str
+        :param Region: 区域
+        :type Region: str
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+        :type UpdateTime: str
+        :param Status: 1 未初始化 2 可用  -1 已删除
+        :type Status: int
+        :param Description: 工作空间描述
+        :type Description: str
+        :param ClusterGroupSetItem: 工作空间包含集群信息
+        :type ClusterGroupSetItem: list of ClusterGroupSetItem
+        :param RoleAuth: 工作空间角色的信息
+        :type RoleAuth: list of RoleAuth
+        :param RoleAuthCount: 工作空间成员数量
+        :type RoleAuthCount: int
+        :param WorkSpaceId: 工作空间 SerialId
+        :type WorkSpaceId: str
+        :param JobsCount: 1
+注意：此字段可能返回 null，表示取不到有效值。
+        :type JobsCount: int
+        """
+        self.SerialId = None
+        self.AppId = None
+        self.OwnerUin = None
+        self.CreatorUin = None
+        self.WorkSpaceName = None
+        self.Region = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Status = None
+        self.Description = None
+        self.ClusterGroupSetItem = None
+        self.RoleAuth = None
+        self.RoleAuthCount = None
+        self.WorkSpaceId = None
+        self.JobsCount = None
+
+
+    def _deserialize(self, params):
+        self.SerialId = params.get("SerialId")
+        self.AppId = params.get("AppId")
+        self.OwnerUin = params.get("OwnerUin")
+        self.CreatorUin = params.get("CreatorUin")
+        self.WorkSpaceName = params.get("WorkSpaceName")
+        self.Region = params.get("Region")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Status = params.get("Status")
+        self.Description = params.get("Description")
+        if params.get("ClusterGroupSetItem") is not None:
+            self.ClusterGroupSetItem = []
+            for item in params.get("ClusterGroupSetItem"):
+                obj = ClusterGroupSetItem()
+                obj._deserialize(item)
+                self.ClusterGroupSetItem.append(obj)
+        if params.get("RoleAuth") is not None:
+            self.RoleAuth = []
+            for item in params.get("RoleAuth"):
+                obj = RoleAuth()
+                obj._deserialize(item)
+                self.RoleAuth.append(obj)
+        self.RoleAuthCount = params.get("RoleAuthCount")
+        self.WorkSpaceId = params.get("WorkSpaceId")
+        self.JobsCount = params.get("JobsCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.917/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.917/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.916/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.917/setup.py`

 * *Files identical despite different names*

