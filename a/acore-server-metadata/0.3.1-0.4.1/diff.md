# Comparing `tmp/acore_server_metadata-0.3.1.tar.gz` & `tmp/acore_server_metadata-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.3.1.tar", last modified: Mon Jun 19 14:32:27 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.4.1.tar", last modified: Mon Jun 19 18:58:17 2023, max compression
```

## Comparing `acore_server_metadata-0.3.1.tar` & `acore_server_metadata-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.614038 acore_server_metadata-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6703 2023-06-19 14:32:27.613880 acore_server_metadata-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5554 2023-06-19 14:31:51.000000 acore_server_metadata-0.3.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.610559 acore_server_metadata-0.3.1/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.3.1/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 02:15:38.000000 acore_server_metadata-0.3.1/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.3.1/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.611575 acore_server_metadata-0.3.1/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.3.1/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    23405 2023-06-19 14:29:29.000000 acore_server_metadata-0.3.1/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.3.1/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.612232 acore_server_metadata-0.3.1/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.3.1/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.3.1/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.612915 acore_server_metadata-0.3.1/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.611426 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6703 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 14:32:27.000000 acore_server_metadata-0.3.1/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1764 2023-06-19 14:30:41.000000 acore_server_metadata-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 14:32:27.614091 acore_server_metadata-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 14:32:27.613454 acore_server_metadata-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      983 2023-06-18 02:15:54.000000 acore_server_metadata-0.3.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.3.1/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.157652 acore_server_metadata-0.4.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 18:58:17.157496 acore_server_metadata-0.4.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.154486 acore_server_metadata-0.4.1/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.1/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 18:54:04.000000 acore_server_metadata-0.4.1/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.1/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.155410 acore_server_metadata-0.4.1/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.1/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    25420 2023-06-19 18:53:00.000000 acore_server_metadata-0.4.1/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.1/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.156008 acore_server_metadata-0.4.1/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.1/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.156785 acore_server_metadata-0.4.1/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.155282 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2245 2023-06-19 18:55:10.000000 acore_server_metadata-0.4.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 18:58:17.157698 acore_server_metadata-0.4.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.157123 acore_server_metadata-0.4.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.1/tests/test_server.py
```

### Comparing `acore_server_metadata-0.3.1/AUTHORS.rst` & `acore_server_metadata-0.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/LICENSE.txt` & `acore_server_metadata-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/PKG-INFO` & `acore_server_metadata-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.3.1
+Version: 0.4.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -144,18 +144,30 @@
         "dev-2": <Server id="dev-2">,
     }
 
 **对服务器进行操作**
 
 .. code-block:: python
 
-    # 启动新的 EC2
-    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
-    # 启动新的 DB Instance
+    # 创建新的 EC2
+    >>> server.run_ec2(ec2_client, ami_id, instance_type, ...)
+    # 创建新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 启动 EC2
+    >>> server.start_ec2(ec2_client)
+    # 启动 RDS
+    >>> server.start_rds(rds_client)
+    # 停止 EC2
+    >>> server.stop_ec2(ec2_client)
+    # 停止 RDS
+    >>> server.stop_rds(rds_client)
+    # 删除 EC2
+    >>> server.delete_ec2(ec2_client)
+    # 删除 RDS
+    >>> server.delete_rds(rds_client)
     # 更新 DB 的 master password
     >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
```

### Comparing `acore_server_metadata-0.3.1/README.rst` & `acore_server_metadata-0.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -112,18 +112,30 @@
         "dev-2": <Server id="dev-2">,
     }
 
 **对服务器进行操作**
 
 .. code-block:: python
 
-    # 启动新的 EC2
-    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
-    # 启动新的 DB Instance
+    # 创建新的 EC2
+    >>> server.run_ec2(ec2_client, ami_id, instance_type, ...)
+    # 创建新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 启动 EC2
+    >>> server.start_ec2(ec2_client)
+    # 启动 RDS
+    >>> server.start_rds(rds_client)
+    # 停止 EC2
+    >>> server.stop_ec2(ec2_client)
+    # 停止 RDS
+    >>> server.stop_rds(rds_client)
+    # 删除 EC2
+    >>> server.delete_ec2(ec2_client)
+    # 删除 RDS
+    >>> server.delete_rds(rds_client)
     # 更新 DB 的 master password
     >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
