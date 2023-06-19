# Comparing `tmp/fs-s3fs-forked-1.1.2.tar.gz` & `tmp/fs-s3fs-forked-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs-s3fs-forked-1.1.2.tar", last modified: Fri May 26 12:58:12 2023, max compression
+gzip compressed data, was "fs-s3fs-forked-1.1.3.tar", last modified: Mon Jun 19 07:58:43 2023, max compression
```

## Comparing `fs-s3fs-forked-1.1.2.tar` & `fs-s3fs-forked-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-05-26 12:58:12.116824 fs-s3fs-forked-1.1.2/
--rw-r--r--   0 antoine   (1001) antoine   (1001)     1069 2023-01-04 13:51:58.000000 fs-s3fs-forked-1.1.2/LICENSE
--rw-r--r--   0 antoine   (1001) antoine   (1001)     4242 2023-05-26 12:58:12.116824 fs-s3fs-forked-1.1.2/PKG-INFO
--rw-r--r--   0 antoine   (1001) antoine   (1001)     3314 2023-05-26 12:58:11.000000 fs-s3fs-forked-1.1.2/README.rst
-drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-05-26 12:58:12.116824 fs-s3fs-forked-1.1.2/fs_s3fs/
--rw-r--r--   0 antoine   (1001) antoine   (1001)       58 2023-01-04 13:51:58.000000 fs-s3fs-forked-1.1.2/fs_s3fs/__init__.py
--rw-r--r--   0 antoine   (1001) antoine   (1001)    27823 2023-05-26 12:39:19.000000 fs-s3fs-forked-1.1.2/fs_s3fs/_s3fs.py
--rw-r--r--   0 antoine   (1001) antoine   (1001)       22 2023-05-26 12:39:30.000000 fs-s3fs-forked-1.1.2/fs_s3fs/_version.py
--rw-r--r--   0 antoine   (1001) antoine   (1001)     1258 2023-01-04 13:53:06.000000 fs-s3fs-forked-1.1.2/fs_s3fs/opener.py
-drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-05-26 12:58:12.116824 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/
--rw-r--r--   0 antoine   (1001) antoine   (1001)     4242 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/PKG-INFO
--rw-r--r--   0 antoine   (1001) antoine   (1001)      342 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/SOURCES.txt
--rw-r--r--   0 antoine   (1001) antoine   (1001)        1 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/dependency_links.txt
--rw-r--r--   0 antoine   (1001) antoine   (1001)       43 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/entry_points.txt
--rw-r--r--   0 antoine   (1001) antoine   (1001)       29 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/requires.txt
--rw-r--r--   0 antoine   (1001) antoine   (1001)        8 2023-05-26 12:58:12.000000 fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/top_level.txt
--rw-r--r--   0 antoine   (1001) antoine   (1001)       83 2023-05-26 12:58:12.116824 fs-s3fs-forked-1.1.2/setup.cfg
--rw-r--r--   0 antoine   (1001) antoine   (1001)     1393 2023-05-26 12:39:30.000000 fs-s3fs-forked-1.1.2/setup.py
+drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-06-19 07:58:43.546620 fs-s3fs-forked-1.1.3/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     1069 2023-01-04 13:51:58.000000 fs-s3fs-forked-1.1.3/LICENSE
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     4413 2023-06-19 07:58:43.546620 fs-s3fs-forked-1.1.3/PKG-INFO
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     3485 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/README.rst
+drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-06-19 07:58:43.546620 fs-s3fs-forked-1.1.3/fs_s3fs/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)       58 2023-01-04 13:51:58.000000 fs-s3fs-forked-1.1.3/fs_s3fs/__init__.py
+-rw-r--r--   0 antoine   (1001) antoine   (1001)    27906 2023-06-19 06:55:28.000000 fs-s3fs-forked-1.1.3/fs_s3fs/_s3fs.py
+-rw-r--r--   0 antoine   (1001) antoine   (1001)       22 2023-06-19 06:55:28.000000 fs-s3fs-forked-1.1.3/fs_s3fs/_version.py
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     1258 2023-01-04 13:53:06.000000 fs-s3fs-forked-1.1.3/fs_s3fs/opener.py
+drwxr-xr-x   0 antoine   (1001) antoine   (1001)        0 2023-06-19 07:58:43.546620 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     4413 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/PKG-INFO
+-rw-r--r--   0 antoine   (1001) antoine   (1001)      342 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine   (1001) antoine   (1001)        1 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine   (1001) antoine   (1001)       43 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/entry_points.txt
+-rw-r--r--   0 antoine   (1001) antoine   (1001)       29 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/requires.txt
+-rw-r--r--   0 antoine   (1001) antoine   (1001)        8 2023-06-19 07:58:43.000000 fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/top_level.txt
+-rw-r--r--   0 antoine   (1001) antoine   (1001)       83 2023-06-19 07:58:43.546620 fs-s3fs-forked-1.1.3/setup.cfg
+-rw-r--r--   0 antoine   (1001) antoine   (1001)     1393 2023-06-16 15:55:02.000000 fs-s3fs-forked-1.1.3/setup.py
```

### Comparing `fs-s3fs-forked-1.1.2/LICENSE` & `fs-s3fs-forked-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fs-s3fs-forked-1.1.2/PKG-INFO` & `fs-s3fs-forked-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-s3fs-forked
-Version: 1.1.2
+Version: 1.1.3
 Summary: Amazon S3 filesystem for PyFilesystem2, forked from https://github.com/PyFilesystem/s3fs
 Home-page: https://gitlab.com/geovisio/infra/s3fs
 Author: Antoine Desbordes
 Author-email: antoine.desbordes@gmail.com
 License: MIT
 Keywords: pyfilesystem,Amazon,s3
 Platform: any
