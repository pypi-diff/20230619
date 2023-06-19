# Comparing `tmp/simple_aws_rds-0.3.1.tar.gz` & `tmp/simple_aws_rds-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_rds-0.3.1.tar", last modified: Fri Jun 16 01:03:04 2023, max compression
+gzip compressed data, was "simple_aws_rds-0.4.1.tar", last modified: Mon Jun 19 18:43:54 2023, max compression
```

## Comparing `simple_aws_rds-0.3.1.tar` & `simple_aws_rds-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.896461 simple_aws_rds-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:21.000000 simple_aws_rds-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-16 01:03:04.896308 simple_aws_rds-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3833 2023-06-15 18:43:35.000000 simple_aws_rds-0.3.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1302 2023-06-16 00:51:56.000000 simple_aws_rds-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-15 16:48:33.000000 simple_aws_rds-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-15 16:48:10.000000 simple_aws_rds-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 01:03:04.896506 simple_aws_rds-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7563 2023-06-15 18:42:44.000000 simple_aws_rds-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894204 simple_aws_rds-0.3.1/simple_aws_rds/
--rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.3.1/simple_aws_rds/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 00:50:28.000000 simple_aws_rds-0.3.1/simple_aws_rds/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-15 22:04:45.000000 simple_aws_rds-0.3.1/simple_aws_rds/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894991 simple_aws_rds-0.3.1/simple_aws_rds/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.3.1/simple_aws_rds/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_rds-0.3.1/simple_aws_rds/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    27497 2023-06-16 00:55:46.000000 simple_aws_rds-0.3.1/simple_aws_rds/rds.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.895506 simple_aws_rds-0.3.1/simple_aws_rds/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_rds-0.3.1/simple_aws_rds/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_rds-0.3.1/simple_aws_rds/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.894877 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-16 01:03:04.000000 simple_aws_rds-0.3.1/simple_aws_rds.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:03:04.895970 simple_aws_rds-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      321 2023-05-03 16:11:52.000000 simple_aws_rds-0.3.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3957 2023-06-15 22:06:25.000000 simple_aws_rds-0.3.1/tests/test_rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.374193 simple_aws_rds-0.4.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:21.000000 simple_aws_rds-0.4.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 15:29:20.000000 simple_aws_rds-0.4.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 15:29:20.000000 simple_aws_rds-0.4.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-19 18:43:54.373994 simple_aws_rds-0.4.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3833 2023-06-15 18:43:35.000000 simple_aws_rds-0.4.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1476 2023-06-19 18:40:36.000000 simple_aws_rds-0.4.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 15:29:20.000000 simple_aws_rds-0.4.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 15:29:20.000000 simple_aws_rds-0.4.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-15 16:48:33.000000 simple_aws_rds-0.4.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-15 16:48:10.000000 simple_aws_rds-0.4.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 18:43:54.374247 simple_aws_rds-0.4.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7563 2023-06-15 18:42:44.000000 simple_aws_rds-0.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.371556 simple_aws_rds-0.4.1/simple_aws_rds/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      406 2023-05-03 16:11:27.000000 simple_aws_rds-0.4.1/simple_aws_rds/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 18:40:02.000000 simple_aws_rds-0.4.1/simple_aws_rds/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-15 22:04:45.000000 simple_aws_rds-0.4.1/simple_aws_rds/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.372800 simple_aws_rds-0.4.1/simple_aws_rds/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 15:29:20.000000 simple_aws_rds-0.4.1/simple_aws_rds/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_rds-0.4.1/simple_aws_rds/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    28203 2023-06-19 18:32:01.000000 simple_aws_rds-0.4.1/simple_aws_rds/rds.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.373236 simple_aws_rds-0.4.1/simple_aws_rds/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_rds-0.4.1/simple_aws_rds/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_rds-0.4.1/simple_aws_rds/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.372677 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4948 2023-06-19 18:43:54.000000 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-19 18:43:54.000000 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 18:43:54.000000 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-19 18:43:54.000000 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-19 18:43:54.000000 simple_aws_rds-0.4.1/simple_aws_rds.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:43:54.373663 simple_aws_rds-0.4.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2384 2023-06-19 18:43:22.000000 simple_aws_rds-0.4.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4433 2023-06-19 18:38:12.000000 simple_aws_rds-0.4.1/tests/test_rds.py
```

### Comparing `simple_aws_rds-0.3.1/AUTHORS.rst` & `simple_aws_rds-0.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/LICENSE.txt` & `simple_aws_rds-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/PKG-INFO` & `simple_aws_rds-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_rds
-Version: 0.3.1
+Version: 0.4.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.3.1/README.rst` & `simple_aws_rds-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/release-history.rst` & `simple_aws_rds-0.4.1/release-history.rst`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.4.1 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``RDSDBInstance.delete_db_instance``
+
+
 0.3.1 (2023-06-15)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``RDSDBInstanceStatusGroupEnum``
 - add ``RDSDBInstance.wait_for_available``
 - add ``RDSDBInstance.wait_for_stopped``
```

