# Comparing `tmp/pp_project_pkg-1.0.202306190122-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306190124-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10198 bytes, number of entries: 13
+Zip file size: 10194 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Jun-18 23:43 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     5468 b- defN 23-Jun-19 01:22 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-19 01:22 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5462 b- defN 23-Jun-19 01:24 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-19 01:24 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306190122.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306190122.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-19 01:22 pp_project_pkg-1.0.202306190122.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 01:22 pp_project_pkg-1.0.202306190122.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-19 01:22 pp_project_pkg-1.0.202306190122.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-19 01:22 pp_project_pkg-1.0.202306190122.dist-info/RECORD
-13 files, 25870 bytes uncompressed, 8176 bytes compressed:  68.4%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306190124.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306190124.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-19 01:24 pp_project_pkg-1.0.202306190124.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 01:24 pp_project_pkg-1.0.202306190124.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-19 01:24 pp_project_pkg-1.0.202306190124.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-19 01:24 pp_project_pkg-1.0.202306190124.dist-info/RECORD
+13 files, 25864 bytes uncompressed, 8172 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306190124.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306190124.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306190124.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306190124.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306190124.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190122.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306190124.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -117,15 +117,15 @@
     q1 = """ 
     SELECT * FROM pp_tables.waldorf_report_closed_data
     """
     download_file = wv.read_sql(q1,wv.ml_engine)
     res_rep = compare_report_dates(res_new,download_file)
     if logger:
         logger.info("Uploading records total : {}".format(len(res_rep)))
-    res_rep.to_sql(table_name='waldorf_report_closed_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='replace',index=False)
+    res_rep.to_sql(name='waldorf_report_closed_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='replace',index=False)
     return res_rep
     
 def upload_waste_data(res_rep,logger=None):
     """
     function to get the new waste data for each date which are not there in DB and upload to the database
     
     Args:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('19')
 VERSION_HOUR = int('01')
-VERSION_MINUTE = int('22')
+VERSION_MINUTE = int('24')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306190122
-version_date = '2023/06/19 01:22'
+PATCH_VERSION = 202306190124
+version_date = '2023/06/19 01:24'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306190122.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306190124.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306190122.dist-info/RECORD` & `pp_project_pkg-1.0.202306190124.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=WnDXi7hkHDnF4typd5weO7pw5W36Qq6-RsQdtntneWw,4780
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=l1tap47X-Y9B1hV5Ps1kj-6VIBYLV9vlEiVmP-kLA4I,5468
-pp_project_pkg/version.py,sha256=CvphLkHLbh5TfIT9TbbGJ7agye_zXVwiaefDcbQOCPg,396
+pp_project_pkg/utils.py,sha256=oOZtnrtHBd04IIzU5tM3gU5xwfcdNp89psK7djYlDIc,5462
+pp_project_pkg/version.py,sha256=r3h1LBA-PEviPuHYmv8p_RDIm4Iva2xf336_1XV1Bew,396
 pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306190122.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306190122.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306190122.dist-info/METADATA,sha256=AmnZy7vw19jWEr3-AHc70yH61sIEW4eoVSsxM-3nUYw,191
-pp_project_pkg-1.0.202306190122.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306190122.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306190122.dist-info/RECORD,,
+pp_project_pkg-1.0.202306190124.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306190124.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306190124.dist-info/METADATA,sha256=wCW8L9BeoNHiZMQtoiGVb3h4HD0Cl61GoY9plecTM_o,191
+pp_project_pkg-1.0.202306190124.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306190124.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306190124.dist-info/RECORD,,
```

