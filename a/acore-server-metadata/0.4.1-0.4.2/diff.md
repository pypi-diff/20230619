# Comparing `tmp/acore_server_metadata-0.4.1.tar.gz` & `tmp/acore_server_metadata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.4.1.tar", last modified: Mon Jun 19 18:58:17 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.4.2.tar", last modified: Mon Jun 19 20:48:53 2023, max compression
```

## Comparing `acore_server_metadata-0.4.1.tar` & `acore_server_metadata-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.157652 acore_server_metadata-0.4.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 18:58:17.157496 acore_server_metadata-0.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.154486 acore_server_metadata-0.4.1/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.1/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 18:54:04.000000 acore_server_metadata-0.4.1/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.1/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.155410 acore_server_metadata-0.4.1/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.1/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    25420 2023-06-19 18:53:00.000000 acore_server_metadata-0.4.1/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.1/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.156008 acore_server_metadata-0.4.1/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.1/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.1/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.156785 acore_server_metadata-0.4.1/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.155282 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 18:58:17.000000 acore_server_metadata-0.4.1/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2245 2023-06-19 18:55:10.000000 acore_server_metadata-0.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 18:58:17.157698 acore_server_metadata-0.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:58:17.157123 acore_server_metadata-0.4.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.1/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.517553 acore_server_metadata-0.4.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 20:48:53.517422 acore_server_metadata-0.4.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.514417 acore_server_metadata-0.4.2/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.2/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 20:47:25.000000 acore_server_metadata-0.4.2/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.2/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.515300 acore_server_metadata-0.4.2/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.2/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    26210 2023-06-19 20:43:44.000000 acore_server_metadata-0.4.2/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.2/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.516022 acore_server_metadata-0.4.2/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.2/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.2/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.516769 acore_server_metadata-0.4.2/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.515158 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-19 20:48:53.000000 acore_server_metadata-0.4.2/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2852 2023-06-19 20:47:19.000000 acore_server_metadata-0.4.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 20:48:53.517593 acore_server_metadata-0.4.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 20:48:53.517103 acore_server_metadata-0.4.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.2/tests/test_server.py
```

### Comparing `acore_server_metadata-0.4.1/AUTHORS.rst` & `acore_server_metadata-0.4.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/LICENSE.txt` & `acore_server_metadata-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/PKG-INFO` & `acore_server_metadata-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.1/README.rst` & `acore_server_metadata-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata/paths.py` & `acore_server_metadata-0.4.2/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata/server.py` & `acore_server_metadata-0.4.2/acore_server_metadata/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -395,14 +395,16 @@
                 dict(
                     ResourceType="instance",
                     Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
                 ),
             ],
         )
 
+    create_ec2 = run_ec2  # alias
+
     def run_rds(
         self,
         rds_client,
         db_snapshot_identifier: str,
         db_instance_class: str,
         db_subnet_group_name: str,
         security_group_ids: T.List[str],
@@ -453,14 +455,16 @@
             AllocatedStorage=allocated_storage,
             PubliclyAccessible=False,  # you should never expose your database to the public
             AutoMinorVersionUpgrade=False,  # don't update MySQL minor version, PLEASE!
             VpcSecurityGroupIds=security_group_ids,
             Tags=[dict(Key=k, Value=v) for k, v in tags.items()],
         )
 
+    create_rds = run_rds  # alias
+
     def start_ec2(self, ec2_client):
         """
         Start the EC2 instance of this server.
         """
         self.ec2_inst.start_instance(ec2_client)
 
     def start_rds(self, rds_client):
@@ -512,15 +516,15 @@
             )
 
     def associate_eip_address(
         self,
         ec2_client,
         allocation_id: str,
         check_exists: bool = True,
-    ):
+    ) -> T.Optional[dict]:
         """
         Associate the given Elastic IP address with the EC2 instance.
         Note that this operation is idempotent, it will disassociate and re-associate
         the Elastic IP address if it is already associated with another EC2 instance
         or this one, and each association will incur a small fee. So I would like
         to check before doing this.
 
@@ -528,52 +532,58 @@
         映射表, 然后用这个方法确保每个服务器的 IP 是正确的 (该方法是幂等的, 如果已经设置好了
         则什么也不会做).
 
         :param ec2_client: boto3 ec2 client
         :param allocation_id: the EIP allocation id, not the pulibc ip,
             example "eipalloc-1a2b3c4d"
         :param check_exists: check if the EC2 instance exists before associating.
+
+        :return: if we actually send the ``rds_client.associate_address`` API,
+            it returns the response of that API. Otherwise, it returns None.
         """
         if check_exists:
             ec2_inst = self.get_ec2(ec2_client, id=self.id)
             if ec2_inst is None:
                 raise ServerAlreadyExistsError(
                     f"EC2 instance {self.id!r} does not exist"
                 )
 
         # check if this allocation id is already associated with an instance
         res = ec2_client.describe_addresses(AllocationIds=[allocation_id])
         address_data = res["Addresses"][0]
         public_id = address_data["PublicIp"]
         instance_id = address_data.get("InstanceId", "invalid-instance-id")
-        if instance_id == self.ec2_inst.id:
-            return  # already associated
+        if instance_id == self.ec2_inst.id:  # already associated
+            return None
 
         # associate eip address
