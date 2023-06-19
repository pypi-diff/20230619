# Comparing `tmp/acore_server_config-0.2.3.tar.gz` & `tmp/acore_server_config-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.2.3.tar", last modified: Sun Jun 18 04:28:42 2023, max compression
+gzip compressed data, was "acore_server_config-0.3.1.tar", last modified: Mon Jun 19 17:20:24 2023, max compression
```

## Comparing `acore_server_config-0.2.3.tar` & `acore_server_config-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099775 acore_server_config-0.2.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:28:42.099644 acore_server_config-0.2.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.2.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.096229 acore_server_config-0.2.3/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.2.3/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 04:27:52.000000 acore_server_config-0.2.3/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.2.3/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.2.3/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.2.3/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.097494 acore_server_config-0.2.3/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.2.3/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098253 acore_server_config-0.2.3/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.2.3/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.2.3/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1344 2023-06-18 03:28:21.000000 acore_server_config-0.2.3/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.2.3/acore_server_config/config/init.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098456 acore_server_config-0.2.3/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3779 2023-06-18 04:27:33.000000 acore_server_config-0.2.3/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.2.3/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.2.3/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098892 acore_server_config-0.2.3/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099232 acore_server_config-0.2.3/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.097043 acore_server_config-0.2.3/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2265 2023-06-18 04:28:15.000000 acore_server_config-0.2.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.2.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.2.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 04:28:42.099820 acore_server_config-0.2.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099378 acore_server_config-0.2.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.2.3/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.499216 acore_server_config-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-19 17:20:24.499072 acore_server_config-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.495279 acore_server_config-0.3.1/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.1/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 16:53:00.000000 acore_server_config-0.3.1/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.1/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.3.1/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.1/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.496443 acore_server_config-0.3.1/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.1/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.496939 acore_server_config-0.3.1/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.1/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.1/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1370 2023-06-19 17:13:51.000000 acore_server_config-0.3.1/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.1/acore_server_config/config/init.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8011 2023-06-19 17:03:54.000000 acore_server_config-0.3.1/acore_server_config/config/loader.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.497105 acore_server_config-0.3.1/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3938 2023-06-19 16:51:35.000000 acore_server_config-0.3.1/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.1/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.3.1/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498099 acore_server_config-0.3.1/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.1/acore_server_config/tests/dummy_config.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.1/acore_server_config/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498617 acore_server_config-0.3.1/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.495984 acore_server_config-0.3.1/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      285 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2631 2023-06-19 16:57:27.000000 acore_server_config-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 17:20:24.499273 acore_server_config-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498777 acore_server_config-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.1/tests/test_api.py
```

### Comparing `acore_server_config-0.2.3/AUTHORS.rst` & `acore_server_config-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/LICENSE.txt` & `acore_server_config-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/PKG-INFO` & `acore_server_config-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.2.3
+Version: 0.3.1
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.2.3/README.rst` & `acore_server_config-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/boto_ses.py` & `acore_server_config-0.3.1/acore_server_config/boto_ses.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/config/define/main.py` & `acore_server_config-0.3.1/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/config/define/server.py` & `acore_server_config-0.3.1/acore_server_config/config/define/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # -*- coding: utf-8 -*-
 
+"""
+todo: doc string
+"""
+
 import typing as T
 import dataclasses
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .main import Env
```

### Comparing `acore_server_config-0.2.3/acore_server_config/config/init.py` & `acore_server_config-0.3.1/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/in_ec2.py` & `acore_server_config-0.3.1/acore_server_config/in_ec2.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     >>> server = get_server()
     >>> server
     Server(id='sbx-blue', db_admin_password='sbx*dummy4test', db_username='myuser', db_password='sbx*dummy4test')
 """
 
 
 import typing as T
+import warnings
 
 from s3pathlib import S3Path
 from simple_aws_ec2.api import Ec2Instance
 from acore_server_metadata.api import settings
 
 from .boto_ses import bsm as default_bsm
 from .config.define import EnvEnum, Env, Config, Server
@@ -66,14 +67,18 @@
     :param use_s3: 是否从 S3 读取配置数据, 默认使用 S3, 因为配置数据可能会很大.
     :param use_parameter_store: 是否从 AWS Parameter Store 读取配置数据
     :param s3folder_config: S3 配置数据的根目录, 默认为
         s3://aws_account_id}-{aws_region}-artifacts/projects/acore_server_config/config/
     :param server_id: 强制指定 server_id, 跳过 "自省" 阶段. 常用于测试. 这个 server_id
         的格式为: ${env_name}-${server_name}, 例如: sbx-blue
     """
+    warnings.warn(
+        "you should not use this function anymore, use "
+        "'acore_server_config.api.Ec2ConfigLoader' instead."
+    )
     if sum([use_s3, use_parameter_store]) != 1:
         raise ValueError(
             "Only one of use_s3 and use_parameter_store can be True at the same time."
         )
 
     if server_id is None:
         ec2_inst = Ec2Instance.from_ec2_inside(bsm.ec2_client)
```

### Comparing `acore_server_config-0.2.3/acore_server_config/paths.py` & `acore_server_config-0.3.1/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/runtime.py` & `acore_server_config-0.3.1/acore_server_config/runtime.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.3.1/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.3.1/acore_server_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.2.3
+Version: 0.3.1
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.2.3/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.3.1/acore_server_config.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 acore_server_config.egg-info/PKG-INFO
 acore_server_config.egg-info/SOURCES.txt
 acore_server_config.egg-info/dependency_links.txt
 acore_server_config.egg-info/requires.txt
 acore_server_config.egg-info/top_level.txt
 acore_server_config/config/__init__.py
 acore_server_config/config/init.py
+acore_server_config/config/loader.py
 acore_server_config/config/define/__init__.py
 acore_server_config/config/define/main.py
 acore_server_config/config/define/server.py
 acore_server_config/docs/__init__.py
 acore_server_config/tests/__init__.py
+acore_server_config/tests/dummy_config.py
 acore_server_config/tests/helper.py
+acore_server_config/tests/mock_aws.py
 acore_server_config/vendor/__init__.py
 acore_server_config/vendor/pytest_cov_helper.py
 tests/test_api.py
```

### Comparing `acore_server_config-0.2.3/release-history.rst` & `acore_server_config-0.3.1/release-history.rst`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Create two new API ``acore_server_config.api.Ec2ConfigLoader``, ``acore_server_config.api.ConfigLoader`` to replace ``acore_server_config.api.get_server``. The old api remains for backward compatibility until the next major release.
+
+
 0.2.3 (2023-06-18)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a parameter default value typo in ``acore_server_config.api.get_server`` API.
```

### Comparing `acore_server_config-0.2.3/requirements-doc.txt` & `acore_server_config-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.3/setup.py` & `acore_server_config-0.3.1/setup.py`

 * *Files identical despite different names*