@@ -22,15 +22,16 @@
 Classifier: Topic :: System :: Filesystems
 License-File: LICENSE
 
 Forked from https://github.com/PyFilesystem/s3fs/
 =================================================
 
 -  to be able to set the endpoint in the url
--  to be able to skip to directory creation to improve performance
+-  to be able to skip to directory creation/removal to improve
+   performance
 
 S3FS
 ====
 
 S3FS is a `PyFilesystem <https://www.pyfilesystem.org/>`__ interface to
 Amazon S3 cloud storage.
 
@@ -137,7 +138,15 @@
 Documentation
 -------------
 
 -  `PyFilesystem Wiki <https://www.pyfilesystem.org>`__
 -  `S3FS Reference <http://fs-s3fs.readthedocs.io/en/latest/>`__
 -  `PyFilesystem
    Reference <https://docs.pyfilesystem.org/en/latest/reference/base.html>`__
+
+Releasing
+---------
+
+-  Update version number in \_version.py
+-  install build dependencies: ``pip install wheel twine``
+-  install pandoc
+-  ``make release``
```

### Comparing `fs-s3fs-forked-1.1.2/README.rst` & `fs-s3fs-forked-1.1.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Forked from https://github.com/PyFilesystem/s3fs/
 =================================================
 
 -  to be able to set the endpoint in the url
--  to be able to skip to directory creation to improve performance
+-  to be able to skip to directory creation/removal to improve
+   performance
 
 S3FS
 ====
 
 S3FS is a `PyFilesystem <https://www.pyfilesystem.org/>`__ interface to
 Amazon S3 cloud storage.
 
@@ -113,7 +114,15 @@
 Documentation
 -------------
 
 -  `PyFilesystem Wiki <https://www.pyfilesystem.org>`__
 -  `S3FS Reference <http://fs-s3fs.readthedocs.io/en/latest/>`__
 -  `PyFilesystem
    Reference <https://docs.pyfilesystem.org/en/latest/reference/base.html>`__
+
+Releasing
+---------
+
+-  Update version number in \_version.py
+-  install build dependencies: ``pip install wheel twine``
+-  install pandoc
+-  ``make release``
```

### Comparing `fs-s3fs-forked-1.1.2/fs_s3fs/_s3fs.py` & `fs-s3fs-forked-1.1.3/fs_s3fs/_s3fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,14 +641,16 @@
         contents = response.get("Contents", ())
         for obj in contents:
             if obj["Key"] != _key:
                 return False
         return True
 
     def removedir(self, path):
+        if not self.strict:
+            return
         self.check()
         _path = self.validatepath(path)
         if _path == "/":
             raise errors.RemoveRootError()
         info = self.getinfo(_path)
         if not info.is_dir:
             raise errors.DirectoryExpected(path)
@@ -703,17 +705,18 @@
 
     def scandir(self, path, namespaces=None, page=None):
         _path = self.validatepath(path)
         namespaces = namespaces or ()
         _s3_key = self._path_to_dir_key(_path)
         prefix_len = len(_s3_key)
 
-        info = self.getinfo(path)
-        if not info.is_dir:
-            raise errors.DirectoryExpected(path)
+        if self.strict:
+            info = self.getinfo(path)
+            if not info.is_dir:
+                raise errors.DirectoryExpected(path)
 
         paginator = self.client.get_paginator("list_objects")
         _paginate = paginator.paginate(
             Bucket=self._bucket_name, Prefix=_s3_key, Delimiter=self.delimiter
         )
 
         def gen_info():
```

### Comparing `fs-s3fs-forked-1.1.2/fs_s3fs/opener.py` & `fs-s3fs-forked-1.1.3/fs_s3fs/opener.py`

 * *Files identical despite different names*

### Comparing `fs-s3fs-forked-1.1.2/fs_s3fs_forked.egg-info/PKG-INFO` & `fs-s3fs-forked-1.1.3/fs_s3fs_forked.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-s3fs-forked
-Version: 1.1.2
+Version: 1.1.3
 Summary: Amazon S3 filesystem for PyFilesystem2, forked from https://github.com/PyFilesystem/s3fs
 Home-page: https://gitlab.com/geovisio/infra/s3fs
 Author: Antoine Desbordes
 Author-email: antoine.desbordes@gmail.com
 License: MIT
 Keywords: pyfilesystem,Amazon,s3
 Platform: any
@@ -22,15 +22,16 @@
 Classifier: Topic :: System :: Filesystems
 License-File: LICENSE
 
 Forked from https://github.com/PyFilesystem/s3fs/
 =================================================
 
 -  to be able to set the endpoint in the url
--  to be able to skip to directory creation to improve performance
+-  to be able to skip to directory creation/removal to improve
+   performance
 
 S3FS
 ====
 
 S3FS is a `PyFilesystem <https://www.pyfilesystem.org/>`__ interface to
 Amazon S3 cloud storage.
 
@@ -137,7 +138,15 @@
 Documentation
 -------------
 
 -  `PyFilesystem Wiki <https://www.pyfilesystem.org>`__
 -  `S3FS Reference <http://fs-s3fs.readthedocs.io/en/latest/>`__
 -  `PyFilesystem
    Reference <https://docs.pyfilesystem.org/en/latest/reference/base.html>`__
+
+Releasing
+---------
+
+-  Update version number in \_version.py
+-  install build dependencies: ``pip install wheel twine``
+-  install pandoc
+-  ``make release``
```

### Comparing `fs-s3fs-forked-1.1.2/setup.py` & `fs-s3fs-forked-1.1.3/setup.py`

 * *Files identical despite different names*