### Comparing `simple_aws_rds-0.3.1/requirements-doc.txt` & `simple_aws_rds-0.4.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/setup.py` & `simple_aws_rds-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/simple_aws_rds/rds.py` & `simple_aws_rds-0.4.1/simple_aws_rds/rds.py`

 * *Files 6% similar despite different names*

```diff
@@ -466,21 +466,44 @@
     def is_in_transition(self) -> bool:
         """ """
         return self.status in {
             status.value for status in RDSDBInstanceStatusGroupEnum.in_transition
         }
 
     def start_db_instance(self, rds_client) -> dict:
-        """ """
+        """
+        Start the RDS DB instance
+        """
         return rds_client.start_db_instance(DBInstanceIdentifier=self.id)
 
     def stop_db_instance(self, rds_client) -> dict:
-        """ """
+        """
+        Stop the RDS DB instance
+        """
         return rds_client.stop_db_instance(DBInstanceIdentifier=self.id)
 
+    def delete_db_instance(
+        self,
+        rds_client,
+        skip_final_snapshot: bool = NOTHING,
+        final_db_snapshot_identifier: str = NOTHING,
+        delete_automated_backups: bool = NOTHING,
+    ) -> dict:
+        """
+        Delete the RDS DB instance
+        """
+        return rds_client.delete_db_instance(
+            **resolve_kwargs(
+                DBInstanceIdentifier=self.id,
+                SkipFinalSnapshot=skip_final_snapshot,
+                FinalDBSnapshotIdentifier=final_db_snapshot_identifier,
+                DeleteAutomatedBackups=delete_automated_backups,
+            )
+        )
+
     def wait_for_status(
         self,
         rds_client,
         stop_status: T.Union[RDSDBInstanceStatusEnum, T.List[RDSDBInstanceStatusEnum]],
         delays: T.Union[int, float] = 10,
         timeout: T.Union[int, float] = 300,
         error_status: T.Optional[
```

### Comparing `simple_aws_rds-0.3.1/simple_aws_rds/vendor/waiter.py` & `simple_aws_rds-0.4.1/simple_aws_rds/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/simple_aws_rds.egg-info/PKG-INFO` & `simple_aws_rds-0.4.1/simple_aws_rds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-rds
-Version: 0.3.1
+Version: 0.4.1
 Summary: Simple AWS RDS dev tools.
 Home-page: https://github.com/MacHu-GWU/simple_aws_rds-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_rds/0.4.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_rds-0.3.1/simple_aws_rds.egg-info/SOURCES.txt` & `simple_aws_rds-0.4.1/simple_aws_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_rds-0.3.1/tests/test_rds.py` & `simple_aws_rds-0.4.1/tests/test_rds.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,15 +109,26 @@
         assert new_db_inst.is_stopped() is True
         with pytest.raises(StatusError):
             db_inst.wait_for_available(
                 rds_client=self.bsm.rds_client,
                 verbose=False,
             )
 
+    def _test_delete_db_instance(self):
+        db_inst = RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
+        db_inst.delete_db_instance(self.bsm.rds_client)
+        try:
+            RDSDBInstance.from_id(self.bsm.rds_client, self.inst_id_1)
+        except Exception as e:
+            assert "not found" in str(e)
+
     def test(self):
+        # these test has to run in sequence, the next test depends on the state
+        # of previous one
         self._test()
         self._test_wait_for_status()
+        self._test_delete_db_instance()
 
 
 if __name__ == "__main__":
     basename = os.path.basename(__file__)
     pytest.main([basename, "-s", "--tb=native"])
```

