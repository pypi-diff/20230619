# Comparing `tmp/pp_project_pkg-1.0.202306182156-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306182221-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8641 bytes, number of entries: 13
+Zip file size: 8656 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-18 21:29 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     4190 b- defN 23-Jun-18 21:13 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-18 21:56 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     4595 b- defN 23-Jun-18 21:56 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306182156.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1179 b- defN 23-Jun-18 21:56 pp_project_pkg-1.0.202306182156.dist-info/RECORD
-13 files, 19802 bytes uncompressed, 6619 bytes compressed:  66.6%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-18 22:21 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306182221.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306182221.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-18 22:21 pp_project_pkg-1.0.202306182221.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-18 22:21 pp_project_pkg-1.0.202306182221.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 22:21 pp_project_pkg-1.0.202306182221.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1179 b- defN 23-Jun-18 22:21 pp_project_pkg-1.0.202306182221.dist-info/RECORD
+13 files, 19809 bytes uncompressed, 6634 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306182221.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306182221.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306182221.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306182221.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306182221.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306182156.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306182221.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('18')
-VERSION_HOUR = int('21')
-VERSION_MINUTE = int('56')
+VERSION_HOUR = int('22')
+VERSION_MINUTE = int('21')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306182156
-version_date = '2023/06/18 21:56'
+PATCH_VERSION = 202306182221
+version_date = '2023/06/18 22:21'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -1,14 +1,14 @@
 ## function for wrangling data
 from dateutil import parser
 import mb.pandas as pd
 
 __all__ = ['wrangling_data']
 
-def wrangling_data(queries_res,site_data=None,logger=None):
+def wrangling_data(queries_res,site_data=None,date = '2023-06-06',logger=None):
     """
     Args:
         query_res: query result from database
     Output:
         wrangled data : csv file
     """
     
@@ -79,14 +79,14 @@
     meal_service_summary_df['covers'] = cover_count
     meal_service_summary_df['actual_consumption'] = meal_service_summary_df['actual_production'] - meal_service_summary_df['rework_or_reuse'] - meal_service_summary_df['waste']
     meal_service_summary_df['consumption_per_cover'] = meal_service_summary_df['actual_consumption'] / cover_count
     meal_service_summary_df['scaling_factor'] = meal_service_summary_df['actual_consumption'] / (cover_count * 1000)
 
     # Select all columns from the resulting dataframe
     result_df = meal_service_summary_df.loc[:, :]
-    result_df['date'] = site_data['date']
+    result_df['date'] = date
 
     if logger:
         logger.info("Added date column to the result_df")
         logger.info("result_df : {}".format(result_df.head(2)))
                         
     return result_df
```

## Comparing `pp_project_pkg-1.0.202306182156.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306182221.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

