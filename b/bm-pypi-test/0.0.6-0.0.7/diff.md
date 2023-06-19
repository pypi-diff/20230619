# Comparing `tmp/bm_pypi_test-0.0.6-py3-none-any.whl.zip` & `tmp/bm_pypi_test-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5811 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 09:31 bm_pypi_test-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2673 b- defN 23-Jun-19 09:31 bm_pypi_test-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 09:31 bm_pypi_test-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 09:31 bm_pypi_test-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 09:31 bm_pypi_test-0.0.6.dist-info/RECORD
-5 files, 14735 bytes uncompressed, 5041 bytes compressed:  65.8%
+Zip file size: 5754 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 09:35 bm_pypi_test-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2383 b- defN 23-Jun-19 09:35 bm_pypi_test-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 09:35 bm_pypi_test-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 09:35 bm_pypi_test-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 09:35 bm_pypi_test-0.0.7.dist-info/RECORD
+5 files, 14445 bytes uncompressed, 4984 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: bm_pypi_test-0.0.6.dist-info/LICENSE
+Filename: bm_pypi_test-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: bm_pypi_test-0.0.6.dist-info/METADATA
+Filename: bm_pypi_test-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: bm_pypi_test-0.0.6.dist-info/WHEEL
+Filename: bm_pypi_test-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: bm_pypi_test-0.0.6.dist-info/top_level.txt
+Filename: bm_pypi_test-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: bm_pypi_test-0.0.6.dist-info/RECORD
+Filename: bm_pypi_test-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bm_pypi_test-0.0.6.dist-info/LICENSE` & `bm_pypi_test-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bm_pypi_test-0.0.6.dist-info/METADATA` & `bm_pypi_test-0.0.7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-pypi-test
-Version: 0.0.6
+Version: 0.0.7
 Summary: Test
 Home-page: https://github.com/Only-bottle/pypi_test
 Author: ByeongmanLee
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,28 +24,28 @@
 
 <div align="center">
     <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/banner/pynp_main.png"/>
 </div>
 </br>
 
 
-<div align="center" style="justify-content:center;">
-    <a href="https://github.com/Nota-NetsPresso" style="text-decoration:none; margin-right:10px;">
+<div align="center">
+    <a href="https://github.com/Nota-NetsPresso">
         <img alt="github" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/github.png" width="3%">
     </a>
-    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.facebook.com/NotaAI" style="text-decoration:none; margin-right:10px;">
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.facebook.com/NotaAI">
         <img alt="facebook" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/facebook.png" width="3%">
     </a>
-    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://twitter.com/nota_ai" style="text-decoration:none; margin-right:10px;">
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://twitter.com/nota_ai">
         <img alt="twitter" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/twitter.png" width="3%">
     </a>
-    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.youtube.com/channel/UCeewYFAqb2EqwEXZCfH9DVQ" style="text-decoration:none; margin-right:10px;">
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.youtube.com/channel/UCeewYFAqb2EqwEXZCfH9DVQ">
         <img alt="youtube" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/youtube.png" width="3%">
     </a>
-    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%" alt="" />
-    <a href="https://www.linkedin.com/company/nota-incorporated" style="text-decoration:none;">
+    <img src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-transparent.png" width="3%"/>
+    <a href="https://www.linkedin.com/company/nota-incorporated">
         <img alt="youtube" src="https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/linkedin.png" width="3%">
     </a>
 </div>
```

### html2text {}

```diff
@@ -1,13 +1,18 @@
-Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.6 Summary: Test Home-
+Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.7 Summary: Test Home-
 page: https://github.com/Only-bottle/pypi_test Author: ByeongmanLee Author-
 email: bmlee@nota.ai Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: loguru (==0.7.0) Requires-
 Dist: urllib3 (==2.0.2) Requires-Dist: PyJWT (==2.7.0) Requires-Dist: pydantic
 (==1.10.4) Requires-Dist: requests (==2.30.0) Requires-Dist: email-validator
 (==2.0.0) Requires-Dist: pytz (==2023.3) Requires-Dist: typing-extensions
 (==4.5.0) # pypi_test
   [https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/banner/
                                 pynp_main.png]
-             [github]  [facebook]  [twitter]  [youtube]  [youtube]
+ [github] [https://netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/
+ common/logo-transparent.png] [facebook] [https://netspresso-docs-imgs.s3.ap-
+northeast-2.amazonaws.com/imgs/common/logo-transparent.png] [twitter] [https://
+    netspresso-docs-imgs.s3.ap-northeast-2.amazonaws.com/imgs/common/logo-
+   transparent.png] [youtube] [https://netspresso-docs-imgs.s3.ap-northeast-
+          2.amazonaws.com/imgs/common/logo-transparent.png] [youtube]
```

