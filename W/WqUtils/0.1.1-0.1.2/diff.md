# Comparing `tmp/WqUtils-0.1.1-py3-none-any.whl.zip` & `tmp/WqUtils-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6638 bytes, number of entries: 9
+Zip file size: 6666 bytes, number of entries: 9
 -rw-r--r--  2.0 unx     5333 b- defN 23-Jun-19 08:15 WqUtils/Utils.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Jun-19 15:54 WqUtils/__init__.py
--rw-r--r--  2.0 unx     6493 b- defN 23-Jun-19 15:19 WqUtils/DB_Utils/SqlServer_DB.py
+-rw-r--r--  2.0 unx     6557 b- defN 23-Jun-19 16:59 WqUtils/DB_Utils/SqlServer_DB.py
 -rw-r--r--  2.0 unx      267 b- defN 23-Jun-19 06:58 WqUtils/DB_Utils/__init__.py
 -rw-r--r--  2.0 unx      255 b- defN 23-Jun-19 07:32 WqUtils/DB_Utils/db_config.toml
--rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      704 b- defN 23-Jun-19 16:40 WqUtils-0.1.1.dist-info/RECORD
-9 files, 13652 bytes uncompressed, 5424 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      704 b- defN 23-Jun-19 16:59 WqUtils-0.1.2.dist-info/RECORD
+9 files, 13716 bytes uncompressed, 5452 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: WqUtils/DB_Utils/__init__.py
 Comment: 
 
 Filename: WqUtils/DB_Utils/db_config.toml
 Comment: 
 
-Filename: WqUtils-0.1.1.dist-info/METADATA
+Filename: WqUtils-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: WqUtils-0.1.1.dist-info/WHEEL
+Filename: WqUtils-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: WqUtils-0.1.1.dist-info/top_level.txt
+Filename: WqUtils-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: WqUtils-0.1.1.dist-info/RECORD
+Filename: WqUtils-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## WqUtils/DB_Utils/SqlServer_DB.py

```diff
@@ -19,15 +19,15 @@
 import pandas as pd
 
 
 class TomlConfig:
 
     def __init__(self, toml_filename):
         self.t_dict = dict()  # 创建空字典
-        self.toml_file_path = toml_filename
+        self.toml_file_path = os.path.join(os.path.dirname(__file__), toml_filename)
 
     def update(self, t_data):
         # 给toml文件添加配置
         self.t_dict.update(t_data)
         return self.t_dict
 
     def write(self, t_data):
@@ -72,18 +72,20 @@
         self.pymssql_config = TomlConfig('db_config.toml').read()
         self.sql_conf = self._get_sql_conf()
         self.host = self.sql_conf['HOST']
         self.user = self.sql_conf['USERNAME']
         self.pwd = self.sql_conf['PASSWORD']
         self.test_db = self.sql_conf['DB']
 
+
     def load_config(self):
         # 读取环境变量数据库信息如果有|直接使用，如果没有再读取本地配置文件
         if os.getenv("MSSQL_HOST", None):
-            config = {"HOST": os.getenv("MSSQL_HOST"), "PORT": os.getenv("MSSQL_PORT"), "USERNAME":
+            config = {"HOST": os.getenv("MSSQL_HOST"), "PORT": int(os.getenv(
+                "MSSQL_PORT")), "USERNAME":
                 os.getenv("MSSQL_USERNAME"), "PASSWORD": os.getenv("MSSQL_PASSWORD"),
                 "DB": os.getenv("MSSQL_DB")}
 
         else:
             config = self.pymssql_config['sqlserver_database']
         return config
```

## Comparing `WqUtils-0.1.1.dist-info/RECORD` & `WqUtils-0.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 WqUtils/Utils.py,sha256=5rCtSyMBSETtUzG1qdK5rBzylKmMFIvq7M2AXhbwubY,5333
 WqUtils/__init__.py,sha256=QLimFLkeVLJC1KGdIM4TwwvKdEG5by62_9MqaGeUcH8,292
-WqUtils/DB_Utils/SqlServer_DB.py,sha256=g2ofaVr1zKpIrpLfFT-rRdJJCz1eIi2uR80M5nmpzpo,6493
+WqUtils/DB_Utils/SqlServer_DB.py,sha256=QlSCVxMEogmk7STQpCHhiFEI9SFnvCXViMdJ5jdZ5f0,6557
 WqUtils/DB_Utils/__init__.py,sha256=U1spx2Yz0uxJA1A_7-Yb-ZKoy47wJM1VZEuZ4vIB00M,267
 WqUtils/DB_Utils/db_config.toml,sha256=TrVM8oTp6RsFAmeGHTaONoC2PRyf5GOeawvZALKplJI,255
-WqUtils-0.1.1.dist-info/METADATA,sha256=uHhtvj1Y1auTCncaPhfaZyvW-Z2h3nF609Urt0I1k_M,208
-WqUtils-0.1.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-WqUtils-0.1.1.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
-WqUtils-0.1.1.dist-info/RECORD,,
+WqUtils-0.1.2.dist-info/METADATA,sha256=k5m_57GKTxxw0jzWcboHYLlW0_z56urvmCBn1H_dz3g,208
+WqUtils-0.1.2.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+WqUtils-0.1.2.dist-info/top_level.txt,sha256=XpUtbHzxrhqE5cOFUxWQrZAlMz2b2ww_pX2dKJrr9cs,8
+WqUtils-0.1.2.dist-info/RECORD,,
```

