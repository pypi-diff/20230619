# Comparing `tmp/bm_pypi_test-0.0.4-py3-none-any.whl.zip` & `tmp/bm_pypi_test-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5781 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 09:15 bm_pypi_test-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2565 b- defN 23-Jun-19 09:15 bm_pypi_test-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 09:15 bm_pypi_test-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 09:15 bm_pypi_test-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 09:15 bm_pypi_test-0.0.4.dist-info/RECORD
-5 files, 14627 bytes uncompressed, 5011 bytes compressed:  65.7%
+Zip file size: 5777 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 09:17 bm_pypi_test-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2572 b- defN 23-Jun-19 09:17 bm_pypi_test-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 09:17 bm_pypi_test-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 09:17 bm_pypi_test-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 09:17 bm_pypi_test-0.0.5.dist-info/RECORD
+5 files, 14634 bytes uncompressed, 5007 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: bm_pypi_test-0.0.4.dist-info/LICENSE
+Filename: bm_pypi_test-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: bm_pypi_test-0.0.4.dist-info/METADATA
+Filename: bm_pypi_test-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: bm_pypi_test-0.0.4.dist-info/WHEEL
+Filename: bm_pypi_test-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: bm_pypi_test-0.0.4.dist-info/top_level.txt
+Filename: bm_pypi_test-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: bm_pypi_test-0.0.4.dist-info/RECORD
+Filename: bm_pypi_test-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bm_pypi_test-0.0.4.dist-info/LICENSE` & `bm_pypi_test-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bm_pypi_test-0.0.4.dist-info/METADATA` & `bm_pypi_test-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-pypi-test
-Version: 0.0.4
+Version: 0.0.5
 Summary: Test
 Home-page: https://github.com/Only-bottle/pypi_test
 Author: ByeongmanLee
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,15 @@
 Requires-Dist: typing-extensions (==4.5.0)
 
 # pypi_test
 
 <div align="center">
     <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/banner/pynp_main.png"/>
 </div>
+</br>
 
 
 <div align="center">
     <a href="https://github.com/Nota-NetsPresso" style="text-decoration:none;">
         <img alt="github" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/github.png" width="3%">
     </a>
     <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%" alt="" />
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.4 Summary: Test Home-
+Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.5 Summary: Test Home-
 page: https://github.com/Only-bottle/pypi_test Author: ByeongmanLee Author-
 email: bmlee@nota.ai Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: loguru (==0.7.0) Requires-
 Dist: urllib3 (==2.0.2) Requires-Dist: PyJWT (==2.7.0) Requires-Dist: pydantic
 (==1.10.4) Requires-Dist: requests (==2.30.0) Requires-Dist: email-validator
```

