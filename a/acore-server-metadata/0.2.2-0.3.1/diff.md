# Comparing `tmp/acore_server_metadata-0.2.2.tar.gz` & `tmp/acore_server_metadata-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.2.2.tar", last modified: Sat Jun 17 18:03:11 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.3.1.tar", last modified: Mon Jun 19 14:32:27 2023, max compression
```

## Comparing `acore_server_metadata-0.2.2.tar` & `acore_server_metadata-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.713547 acore_server_metadata-0.2.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6597 2023-06-17 18:03:11.713402 acore_server_metadata-0.2.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5448 2023-06-17 17:14:49.000000 acore_server_metadata-0.2.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.711699 acore_server_metadata-0.2.2/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.2.2/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-17 18:02:47.000000 acore_server_metadata-0.2.2/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.2.2/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712395 acore_server_metadata-0.2.2/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.2.2/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    21479 2023-06-17 17:52:30.000000 acore_server_metadata-0.2.2/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.2.2/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712752 acore_server_metadata-0.2.2/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.2.2/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712983 acore_server_metadata-0.2.2/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712274 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6597 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      949 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1514 2023-06-17 17:06:47.000000 acore_server_metadata-0.2.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.2.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.2.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-17 18:03:11.713588 acore_server_metadata-0.2.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.713217 acore_server_metadata-0.2.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      938 2023-06-17 03:01:13.000000 acore_server_metadata-0.2.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.2.2/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.614038 acore_server_metadata-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6703 2023-06-19 14:32:27.613880 acore_server_metadata-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5554 2023-06-19 14:31:51.000000 acore_server_metadata-0.3.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.610559 acore_server_metadata-0.3.1/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.3.1/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 02:15:38.000000 acore_server_metadata-0.3.1/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.3.1/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.611575 acore_server_metadata-0.3.1/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.3.1/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    23405 2023-06-19 14:29:29.000000 acore_server_metadata-0.3.1/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.3.1/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.612232 acore_server_metadata-0.3.1/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.3.1/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.612915 acore_server_metadata-0.3.1/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.611426 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6703 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1764 2023-06-19 14:30:41.000000 acore_server_metadata-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 14:32:27.614091 acore_server_metadata-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.613454 acore_server_metadata-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      983 2023-06-18 02:15:54.000000 acore_server_metadata-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.3.1/tests/test_server.py
```

### Comparing `acore_server_metadata-0.2.2/AUTHORS.rst` & `acore_server_metadata-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/LICENSE.txt` & `acore_server_metadata-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/PKG-INFO` & `acore_server_metadata-0.3.1/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore_server_metadata
-Version: 0.2.2
+Name: acore-server-metadata
+Version: 0.3.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -148,14 +148,16 @@
 
 .. code-block:: python
 
     # 启动新的 EC2
     >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 更新 DB 的 master password
+    >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.2/README.rst` & `acore_server_metadata-0.3.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -116,14 +116,16 @@
 
 .. code-block:: python
 
     # 启动新的 EC2
     >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 更新 DB 的 master password
+    >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata/paths.py` & `acore_server_metadata-0.3.1/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata/server.py` & `acore_server_metadata-0.3.1/acore_server_metadata/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing as T
 import dataclasses
 from datetime import timezone
 
 from simple_aws_ec2.api import Ec2Instance, EC2InstanceStatusEnum
 from simple_aws_rds.api import RDSDBInstance, RDSDBInstanceStatusEnum
 
+from .vendor.hashes import hashes
 from .exc import (
     ServerNotFoundError,
     ServerNotUniqueError,
     ServerAlreadyExistsError,
 )
 from .settings import settings
 from .utils import get_utc_now
@@ -483,14 +484,60 @@
 
         # associate eip address
         ec2_client.associate_address(
             AllocationId=allocation_id,
             InstanceId=self.ec2_inst.id,
         )
 
