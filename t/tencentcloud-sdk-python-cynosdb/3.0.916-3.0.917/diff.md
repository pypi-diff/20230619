# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.916.tar", last modified: Fri Jun 16 00:31:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.917.tar", last modified: Mon Jun 19 00:23:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.916.tar` & `tencentcloud-sdk-python-cynosdb-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   370876 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)   107865 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    11040 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-16 00:31:45.000000 tencentcloud-sdk-python-cynosdb-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   412392 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)   116655 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    11095 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-19 00:23:07.000000 tencentcloud-sdk-python-cynosdb-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1008,14 +1008,71 @@
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
+class CloseProxyRequest(AbstractModel):
+    """CloseProxy请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param OnlyCloseRW: 是否只关闭读写分离，取值：是 "true","false"
+        :type OnlyCloseRW: bool
+        """
+        self.ClusterId = None
+        self.ProxyGroupId = None
+        self.OnlyCloseRW = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.OnlyCloseRW = params.get("OnlyCloseRW")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CloseProxyResponse(AbstractModel):
+    """CloseProxy返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class CloseWanRequest(AbstractModel):
     """CloseWan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1853,14 +1910,238 @@
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateProxyEndPointRequest(AbstractModel):
+    """CreateProxyEndPoint请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param UniqueVpcId: 私有网络ID，默认与集群私有网络ID保持一致
+        :type UniqueVpcId: str
+        :param UniqueSubnetId: 私有网络子网ID，默认与集群子网ID保持一致
+        :type UniqueSubnetId: str
+        :param ConnectionPoolType: 连接池类型：SessionConnectionPool(会话级别连接池 )
+        :type ConnectionPoolType: str
+        :param OpenConnectionPool: 是否开启连接池,yes-开启，no-不开启
+        :type OpenConnectionPool: str
+        :param ConnectionPoolTimeOut: 连接池阀值：单位（秒）
+        :type ConnectionPoolTimeOut: int
+        :param SecurityGroupIds: 安全组ID数组
+        :type SecurityGroupIds: list of str
+        :param Description: 描述说明
+        :type Description: str
+        :param Vip: vip信息
+        :type Vip: str
+        :param WeightMode: 权重模式：
+system-系统分配，custom-自定义
+        :type WeightMode: str
+        :param AutoAddRo: 是否自动添加只读实例，yes-是，no-不自动添加
+        :type AutoAddRo: str
+        :param FailOver: 是否开启故障转移
+        :type FailOver: str
+        :param ConsistencyType: 一致性类型：
+eventual,global,session
+        :type ConsistencyType: str
+        :param RwType: 读写属性：
+READWRITE,READONLY
+        :type RwType: str
+        :param ConsistencyTimeOut: 一致性超时时间
+        :type ConsistencyTimeOut: int
+        :param TransSplit: 事务拆分
+        :type TransSplit: bool
+        :param AccessMode: 连接模式：
+nearby,balance
+        :type AccessMode: str
+        :param InstanceWeights: 实例权重
+        :type InstanceWeights: list of ProxyInstanceWeight
+        """
+        self.ClusterId = None
+        self.UniqueVpcId = None
+        self.UniqueSubnetId = None
+        self.ConnectionPoolType = None
+        self.OpenConnectionPool = None
+        self.ConnectionPoolTimeOut = None
+        self.SecurityGroupIds = None
+        self.Description = None
+        self.Vip = None
+        self.WeightMode = None
+        self.AutoAddRo = None
+        self.FailOver = None
+        self.ConsistencyType = None
+        self.RwType = None
+        self.ConsistencyTimeOut = None
+        self.TransSplit = None
+        self.AccessMode = None
+        self.InstanceWeights = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.UniqueVpcId = params.get("UniqueVpcId")
+        self.UniqueSubnetId = params.get("UniqueSubnetId")
+        self.ConnectionPoolType = params.get("ConnectionPoolType")
+        self.OpenConnectionPool = params.get("OpenConnectionPool")
+        self.ConnectionPoolTimeOut = params.get("ConnectionPoolTimeOut")
+        self.SecurityGroupIds = params.get("SecurityGroupIds")
+        self.Description = params.get("Description")
+        self.Vip = params.get("Vip")
+        self.WeightMode = params.get("WeightMode")
+        self.AutoAddRo = params.get("AutoAddRo")
+        self.FailOver = params.get("FailOver")
+        self.ConsistencyType = params.get("ConsistencyType")
+        self.RwType = params.get("RwType")
+        self.ConsistencyTimeOut = params.get("ConsistencyTimeOut")
+        self.TransSplit = params.get("TransSplit")
+        self.AccessMode = params.get("AccessMode")
+        if params.get("InstanceWeights") is not None:
+            self.InstanceWeights = []
+            for item in params.get("InstanceWeights"):
+                obj = ProxyInstanceWeight()
+                obj._deserialize(item)
+                self.InstanceWeights.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateProxyEndPointResponse(AbstractModel):
+    """CreateProxyEndPoint返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
+class CreateProxyRequest(AbstractModel):
+    """CreateProxy请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param Cpu: cpu核数
+        :type Cpu: int
+        :param Mem: 内存
+        :type Mem: int
+        :param UniqueVpcId: 私有网络ID，默认与集群私有网络ID保持一致
+        :type UniqueVpcId: str
+        :param UniqueSubnetId: 私有网络子网ID，默认与集群子网ID保持一致
+        :type UniqueSubnetId: str
+        :param ProxyCount: 数据库代理组节点个数
+        :type ProxyCount: int
+        :param ConnectionPoolType: 连接池类型：SessionConnectionPool(会话级别连接池 )
+        :type ConnectionPoolType: str
+        :param OpenConnectionPool: 是否开启连接池,yes-开启，no-不开启
+        :type OpenConnectionPool: str
+        :param ConnectionPoolTimeOut: 连接池阀值：单位（秒）
+        :type ConnectionPoolTimeOut: int
+        :param SecurityGroupIds: 安全组ID数组
+        :type SecurityGroupIds: list of str
+        :param Description: 描述说明
+        :type Description: str
+        :param ProxyZones: 数据库节点信息
+        :type ProxyZones: list of ProxyZone
+        """
+        self.ClusterId = None
+        self.Cpu = None
+        self.Mem = None
+        self.UniqueVpcId = None
+        self.UniqueSubnetId = None
+        self.ProxyCount = None
+        self.ConnectionPoolType = None
+        self.OpenConnectionPool = None
+        self.ConnectionPoolTimeOut = None
+        self.SecurityGroupIds = None
+        self.Description = None
+        self.ProxyZones = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.Cpu = params.get("Cpu")
+        self.Mem = params.get("Mem")
+        self.UniqueVpcId = params.get("UniqueVpcId")
+        self.UniqueSubnetId = params.get("UniqueSubnetId")
+        self.ProxyCount = params.get("ProxyCount")
+        self.ConnectionPoolType = params.get("ConnectionPoolType")
+        self.OpenConnectionPool = params.get("OpenConnectionPool")
+        self.ConnectionPoolTimeOut = params.get("ConnectionPoolTimeOut")
+        self.SecurityGroupIds = params.get("SecurityGroupIds")
+        self.Description = params.get("Description")
+        if params.get("ProxyZones") is not None:
+            self.ProxyZones = []
+            for item in params.get("ProxyZones"):
+                obj = ProxyZone()
+                obj._deserialize(item)
+                self.ProxyZones.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateProxyResponse(AbstractModel):
+    """CreateProxy返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateResourcePackageRequest(AbstractModel):
     """CreateResourcePackage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5631,14 +5912,187 @@
                 obj = SecurityGroup()
                 obj._deserialize(item)
                 self.Groups.append(obj)
         self.Total = params.get("Total")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeProxiesRequest(AbstractModel):
+    """DescribeProxies请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param Limit: 返回数量，默认为 20，最大值为 100
+        :type Limit: int
+        :param Offset: 记录偏移量，默认值为0
+        :type Offset: int
+        :param OrderBy: 排序字段，取值范围：
+<li> CREATETIME：创建时间</li>
+<li> PERIODENDTIME：过期时间</li>
+        :type OrderBy: str
+        :param OrderByType: 排序类型，取值范围：
+<li> ASC：升序排序 </li>
+<li> DESC：降序排序 </li>
+        :type OrderByType: str
+        :param Filters: 搜索条件，若存在多个Filter时，Filter间的关系为逻辑与（AND）关系。
+        :type Filters: list of QueryParamFilter
+        """
+        self.ClusterId = None
+        self.Limit = None
+        self.Offset = None
+        self.OrderBy = None
+        self.OrderByType = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.OrderBy = params.get("OrderBy")
+        self.OrderByType = params.get("OrderByType")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = QueryParamFilter()
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
+class DescribeProxiesResponse(AbstractModel):
+    """DescribeProxies返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 数据库代理组数
+        :type TotalCount: int
+        :param ProxyGroupInfos: 数据库代理组列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProxyGroupInfos: list of ProxyGroupInfo
+        :param ProxyNodeInfos: 数据库代理节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProxyNodeInfos: list of ProxyNodeInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.ProxyGroupInfos = None
+        self.ProxyNodeInfos = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("ProxyGroupInfos") is not None:
+            self.ProxyGroupInfos = []
+            for item in params.get("ProxyGroupInfos"):
+                obj = ProxyGroupInfo()
+                obj._deserialize(item)
+                self.ProxyGroupInfos.append(obj)
+        if params.get("ProxyNodeInfos") is not None:
+            self.ProxyNodeInfos = []
+            for item in params.get("ProxyNodeInfos"):
+                obj = ProxyNodeInfo()
+                obj._deserialize(item)
+                self.ProxyNodeInfos.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeProxyNodesRequest(AbstractModel):
+    """DescribeProxyNodes请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Limit: 返回数量，默认为 20，最大值为 100
+        :type Limit: int
+        :param Offset: 记录偏移量，默认值为0
+        :type Offset: int
+        :param OrderBy: 排序字段，取值范围：
+<li> CREATETIME：创建时间</li>
+<li> PERIODENDTIME：过期时间</li>
+        :type OrderBy: str
+        :param OrderByType: 排序类型，取值范围：
+<li> ASC：升序排序 </li>
+<li> DESC：降序排序 </li>
+        :type OrderByType: str
+        :param Filters: 搜索条件，若存在多个Filter时，Filter间的关系为逻辑与（AND）关系。
+        :type Filters: list of QueryFilter
+        """
+        self.Limit = None
+        self.Offset = None
+        self.OrderBy = None
+        self.OrderByType = None
+        self.Filters = None
+
+
+    def _deserialize(self, params):
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.OrderBy = params.get("OrderBy")
+        self.OrderByType = params.get("OrderByType")
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = QueryFilter()
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
+class DescribeProxyNodesResponse(AbstractModel):
+    """DescribeProxyNodes返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 数据库代理节点总数
+        :type TotalCount: int
+        :param ProxyNodeInfos: 数据库代理节点列表
+        :type ProxyNodeInfos: list of ProxyNodeInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.ProxyNodeInfos = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("ProxyNodeInfos") is not None:
+            self.ProxyNodeInfos = []
+            for item in params.get("ProxyNodeInfos"):
+                obj = ProxyNodeInfo()
+                obj._deserialize(item)
+                self.ProxyNodeInfos.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeResourcePackageDetailRequest(AbstractModel):
     """DescribeResourcePackageDetail请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8154,14 +8608,177 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyProxyDescRequest(AbstractModel):
