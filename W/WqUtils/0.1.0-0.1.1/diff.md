# Comparing `tmp/WqUtils-0.1.0-py3-none-any.whl.zip` & `tmp/WqUtils-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 6245 bytes, number of entries: 8
+Zip file size: 6638 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Jun-19 15:54 WqUtils/__init__.py
 -rw-r--r--  2.0 unx     6493 b- defN 23-Jun-19 15:19 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 15:54 WqUtils-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 15:54 WqUtils-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 15:54 WqUtils-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      617 b- defN 23-Jun-19 15:54 WqUtils-0.1.0.dist-info/RECORD
-8 files, 13310 bytes uncompressed, 5169 bytes compressed:  61.2%
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-19 07:32 WqUtils/DB_Utils/db_config.toml
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      704 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/RECORD
+9 files, 13652 bytes uncompressed, 5424 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: WqUtils/DB_Utils/SqlServer_DB.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
-Filename: WqUtils-0.1.0.dist-info/METADATA
+Filename: WqUtils/DB_Utils/db_config.toml
 Comment: 
 
-Filename: WqUtils-0.1.0.dist-info/WHEEL
+Filename: WqUtils-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.1.0.dist-info/top_level.txt
+Filename: WqUtils-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.1.0.dist-info/RECORD
+Filename: WqUtils-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: WqUtils-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `WqUtils-0.1.0.dist-info/RECORD` & `WqUtils-0.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 WqUtils/Utils.py,sha256=5rCtSyMBSETtUzG1qdK5rBzylKmMFIvq7M2AXhbwubY,5333
 WqUtils/__init__.py,sha256=QLimFLkeVLJC1KGdIM4TwwvKdEG5by62_9MqaGeUcH8,292
 WqUtils/DB_Utils/SqlServer_DB.py,sha256=g2ofaVr1zKpIrpLfFT-rRdJJCz1eIi2uR80M5nmpzpo,6493
 WqUtils/DB_Utils/__init__.py,sha256=U1spx2Yz0uxJA1A_7-Yb-ZKoy47wJM1VZEuZ4vIB00M,267
-WqUtils-0.1.0.dist-info/METADATA,sha256=oOpwyTc5_a2oIdRoMhkOe7CuV5T89de4RjodrEdYexk,208
-WqUtils-0.1.0.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-WqUtils-0.1.0.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
-WqUtils-0.1.0.dist-info/RECORD,,
+WqUtils/DB_Utils/db_config.toml,sha256=TrVM8oTp6RsFAmeGHTaONoC2PRyf5GOeawvZALKplJI,255
+WqUtils-0.1.1.dist-info/METADATA,sha256=uHhtvj1Y1auTCncaPhfaZyvW-Z2h3nF609Urt0I1k_M,208
+WqUtils-0.1.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+WqUtils-0.1.1.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
+WqUtils-0.1.1.dist-info/RECORD,,
```

