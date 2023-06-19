# Comparing `tmp/netspresso-1.0.1-py3-none-any.whl.zip` & `tmp/netspresso-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 23609 bytes, number of entries: 27
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-19 07:37 netspresso/__init__.py
+Zip file size: 23607 bytes, number of entries: 27
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-19 07:53 netspresso/__init__.py
 -rw-rw-rw-  2.0 fat    23619 b- defN 23-Jun-13 07:57 netspresso/compressor/__init__.py
 -rw-rw-rw-  2.0 fat     8479 b- defN 23-Jun-19 05:43 netspresso/compressor/client/__init__.py
 -rw-rw-rw-  2.0 fat      536 b- defN 23-Jun-16 05:06 netspresso/compressor/client/config.py
 -rw-rw-rw-  2.0 fat       41 b- defN 23-Jun-13 06:13 netspresso/compressor/client/configs/config-local.ini
 -rw-rw-rw-  2.0 fat       61 b- defN 23-Jun-13 06:13 netspresso/compressor/client/configs/config-prod.ini
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/__init__.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jun-13 06:13 netspresso/compressor/client/schemas/auth.py
@@ -17,13 +17,13 @@
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-13 06:13 netspresso/compressor/client/utils/validator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/core/__init__.py
 -rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-13 06:13 netspresso/compressor/core/compression.py
 -rw-rw-rw-  2.0 fat     2966 b- defN 23-Jun-13 06:13 netspresso/compressor/core/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2035 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/model.py
 -rw-rw-rw-  2.0 fat      236 b- defN 23-Jun-13 06:13 netspresso/compressor/utils/token.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7286 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2553 b- defN 23-Jun-19 07:39 netspresso-1.0.1.dist-info/RECORD
-27 files, 80559 bytes uncompressed, 19347 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-19 08:15 netspresso-1.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7286 b- defN 23-Jun-19 08:15 netspresso-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-19 08:15 netspresso-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-19 08:15 netspresso-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2553 b- defN 23-Jun-19 08:15 netspresso-1.0.2.dist-info/RECORD
+27 files, 80559 bytes uncompressed, 19345 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: netspresso/compressor/utils/model.py
 Comment: 
 
 Filename: netspresso/compressor/utils/token.py
 Comment: 
 
-Filename: netspresso-1.0.1.dist-info/LICENSE
+Filename: netspresso-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-1.0.1.dist-info/METADATA
+Filename: netspresso-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-1.0.1.dist-info/WHEEL
+Filename: netspresso-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: netspresso-1.0.1.dist-info/top_level.txt
+Filename: netspresso-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: netspresso-1.0.1.dist-info/RECORD
+Filename: netspresso-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

## Comparing `netspresso-1.0.1.dist-info/LICENSE` & `netspresso-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-1.0.1.dist-info/METADATA` & `netspresso-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 1.0.1
+Version: 1.0.2
 Summary: NetsPresso Python Package
 Home-page: https://github.com/Nota-NetsPresso/netspresso-python
 Author: NetsPresso
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netspresso Version: 1.0.1 Summary: NetsPresso
+Metadata-Version: 2.1 Name: netspresso Version: 1.0.2 Summary: NetsPresso
 Python Package Home-page: https://github.com/Nota-NetsPresso/netspresso-python
 Author: NetsPresso Author-email: bmlee@nota.ai Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: loguru
 (==0.7.0) Requires-Dist: urllib3 (==2.0.2) Requires-Dist: PyJWT (==2.7.0)
 Requires-Dist: pydantic (==1.10.4) Requires-Dist: requests (==2.30.0) Requires-
```

## Comparing `netspresso-1.0.1.dist-info/RECORD` & `netspresso-1.0.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-netspresso/__init__.py,sha256=j9q3lYMZra0QrErNnn9E5GNXxWLOlDgeOkmX8oXa7ro,23
+netspresso/__init__.py,sha256=LZTFaiDdXahAtu6Prb5WEPk4QX_pfMd7zDoNQSzcGsI,23
 netspresso/compressor/__init__.py,sha256=4gKZzZCd3BJUSCfLOu8crijVVY7sIVe5qQNZAvjEFpI,23619
 netspresso/compressor/client/__init__.py,sha256=c2HyrKbG8gdRvaWSNAy5g_t9uh3hilG9Y2ReB7Bjyo4,8479
 netspresso/compressor/client/config.py,sha256=i3EZTWDZJEq527YY1hiyiSN-DIVQyjE7zgOI7_kLY9Y,536
 netspresso/compressor/client/configs/config-local.ini,sha256=0trP47pxMTnQCy-KAnsVpKbdcr2aJffbnAJDfTxSQu4,41
 netspresso/compressor/client/configs/config-prod.ini,sha256=en_y9NB0Rj3lfU58h4JGK6PPNAusN2hs3mXSMpEQhOQ,61
 netspresso/compressor/client/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/schemas/auth.py,sha256=NGudVfx4Q7E8XppeDgcKmQlU_3UwKDu3YjYiIwsii1g,2644
@@ -16,12 +16,12 @@
 netspresso/compressor/client/utils/validator.py,sha256=0pONKSTlxTWcpSIiUw3P2ItPARoLXvu5YSGGxhUFPNU,3814
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/core/compression.py,sha256=OMrI-SsDXmwzZdz_1jRmv30KTGRRluRszJPqcXFQOwU,1900
 netspresso/compressor/core/model.py,sha256=kH0VBvcpwyxO9QsUpaQZXLB-IZXfw3T-mp613qX3_mE,2966
 netspresso/compressor/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/utils/model.py,sha256=tPojNWMvvHTNT8EgLIJfq_3EWIOIb0HuZHDbF1ANBc0,2035
 netspresso/compressor/utils/token.py,sha256=zWKx6olb8N2c3nSQhUS22IRG7ILQZYIERScETEFeUXY,236
-netspresso-1.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-netspresso-1.0.1.dist-info/METADATA,sha256=iLHSxl5iMgOI71UeZUcyVP4NtqEpy_-UpJOQoCvYhnk,7286
-netspresso-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-1.0.1.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-1.0.1.dist-info/RECORD,,
+netspresso-1.0.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+netspresso-1.0.2.dist-info/METADATA,sha256=PiZZR4WJbz-4ApyF_sAKwbPefKtU7bIdxmxS4oSyzNQ,7286
+netspresso-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-1.0.2.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-1.0.2.dist-info/RECORD,,
```

