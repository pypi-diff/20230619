# Comparing `tmp/openi-beta-0.1.6.tar.gz` & `tmp/openi-beta-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.6.tar", last modified: Mon Jun 19 07:53:05 2023, max compression
+gzip compressed data, was "openi-beta-0.1.7.tar", last modified: Mon Jun 19 08:02:55 2023, max compression
```

## Comparing `openi-beta-0.1.6.tar` & `openi-beta-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.437321 openi-beta-0.1.6/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 07:53:05.437167 openi-beta-0.1.6/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-19 07:48:49.000000 openi-beta-0.1.6/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 07:53:05.437380 openi-beta-0.1.6/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-19 07:53:03.000000 openi-beta-0.1.6/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.434768 openi-beta-0.1.6/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.435514 openi-beta-0.1.6/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-19 07:48:49.000000 openi-beta-0.1.6/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 07:48:49.000000 openi-beta-0.1.6/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.435814 openi-beta-0.1.6/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.6/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    12384 2023-06-19 07:52:05.000000 openi-beta-0.1.6/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.435959 openi-beta-0.1.6/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-19 07:48:49.000000 openi-beta-0.1.6/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.436664 openi-beta-0.1.6/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 07:53:05.000000 openi-beta-0.1.6/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 07:53:05.000000 openi-beta-0.1.6/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 07:53:05.000000 openi-beta-0.1.6/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 07:53:05.000000 openi-beta-0.1.6/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 07:53:05.000000 openi-beta-0.1.6/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 07:53:05.436818 openi-beta-0.1.6/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-19 07:48:49.000000 openi-beta-0.1.6/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.457109 openi-beta-0.1.7/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 08:02:55.456969 openi-beta-0.1.7/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-19 07:48:49.000000 openi-beta-0.1.7/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 08:02:55.457164 openi-beta-0.1.7/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-19 08:02:50.000000 openi-beta-0.1.7/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.454261 openi-beta-0.1.7/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455076 openi-beta-0.1.7/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455564 openi-beta-0.1.7/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.7/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    12807 2023-06-19 08:01:59.000000 openi-beta-0.1.7/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455812 openi-beta-0.1.7/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.456565 openi-beta-0.1.7/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.456710 openi-beta-0.1.7/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-19 07:48:49.000000 openi-beta-0.1.7/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.6/PKG-INFO` & `openi-beta-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.6
+Version: 0.1.7
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.6/README.md` & `openi-beta-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.6/setup.py` & `openi-beta-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.6',
+    version='0.1.7',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.6/src/openi/dataset/dataset.py` & `openi-beta-0.1.7/src/openi/dataset/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -139,15 +139,18 @@
 
         retry = 0
         while retry < 3:
             try:
                 x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
                 logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
                 return x.json()["url"]
-            except:
+            except ConnectionError:
+                logging.error(f'getMultiUrl chunk [{chunk_number}], retry={retry+1} ')
+                print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
+            except RuntimeError:
                 logging.error(f'getMultiUrl chunk [{chunk_number}], retry={retry+1} ')
                 print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
             retry += 1
             time.sleep(0.5)
         logging.error(f'reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
             f'❌ reach max retry {retry}, `getMultiUrl` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
@@ -157,15 +160,18 @@
 
         retry = 0
         while retry < 3:
             try:
                 x = requests.put(url, data=file_chunk_data, headers=headers)
                 logging.info(f'{x} {x.reason} {x.url} | etag: {x.headers["ETag"]}')
                 return x.headers["ETag"]
-            except:
+            except ConnectionError:
+                logging.error(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+                print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+            except RuntimeError:
                 logging.error(f'putUpload chunk [{chunk_number}], retry={retry+1}')
                 print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
             retry += 1
             time.sleep(0.5)
         logging.error(f'reach max retry, putUpload chunk [{chunk_number}] failed.')
         raise ConnectionRefusedError(
             f'❌ reach max retry {retry}, `putUpload` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
```

### Comparing `openi-beta-0.1.6/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.7/src/openi_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.6
+Version: 0.1.7
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.6/test/test_upload_multi.py` & `openi-beta-0.1.7/test/test_upload_multi.py`

 * *Files identical despite different names*

