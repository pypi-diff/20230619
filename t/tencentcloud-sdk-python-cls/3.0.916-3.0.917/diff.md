# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.916.tar", last modified: Fri Jun 16 00:30:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.917.tar", last modified: Mon Jun 19 00:21:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.916.tar` & `tencentcloud-sdk-python-cls-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254810 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)     8715 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    67913 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:30:37.000000 tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   256323 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)     8715 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67913 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:21:48.000000 tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cls-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6270,14 +6270,42 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class MultiTopicSearchInformation(AbstractModel):
+    """多日志主题检索相关信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TopicId: 要检索分析的日志主题ID
+        :type TopicId: str
+        :param Context: 透传上次接口返回的Context值，可获取后续更多日志，总计最多可获取1万条原始日志，过期时间1小时
+        :type Context: str
+        """
+        self.TopicId = None
+        self.Context = None
+
+
+    def _deserialize(self, params):
+        self.TopicId = params.get("TopicId")
+        self.Context = params.get("Context")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class NoticeReceiver(AbstractModel):
     """告警通知接收者信息
 
     """
 
     def __init__(self):
         r"""
@@ -6651,15 +6679,16 @@
         :type From: int
         :param To: 要检索分析的日志的结束时间，Unix时间戳（毫秒）
         :type To: int
         :param Query: 检索分析语句，最大长度为12KB
 语句由 <a href="https://cloud.tencent.com/document/product/614/47044" target="_blank">[检索条件]</a> | <a href="https://cloud.tencent.com/document/product/614/44061" target="_blank">[SQL语句]</a>构成，无需对日志进行统计分析时，可省略其中的管道符<code> | </code>及SQL语句
 使用*或空字符串可查询所有日志
         :type Query: str
-        :param TopicId: 要检索分析的日志主题ID
+        :param TopicId: - 要检索分析的日志主题ID，仅能指定一个日志主题。
+- 如需同时检索多个日志主题，请使用Topics参数。
         :type TopicId: str
         :param Limit: 表示单次查询返回的原始日志条数，最大值为1000，获取后续日志需使用Context参数
 注意：
 * 仅当检索分析语句(Query)不包含SQL时有效
 * SQL结果条数指定方式参考<a href="https://cloud.tencent.com/document/product/614/58977" target="_blank">SQL LIMIT语法</a>
         :type Limit: int
         :param Context: 透传上次接口返回的Context值，可获取后续更多日志，总计最多可获取1万条原始日志，过期时间1小时
@@ -6683,38 +6712,49 @@
 1：不采样，即精确分析
 默认值为1
         :type SamplingRate: float
         :param SyntaxRule: 检索语法规则，默认值为0。
 0：Lucene语法，1：CQL语法。
 详细说明参见<a href="https://cloud.tencent.com/document/product/614/47044#RetrievesConditionalRules" target="_blank">检索条件语法规则</a>
         :type SyntaxRule: int
+        :param Topics: - 要检索分析的日志主题列表，最大支持20个日志主题。
+- 检索单个日志主题时请使用TopicId。
+- 不能同时使用TopicId和Topics。
+        :type Topics: list of MultiTopicSearchInformation
         """
         self.From = None
         self.To = None
         self.Query = None
         self.TopicId = None
         self.Limit = None
         self.Context = None
         self.Sort = None
         self.UseNewAnalysis = None
         self.SamplingRate = None
         self.SyntaxRule = None
+        self.Topics = None
 
 
     def _deserialize(self, params):
         self.From = params.get("From")
         self.To = params.get("To")
         self.Query = params.get("Query")
         self.TopicId = params.get("TopicId")
         self.Limit = params.get("Limit")
         self.Context = params.get("Context")
         self.Sort = params.get("Sort")
         self.UseNewAnalysis = params.get("UseNewAnalysis")
         self.SamplingRate = params.get("SamplingRate")
         self.SyntaxRule = params.get("SyntaxRule")
+        if params.get("Topics") is not None:
+            self.Topics = []
+            for item in params.get("Topics"):
+                obj = MultiTopicSearchInformation()
+                obj._deserialize(item)
+                self.Topics.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.916/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.917/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.916/README.rst` & `tencentcloud-sdk-python-cls-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.917/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.916/setup.py` & `tencentcloud-sdk-python-cls-3.0.917/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.916/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.917/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

