# Comparing `tmp/pp_project_pkg-1.0.202306190104-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306190108-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10209 bytes, number of entries: 13
+Zip file size: 10205 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     4780 b- defN 23-Jun-18 23:43 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     5504 b- defN 23-Jun-19 01:04 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-19 01:04 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5503 b- defN 23-Jun-19 01:08 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-19 01:08 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306190104.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306190104.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-19 01:04 pp_project_pkg-1.0.202306190104.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 01:04 pp_project_pkg-1.0.202306190104.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-19 01:04 pp_project_pkg-1.0.202306190104.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-19 01:04 pp_project_pkg-1.0.202306190104.dist-info/RECORD
-13 files, 25906 bytes uncompressed, 8187 bytes compressed:  68.4%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306190108.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306190108.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-19 01:08 pp_project_pkg-1.0.202306190108.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 01:08 pp_project_pkg-1.0.202306190108.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-19 01:08 pp_project_pkg-1.0.202306190108.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-19 01:08 pp_project_pkg-1.0.202306190108.dist-info/RECORD
+13 files, 25905 bytes uncompressed, 8183 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306190108.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306190108.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306190108.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306190108.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306190108.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306190104.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306190108.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -75,15 +75,15 @@
     """
     
     create_date_table_res = create_date_table(start_date=start_date,end_date=end_date)
     site_res_date = site_res[['start_date','closed','meal_service_state']]
     today = datetime.datetime.today().date()
     start_date =datetime.datetime.strptime(start_date,'%Y-%m-%d').date()
     site_res_date_new = site_res_date[(site_res_date['start_date']<=today) & (site_res_date['start_date']>=start_date) & 
-                                      (site_res_date['meal_service_state']=='REPORT') & (site_date_res['closed']>=site_date_res['start_date'])]
+                                      (site_res_date['meal_service_state']=='REPORT') & (site_date_res['closed']>site_date_res['start_date'])]
     for i in range(len(site_res_date_new)):
         k = site_res_date_new.iloc[i]['start_date']
         l = site_res_date_new.iloc[i]['closed']
         if l is not None or l is not pd.NaT:
             l = l.to_pydatetime().date()
         else:
             l = None
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('19')
 VERSION_HOUR = int('01')
-VERSION_MINUTE = int('04')
+VERSION_MINUTE = int('08')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306190104
-version_date = '2023/06/19 01:04'
+PATCH_VERSION = 202306190108
+version_date = '2023/06/19 01:08'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306190104.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306190108.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306190104.dist-info/RECORD` & `pp_project_pkg-1.0.202306190108.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=WnDXi7hkHDnF4typd5weO7pw5W36Qq6-RsQdtntneWw,4780
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=KqF3hHI8eRE6Ldx8Nlvb2sM9AJgJ35rTqdIIs_N5zXM,5504
-pp_project_pkg/version.py,sha256=8rvLv2aZ8_hXtLHzWruf53bJTv3BlGfup-ts1w1PFHs,396
+pp_project_pkg/utils.py,sha256=7EesuLjnW9IsKo8RL9TkgkL5QtdKggZAai_2gm4BO_Y,5503
+pp_project_pkg/version.py,sha256=7Z7bYIsdRnwgzO5SXYRPb7Om_mWGDu7OUt1tjunymm4,396
 pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306190104.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306190104.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306190104.dist-info/METADATA,sha256=G4n0NfbOG0rq0OE1NlLKBaNre2403AZnKZx8ev4tTvA,191
-pp_project_pkg-1.0.202306190104.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202306190104.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306190104.dist-info/RECORD,,
+pp_project_pkg-1.0.202306190108.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306190108.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306190108.dist-info/METADATA,sha256=Q7I4UU_JDdGUl5CBJKrSd8Qk9qAVTja4NpzbUJvDgoE,191
+pp_project_pkg-1.0.202306190108.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202306190108.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306190108.dist-info/RECORD,,
```