```

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata/paths.py` & `acore_server_metadata-0.4.1/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata/server.py` & `acore_server_metadata-0.4.1/acore_server_metadata/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,14 +317,26 @@
     ):
         """
         重新获取 EC2 和 RDS 实例的信息. 刷新当前类的 ``ec2_inst`` 和 ``rds_inst`` 属性.
         """
         self.ec2_inst = self.get_ec2(ec2_client, self.id)
         self.rds_inst = self.get_rds(rds_client, self.id)
 
+    def _get_db_snapshot_id(self) -> str:
+        """
+        Get the db snapshot id for this server, the snapshot id
+        naming convention is "${server_id}-%Y-%m-%d-%H-%M-%S".
+        """
+        now = get_utc_now()
+        snapshot_id = "{}-{}".format(
+            self.id,
+            now.strftime("%Y-%m-%d-%H-%M-%S"),
+        )
+        return snapshot_id
+
     # --------------------------------------------------------------------------
     # Operations
     # --------------------------------------------------------------------------
     def run_ec2(
         self,
         ec2_client,
         ami_id: str,
@@ -441,14 +453,68 @@
             AllocatedStorage=allocated_storage,
             PubliclyAccessible=False,  # you should never expose your database to the public
             AutoMinorVersionUpgrade=False,  # don't update MySQL minor version, PLEASE!
             VpcSecurityGroupIds=security_group_ids,
             Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
         )
 
+    def start_ec2(self, ec2_client):
+        """
+        Start the EC2 instance of this server.
+        """
+        self.ec2_inst.start_instance(ec2_client)
+
+    def start_rds(self, rds_client):
+        """
+        Start the RDS DB instance of this server.
+        """
+        self.rds_inst.start_db_instance(rds_client)
+
+    def stop_ec2(self, ec2_client):
+        """
+        Stop the EC2 instance of this server.
+        """
+        self.ec2_inst.stop_instance(ec2_client)
+
+    def stop_rds(self, rds_client):
+        """
+        Stop the RDS DB instance of this server.
+        """
+        self.rds_inst.stop_db_instance(rds_client)
+
+    def delete_ec2(self, ec2_client):
+        """
+        Delete the EC2 instance of this server.
+        """
+        self.ec2_inst.terminate_instance(ec2_client)
+
+    def delete_rds(self, rds_client, create_final_snapshot: bool = True):
+        """
+        Delete the RDS DB instance of this server.
+
+        :param create_final_snapshot: if True, then create a final snapshot
+            before deleting the DB instance. and keep automated backups.
+            if False, then will not create final snapshot, and also delete
+            automated backups.
+        """
+        if create_final_snapshot:
+            snapshot_id = self._get_db_snapshot_id()
+            self.rds_inst.delete_db_instance(
+                rds_client=rds_client,
+                skip_final_snapshot=False,
+                final_db_snapshot_identifier=snapshot_id,
+                delete_automated_backups=False,
+            )
+        else:
+            self.rds_inst.delete_db_instance(
+                rds_client=rds_client,
+                skip_final_snapshot=True,
+                delete_automated_backups=True,
+            )
+
     def associate_eip_address(
         self,
         ec2_client,
         allocation_id: str,
         check_exists: bool = True,
     ):
         """
@@ -546,19 +612,15 @@
         在数据库运维过程中, 我们需要定期备份生产服务器的数据库. 该方法能为我们创建 DB snapshot
         并合理明明, 打上对应的 Tag.
         """
         if check_exists:
             rds_inst = self.get_rds(rds_client, id=self.id)
             if rds_inst is None:
                 raise ServerNotFoundError(f"RDS DB instance {self.id!r} does not exist")
-        now = get_utc_now()
-        snapshot_id = "{}-{}".format(
-            self.id,
-            now.strftime("%Y-%m-%d-%H-%M-%S"),
-        )
+        snapshot_id = self._get_db_snapshot_id()
         rds_client.create_db_snapshot(
             DBSnapshotIdentifier=snapshot_id,
             DBInstanceIdentifier=self.rds_inst.id,
             Tags=[
                 dict(Key=settings.ID_TAG_KEY, Value=self.id),
                 dict(Key="tech:machine_creator", Value="acore_server_metadata"),
             ],
```

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.4.1/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.4.1/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.4.1/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.4.1/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.3.1
+Version: 0.4.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -144,18 +144,30 @@
         "dev-2": <Server id="dev-2">,
     }
 
 **对服务器进行操作**
 
 .. code-block:: python
 
-    # 启动新的 EC2
-    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
-    # 启动新的 DB Instance
+    # 创建新的 EC2
+    >>> server.run_ec2(ec2_client, ami_id, instance_type, ...)
+    # 创建新的 DB Instance
     >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
+    # 启动 EC2
+    >>> server.start_ec2(ec2_client)
+    # 启动 RDS
+    >>> server.start_rds(rds_client)
+    # 停止 EC2
+    >>> server.stop_ec2(ec2_client)
+    # 停止 RDS
+    >>> server.stop_rds(rds_client)
+    # 删除 EC2
+    >>> server.delete_ec2(ec2_client)
+    # 删除 RDS
+    >>> server.delete_rds(rds_client)
     # 更新 DB 的 master password
     >>> server.update_db_master_password(rds_client, master_password)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
```

### Comparing `acore_server_metadata-0.3.1/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.4.1/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/release-history.rst` & `acore_server_metadata-0.4.1/release-history.rst`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.1 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add the following public API:
+    - ``acore_server_metadata.api.Server.start_ec2``
+    - ``acore_server_metadata.api.Server.start_rds``
+    - ``acore_server_metadata.api.Server.stop_ec2``
+    - ``acore_server_metadata.api.Server.stop_rds``
+    - ``acore_server_metadata.api.Server.delete_ec2``
+    - ``acore_server_metadata.api.Server.delete_rds``
+
+
 0.3.1 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``acore_server_metadata.api.Server.update_db_master_password`` to update the master password of RDS DB instance.
```

### Comparing `acore_server_metadata-0.3.1/requirements-doc.txt` & `acore_server_metadata-0.4.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/setup.py` & `acore_server_metadata-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.3.1/tests/test_api.py` & `acore_server_metadata-0.4.1/tests/test_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     _ = api.Server.is_ec2_exists
     _ = api.Server.is_ec2_running
     _ = api.Server.is_rds_exists
     _ = api.Server.is_rds_running
     _ = api.Server.refresh
     _ = api.Server.run_ec2
     _ = api.Server.run_rds
+    _ = api.Server.start_ec2
+    _ = api.Server.start_rds
+    _ = api.Server.stop_ec2
+    _ = api.Server.stop_rds
+    _ = api.Server.delete_ec2
+    _ = api.Server.delete_rds
     _ = api.Server.update_db_master_password
     _ = api.Server.associate_eip_address
     _ = api.Server.create_db_snapshot
     _ = api.Server.cleanup_db_snapshot
 
 
 if __name__ == "__main__":
```

### Comparing `acore_server_metadata-0.3.1/tests/test_server.py` & `acore_server_metadata-0.4.1/tests/test_server.py`

 * *Files identical despite different names*