+    """ModifyProxyDesc请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param Description: 数据库代理描述
+        :type Description: str
+        """
+        self.ClusterId = None
+        self.ProxyGroupId = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyProxyDescResponse(AbstractModel):
+    """ModifyProxyDesc返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyProxyRwSplitRequest(AbstractModel):
+    """ModifyProxyRwSplit请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param ConsistencyType: 一致性类型；“eventual"-最终一致性, "session"-会话一致性, "global"-全局一致性
+        :type ConsistencyType: str
+        :param ConsistencyTimeOut: 一致性超时时间
+        :type ConsistencyTimeOut: str
+        :param WeightMode: 读写权重分配模式；系统自动分配："system"， 自定义："custom"
+        :type WeightMode: str
+        :param InstanceWeights: 实例只读权重
+        :type InstanceWeights: list of ProxyInstanceWeight
+        :param FailOver: 是否开启故障转移，代理出现故障后，连接地址将路由到主实例，取值："yes" , "no"
+        :type FailOver: str
+        :param AutoAddRo: 是否自动添加只读实例，取值："yes" , "no"
+        :type AutoAddRo: str
+        :param OpenRw: 是否打开读写分离
+        :type OpenRw: str
+        :param RwType: 读写类型：
+READWRITE,READONLY
+        :type RwType: str
+        :param TransSplit: 事务拆分
+        :type TransSplit: bool
+        :param AccessMode: 连接模式：
+nearby,balance
+        :type AccessMode: str
+        :param OpenConnectionPool: 是否打开连接池：
+yes,no
+        :type OpenConnectionPool: str
+        :param ConnectionPoolType: 连接池类型：
+SessionConnectionPool
+        :type ConnectionPoolType: str
+        :param ConnectionPoolTimeOut: 连接池时间
+        :type ConnectionPoolTimeOut: int
+        """
+        self.ClusterId = None
+        self.ProxyGroupId = None
+        self.ConsistencyType = None
+        self.ConsistencyTimeOut = None
+        self.WeightMode = None
+        self.InstanceWeights = None
+        self.FailOver = None
+        self.AutoAddRo = None
+        self.OpenRw = None
+        self.RwType = None
+        self.TransSplit = None
+        self.AccessMode = None
+        self.OpenConnectionPool = None
+        self.ConnectionPoolType = None
+        self.ConnectionPoolTimeOut = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.ConsistencyType = params.get("ConsistencyType")
+        self.ConsistencyTimeOut = params.get("ConsistencyTimeOut")
+        self.WeightMode = params.get("WeightMode")
+        if params.get("InstanceWeights") is not None:
+            self.InstanceWeights = []
+            for item in params.get("InstanceWeights"):
+                obj = ProxyInstanceWeight()
+                obj._deserialize(item)
+                self.InstanceWeights.append(obj)
+        self.FailOver = params.get("FailOver")
+        self.AutoAddRo = params.get("AutoAddRo")
+        self.OpenRw = params.get("OpenRw")
+        self.RwType = params.get("RwType")
+        self.TransSplit = params.get("TransSplit")
+        self.AccessMode = params.get("AccessMode")
+        self.OpenConnectionPool = params.get("OpenConnectionPool")
+        self.ConnectionPoolType = params.get("ConnectionPoolType")
+        self.ConnectionPoolTimeOut = params.get("ConnectionPoolTimeOut")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyProxyRwSplitResponse(AbstractModel):
+    """ModifyProxyRwSplit返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步FlowId
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyResourcePackageClustersRequest(AbstractModel):
     """ModifyResourcePackageClusters请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9455,14 +10072,361 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ProxyConnectionPoolInfo(AbstractModel):
+    """数据库代理连接池信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ConnectionPoolTimeOut: 连接池保持阈值：单位（秒）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConnectionPoolTimeOut: int
+        :param OpenConnectionPool: 是否开启了连接池
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OpenConnectionPool: str
+        :param ConnectionPoolType: 连接池类型：SessionConnectionPool（会话级别连接池
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConnectionPoolType: str
+        """
+        self.ConnectionPoolTimeOut = None
+        self.OpenConnectionPool = None
+        self.ConnectionPoolType = None
+
+
+    def _deserialize(self, params):
+        self.ConnectionPoolTimeOut = params.get("ConnectionPoolTimeOut")
+        self.OpenConnectionPool = params.get("OpenConnectionPool")
+        self.ConnectionPoolType = params.get("ConnectionPoolType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyGroup(AbstractModel):
+    """proxy组
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param ProxyNodeCount: 数据库代理组节点个数
+        :type ProxyNodeCount: int
+        :param Status: 数据库代理组状态
+        :type Status: str
+        :param Region: 地域
+        :type Region: str
+        :param Zone: 可用区
+        :type Zone: str
+        :param CurrentProxyVersion: 当前代理版本
+        :type CurrentProxyVersion: str
+        :param ClusterId: 集群ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param AppId: 用户AppId
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param OpenRw: 读写节点开通数据库代理
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OpenRw: str
+        """
+        self.ProxyGroupId = None
+        self.ProxyNodeCount = None
+        self.Status = None
+        self.Region = None
+        self.Zone = None
+        self.CurrentProxyVersion = None
+        self.ClusterId = None
+        self.AppId = None
+        self.OpenRw = None
+
+
+    def _deserialize(self, params):
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.ProxyNodeCount = params.get("ProxyNodeCount")
+        self.Status = params.get("Status")
+        self.Region = params.get("Region")
+        self.Zone = params.get("Zone")
+        self.CurrentProxyVersion = params.get("CurrentProxyVersion")
+        self.ClusterId = params.get("ClusterId")
+        self.AppId = params.get("AppId")
+        self.OpenRw = params.get("OpenRw")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyGroupInfo(AbstractModel):
+    """数据库代理组详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProxyGroup: 数据库代理组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProxyGroup: :class:`tencentcloud.cynosdb.v20190107.models.ProxyGroup`
+        :param ProxyGroupRwInfo: 数据库代理组读写分离信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProxyGroupRwInfo: :class:`tencentcloud.cynosdb.v20190107.models.ProxyGroupRwInfo`
+        :param ProxyNodes: 数据库代理节点信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProxyNodes: list of ProxyNodeInfo
+        :param ConnectionPool: 数据库代理连接池信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConnectionPool: :class:`tencentcloud.cynosdb.v20190107.models.ProxyConnectionPoolInfo`
+        :param NetAddrInfos: 数据库代理网络信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NetAddrInfos: list of NetAddr
+        :param Tasks: 数据库代理任务集
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tasks: list of ObjectTask
+        """
+        self.ProxyGroup = None
+        self.ProxyGroupRwInfo = None
+        self.ProxyNodes = None
+        self.ConnectionPool = None
+        self.NetAddrInfos = None
+        self.Tasks = None
+
+
+    def _deserialize(self, params):
+        if params.get("ProxyGroup") is not None:
+            self.ProxyGroup = ProxyGroup()
+            self.ProxyGroup._deserialize(params.get("ProxyGroup"))
+        if params.get("ProxyGroupRwInfo") is not None:
+            self.ProxyGroupRwInfo = ProxyGroupRwInfo()
+            self.ProxyGroupRwInfo._deserialize(params.get("ProxyGroupRwInfo"))
+        if params.get("ProxyNodes") is not None:
+            self.ProxyNodes = []
+            for item in params.get("ProxyNodes"):
+                obj = ProxyNodeInfo()
+                obj._deserialize(item)
+                self.ProxyNodes.append(obj)
+        if params.get("ConnectionPool") is not None:
+            self.ConnectionPool = ProxyConnectionPoolInfo()
+            self.ConnectionPool._deserialize(params.get("ConnectionPool"))
+        if params.get("NetAddrInfos") is not None:
+            self.NetAddrInfos = []
+            for item in params.get("NetAddrInfos"):
+                obj = NetAddr()
+                obj._deserialize(item)
+                self.NetAddrInfos.append(obj)
+        if params.get("Tasks") is not None:
+            self.Tasks = []
+            for item in params.get("Tasks"):
+                obj = ObjectTask()
+                obj._deserialize(item)
+                self.Tasks.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyGroupRwInfo(AbstractModel):
+    """数据库代理组读写分离信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ConsistencyType: 一致性类型 eventual-最终一致性,global-全局一致性,session-会话一致性
+        :type ConsistencyType: str
+        :param ConsistencyTimeOut: 一致性超时时间
+        :type ConsistencyTimeOut: int
+        :param WeightMode: 权重模式 system-系统分配，custom-自定义
+        :type WeightMode: str
+        :param FailOver: 是否开启故障转移
+        :type FailOver: str
+        :param AutoAddRo: 是否自动添加只读实例，yes-是，no-不自动添加
+        :type AutoAddRo: str
+        :param InstanceWeights: 实例权重数组
+        :type InstanceWeights: list of ProxyInstanceWeight
+        :param OpenRw: 是否开通读写节点，yse-是，no-否
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OpenRw: str
+        :param RwType: 读写属性，可选值：READWRITE,READONLY
+        :type RwType: str
+        :param TransSplit: 事务拆分
+        :type TransSplit: bool
+        :param AccessMode: 连接模式，可选值：balance，nearby
+        :type AccessMode: str
+        """
+        self.ConsistencyType = None
+        self.ConsistencyTimeOut = None
+        self.WeightMode = None
+        self.FailOver = None
+        self.AutoAddRo = None
+        self.InstanceWeights = None
+        self.OpenRw = None
+        self.RwType = None
+        self.TransSplit = None
+        self.AccessMode = None
+
+
+    def _deserialize(self, params):
+        self.ConsistencyType = params.get("ConsistencyType")
+        self.ConsistencyTimeOut = params.get("ConsistencyTimeOut")
+        self.WeightMode = params.get("WeightMode")
+        self.FailOver = params.get("FailOver")
+        self.AutoAddRo = params.get("AutoAddRo")
+        if params.get("InstanceWeights") is not None:
+            self.InstanceWeights = []
+            for item in params.get("InstanceWeights"):
+                obj = ProxyInstanceWeight()
+                obj._deserialize(item)
+                self.InstanceWeights.append(obj)
+        self.OpenRw = params.get("OpenRw")
+        self.RwType = params.get("RwType")
+        self.TransSplit = params.get("TransSplit")
+        self.AccessMode = params.get("AccessMode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyInstanceWeight(AbstractModel):
+    """数据库代理，读写分离实例权重
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例Id
+        :type InstanceId: str
+        :param Weight: 实例权重
+        :type Weight: int
+        """
+        self.InstanceId = None
+        self.Weight = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Weight = params.get("Weight")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyNodeInfo(AbstractModel):
+    """数据库代理组节点
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProxyNodeId: 数据库代理节点ID
+        :type ProxyNodeId: str
+        :param ProxyNodeConnections: 节点当前连接数, DescribeProxyNodes接口此字段值不返回
+        :type ProxyNodeConnections: int
+        :param Cpu: 数据库代理节点cpu
+        :type Cpu: int
+        :param Mem: 数据库代理节点内存
+        :type Mem: int
+        :param Status: 数据库代理节点状态
+        :type Status: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AppId: 用户AppID
+        :type AppId: int
+        :param Region: 地域
+        :type Region: str
+        :param Zone: 可用区
+        :type Zone: str
+        """
+        self.ProxyNodeId = None
+        self.ProxyNodeConnections = None
+        self.Cpu = None
+        self.Mem = None
+        self.Status = None
+        self.ProxyGroupId = None
+        self.ClusterId = None
+        self.AppId = None
+        self.Region = None
+        self.Zone = None
+
+
+    def _deserialize(self, params):
+        self.ProxyNodeId = params.get("ProxyNodeId")
+        self.ProxyNodeConnections = params.get("ProxyNodeConnections")
+        self.Cpu = params.get("Cpu")
+        self.Mem = params.get("Mem")
+        self.Status = params.get("Status")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.ClusterId = params.get("ClusterId")
+        self.AppId = params.get("AppId")
+        self.Region = params.get("Region")
+        self.Zone = params.get("Zone")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ProxyZone(AbstractModel):
+    """proxy节点可用区内个数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProxyNodeZone: proxy节点可用区
+        :type ProxyNodeZone: str
+        :param ProxyNodeCount: proxy节点数量
+        :type ProxyNodeCount: int
+        """
+        self.ProxyNodeZone = None
+        self.ProxyNodeCount = None
+
+
+    def _deserialize(self, params):
+        self.ProxyNodeZone = params.get("ProxyNodeZone")
+        self.ProxyNodeCount = params.get("ProxyNodeCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class QueryFilter(AbstractModel):
     """查询过滤器
 
     """
 
     def __init__(self):
         r"""
