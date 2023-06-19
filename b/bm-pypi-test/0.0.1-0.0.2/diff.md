# Comparing `tmp/bm_pypi_test-0.0.1-py3-none-any.whl.zip` & `tmp/bm_pypi_test-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5816 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 08:48 bm_pypi_test-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3049 b- defN 23-Jun-19 08:48 bm_pypi_test-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 08:48 bm_pypi_test-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 08:48 bm_pypi_test-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 08:48 bm_pypi_test-0.0.1.dist-info/RECORD
-5 files, 15111 bytes uncompressed, 5046 bytes compressed:  66.6%
+Zip file size: 5818 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 08:54 bm_pypi_test-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3087 b- defN 23-Jun-19 08:54 bm_pypi_test-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 08:54 bm_pypi_test-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-19 08:54 bm_pypi_test-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      411 b- defN 23-Jun-19 08:54 bm_pypi_test-0.0.2.dist-info/RECORD
+5 files, 15149 bytes uncompressed, 5048 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: bm_pypi_test-0.0.1.dist-info/LICENSE
+Filename: bm_pypi_test-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: bm_pypi_test-0.0.1.dist-info/METADATA
+Filename: bm_pypi_test-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bm_pypi_test-0.0.1.dist-info/WHEEL
+Filename: bm_pypi_test-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bm_pypi_test-0.0.1.dist-info/top_level.txt
+Filename: bm_pypi_test-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bm_pypi_test-0.0.1.dist-info/RECORD
+Filename: bm_pypi_test-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bm_pypi_test-0.0.1.dist-info/LICENSE` & `bm_pypi_test-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bm_pypi_test-0.0.1.dist-info/METADATA` & `bm_pypi_test-0.0.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-pypi-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: Test
 Home-page: https://github.com/Only-bottle/pypi_test
 Author: ByeongmanLee
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,46 +21,46 @@
 Requires-Dist: typing-extensions (==4.5.0)
 
 # pypi_test
 
 <div align="center">
     <a href="https://github.com/Nota-NetsPresso" style="text-decoration:none;">
         <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/github_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/github.png">
-            <img alt="github" src="imgs/common/github.png" width="3%">
+            <source media="(prefers-color-scheme: dark)" srcset="./imgs/common/github_white.png">
+            <source media="(prefers-color-scheme: light)" srcset="./imgs/common/github.png">
+            <img alt="github" src="./imgs/common/github.png" width="3%">
         </picture>
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
+    <img src="./imgs/common/logo-transparent.png" width="3%" alt="" />
     <a href="https://www.facebook.com/NotaAI" style="text-decoration:none;">
         <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/facebook_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/facebook.png">
-            <img alt="facebook" src="imgs/common/facebook.png" width="3%">
+            <source media="(prefers-color-scheme: dark)" srcset="./imgs/common/facebook_white.png">
+            <source media="(prefers-color-scheme: light)" srcset="./imgs/common/facebook.png">
+            <img alt="facebook" src="./imgs/common/facebook.png" width="3%">
         </picture>
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
+    <img src="./imgs/common/logo-transparent.png" width="3%" alt="" />
     <a href="https://twitter.com/nota_ai" style="text-decoration:none;">
         <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/twitter_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/twitter.png">
-            <img alt="twitter" src="imgs/common/twitter.png" width="3%">
+            <source media="(prefers-color-scheme: dark)" srcset="./imgs/common/twitter_white.png">
+            <source media="(prefers-color-scheme: light)" srcset="./imgs/common/twitter.png">
+            <img alt="twitter" src="./imgs/common/twitter.png" width="3%">
         </picture>
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
+    <img src="./imgs/common/logo-transparent.png" width="3%" alt="" />
     <a href="https://www.youtube.com/channel/UCeewYFAqb2EqwEXZCfH9DVQ" style="text-decoration:none;">
         <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/youtube_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/youtube.png">
-            <img alt="youtube" src="imgs/common/youtube.png" width="3%">
+            <source media="(prefers-color-scheme: dark)" srcset="./imgs/common/youtube_white.png">
+            <source media="(prefers-color-scheme: light)" srcset="./imgs/common/youtube.png">
+            <img alt="youtube" src="./imgs/common/youtube.png" width="3%">
         </picture>
     </a>
-    <img src="imgs/common/logo-transparent.png" width="3%" alt="" />
+    <img src="./imgs/common/logo-transparent.png" width="3%" alt="" />
     <a href="https://www.linkedin.com/company/nota-incorporated" style="text-decoration:none;">
         <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="imgs/common/linkedin_white.png">
-            <source media="(prefers-color-scheme: light)" srcset="imgs/common/linkedin.png">
-            <img alt="youtube" src="imgs/common/linkedin.png" width="3%">
+            <source media="(prefers-color-scheme: dark)" srcset="./imgs/common/linkedin_white.png">
+            <source media="(prefers-color-scheme: light)" srcset="./imgs/common/linkedin.png">
+            <img alt="youtube" src="./imgs/common/linkedin.png" width="3%">
         </picture>
     </a>
 </div>
 </br>
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.1 Summary: Test Home-
+Metadata-Version: 2.1 Name: bm-pypi-test Version: 0.0.2 Summary: Test Home-
 page: https://github.com/Only-bottle/pypi_test Author: ByeongmanLee Author-
 email: bmlee@nota.ai Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: loguru (==0.7.0) Requires-
 Dist: urllib3 (==2.0.2) Requires-Dist: PyJWT (==2.7.0) Requires-Dist: pydantic
 (==1.10.4) Requires-Dist: requests (==2.30.0) Requires-Dist: email-validator
```

