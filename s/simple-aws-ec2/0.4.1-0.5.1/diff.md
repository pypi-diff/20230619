# Comparing `tmp/simple_aws_ec2-0.4.1.tar.gz` & `tmp/simple_aws_ec2-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.4.1.tar", last modified: Fri Jun 16 01:24:31 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.5.1.tar", last modified: Mon Jun 19 18:45:38 2023, max compression
```

## Comparing `simple_aws_ec2-0.4.1.tar` & `simple_aws_ec2-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637974 simple_aws_ec2-0.4.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:16.000000 simple_aws_ec2-0.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-16 01:24:31.637837 simple_aws_ec2-0.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.4.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2621 2023-06-16 01:09:03.000000 simple_aws_ec2-0.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.4.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 01:24:31.638017 simple_aws_ec2-0.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.4.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.635519 simple_aws_ec2-0.4.1/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 01:21:55.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-16 01:11:20.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.636559 simple_aws_ec2-0.4.1/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    33285 2023-06-16 01:10:53.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/exc.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637065 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.636425 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-16 01:24:31.000000 simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 01:24:31.637524 simple_aws_ec2-0.4.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3071 2023-06-16 01:21:32.000000 simple_aws_ec2-0.4.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8114 2023-06-16 01:06:20.000000 simple_aws_ec2-0.4.1/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.256548 simple_aws_ec2-0.5.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:16.000000 simple_aws_ec2-0.5.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-19 18:45:38.256381 simple_aws_ec2-0.5.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.5.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2825 2023-06-19 18:45:02.000000 simple_aws_ec2-0.5.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.5.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.5.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 18:45:38.256605 simple_aws_ec2-0.5.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.5.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.254222 simple_aws_ec2-0.5.1/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 18:27:29.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-16 01:11:20.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.255104 simple_aws_ec2-0.5.1/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    33502 2023-06-19 18:24:31.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/exc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.255612 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.254980 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.256030 simple_aws_ec2-0.5.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3114 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8301 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.1/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.4.1/AUTHORS.rst` & `simple_aws_ec2-0.5.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/LICENSE.txt` & `simple_aws_ec2-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/PKG-INFO` & `simple_aws_ec2-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_ec2
-Version: 0.4.1
+Version: 0.5.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.4.1/README.rst` & `simple_aws_ec2-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/release-history.rst` & `simple_aws_ec2-0.5.1/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.1 (2023-06-19)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add :meth:`~simple_aws_ec2.ec2.Ec2Instance.terminate_instance` method.
+
+
 0.4.1 (2023-06-15)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_status` waiter method.
 - add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_running` waiter method.
 - add :meth:`~simple_aws_ec2.ec2.Ec2Instance.wait_for_stopped` waiter method.
```

### Comparing `simple_aws_ec2-0.4.1/requirements-doc.txt` & `simple_aws_ec2-0.5.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/setup.py` & `simple_aws_ec2-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/simple_aws_ec2/api.py` & `simple_aws_ec2-0.5.1/simple_aws_ec2/api.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.5.1/simple_aws_ec2/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,23 @@
         Stop instance.
         """
         return ec2_client.stop_instances(
             InstanceIds=[self.id],
             DryRun=False,
         )
 
+    def terminate_instance(self, ec2_client):
+        """
+        Terminate instance.
+        """
+        return ec2_client.terminate_instances(
+            InstanceIds=[self.id],
+            DryRun=False,
+        )
+
     # --------------------------------------------------------------------------
     # Waiter
     # --------------------------------------------------------------------------
     def wait_for_status(
         self,
         ec2_client,
         stop_status: T.Union[EC2InstanceStatusEnum, T.List[EC2InstanceStatusEnum]],
```

### Comparing `simple_aws_ec2-0.4.1/simple_aws_ec2/vendor/waiter.py` & `simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-ec2
-Version: 0.4.1
+Version: 0.5.1
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.4.1/simple_aws_ec2.egg-info/SOURCES.txt` & `simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.4.1/tests/test_api.py` & `simple_aws_ec2-0.5.1/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     _ = api.Ec2Instance.is_terminated
     _ = api.Ec2Instance.is_stopping
     _ = api.Ec2Instance.is_stopped
     _ = api.Ec2Instance.is_ready_to_stop
     _ = api.Ec2Instance.is_ready_to_start
     _ = api.Ec2Instance.start_instance
     _ = api.Ec2Instance.stop_instance
+    _ = api.Ec2Instance.terminate_instance
     _ = api.Ec2Instance.wait_for_status
     _ = api.Ec2Instance.wait_for_running
     _ = api.Ec2Instance.wait_for_stopped
     _ = api.Ec2Instance.wait_for_terminated
     _ = api.Ec2Instance.query
     _ = api.Ec2Instance.from_id
     _ = api.Ec2Instance.from_ec2_inside
```

### Comparing `simple_aws_ec2-0.4.1/tests/test_ec2.py` & `simple_aws_ec2-0.5.1/tests/test_ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,19 @@
         assert new_ec2_inst.is_stopped() is True
         with pytest.raises(StatusError):
             new_ec2_inst.wait_for_running(
                 ec2_client=self.bsm.ec2_client,
                 verbose=False,
             )
 
+        new_ec2_inst.terminate_instance(self.bsm.ec2_client)
+        new_ec2_inst = Ec2Instance.from_id(self.bsm.ec2_client, self.inst_id_1)
+        assert new_ec2_inst.is_terminated()
+
+
     def test(self):
         self._test_ec2()
         self._test_ec2_start_and_stop()
         self._test_wait_for_status()
         self._test_image()
```

