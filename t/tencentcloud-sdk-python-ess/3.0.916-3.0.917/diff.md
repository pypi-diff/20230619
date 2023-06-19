# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.916.tar", last modified: Fri Jun 16 00:33:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.917.tar", last modified: Mon Jun 19 00:25:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.916.tar` & `tencentcloud-sdk-python-ess-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248189 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    57653 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:33:48.000000 tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:33:47.000000 tencentcloud-sdk-python-ess-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252397 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    58476 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:25:18.000000 tencentcloud-sdk-python-ess-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,15 +664,15 @@
         r"""
         :param ComponentType: 如果是Component填写控件类型，则可选的字段为：
 TEXT - 普通文本控件，输入文本字符串；
 MULTI_LINE_TEXT - 多行文本控件，输入文本字符串；
 CHECK_BOX - 勾选框控件，若选中填写ComponentValue 填写 true或者 false 字符串；
 FILL_IMAGE - 图片控件，ComponentValue 填写图片的资源 ID；
 DYNAMIC_TABLE - 动态表格控件；
-ATTACHMENT - 附件控件,ComponentValue 填写附件图片的资源 ID列表，以逗号分割；
+ATTACHMENT - 附件控件,ComponentValue 填写附件图片的资源 ID列表，以逗号分隔；
 SELECTOR - 选择器控件，ComponentValue填写选择的字符串内容；
 DATE - 日期控件；默认是格式化为xxxx年xx月xx日字符串；
 DISTRICT - 省市区行政区控件，ComponentValue填写省市区行政区字符串内容；
 
 如果是SignComponent签署控件类型，则可选的字段为
 SIGN_SEAL - 签署印章控件；
 SIGN_DATE - 签署日期控件；
@@ -721,15 +721,15 @@
 如：{“ComponentTypeLimit”: [“SYSTEM_ESIGN”]}
 
 ComponentType为SIGN_DATE时，支持以下参数：
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
-5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
+5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
 参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
         :type ComponentExtra: str
         :param IsFormType: 是否是表单域类型，默认不false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
@@ -2512,14 +2512,124 @@
 
 
     def _deserialize(self, params):
         self.UserIds = params.get("UserIds")
         self.RequestId = params.get("RequestId")
 
 
+class CreateSealRequest(AbstractModel):
+    """CreateSeal请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param SealName: 电子印章名字
+        :type SealName: str
+        :param Agent: 应用相关信息
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param SealType: 电子印章类型，PERSONAL-个人私章,OFFICIAL-公章,SPECIAL_FINANCIAL-财务专用章,CONTRACT-合同专用章,LEGAL_REPRESENTATIVE-法定代表人章,SPECIAL_NATIONWIDE_INVOICE-发票专用章
+        :type SealType: str
+        :param FileName: 电子印章图片文件名称
+        :type FileName: str
+        :param Image: 电子印章图片base64编码
+参数Image,FileToken或GenerateSource=SealGenerateSourceSystem三选一。
+        :type Image: str
+        :param Width: 电子印章宽度,单位px
+参数不再启用，系统会设置印章大小为标准尺寸。
+        :type Width: int
+        :param Height: 电子印章高度,单位px
+参数不再启用，系统会设置印章大小为标准尺寸。
+        :type Height: int
+        :param Color: 电子印章印章颜色(默认红色RED),RED-红色
+
+系统目前只支持红色印章创建。
+        :type Color: str
+        :param SealHorizontalText: 电子印章生成时的横向文字。
+        :type SealHorizontalText: str
+        :param SealChordText: 电子印章下弦文字
+        :type SealChordText: str
+        :param SealCentralType: 电子印章中心图案类型,STAR-圆形有五角星,NONE-圆形无五角星
+系统生成的印章只支持STAR
+        :type SealCentralType: str
+        :param FileToken: 通过文件上传时，服务端生成的电子印章上传图片的token
+
+        :type FileToken: str
+        :param GenerateSource: 印章生成来源方式
+取值：
+SealGenerateSourceSystem 表示系统生成企业印章
+        :type GenerateSource: str
+        """
+        self.Operator = None
+        self.SealName = None
+        self.Agent = None
+        self.SealType = None
+        self.FileName = None
+        self.Image = None
+        self.Width = None
+        self.Height = None
+        self.Color = None
+        self.SealHorizontalText = None
+        self.SealChordText = None
+        self.SealCentralType = None
+        self.FileToken = None
+        self.GenerateSource = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.SealName = params.get("SealName")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
+        self.SealType = params.get("SealType")
+        self.FileName = params.get("FileName")
+        self.Image = params.get("Image")
+        self.Width = params.get("Width")
+        self.Height = params.get("Height")
+        self.Color = params.get("Color")
+        self.SealHorizontalText = params.get("SealHorizontalText")
+        self.SealChordText = params.get("SealChordText")
+        self.SealCentralType = params.get("SealCentralType")
+        self.FileToken = params.get("FileToken")
+        self.GenerateSource = params.get("GenerateSource")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateSealResponse(AbstractModel):
+    """CreateSeal返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SealId: 电子印章编号
+        :type SealId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SealId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.SealId = params.get("SealId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateStaffResult(AbstractModel):
     """创建员工的结果
 
     """
 
     def __init__(self):
         r"""
@@ -2657,15 +2767,15 @@
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param DeptId: 电子签中的部门id
         :type DeptId: str
-        :param ReceiveDeptId: 交接部门ID。待删除部门中的合同、印章和模版数据，交接至该部门ID下，未填写交接至公司根部门。
+        :param ReceiveDeptId: 交接部门ID。待删除部门中的合同、印章和模板数据，交接至该部门ID下，未填写交接至公司根部门。
         :type ReceiveDeptId: str
         """
         self.Operator = None
         self.DeptId = None
         self.ReceiveDeptId = None
 
 
@@ -6034,15 +6144,15 @@
         r"""
         :param DisplayName: 员工名
         :type DisplayName: str
         :param Mobile: 员工手机号
         :type Mobile: str
         :param UserId: 员工在电子签平台的id
         :type UserId: str
-        :param Note: 提示，当创建已存在未实名用户时，改字段有值
+        :param Note: 提示，当创建已存在未实名用户时，该字段有值
 注意：此字段可能返回 null，表示取不到有效值。
         :type Note: str
         """
         self.DisplayName = None
         self.Mobile = None
         self.UserId = None
         self.Note = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,14 +599,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateSeal(self, request):
+        """创建电子印章
+
+        :param request: Request instance for CreateSeal.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateSealRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateSealResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateSeal", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateSealResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateSealPolicy(self, request):
         """对企业员工进行印章授权
 
         :param request: Request instance for CreateSealPolicy.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateSealPolicyRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateSealPolicyResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.916/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.917/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.916/README.rst` & `tencentcloud-sdk-python-ess-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.917/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.916/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.917/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.916/setup.py` & `tencentcloud-sdk-python-ess-3.0.917/setup.py`

 * *Files identical despite different names*

