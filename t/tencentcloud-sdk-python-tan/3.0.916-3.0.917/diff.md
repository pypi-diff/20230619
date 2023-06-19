# Comparing `tmp/tencentcloud-sdk-python-tan-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-tan-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.916.tar", last modified: Fri Jun 16 00:41:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tan-3.0.917.tar", last modified: Mon Jun 19 00:32:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tan-3.0.916.tar` & `tencentcloud-sdk-python-tan-3.0.917.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2285 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/models.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/tan_client.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-16 00:41:11.000000 tencentcloud-sdk-python-tan-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/models.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/tan_client.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:32:58.000000 tencentcloud-sdk-python-tan-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-tan-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tan-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/models.py` & `tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/tan_client.py` & `tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/tan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.916/tencentcloud/tan/v20220420/errorcodes.py` & `tencentcloud-sdk-python-tan-3.0.917/tencentcloud/tan/v20220420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.916/README.rst` & `tencentcloud-sdk-python-tan-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tan-3.0.916/tencentcloud_sdk_python_tan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.917/tencentcloud_sdk_python_tan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tan-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-tan-3.0.917/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tan
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Tan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tan-3.0.916/setup.py` & `tencentcloud-sdk-python-tan-3.0.917/setup.py`

 * *Files identical despite different names*

