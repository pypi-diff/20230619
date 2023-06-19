# Comparing `tmp/dbt-glue-1.4.21.tar.gz` & `tmp/dbt-glue-1.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.4.21.tar", last modified: Thu Apr 27 16:07:05 2023, max compression
+gzip compressed data, was "dbt-glue-1.4.22.tar", last modified: Mon Jun 19 11:54:52 2023, max compression
```

## Comparing `dbt-glue-1.4.21.tar` & `dbt-glue-1.4.22.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.193398 dbt-glue-1.4.21/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.21/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.21/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    43805 2023-04-27 16:07:05.192822 dbt-glue-1.4.21/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    42903 2023-04-06 14:05:38.000000 dbt-glue-1.4.21/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.166166 dbt-glue-1.4.21/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.165525 dbt-glue-1.4.21/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.176335 dbt-glue-1.4.21/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.21/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       18 2023-04-27 16:07:00.000000 dbt-glue-1.4.21/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.21/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.21/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.179243 dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.21/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.21/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.166454 dbt-glue-1.4.21/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.181106 dbt-glue-1.4.21/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.21/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.21/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.181740 dbt-glue-1.4.21/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.21/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.182985 dbt-glue-1.4.21/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.21/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.21/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.185631 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.186882 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4348 2023-01-18 17:12:34.000000 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/snapshot.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.21/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      592 2022-10-21 07:23:23.000000 dbt-glue-1.4.21/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.169006 dbt-glue-1.4.21/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.187646 dbt-glue-1.4.21/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.21/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-04-27 16:07:05.191883 dbt-glue-1.4.21/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    43805 2023-04-27 16:07:05.000000 dbt-glue-1.4.21/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1157 2023-04-27 16:07:05.000000 dbt-glue-1.4.21/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-04-27 16:07:05.000000 dbt-glue-1.4.21/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.21/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-04-27 16:07:05.000000 dbt-glue-1.4.21/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-04-27 16:07:05.000000 dbt-glue-1.4.21/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-04-27 16:07:05.193626 dbt-glue-1.4.21/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.21/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.505817 dbt-glue-1.4.22/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 11:54:52.505642 dbt-glue-1.4.22/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.4.22/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495724 dbt-glue-1.4.22/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495497 dbt-glue-1.4.22/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.499901 dbt-glue-1.4.22/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.22/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       18 2023-06-15 08:25:55.000000 dbt-glue-1.4.22/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.22/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.22/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501076 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.22/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.22/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.495786 dbt-glue-1.4.22/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501689 dbt-glue-1.4.22/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.22/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.501970 dbt-glue-1.4.22/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.22/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.502653 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.503297 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.503816 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4348 2023-01-18 17:12:34.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.504012 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.4.22/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.496376 dbt-glue-1.4.22/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.504241 dbt-glue-1.4.22/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.22/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 11:54:52.505378 dbt-glue-1.4.22/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.22/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-19 11:54:52.000000 dbt-glue-1.4.22/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-19 11:54:52.505873 dbt-glue-1.4.22/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.22/setup.py
```

### Comparing `dbt-glue-1.4.21/LICENSE` & `dbt-glue-1.4.22/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/PKG-INFO` & `dbt-glue-1.4.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.21
+Version: 1.4.22
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -433,15 +433,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_hudi_connector
       conf: "spark.serializer=org.apache.spark.serializer.KryoSerializer"
 ```
 
 #### Source Code example
 ```sql
