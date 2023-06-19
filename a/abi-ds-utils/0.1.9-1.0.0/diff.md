# Comparing `tmp/abi_ds_utils-0.1.9.tar.gz` & `tmp/abi_ds_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi_ds_utils-0.1.9.tar", max compression
+gzip compressed data, was "abi_ds_utils-1.0.0.tar", max compression
```

## Comparing `abi_ds_utils-0.1.9.tar` & `abi_ds_utils-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      823 2023-01-09 13:07:26.921658 abi_ds_utils-0.1.9/abi_ds_utils/airflow.py
--rw-r--r--   0        0        0     1737 2023-01-09 13:07:26.921658 abi_ds_utils-0.1.9/abi_ds_utils/aws.py
--rw-r--r--   0        0        0     1394 2023-01-09 13:07:26.921658 abi_ds_utils-0.1.9/abi_ds_utils/spark.py
--rw-r--r--   0        0        0      483 2023-01-09 13:07:26.921658 abi_ds_utils-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      747 2023-01-09 13:08:02.284189 abi_ds_utils-0.1.9/setup.py
--rw-r--r--   0        0        0      495 2023-01-09 13:08:02.284453 abi_ds_utils-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      823 2023-06-19 09:15:52.640882 abi_ds_utils-1.0.0/abi_ds_utils/airflow.py
+-rw-r--r--   0        0        0     1737 2023-06-19 09:15:52.640882 abi_ds_utils-1.0.0/abi_ds_utils/aws.py
+-rw-r--r--   0        0        0     1356 2023-06-19 09:15:52.640882 abi_ds_utils-1.0.0/abi_ds_utils/spark.py
+-rw-r--r--   0        0        0      433 2023-06-19 09:15:52.640882 abi_ds_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      688 2023-06-19 09:16:42.004463 abi_ds_utils-1.0.0/setup.py
+-rw-r--r--   0        0        0      561 2023-06-19 09:16:42.004737 abi_ds_utils-1.0.0/PKG-INFO
```

### Comparing `abi_ds_utils-0.1.9/abi_ds_utils/airflow.py` & `abi_ds_utils-1.0.0/abi_ds_utils/airflow.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-0.1.9/abi_ds_utils/aws.py` & `abi_ds_utils-1.0.0/abi_ds_utils/aws.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-0.1.9/abi_ds_utils/spark.py` & `abi_ds_utils-1.0.0/abi_ds_utils/spark.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from pyspark.sql import SparkSession
-import pyspark.sql.functions as F
 
 
 def getSpark(driver_memory: str = "21g") -> SparkSession:
     spark = (
         SparkSession.builder
         # General
         .master('local[*]')
@@ -13,24 +12,22 @@
         # Get 80% of free memory (this might be a bad idea)
         .config("spark.driver.memory", driver_memory)
         .config("spark.dynamicAllocation.enabled", "true")
 
         # PyArrow for dtypes conversions
         .config("spark.sql.execution.arrow.pyspark.enabled", "true")
 
-        # Jars compatible with the base-notebook image (Python 3.8.8, PySpark 3.1.1)
-        .config('spark.jars.packages', 'org.apache.hadoop:hadoop-aws:3.1.1,io.delta:delta-core_2.12:1.0.1')
+        # Jars compatible with the base-notebook image (Python 3.8, PySpark 3.3.2)
+        .config('spark.jars.packages', 'org.apache.hadoop:hadoop-aws:3.3.2,io.delta:delta-core_2.13:2.2.0')
 
         # Delta Lake setup
         .config("spark.hadoop.fs.s3a.connection.maximum", 128)
         .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
         .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog")
         .config("spark.delta.logStore.class", "org.apache.spark.sql.delta.storage.S3SingleDriverLogStore")
     )
     if os.environ.get('AWS_SESSION_TOKEN') is not None:
         spark = spark.config(
             "fs.s3a.aws.credentials.provider",
             "org.apache.hadoop.fs.s3a.TemporaryAWSCredentialsProvider"
         )
     return spark.getOrCreate()
-
-
```

### Comparing `abi_ds_utils-0.1.9/setup.py` & `abi_ds_utils-1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,27 @@
 packages = \
 ['abi_ds_utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.21.14,<2.0.0',
- 'hurry.filesize>=0.9,<0.10',
- 'psutil>=5.9.3,<6.0.0',
- 'pyarrow>=7.0.0,<8.0.0',
- 'pyspark==3.1.1']
+['boto3>=1.21.14,<2.0.0', 'pyarrow>=7.0.0,<8.0.0', 'pyspark==3.3.2']
 
 setup_kwargs = {
     'name': 'abi-ds-utils',
-    'version': '0.1.9',
-    'description': 'Utility modules for working with spark, containers, aws and many more.',
+    'version': '1.0.0',
+    'description': 'Utility modules for working with spark, containers, aws and more.',
     'long_description': None,
     'author': 'Martin Matousek',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '==3.8.8',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

