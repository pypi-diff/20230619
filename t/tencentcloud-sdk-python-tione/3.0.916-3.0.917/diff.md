# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.916.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.916.tar", last modified: Fri Jun 16 00:43:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.917.tar", last modified: Mon Jun 19 00:35:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.916.tar` & `tencentcloud-sdk-python-tione-3.0.917.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)    22010 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   336462 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)    51024 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    12587 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-16 00:43:37.000000 tencentcloud-sdk-python-tione-3.0.916/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   336462 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    12587 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-19 00:35:33.000000 tencentcloud-sdk-python-tione-3.0.917/setup.py
```

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.917/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/README.rst` & `tencentcloud-sdk-python-tione-3.0.917/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.916/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.917/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.916
+Version: 3.0.917
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.916/setup.py` & `tencentcloud-sdk-python-tione-3.0.917/setup.py`

 * *Files identical despite different names*

