# Comparing `tmp/quorum_fullnode_py-1.3.1.tar.gz` & `tmp/quorum_fullnode_py-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_fullnode_py-1.3.1.tar", last modified: Sat Jun 10 02:36:09 2023, max compression
+gzip compressed data, was "quorum_fullnode_py-1.3.2.tar", last modified: Mon Jun 19 03:13:23 2023, max compression
```

## Comparing `quorum_fullnode_py-1.3.1.tar` & `quorum_fullnode_py-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.742017 quorum_fullnode_py-1.3.1/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2522 2023-06-10 02:36:09.742017 quorum_fullnode_py-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.3.1/README.md
--rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.697473 quorum_fullnode_py-1.3.1/quorum_fullnode_py/
--rw-rw-rw-   0        0        0      329 2023-06-10 02:33:10.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.732045 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/
--rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/__init__.py
--rw-rw-rw-   0        0        0     6762 2023-05-19 08:38:21.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/base.py
--rw-rw-rw-   0        0        0    23960 2023-06-10 02:35:00.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/fullnode.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.738049 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/
--rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/_http.py
--rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/fullnode.py
--rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.726073 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/
--rw-rw-rw-   0        0        0     2522 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-10 02:36:09.000000 quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 02:36:09.743017 quorum_fullnode_py-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-06-10 02:33:10.000000 quorum_fullnode_py-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 02:36:09.739050 quorum_fullnode_py-1.3.1/tests/
--rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.3.1/tests/test_fullnode.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.486081 quorum_fullnode_py-1.3.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:18.000000 quorum_fullnode_py-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2522 2023-06-19 03:13:23.485090 quorum_fullnode_py-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-04-03 04:33:04.000000 quorum_fullnode_py-1.3.2/README.md
+-rw-rw-rw-   0        0        0      169 2023-02-23 03:21:16.000000 quorum_fullnode_py-1.3.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.426867 quorum_fullnode_py-1.3.2/quorum_fullnode_py/
+-rw-rw-rw-   0        0        0      329 2023-06-19 03:10:33.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.473112 quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/
+-rw-rw-rw-   0        0        0      164 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     6762 2023-05-19 08:38:21.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/base.py
+-rw-rw-rw-   0        0        0    24120 2023-06-19 03:10:20.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/fullnode.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.480098 quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/
+-rw-rw-rw-   0        0        0      114 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     1460 2023-04-06 03:32:26.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/_http.py
+-rw-rw-rw-   0        0        0      871 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/fullnode.py
+-rw-rw-rw-   0        0        0     1490 2023-02-24 06:37:34.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.466141 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-06-19 03:13:23.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-19 03:13:23.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:13:23.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 03:13:23.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 03:13:23.000000 quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:13:23.486081 quorum_fullnode_py-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-06-19 03:10:33.000000 quorum_fullnode_py-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:13:23.483086 quorum_fullnode_py-1.3.2/tests/
+-rw-rw-rw-   0        0        0     2847 2023-03-27 06:09:37.000000 quorum_fullnode_py-1.3.2/tests/test_fullnode.py
```

### Comparing `quorum_fullnode_py-1.3.1/LICENSE` & `quorum_fullnode_py-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/PKG-INFO` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum_fullnode_py
-Version: 1.3.1
+Name: quorum-fullnode-py
+Version: 1.3.2
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.3.1/README.md` & `quorum_fullnode_py-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/base.py` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/base.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py/api/fullnode.py` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py/api/fullnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,16 +568,22 @@
         agreement_tick_length: int = None,
         agreement_tick_count=None,
         producer_pubkey: list = None,
         group_id: str = None,
     ):
         group_id = self._check_group_id_as_required(group_id)
         req_id = self.get_consensus(group_id).get("proof_req_id")
-        req = self.get_consensus_req(req_id, group_id).get("resps")[0]["Req"]
+        reqs = self.get_consensus_req(req_id, group_id).get("resps", [])
+        if not reqs:
+            req = {}
+        else:
+            req = reqs[0]["Req"]
 
+        if start_from_epoch is None:
+            start_from_epoch = 1
         if trx_epoch_tick and trx_epoch_tick < 500:
             raise ValueError("trx_epoch_tick should be greater than 500(ms)")
         if agreement_tick_length and agreement_tick_length < 1000:
             raise ValueError(
                 "agreement_tick_length should be greater than 1000(ms)"
             )
         if agreement_tick_count and agreement_tick_count < 10:
```

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/_http.py` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py/client/fullnode.py` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py/client/fullnode.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py/exceptions.py` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py/exceptions.py`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/PKG-INFO` & `quorum_fullnode_py-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: quorum-fullnode-py
-Version: 1.3.1
+Name: quorum_fullnode_py
+Version: 1.3.2
 Summary: Python SDK for FullNode of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_fullnode_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_fullnode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_fullnode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_fullnode_py-1.3.1/quorum_fullnode_py.egg-info/SOURCES.txt` & `quorum_fullnode_py-1.3.2/quorum_fullnode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_fullnode_py-1.3.1/setup.py` & `quorum_fullnode_py-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_fullnode_py",
-    version="1.3.1",
+    version="1.3.2",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python SDK for FullNode of QuoRum",
     keywords=["quorum_fullnode_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_fullnode_py",
```

### Comparing `quorum_fullnode_py-1.3.1/tests/test_fullnode.py` & `quorum_fullnode_py-1.3.2/tests/test_fullnode.py`

 * *Files identical despite different names*

