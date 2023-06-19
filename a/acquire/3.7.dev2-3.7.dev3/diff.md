# Comparing `tmp/acquire-3.7.dev2.tar.gz` & `tmp/acquire-3.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.7.dev2.tar", last modified: Fri Jun 16 12:48:21 2023, max compression
+gzip compressed data, was "acquire-3.7.dev3.tar", last modified: Mon Jun 19 15:52:55 2023, max compression
```

## Comparing `acquire-3.7.dev2.tar` & `acquire-3.7.dev3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.741311 acquire-3.7.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 12:48:07.000000 acquire-3.7.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:48:07.000000 acquire-3.7.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:48:07.000000 acquire-3.7.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-16 12:48:21.741311 acquire-3.7.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-16 12:48:07.000000 acquire-3.7.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.725311 acquire-3.7.dev2/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.729311 acquire-3.7.dev2/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.733311 acquire-3.7.dev2/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.733311 acquire-3.7.dev2/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.737311 acquire-3.7.dev2/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.737311 acquire-3.7.dev2/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-16 12:48:07.000000 acquire-3.7.dev2/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.729311 acquire-3.7.dev2/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:48:21.000000 acquire-3.7.dev2/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-16 12:48:11.000000 acquire-3.7.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:48:21.741311 acquire-3.7.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.741311 acquire-3.7.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:08.000000 acquire-3.7.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:48:21.741311 acquire-3.7.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-16 12:48:07.000000 acquire-3.7.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-19 15:52:41.000000 acquire-3.7.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-19 15:52:41.000000 acquire-3.7.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 15:52:41.000000 acquire-3.7.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-19 15:52:55.142928 acquire-3.7.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-19 15:52:41.000000 acquire-3.7.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76017 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-19 15:52:41.000000 acquire-3.7.dev3/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.138928 acquire-3.7.dev3/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:52:55.000000 acquire-3.7.dev3/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-19 15:52:45.000000 acquire-3.7.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:52:55.142928 acquire-3.7.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:52:55.142928 acquire-3.7.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 15:52:41.000000 acquire-3.7.dev3/tox.ini
```

### Comparing `acquire-3.7.dev2/LICENSE` & `acquire-3.7.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/PKG-INFO` & `acquire-3.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev2
+Version: 3.7.dev3
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev2/README.md` & `acquire-3.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/acquire.py` & `acquire-3.7.dev3/acquire/acquire.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,14 +942,15 @@
         ("dir", "sysvol/ProgramData/Trend Micro/AMSP/quarantine"),
         # McAfee
         ("dir", "sysvol/Quarantine"),
         ("dir", "sysvol/ProgramData/McAfee/VirusScan/Quarantine"),
         # Sophos
         ("glob", "sysvol/ProgramData/Sophos/Sophos/*/Quarantine"),
         ("glob", "sysvol/ProgramData/Sophos/Sophos */INFECTED"),
+        ("dir", "sysvol/ProgramData/Sophos/Safestore"),
         # HitmanPRO
         ("dir", "sysvol/ProgramData/HitmanPro/Quarantine"),
     ]
 
 
 @register_module("--history")
 class History(Module):
```

### Comparing `acquire-3.7.dev2/acquire/collector.py` & `acquire-3.7.dev3/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/crypt.py` & `acquire-3.7.dev3/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/dynamic/windows/collect.py` & `acquire-3.7.dev3/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/dynamic/windows/handles.py` & `acquire-3.7.dev3/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/dynamic/windows/named_objects.py` & `acquire-3.7.dev3/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/dynamic/windows/ntdll.py` & `acquire-3.7.dev3/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/dynamic/windows/types.py` & `acquire-3.7.dev3/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/esxi.py` & `acquire-3.7.dev3/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/hashes.py` & `acquire-3.7.dev3/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/log.py` & `acquire-3.7.dev3/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/outputs/base.py` & `acquire-3.7.dev3/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/outputs/dir.py` & `acquire-3.7.dev3/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/outputs/tar.py` & `acquire-3.7.dev3/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/tools/decrypter.py` & `acquire-3.7.dev3/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/uploaders/minio.py` & `acquire-3.7.dev3/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/uploaders/plugin.py` & `acquire-3.7.dev3/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/uploaders/plugin_registry.py` & `acquire-3.7.dev3/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire/utils.py` & `acquire-3.7.dev3/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/acquire.egg-info/PKG-INFO` & `acquire-3.7.dev3/acquire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.7.dev2
+Version: 3.7.dev3
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.7.dev2/acquire.egg-info/SOURCES.txt` & `acquire-3.7.dev3/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/pyproject.toml` & `acquire-3.7.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/conftest.py` & `acquire-3.7.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/docs/Makefile` & `acquire-3.7.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/docs/conf.py` & `acquire-3.7.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_acquire_command.py` & `acquire-3.7.dev3/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_collector.py` & `acquire-3.7.dev3/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_esxi_memory.py` & `acquire-3.7.dev3/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_file_sorting.py` & `acquire-3.7.dev3/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_minio_uploader.py` & `acquire-3.7.dev3/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_plugin.py` & `acquire-3.7.dev3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tests/test_utils.py` & `acquire-3.7.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.7.dev2/tox.ini` & `acquire-3.7.dev3/tox.ini`

 * *Files identical despite different names*

