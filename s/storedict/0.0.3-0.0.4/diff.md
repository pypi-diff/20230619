# Comparing `tmp/storedict-0.0.3-py3-none-any.whl.zip` & `tmp/storedict-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3264 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       59 b- defN 23-Apr-30 22:10 storedict/__init__.py
+Zip file size: 3267 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jun-19 13:30 storedict/__init__.py
 -rw-rw-r--  2.0 unx     5573 b- defN 23-Apr-30 22:07 storedict/storedict.py
 -rw-rw-r--  2.0 unx     2864 b- defN 23-Apr-30 21:29 storedict/tests.py
--rw-rw-r--  2.0 unx      239 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      535 b- defN 23-Apr-30 22:10 storedict-0.0.3.dist-info/RECORD
-7 files, 9372 bytes uncompressed, 2316 bytes compressed:  75.3%
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-19 13:30 storedict-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 13:30 storedict-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-19 13:30 storedict-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      535 b- defN 23-Jun-19 13:30 storedict-0.0.4.dist-info/RECORD
+7 files, 9372 bytes uncompressed, 2319 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: storedict/storedict.py
 Comment: 
 
 Filename: storedict/tests.py
 Comment: 
 
-Filename: storedict-0.0.3.dist-info/METADATA
+Filename: storedict-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: storedict-0.0.3.dist-info/WHEEL
+Filename: storedict-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: storedict-0.0.3.dist-info/top_level.txt
+Filename: storedict-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: storedict-0.0.3.dist-info/RECORD
+Filename: storedict-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## storedict/__init__.py

```diff
@@ -1,3 +1,3 @@
 from .storedict import create_store
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