@@ -9495,14 +10459,46 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class QueryParamFilter(AbstractModel):
+    """查询参数过滤器
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Names: 搜索字段，目前支持："InstanceId", "ProjectId", "InstanceName", "Vip"
+        :type Names: list of str
+        :param Values: 搜索字符串
+        :type Values: list of str
+        :param ExactMatch: 是否精确匹配
+        :type ExactMatch: bool
+        """
+        self.Names = None
+        self.Values = None
+        self.ExactMatch = None
+
+
+    def _deserialize(self, params):
+        self.Names = params.get("Names")
+        self.Values = params.get("Values")
+        self.ExactMatch = params.get("ExactMatch")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class RefundResourcePackageRequest(AbstractModel):
     """RefundResourcePackage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9540,14 +10536,67 @@
 
 
     def _deserialize(self, params):
         self.DealNames = params.get("DealNames")
         self.RequestId = params.get("RequestId")
 
 
+class ReloadBalanceProxyNodeRequest(AbstractModel):
+    """ReloadBalanceProxyNode请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        """
+        self.ClusterId = None
+        self.ProxyGroupId = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ReloadBalanceProxyNodeResponse(AbstractModel):
+    """ReloadBalanceProxyNode返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class RemoveClusterSlaveZoneRequest(AbstractModel):
     """RemoveClusterSlaveZone请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11039,14 +12088,161 @@
     def _deserialize(self, params):
         self.TranId = params.get("TranId")
         self.BigDealIds = params.get("BigDealIds")
         self.DealNames = params.get("DealNames")
         self.RequestId = params.get("RequestId")
 
 
+class UpgradeProxyRequest(AbstractModel):
+    """UpgradeProxy请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param Cpu: cpu核数
+        :type Cpu: int
+        :param Mem: 内存
+        :type Mem: int
+        :param ProxyCount: 数据库代理组节点个数
+        :type ProxyCount: int
+        :param ProxyGroupId: 数据库代理组ID（已废弃）
+        :type ProxyGroupId: str
+        :param ReloadBalance: 重新负载均衡：auto（自动），manual（手动）
+        :type ReloadBalance: str
+        :param IsInMaintainPeriod: 升级时间 ：no（升级完成时）yes（实例维护时间）
+        :type IsInMaintainPeriod: str
+        :param ProxyZones: 数据库代理节点信息
+        :type ProxyZones: list of ProxyZone
+        """
+        self.ClusterId = None
+        self.Cpu = None
+        self.Mem = None
+        self.ProxyCount = None
+        self.ProxyGroupId = None
+        self.ReloadBalance = None
+        self.IsInMaintainPeriod = None
+        self.ProxyZones = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.Cpu = params.get("Cpu")
+        self.Mem = params.get("Mem")
+        self.ProxyCount = params.get("ProxyCount")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.ReloadBalance = params.get("ReloadBalance")
+        self.IsInMaintainPeriod = params.get("IsInMaintainPeriod")
+        if params.get("ProxyZones") is not None:
+            self.ProxyZones = []
+            for item in params.get("ProxyZones"):
+                obj = ProxyZone()
+                obj._deserialize(item)
+                self.ProxyZones.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpgradeProxyResponse(AbstractModel):
+    """UpgradeProxy返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务ID
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
+class UpgradeProxyVersionRequest(AbstractModel):
+    """UpgradeProxyVersion请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param SrcProxyVersion: 数据库代理当前版本
+        :type SrcProxyVersion: str
+        :param DstProxyVersion: 数据库代理升级版本
+        :type DstProxyVersion: str
+        :param ProxyGroupId: 数据库代理组ID
+        :type ProxyGroupId: str
+        :param IsInMaintainPeriod: 升级时间 ：no（升级完成时）yes（实例维护时间）
+        :type IsInMaintainPeriod: str
+        """
+        self.ClusterId = None
+        self.SrcProxyVersion = None
+        self.DstProxyVersion = None
+        self.ProxyGroupId = None
+        self.IsInMaintainPeriod = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.SrcProxyVersion = params.get("SrcProxyVersion")
+        self.DstProxyVersion = params.get("DstProxyVersion")
+        self.ProxyGroupId = params.get("ProxyGroupId")
+        self.IsInMaintainPeriod = params.get("IsInMaintainPeriod")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpgradeProxyVersionResponse(AbstractModel):
+    """UpgradeProxyVersion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步流程ID
+        :type FlowId: int
+        :param TaskId: 异步任务id
+        :type TaskId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class UserHostPrivilege(AbstractModel):
     """用户主机权限
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CloseProxy(self, request):
+        """关闭数据库代理
+
+        :param request: Request instance for CloseProxy.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseProxyRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CloseProxyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CloseProxy", params, headers=headers)
+            response = json.loads(body)
+            model = models.CloseProxyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CloseWan(self, request):
         """本接口（CloseWan）用于关闭外网
 
         :param request: Request instance for CloseWan.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CloseWanRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CloseWanResponse`
 
@@ -390,14 +413,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateProxy(self, request):
+        """创建数据库代理
+
+        :param request: Request instance for CreateProxy.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateProxy", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateProxyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateProxyEndPoint(self, request):
+        """创建数据库代理连接点
+
+        :param request: Request instance for CreateProxyEndPoint.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyEndPointRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CreateProxyEndPointResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateProxyEndPoint", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateProxyEndPointResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateResourcePackage(self, request):
         """新购资源包
 
         :param request: Request instance for CreateResourcePackage.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateResourcePackageRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CreateResourcePackageResponse`
 