-        ec2_client.associate_address(
+        return ec2_client.associate_address(
             AllocationId=allocation_id,
             InstanceId=self.ec2_inst.id,
         )
 
     def update_db_master_password(
         self,
         rds_client,
         master_password: str,
         check_exists: bool = True,
-    ):
+    ) -> T.Optional[str]:
         """
         Update the DB instance master password. When you recover the DB instance
         from a snapshot, the master password is the same as the password when you
         create the snapshot. This method can be used to update the master password.
 
         在数据库运维过程中, 我们都是从自己备份的 Snapshot 启动 DB 实例. 它的管理员密码会继承
         备份 Snapshot 的时候的密码. 比如我们希望用开发环境的 snapshot 创建生产环境的数据库,
         这时候再继续用开发环境的密码肯定不妥, 所以需要更新密码. 该方法可以做到这一点.
         并且这个方法是幂等的, 如果密码已经设置好了, 则什么也不会做. 如果密码没有被设置过, 则
         会设置密码.
+
+        :return: if we actually send the ``rds_client.modify_db_instance`` API,
+            it returns the response of that API. Otherwise, it returns None.
         """
         if check_exists:
             rds_inst = self.get_rds(rds_client, id=self.id)
             if rds_inst is None:
                 raise ServerNotFoundError(f"RDS DB instance {self.id!r} does not exist")
         else:
             rds_inst = self.rds_inst
@@ -581,29 +591,31 @@
         hashes.use_sha256()
         master_password_digest = hashes.of_str(master_password, hexdigest=True)
         if (
             rds_inst.tags.get("tech:master_password_digest", "invalid")
             == master_password_digest
         ):
             # do nothing
-            return
+            return None
 
-        rds_client.modify_db_instance(
+        response = rds_client.modify_db_instance(
             DBInstanceIdentifier=self.rds_inst.id,
             MasterUserPassword=master_password,
             ApplyImmediately=True,
         )
 
         rds_client.add_tags_to_resource(
             ResourceName=rds_inst.db_instance_arn,
             Tags=[
                 dict(Key="tech:master_password_digest", Value=master_password_digest)
             ],
         )
 
+        return response
+
     def create_db_snapshot(
         self,
         rds_client,
         check_exists: bool = True,
     ):
         """
         Create a 'manual' DB snapshot for the RDS DB instance.
@@ -627,27 +639,30 @@
         )
 
     def cleanup_db_snapshot(
         self,
         rds_client,
         keep_n: int = 3,
         keep_days: int = 365,
-    ):
+    ) -> T.Optional[T.List[dict]]:
         """
         Clean up old RDS DB snapshots of this server.
 
         在数据库运维过程中, 我们需要定期备份生产服务器的数据库. 该方法能为我们创建 DB snapshot
         并合理明明, 打上对应的 Tag.
 
         :param rds_client: boto3 rds client
         :param keep_n: keep the latest N snapshots. this criteria has higher priority.
             for example, even the only N snapshots is very very old, but we still keep them.
         :param keep_days: delete snapshots older than N days if we have more than N snapshots.
 
         todo: use paginator to list existing snapshots
+
+        :return: if we actually send the ``rds_client.delete_db_snapshot`` API,
+            it returns the list of response of that API. Otherwise, it returns None.
         """
         # get the list of manual created snapshots
         res = rds_client.describe_db_snapshots(
             DBInstanceIdentifier=self.rds_inst.id,
             SnapshotType="manual",
             MaxRecords=100,
         )
@@ -656,16 +671,19 @@
             sorted(
                 res.get("DBSnapshots", []),
                 key=lambda d: d["SnapshotCreateTime"],
                 reverse=True,
             )
         )
         if len(snapshot_list) <= keep_n:
-            return
+            return None
         now = get_utc_now()
+        response_list = []
         for snapshot in snapshot_list[keep_n:]:
             create_time = snapshot["SnapshotCreateTime"]
             create_time = create_time.replace(tzinfo=timezone.utc)
             if (now - create_time).total_seconds() > (keep_days * 86400):
-                rds_client.delete_db_snapshot(
+                response = rds_client.delete_db_snapshot(
                     DBSnapshotIdentifier=snapshot["DBSnapshotIdentifier"],
                 )
+                response_list.append(response)
+        return response_list
```

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.4.2/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.4.2/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.4.2/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.4.2/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.4.1
+Version: 0.4.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.1/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.4.2/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/release-history.rst` & `acore_server_metadata-0.4.2/release-history.rst`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.2 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+**Minor Improvements**
+
+- ``acore_server_metadata.api.Server.associate_eip_address`` now returns API response or None
+- ``acore_server_metadata.api.Server.update_db_master_password`` now returns API response or None
+- ``acore_server_metadata.api.Server.cleanup_db_snapshot`` now returns API response or None
+- add ``acore_server_metadata.api.Server.create_ec2``, it is a alias of ``run_ec2``
+- add ``acore_server_metadata.api.Server.create_rds``, it is a alias of ``run_rds``
+
+
 0.4.1 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add the following public API:
     - ``acore_server_metadata.api.Server.start_ec2``
     - ``acore_server_metadata.api.Server.start_rds``
```

### Comparing `acore_server_metadata-0.4.1/requirements-doc.txt` & `acore_server_metadata-0.4.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/setup.py` & `acore_server_metadata-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/tests/test_api.py` & `acore_server_metadata-0.4.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.1/tests/test_server.py` & `acore_server_metadata-0.4.2/tests/test_server.py`

 * *Files identical despite different names*