+    def update_db_master_password(
+        self,
+        rds_client,
+        master_password: str,
+        check_exists: bool = True,
+    ):
+        """
+        Update the DB instance master password. When you recover the DB instance
+        from a snapshot, the master password is the same as the password when you
+        create the snapshot. This method can be used to update the master password.
+
+        在数据库运维过程中, 我们都是从自己备份的 Snapshot 启动 DB 实例. 它的管理员密码会继承
+        备份 Snapshot 的时候的密码. 比如我们希望用开发环境的 snapshot 创建生产环境的数据库,
+        这时候再继续用开发环境的密码肯定不妥, 所以需要更新密码. 该方法可以做到这一点.
+        并且这个方法是幂等的, 如果密码已经设置好了, 则什么也不会做. 如果密码没有被设置过, 则
+        会设置密码.
+        """
+        if check_exists:
+            rds_inst = self.get_rds(rds_client, id=self.id)
+            if rds_inst is None:
+                raise ServerNotFoundError(f"RDS DB instance {self.id!r} does not exist")
+        else:
+            rds_inst = self.rds_inst
+
+        hashes.use_sha256()
+        master_password_digest = hashes.of_str(master_password, hexdigest=True)
+        if (
+            rds_inst.tags.get("tech:master_password_digest", "invalid")
+            == master_password_digest
+        ):
+            # do nothing
+            return
+
+        rds_client.modify_db_instance(
+            DBInstanceIdentifier=self.rds_inst.id,
+            MasterUserPassword=master_password,
+            ApplyImmediately=True,
+        )
+
+        rds_client.add_tags_to_resource(
+            ResourceName=rds_inst.db_instance_arn,
+            Tags=[
+                dict(Key="tech:master_password_digest", Value=master_password_digest)
+            ],
+        )
+
     def create_db_snapshot(
         self,
         rds_client,
         check_exists: bool = True,
     ):
         """
         Create a 'manual' DB snapshot for the RDS DB instance.
```

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.3.1/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.3.1/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore-server-metadata
-Version: 0.2.2
+Name: acore_server_metadata
+Version: 0.3.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -148,14 +148,16 @@
 
 .. code-block:: python
 
     # 启动新的 EC2
     >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 更新 DB 的 master password
+    >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.2/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.3.1/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 acore_server_metadata.egg-info/requires.txt
 acore_server_metadata.egg-info/top_level.txt
 acore_server_metadata/docs/__init__.py
 acore_server_metadata/tests/__init__.py
 acore_server_metadata/tests/helper.py
 acore_server_metadata/tests/mock_aws.py
 acore_server_metadata/vendor/__init__.py
+acore_server_metadata/vendor/hashes.py
 acore_server_metadata/vendor/pytest_cov_helper.py
 tests/test_api.py
 tests/test_server.py
```

### Comparing `acore_server_metadata-0.2.2/release-history.rst` & `acore_server_metadata-0.3.1/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``acore_server_metadata.api.Server.update_db_master_password`` to update the master password of RDS DB instance.
+
+
 0.2.2 (2023-06-17)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - Fix a bug that ``Server.get_ec2`` and ``Server.get_rds`` methods returns terminated ec2 and deleted rds instances. They should be considered as "not exists"
```

### Comparing `acore_server_metadata-0.2.2/requirements-doc.txt` & `acore_server_metadata-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/setup.py` & `acore_server_metadata-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.2/tests/test_api.py` & `acore_server_metadata-0.3.1/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     _ = api.Server.is_ec2_exists
     _ = api.Server.is_ec2_running
     _ = api.Server.is_rds_exists
     _ = api.Server.is_rds_running
     _ = api.Server.refresh
     _ = api.Server.run_ec2
     _ = api.Server.run_rds
+    _ = api.Server.update_db_master_password
     _ = api.Server.associate_eip_address
     _ = api.Server.create_db_snapshot
     _ = api.Server.cleanup_db_snapshot
 
 
 if __name__ == "__main__":
     from acore_server_metadata.tests import run_cov_test
```

### Comparing `acore_server_metadata-0.2.2/tests/test_server.py` & `acore_server_metadata-0.3.1/tests/test_server.py`

 * *Files identical despite different names*