@@ -1287,14 +1356,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeProxies(self, request):
+        """查询数据库代理列表
+
+        :param request: Request instance for DescribeProxies.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxiesRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxiesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeProxies", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeProxiesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeProxyNodes(self, request):
+        """本接口（DescribeProxyNodes）用于查询代理接口列表。
+
+        :param request: Request instance for DescribeProxyNodes.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxyNodesRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeProxyNodesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeProxyNodes", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeProxyNodesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeResourcePackageDetail(self, request):
         """查询资源包使用详情
 
         :param request: Request instance for DescribeResourcePackageDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageDetailRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeResourcePackageDetailResponse`
 
@@ -2092,14 +2207,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyProxyDesc(self, request):
+        """修改数据库代理描述
+
+        :param request: Request instance for ModifyProxyDesc.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyDescRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyDescResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyProxyDesc", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyProxyDescResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyProxyRwSplit(self, request):
+        """配置数据库代理读写分离
+
+        :param request: Request instance for ModifyProxyRwSplit.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyRwSplitRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyProxyRwSplitResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyProxyRwSplit", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyProxyRwSplitResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyResourcePackageClusters(self, request):
         """给资源包绑定集群
 
         :param request: Request instance for ModifyResourcePackageClusters.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageClustersRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyResourcePackageClustersResponse`
 
@@ -2345,14 +2506,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ReloadBalanceProxyNode(self, request):
+        """负载均衡数据库代理
+
+        :param request: Request instance for ReloadBalanceProxyNode.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.ReloadBalanceProxyNodeRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ReloadBalanceProxyNodeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ReloadBalanceProxyNode", params, headers=headers)
+            response = json.loads(body)
+            model = models.ReloadBalanceProxyNodeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RemoveClusterSlaveZone(self, request):
         """删除从可用区
 
         :param request: Request instance for RemoveClusterSlaveZone.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.RemoveClusterSlaveZoneRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.RemoveClusterSlaveZoneResponse`
 
@@ -2687,8 +2871,54 @@
             model = models.UpgradeInstanceResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpgradeProxy(self, request):
+        """升级数据库代理配置
+
+        :param request: Request instance for UpgradeProxy.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpgradeProxy", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpgradeProxyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpgradeProxyVersion(self, request):
+        """升级数据库代理版本
+
+        :param request: Request instance for UpgradeProxyVersion.
+        :type request: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyVersionRequest`
+        :rtype: :class:`tencentcloud.cynosdb.v20190107.models.UpgradeProxyVersionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpgradeProxyVersion", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpgradeProxyVersionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
+# 操作失败。
+FAILEDOPERATION = 'FailedOperation'
+
 # 批量查询失败。
 FAILEDOPERATION_BATCHGETINSTANCEERROR = 'FailedOperation.BatchGetInstanceError'
 
 # 绑定资源包失败
 FAILEDOPERATION_BINDSOURCEPACKAGEERROR = 'FailedOperation.BindSourcePackageError'
 
 # 获取权限失败，请稍后重试。如果持续不成功，请联系客服进行处理。
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.917/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.917/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.916/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.917/setup.py`

 * *Files identical despite different names*

