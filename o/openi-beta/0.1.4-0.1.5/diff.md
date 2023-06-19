# Comparing `tmp/openi-beta-0.1.4.tar.gz` & `tmp/openi-beta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.4.tar", last modified: Mon Jun 19 02:01:05 2023, max compression
+gzip compressed data, was "openi-beta-0.1.5.tar", last modified: Mon Jun 19 07:43:27 2023, max compression
```

## Comparing `openi-beta-0.1.4.tar` & `openi-beta-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257845 openi-beta-0.1.4/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 02:01:05.257670 openi-beta-0.1.4/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-16 13:05:18.000000 openi-beta-0.1.4/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 02:01:05.257906 openi-beta-0.1.4/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-17 17:06:42.000000 openi-beta-0.1.4/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.254075 openi-beta-0.1.4/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.255104 openi-beta-0.1.4/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-16 13:05:18.000000 openi-beta-0.1.4/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 01:06:37.000000 openi-beta-0.1.4/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.255868 openi-beta-0.1.4/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.4/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    12433 2023-06-19 02:00:39.000000 openi-beta-0.1.4/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.256197 openi-beta-0.1.4/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-16 16:05:51.000000 openi-beta-0.1.4/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257194 openi-beta-0.1.4/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 02:01:05.000000 openi-beta-0.1.4/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 02:01:05.257344 openi-beta-0.1.4/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-16 13:05:18.000000 openi-beta-0.1.4/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.899548 openi-beta-0.1.5/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 07:43:27.899402 openi-beta-0.1.5/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-19 07:03:43.000000 openi-beta-0.1.5/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 07:43:27.899594 openi-beta-0.1.5/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-19 07:03:43.000000 openi-beta-0.1.5/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.896370 openi-beta-0.1.5/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.897131 openi-beta-0.1.5/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-19 07:03:43.000000 openi-beta-0.1.5/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 07:36:11.000000 openi-beta-0.1.5/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.897647 openi-beta-0.1.5/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.5/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    12392 2023-06-19 07:40:31.000000 openi-beta-0.1.5/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.898049 openi-beta-0.1.5/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-19 07:03:43.000000 openi-beta-0.1.5/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.898966 openi-beta-0.1.5/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 07:43:27.000000 openi-beta-0.1.5/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 07:43:27.000000 openi-beta-0.1.5/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 07:43:27.000000 openi-beta-0.1.5/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 07:43:27.000000 openi-beta-0.1.5/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 07:43:27.000000 openi-beta-0.1.5/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:43:27.899118 openi-beta-0.1.5/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-19 07:03:43.000000 openi-beta-0.1.5/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.4/PKG-INFO` & `openi-beta-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.4
+Version: 0.1.5
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.4/README.md` & `openi-beta-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.4/setup.py` & `openi-beta-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.4',
+    version='0.1.5',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.4/src/openi/dataset/dataset.py` & `openi-beta-0.1.5/src/openi/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,43 +137,42 @@
             "uuid": self.uuid
         }
 
         retry = 0
         while True:
             try:
                 x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
-                if x.status_code == 200:
-                    logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
-                    return x.json()["url"]
+                logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
+                return x.json()["url"]
             except:
                 logging.error(f'{x.url} {x} retry={retry+1} {x.reason}')
                 print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
-                retry += 1
-                time.sleep(1)
+            retry += 1
+            time.sleep(0.5)
         logging.error(f'reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
-            f'❌ reach max retry, getMultiUrl chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
+            f'❌ reach max retry {retry}, `getMultiUrl` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
 
     def putUpload(self, url, chunk_number, file_chunk_data):
         headers = {"Content-Type": "text/plain"} if self.upload_type == 0 else {}
 
         retry = 0
         while True:
             try:
                 x = requests.put(url, data=file_chunk_data, headers=headers)
                 logging.info(f'{x} {x.reason} {x.url} | etag: {x.headers["ETag"]}')
                 return x.headers["ETag"]
             except:
                 logging.error(f'{x.url} {x} retry={retry+1} {x.reason} | putUpload chunk [{chunk_number}] failed.')
                 print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
-                retry += 1
-                time.sleep(1)
+            retry += 1
+            time.sleep(0.5)
         logging.error(f'reach max retry, putUpload chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
-            f'❌ reach max retry, putUpload chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
+            f'❌ reach max retry {retry}, `putUpload` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
 
     def completeMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
```

### Comparing `openi-beta-0.1.4/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.5/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.4
+Version: 0.1.5
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.4/test/test_upload_multi.py` & `openi-beta-0.1.5/test/test_upload_multi.py`

 * *Files identical despite different names*

