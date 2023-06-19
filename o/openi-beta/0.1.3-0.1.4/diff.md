# Comparing `tmp/openi-beta-0.1.3.tar.gz` & `tmp/openi-beta-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.3.tar", last modified: Sat Jun 17 05:12:08 2023, max compression
+gzip compressed data, was "openi-beta-0.1.4.tar", last modified: Mon Jun 19 02:01:05 2023, max compression
```

## Comparing `openi-beta-0.1.3.tar` & `openi-beta-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418805 openi-beta-0.1.3/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-17 05:12:08.418604 openi-beta-0.1.3/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 13:05:18.000000 openi-beta-0.1.3/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-17 05:12:08.419400 openi-beta-0.1.3/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-17 05:11:58.000000 openi-beta-0.1.3/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.415353 openi-beta-0.1.3/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.416193 openi-beta-0.1.3/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 13:05:18.000000 openi-beta-0.1.3/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      357 2023-06-16 17:19:00.000000 openi-beta-0.1.3/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.416791 openi-beta-0.1.3/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.3/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    13175 2023-06-17 03:46:26.000000 openi-beta-0.1.3/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.417088 openi-beta-0.1.3/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-16 16:05:51.000000 openi-beta-0.1.3/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418098 openi-beta-0.1.3/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-17 05:12:08.000000 openi-beta-0.1.3/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-17 05:12:08.418241 openi-beta-0.1.3/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 13:05:18.000000 openi-beta-0.1.3/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257845 openi-beta-0.1.4/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 02:01:05.257670 openi-beta-0.1.4/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 13:05:18.000000 openi-beta-0.1.4/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 02:01:05.257906 openi-beta-0.1.4/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-17 17:06:42.000000 openi-beta-0.1.4/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.254075 openi-beta-0.1.4/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.255104 openi-beta-0.1.4/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 13:05:18.000000 openi-beta-0.1.4/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 01:06:37.000000 openi-beta-0.1.4/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.255868 openi-beta-0.1.4/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.4/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    12433 2023-06-19 02:00:39.000000 openi-beta-0.1.4/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.256197 openi-beta-0.1.4/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-16 16:05:51.000000 openi-beta-0.1.4/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257194 openi-beta-0.1.4/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257344 openi-beta-0.1.4/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 13:05:18.000000 openi-beta-0.1.4/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.3/PKG-INFO` & `openi-beta-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.3
+Version: 0.1.4
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.3/README.md` & `openi-beta-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.3/setup.py` & `openi-beta-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.3',
+    version='0.1.4',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.3/src/openi/dataset/dataset.py` & `openi-beta-0.1.4/src/openi/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import math
 import requests
 import hashlib
 from tqdm import tqdm
-from collections import OrderedDict
+import time
 from datetime import datetime
 from ..constants import *
 
 import logging
 from openi.utils.logger import setup_logging
 setup_logging()
 
@@ -32,15 +32,14 @@
         self.username = username
         self.repo = repository
         self.token = token
         self.cluster = cluster
         self.app_url = app_url
 
         # preset variables
-        # self.max_chunk_size = MAX_CHUNK_SIZE
         if cluster == "NPU":
             self.upload_type = 1
         elif cluster == "GPU":
             self.upload_type = 0
         else:
             raise ValueError(
                 f"❌ please enter a valid cluster name, 'GPU' or 'NPU'")
@@ -135,45 +134,46 @@
             "chunkNumber": chunk_number,
             "size": chunk_size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
 
         retry = 0
-        while retry < 3:
+        while True:
             try:
                 x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
                 if x.status_code == 200:
                     logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
                     return x.json()["url"]
             except:
                 logging.error(f'{x.url} {x} retry={retry+1} {x.reason}')
                 print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
                 retry += 1
-        logging.error(f'{x.url} {x} {x.reason} | reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
+                time.sleep(1)
+        logging.error(f'reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
-            f'❌ <{x.status_code} {x.reason}> | getMultiUrl chunk [{chunk_number}] failed.')
+            f'❌ reach max retry, getMultiUrl chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
 
     def putUpload(self, url, chunk_number, file_chunk_data):
         headers = {"Content-Type": "text/plain"} if self.upload_type == 0 else {}
 
         retry = 0
-        while retry < 3:
+        while True:
             try:
                 x = requests.put(url, data=file_chunk_data, headers=headers)
                 logging.info(f'{x} {x.reason} {x.url} | etag: {x.headers["ETag"]}')
                 return x.headers["ETag"]
             except:
                 logging.error(f'{x.url} {x} retry={retry+1} {x.reason} | putUpload chunk [{chunk_number}] failed.')
                 print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
                 retry += 1
-
-        logging.error(f'{x.url} {x} {x.reason} | reach max retry, putUpload chunk [{chunk_number}] failed.')
+                time.sleep(1)
+        logging.error(f'reach max retry, putUpload chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
-            f'❌ <{x.status_code} {x.reason}> | upload chunk [{chunk_number}] failed.')
+            f'❌ reach max retry, putUpload chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
 
     def completeMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
@@ -193,15 +193,14 @@
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
     """
     utils functions
     """
 
     def get_time(self, message=""):
         return datetime.now().strftime("%H:%M:%S")
-        #return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
 
     def filePreprocess(self):
         self.getDatasetID()
         if self.size == 0:
             logging.error(f'[{self.filename}] File size is 0 | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size is 0')
@@ -273,22 +272,14 @@
         #upload starts
         if self.uuid != '':
             if self.uploaded:
                 logging.error(f'Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. | FileObject: {self.__dict__}')
                 raise ValueError(
                     f'❌ Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. ')
             else:
-                # uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
-                # continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
-                # re-upload last chunk from checkpoint
-                # if uploaded_chunks:
-                #     last_chunk_index = max(uploaded_chunks)
-                #     continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
-                # continue_chunks = OrderedDict(sorted(continue_chunks.items()))
-                # uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 uploaded_chunks = sorted(uploaded_chunks)[:-1]
                 continue_chunks = [i for i in range(1, self.total_chunk_counts+1) if i not in uploaded_chunks]
                 continue_chunks = sorted(continue_chunks)
                 self.uploadProgressBar(continue_chunks)
 
         else:
         #if not self.uploaded:
```

### Comparing `openi-beta-0.1.3/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.4/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.3
+Version: 0.1.4
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.3/test/test_upload_multi.py` & `openi-beta-0.1.4/test/test_upload_multi.py`

 * *Files identical despite different names*