@@ -497,15 +497,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_delta_connector
       conf: "spark.sql.extensions=io.delta.sql.DeltaSparkSessionExtension --conf spark.sql.catalog.spark_catalog=org.apache.spark.sql.delta.catalog.DeltaCatalog"
       extra_py_files: "/tmp/delta-core_2.12-1.0.0.jar"
       delta_athena_prefix: "delta"
 ```
 
@@ -628,15 +628,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_iceberg_connector
       conf: --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions --conf spark.serializer=org.apache.spark.serializer.KryoSerializer --conf spark.sql.warehouse=s3://aws-dbt-glue-datalake-1234567890-eu-west-1/dbt_test_project --conf spark.sql.catalog.glue_catalog=org.apache.iceberg.spark.SparkCatalog --conf spark.sql.catalog.glue_catalog.catalog-impl=org.apache.iceberg.aws.glue.GlueCatalog --conf spark.sql.catalog.glue_catalog.io-impl=org.apache.iceberg.aws.s3.S3FileIO --conf spark.sql.catalog.glue_catalog.lock-impl=org.apache.iceberg.aws.glue.DynamoLockManager --conf spark.sql.catalog.glue_catalog.lock.table=myGlueLockTable  --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions 
 ```
 
 #### Source Code example
 ```sql
@@ -744,15 +744,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-metrics=true, --enable-continuous-cloudwatch-log=true, --enable-continuous-log-filter=true, --enable-spark-ui=true, --spark-event-logs-path=s3://bucket-to-write-sparkui-logs/dbt/"
 ```
 
 If you want to use the Spark UI, you can launch the Spark history server using a
 AWS CloudFormation template that hosts the server on an EC2 instance,
 or launch locally using Docker. More information on [Launching the Spark history server](https://docs.aws.amazon.com/glue/latest/dg/monitor-spark-ui-history.html#monitor-spark-ui-history-local)
@@ -789,19 +789,47 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-auto-scaling=true"
 ```
 
+## Access Glue catalog in another AWS account
+In many cases, you may need to run you dbt jobs to read from another AWS account.
+
+Review the following link https://repost.aws/knowledge-center/glue-tables-cross-accounts to set up access policies in source and target accounts
+
+Add the following "spark.hadoop.hive.metastore.glue.catalogid=<AWS-ACCOUNT-ID>" to your conf in the DBT profile, as such, you can have multiple outputs for each of the accounts that you have access to.
+
+Note: The access cross-accounts need to be within the same AWS Region
+#### Profile config example
+```yaml
+test_project:
+  target: dev
+  outputsAccountB:
+    dev:
+      type: glue
+      query-comment: my comment
+      role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
+      region: eu-west-1
+      glue_version: "3.0"
+      workers: 2
+      worker_type: G.1X
+      schema: "dbt_test_project"
+      session_provisioning_timeout_in_seconds: 120
+      location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
+      conf: "--conf hive.metastore.client.factory.class=com.amazonaws.glue.catalog.metastore.AWSGlueDataCatalogHiveClientFactory 
+             --conf spark.hadoop.hive.metastore.glue.catalogid=<TARGET-AWS-ACCOUNT-ID-B>"
+```
+
 ## Persisting model descriptions
 
 Relation-level docs persistence is supported since dbt v0.17.0. For more
 information on configuring docs persistence, see [the docs](resource-configs/persist_docs).
 
 When the `persist_docs` option is configured appropriately, you'll be able to
 see model descriptions in the `Comment` field of `describe [table] extended`
```

### Comparing `dbt-glue-1.4.21/README.md` & `dbt-glue-1.4.22/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -411,15 +411,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_hudi_connector
       conf: "spark.serializer=org.apache.spark.serializer.KryoSerializer"
 ```
 
 #### Source Code example
 ```sql
@@ -475,15 +475,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_delta_connector
       conf: "spark.sql.extensions=io.delta.sql.DeltaSparkSessionExtension --conf spark.sql.catalog.spark_catalog=org.apache.spark.sql.delta.catalog.DeltaCatalog"
       extra_py_files: "/tmp/delta-core_2.12-1.0.0.jar"
       delta_athena_prefix: "delta"
 ```
 
@@ -606,15 +606,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_iceberg_connector
       conf: --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions --conf spark.serializer=org.apache.spark.serializer.KryoSerializer --conf spark.sql.warehouse=s3://aws-dbt-glue-datalake-1234567890-eu-west-1/dbt_test_project --conf spark.sql.catalog.glue_catalog=org.apache.iceberg.spark.SparkCatalog --conf spark.sql.catalog.glue_catalog.catalog-impl=org.apache.iceberg.aws.glue.GlueCatalog --conf spark.sql.catalog.glue_catalog.io-impl=org.apache.iceberg.aws.s3.S3FileIO --conf spark.sql.catalog.glue_catalog.lock-impl=org.apache.iceberg.aws.glue.DynamoLockManager --conf spark.sql.catalog.glue_catalog.lock.table=myGlueLockTable  --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions 
 ```
 
 #### Source Code example
 ```sql
@@ -722,15 +722,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-metrics=true, --enable-continuous-cloudwatch-log=true, --enable-continuous-log-filter=true, --enable-spark-ui=true, --spark-event-logs-path=s3://bucket-to-write-sparkui-logs/dbt/"
 ```
 
 If you want to use the Spark UI, you can launch the Spark history server using a
 AWS CloudFormation template that hosts the server on an EC2 instance,
 or launch locally using Docker. More information on [Launching the Spark history server](https://docs.aws.amazon.com/glue/latest/dg/monitor-spark-ui-history.html#monitor-spark-ui-history-local)
@@ -767,19 +767,47 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-auto-scaling=true"
 ```
 
+## Access Glue catalog in another AWS account
+In many cases, you may need to run you dbt jobs to read from another AWS account.
+
+Review the following link https://repost.aws/knowledge-center/glue-tables-cross-accounts to set up access policies in source and target accounts
+
+Add the following "spark.hadoop.hive.metastore.glue.catalogid=<AWS-ACCOUNT-ID>" to your conf in the DBT profile, as such, you can have multiple outputs for each of the accounts that you have access to.
+
+Note: The access cross-accounts need to be within the same AWS Region
+#### Profile config example
+```yaml
+test_project:
+  target: dev
+  outputsAccountB:
+    dev:
+      type: glue
+      query-comment: my comment
+      role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
+      region: eu-west-1
+      glue_version: "3.0"
+      workers: 2
+      worker_type: G.1X
+      schema: "dbt_test_project"
+      session_provisioning_timeout_in_seconds: 120
+      location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
+      conf: "--conf hive.metastore.client.factory.class=com.amazonaws.glue.catalog.metastore.AWSGlueDataCatalogHiveClientFactory 
+             --conf spark.hadoop.hive.metastore.glue.catalogid=<TARGET-AWS-ACCOUNT-ID-B>"
+```
+
 ## Persisting model descriptions
 
 Relation-level docs persistence is supported since dbt v0.17.0. For more
 information on configuring docs persistence, see [the docs](resource-configs/persist_docs).
 
 When the `persist_docs` option is configured appropriately, you'll be able to
 see model descriptions in the `Comment` field of `describe [table] extended`
```

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/connections.py` & `dbt-glue-1.4.22/dbt/adapters/glue/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/credentials.py` & `dbt-glue-1.4.22/dbt/adapters/glue/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.4.22/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/impl.py` & `dbt-glue-1.4.22/dbt/adapters/glue/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/adapters/glue/relation.py` & `dbt-glue-1.4.22/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.4.22/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.4.22/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.21/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.4.22/dbt/include/glue/sample_profiles.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 default:
   outputs:
 
     dev:
-      type: awsglue
+      type: glue
       role_arn: arn:aws:iam::<awss account>:role/GlueInteractiveSessionRole
       region: eu-west-1
       workers: 5
       worker_type: G.1X
       schema: "dbt_test_{{ var('_dbt_random_suffix') }}"
-      session_provisionning_timeout_in_seconds: 20
+      session_provisioning_timeout_in_seconds: 20
 
     prod:
-      type: awsglue
+      type: glue
       role_arn: arn:aws:iam::<aws account>:role/GlueInteractiveSessionRole
       region: eu-west-1
       workers: 5
       worker_type: G.1X
       schema: "dbt_test_{{ var('_dbt_random_suffix') }}"
-      session_provisionning_timeout_in_seconds: 20
+      session_provisioning_timeout_in_seconds: 20
 
   target: dev
```

### Comparing `dbt-glue-1.4.21/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.4.22/dbt_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.21
+Version: 1.4.22
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -433,15 +433,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_hudi_connector
       conf: "spark.serializer=org.apache.spark.serializer.KryoSerializer"
 ```
 
 #### Source Code example
 ```sql
@@ -497,15 +497,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_delta_connector
       conf: "spark.sql.extensions=io.delta.sql.DeltaSparkSessionExtension --conf spark.sql.catalog.spark_catalog=org.apache.spark.sql.delta.catalog.DeltaCatalog"
       extra_py_files: "/tmp/delta-core_2.12-1.0.0.jar"
       delta_athena_prefix: "delta"
 ```
 
@@ -628,15 +628,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       connections: name_of_your_iceberg_connector
       conf: --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions --conf spark.serializer=org.apache.spark.serializer.KryoSerializer --conf spark.sql.warehouse=s3://aws-dbt-glue-datalake-1234567890-eu-west-1/dbt_test_project --conf spark.sql.catalog.glue_catalog=org.apache.iceberg.spark.SparkCatalog --conf spark.sql.catalog.glue_catalog.catalog-impl=org.apache.iceberg.aws.glue.GlueCatalog --conf spark.sql.catalog.glue_catalog.io-impl=org.apache.iceberg.aws.s3.S3FileIO --conf spark.sql.catalog.glue_catalog.lock-impl=org.apache.iceberg.aws.glue.DynamoLockManager --conf spark.sql.catalog.glue_catalog.lock.table=myGlueLockTable  --conf spark.sql.extensions=org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions 
 ```
 
 #### Source Code example
 ```sql
@@ -744,15 +744,15 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-metrics=true, --enable-continuous-cloudwatch-log=true, --enable-continuous-log-filter=true, --enable-spark-ui=true, --spark-event-logs-path=s3://bucket-to-write-sparkui-logs/dbt/"
 ```
 
 If you want to use the Spark UI, you can launch the Spark history server using a
 AWS CloudFormation template that hosts the server on an EC2 instance,
 or launch locally using Docker. More information on [Launching the Spark history server](https://docs.aws.amazon.com/glue/latest/dg/monitor-spark-ui-history.html#monitor-spark-ui-history-local)
@@ -789,19 +789,47 @@
       query-comment: my comment
       role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
       region: eu-west-1
       glue_version: "3.0"
       workers: 2
       worker_type: G.1X
       schema: "dbt_test_project"
-      session_provisionning_timeout_in_seconds: 120
+      session_provisioning_timeout_in_seconds: 120
       location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
       default_arguments: "--enable-auto-scaling=true"
 ```
 
+## Access Glue catalog in another AWS account
+In many cases, you may need to run you dbt jobs to read from another AWS account.
+
+Review the following link https://repost.aws/knowledge-center/glue-tables-cross-accounts to set up access policies in source and target accounts
+
+Add the following "spark.hadoop.hive.metastore.glue.catalogid=<AWS-ACCOUNT-ID>" to your conf in the DBT profile, as such, you can have multiple outputs for each of the accounts that you have access to.
+
+Note: The access cross-accounts need to be within the same AWS Region
+#### Profile config example
+```yaml
+test_project:
+  target: dev
+  outputsAccountB:
+    dev:
+      type: glue
+      query-comment: my comment
+      role_arn: arn:aws:iam::1234567890:role/GlueInteractiveSessionRole
+      region: eu-west-1
+      glue_version: "3.0"
+      workers: 2
+      worker_type: G.1X
+      schema: "dbt_test_project"
+      session_provisioning_timeout_in_seconds: 120
+      location: "s3://aws-dbt-glue-datalake-1234567890-eu-west-1/"
+      conf: "--conf hive.metastore.client.factory.class=com.amazonaws.glue.catalog.metastore.AWSGlueDataCatalogHiveClientFactory 
+             --conf spark.hadoop.hive.metastore.glue.catalogid=<TARGET-AWS-ACCOUNT-ID-B>"
+```
+
 ## Persisting model descriptions
 
 Relation-level docs persistence is supported since dbt v0.17.0. For more
 information on configuring docs persistence, see [the docs](resource-configs/persist_docs).
 
 When the `persist_docs` option is configured appropriately, you'll be able to
 see model descriptions in the `Comment` field of `describe [table] extended`
```

### Comparing `dbt-glue-1.4.21/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.4.22/dbt_glue.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 dbt/include/glue/macros/generic_test_sql/accepted_values.sql
 dbt/include/glue/macros/generic_test_sql/relationships.sql
 dbt/include/glue/macros/materializations/seed.sql
 dbt/include/glue/macros/materializations/snapshot.sql
 dbt/include/glue/macros/materializations/view.sql
 dbt/include/glue/macros/materializations/incremental/incremental.sql
 dbt/include/glue/macros/materializations/incremental/strategies.sql
+dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
 dbt/include/glue/tests/generic/builtin.sql
 dbt_glue.egg-info/PKG-INFO
 dbt_glue.egg-info/SOURCES.txt
 dbt_glue.egg-info/dependency_links.txt
 dbt_glue.egg-info/not-zip-safe
 dbt_glue.egg-info/requires.txt
 dbt_glue.egg-info/top_level.txt
```

### Comparing `dbt-glue-1.4.21/setup.py` & `dbt-glue-1.4.22/setup.py`

 * *Files identical despite different names*

