# Comparing `tmp/cryption-0.3.0-py3-none-any.whl.zip` & `tmp/cryption-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 14224 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1078 b- defN 21-Oct-08 21:36 cryption/__init__.py
--rw-r--r--  2.0 unx    35129 b- defN 21-Oct-08 21:37 cryption-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1250 b- defN 21-Oct-08 21:37 cryption-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-08 21:37 cryption-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Oct-08 21:37 cryption-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      468 b- defN 21-Oct-08 21:37 cryption-0.3.0.dist-info/RECORD
-6 files, 38026 bytes uncompressed, 13378 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     1078 b- defN 23-Jun-19 09:06 cryption/__init__.py
+-rw-r--r--  2.0 unx    35129 b- defN 23-Jun-19 09:06 cryption-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1248 b- defN 23-Jun-19 09:06 cryption-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 09:06 cryption-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-19 09:06 cryption-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      468 b- defN 23-Jun-19 09:06 cryption-0.4.0.dist-info/RECORD
+6 files, 38024 bytes uncompressed, 13378 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: cryption/__init__.py
 Comment: 
 
-Filename: cryption-0.3.0.dist-info/LICENSE
+Filename: cryption-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: cryption-0.3.0.dist-info/METADATA
+Filename: cryption-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: cryption-0.3.0.dist-info/WHEEL
+Filename: cryption-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: cryption-0.3.0.dist-info/top_level.txt
+Filename: cryption-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cryption-0.3.0.dist-info/RECORD
+Filename: cryption-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cryption-0.3.0.dist-info/LICENSE` & `cryption-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cryption-0.3.0.dist-info/METADATA` & `cryption-0.4.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryption
-Version: 0.3.0
+Version: 0.4.0
 Summary: Wrapper for Pycrptodome to encrypt/decrypt text
 Home-page: https://github.com/Pycryptor10/cryption
 Author: Pycryptor10
 Author-email: Pycryptor10@gmail.com
 Maintainer: Pycryptor10
 Maintainer-email: Pycryptor10@gmail.com
 License: GPL3
@@ -27,9 +27,7 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome (==3.11.0)
 
 # cryption
  Wrapper for Pycrptodome to encrypt/decrypt text
-
-
```

