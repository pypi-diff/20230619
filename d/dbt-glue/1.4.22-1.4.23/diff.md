# Comparing `tmp/dbt-glue-1.4.22.tar.gz` & `tmp/dbt-glue-1.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.4.22.tar", last modified: Mon Jun 19 11:54:52 2023, max compression
+gzip compressed data, was "dbt-glue-1.4.23.tar", last modified: Mon Jun 19 12:14:15 2023, max compression
```

## Comparing `dbt-glue-1.4.22.tar` & `dbt-glue-1.4.23.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.505817 dbt-glue-1.4.22/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 11:54:52.505642 dbt-glue-1.4.22/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.4.22/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495724 dbt-glue-1.4.22/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495497 dbt-glue-1.4.22/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.499901 dbt-glue-1.4.22/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.22/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       18 2023-06-15 08:25:55.000000 dbt-glue-1.4.22/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.22/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.22/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501076 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.22/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.22/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495786 dbt-glue-1.4.22/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501689 dbt-glue-1.4.22/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501970 dbt-glue-1.4.22/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.22/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.502653 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.503297 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.503816 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4348 2023-01-18 17:12:34.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.504012 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.4.22/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.496376 dbt-glue-1.4.22/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.504241 dbt-glue-1.4.22/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.505378 dbt-glue-1.4.22/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.22/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-19 11:54:52.505873 dbt-glue-1.4.22/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.22/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.803721 dbt-glue-1.4.23/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 12:14:15.803578 dbt-glue-1.4.23/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.4.23/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794809 dbt-glue-1.4.23/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794619 dbt-glue-1.4.23/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.798246 dbt-glue-1.4.23/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.23/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       18 2023-06-19 12:12:21.000000 dbt-glue-1.4.23/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.23/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.23/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.799288 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.23/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.23/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794867 dbt-glue-1.4.23/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800078 dbt-glue-1.4.23/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800325 dbt-glue-1.4.23/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.23/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800864 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.801539 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.801949 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.802186 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.4.23/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.795441 dbt-glue-1.4.23/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.802322 dbt-glue-1.4.23/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.803348 dbt-glue-1.4.23/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.23/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-19 12:14:15.803777 dbt-glue-1.4.23/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.23/setup.py
```

### Comparing `dbt-glue-1.4.22/LICENSE` & `dbt-glue-1.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/PKG-INFO` & `dbt-glue-1.4.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.22
+Version: 1.4.23
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.4.22/README.md` & `dbt-glue-1.4.23/README.md`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/connections.py` & `dbt-glue-1.4.23/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/credentials.py` & `dbt-glue-1.4.23/dbt/adapters/glue/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/impl.py` & `dbt-glue-1.4.23/dbt/adapters/glue/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/adapters/glue/relation.py` & `dbt-glue-1.4.23/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
   {% set tmp_relation = make_temp_relation(target_relation, '_tmp') %}
   {% set is_incremental = 'False' %}
 
   {% call statement() %}
     set spark.sql.autoBroadcastJoinThreshold=-1
   {% endcall %}
 
+  {{ run_hooks(pre_hooks) }}
+
   {% if file_format == 'hudi' %}
         {%- set hudi_options = config.get('hudi_options', default={}) -%}
         {{ adapter.hudi_merge_table(target_relation, sql, unique_key, partition_by, custom_location, hudi_options) }}
         {% set build_sql = "select * from " + target_relation.schema + "." + target_relation.identifier + " limit 1 "%}
   {% elif file_format == 'iceberg' %}
         {{ adapter.iceberg_write(target_relation, sql, unique_key, partition_by, custom_location, strategy, table_properties) }}
         {% set build_sql = "select * from glue_catalog." + target_relation.schema + "." + target_relation.identifier + " limit 1 "%}
@@ -66,16 +68,14 @@
         {% endif %}
       {% else %}
         {{ glue__create_tmp_table_as(tmp_relation, sql) }}
         {% set is_incremental = 'True' %}
         {% set build_sql = dbt_glue_get_incremental_sql(strategy, tmp_relation, target_relation, unique_key) %}
       {% endif %}
   {% endif %}
-	
-  {{ run_hooks(pre_hooks) }}
 
   {%- call statement('main') -%}
      {{ build_sql }}
   {%- endcall -%}
 
   {{ run_hooks(post_hooks) }}
```

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.4.23/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.4.23/dbt_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.22
+Version: 1.4.23
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-glue-1.4.22/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.4.23/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.22/setup.py` & `dbt-glue-1.4.23/setup.py`

 * *Files identical despite different names*

