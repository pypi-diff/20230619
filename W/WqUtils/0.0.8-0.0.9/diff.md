# Comparing `tmp/WqUtils-0.0.8-py3-none-any.whl.zip` & `tmp/WqUtils-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6212 bytes, number of entries: 8
+Zip file size: 6242 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
--rw-r--r--  2.0 unx      250 b- defN 22-Nov-25 08:56 WqUtils/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Jun-19 15:50 WqUtils/__init__.py
 -rw-r--r--  2.0 unx     6493 b- defN 23-Jun-19 15:19 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 15:46 WqUtils-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 15:46 WqUtils-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 15:46 WqUtils-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      617 b- defN 23-Jun-19 15:46 WqUtils-0.0.8.dist-info/RECORD
-8 files, 13268 bytes uncompressed, 5136 bytes compressed:  61.3%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 15:50 WqUtils-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 15:50 WqUtils-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 15:50 WqUtils-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      617 b- defN 23-Jun-19 15:50 WqUtils-0.0.9.dist-info/RECORD
+8 files, 13309 bytes uncompressed, 5166 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: WqUtils/DB_Utils/SqlServer_DB.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.0.8.dist-info/METADATA
+Filename: WqUtils-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.0.8.dist-info/WHEEL
+Filename: WqUtils-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.0.8.dist-info/top_level.txt
+Filename: WqUtils-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.0.8.dist-info/RECORD
+Filename: WqUtils-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/__init__.py

```diff
@@ -5,7 +5,8 @@
 @ Date: 2022-11-25 16:55
 @ Email: stephen.wan@colourdata.com.cn
 @ LastEditors: stephen.wan
 @ LastEditTime: 2022-11-25 16:55
 @ ProjectName: model_testing
 @ Description: to do
 """
+from DB_Utils.SqlServer_DB import ExecSql
```

