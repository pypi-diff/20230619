# Comparing `tmp/rclone-python-0.1.6.tar.gz` & `tmp/rclone-python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.6.tar", last modified: Thu Jun 15 23:04:22 2023, max compression
+gzip compressed data, was "rclone-python-0.1.7.tar", last modified: Mon Jun 19 09:29:26 2023, max compression
```

## Comparing `rclone-python-0.1.6.tar` & `rclone-python-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.088369 rclone-python-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 23:04:10.000000 rclone-python-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-15 23:04:22.088369 rclone-python-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-15 23:04:10.000000 rclone-python-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.084369 rclone-python-0.1.6/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-15 23:04:10.000000 rclone-python-0.1.6/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:04:22.088369 rclone-python-0.1.6/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 23:04:22.000000 rclone-python-0.1.6/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:04:22.088369 rclone-python-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 23:04:10.000000 rclone-python-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 09:29:14.000000 rclone-python-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-19 09:29:26.798952 rclone-python-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-19 09:29:14.000000 rclone-python-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/extract_remotenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-19 09:29:14.000000 rclone-python-0.1.7/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:29:26.798952 rclone-python-0.1.7/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 09:29:26.000000 rclone-python-0.1.7/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:29:26.798952 rclone-python-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-19 09:29:14.000000 rclone-python-0.1.7/setup.py
```

### Comparing `rclone-python-0.1.6/LICENSE` & `rclone-python-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.6/PKG-INFO` & `rclone-python-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 A python wrapper for rclone that makes rclone's functionality usable in python.
 rclone needs to be installed on the system for the wrapper to work.
 
 ![demo gif](https://raw.githubusercontent.com/Johannes11833/rclone_python/master/demo/demo.gif)
 
 ## Features ⚒️
 
-- Copy and move files between remotes
+- Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
 - Create new remotes
 - Check available remotes
 
 ## Installation 💾
```

### Comparing `rclone-python-0.1.6/README.md` & `rclone-python-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 A python wrapper for rclone that makes rclone's functionality usable in python.
 rclone needs to be installed on the system for the wrapper to work.
 
 ![demo gif](https://raw.githubusercontent.com/Johannes11833/rclone_python/master/demo/demo.gif)
 
 ## Features ⚒️
 
-- Copy and move files between remotes
+- Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
 - Create new remotes
 - Check available remotes
 
 ## Installation 💾
```

### Comparing `rclone-python-0.1.6/rclone_python/rclone.py` & `rclone-python-0.1.7/rclone_python/rclone.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,38 @@
 
     if process.returncode == 0:
         return json.loads(process.stdout)
     else:
         raise Exception(f"ls operation on {path} failed with {process.stderr}")
 
 
+def tree(
+    path: str,
+    args: List[str] = None,
+) -> str:
+    """Returns the contents of the remote path in a tree like fashion.
+
+    Args:
+        path (str): The path from which the tree should be generated
+        args (List[str], optional): Optional additional list of flags (e.g. ['--all', '--modtime']).
+
+    Returns:
+        str: String containing the file tree.
+    """
+    if args is None:
+        args = []
+
+    process = utils.run_cmd(f'rclone tree "{path}"', args)
+
+    if process.returncode != 0:
+        raise Exception(process.stderr)
+    else:
+        return process.stdout
+
+
 @__check_installed
 def _rclone_transfer_operation(
     in_path: str,
     out_path: str,
     command: str,
     command_descr: str,
     ignore_existing=False,
```

### Comparing `rclone-python-0.1.6/rclone_python/utils.py` & `rclone-python-0.1.7/rclone_python/utils.py`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.6/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.7/rclone_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 A python wrapper for rclone that makes rclone's functionality usable in python.
 rclone needs to be installed on the system for the wrapper to work.
 
 ![demo gif](https://raw.githubusercontent.com/Johannes11833/rclone_python/master/demo/demo.gif)
 
 ## Features ⚒️
 
-- Copy and move files between remotes
+- Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
 - Create new remotes
 - Check available remotes
 
 ## Installation 💾
```

### Comparing `rclone-python-0.1.6/setup.py` & `rclone-python-0.1.7/setup.py`

 * *Files identical despite different names*

