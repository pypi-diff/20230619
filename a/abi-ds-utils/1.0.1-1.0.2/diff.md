# Comparing `tmp/abi_ds_utils-1.0.1.tar.gz` & `tmp/abi_ds_utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi_ds_utils-1.0.1.tar", max compression
+gzip compressed data, was "abi_ds_utils-1.0.2.tar", max compression
```

## Comparing `abi_ds_utils-1.0.1.tar` & `abi_ds_utils-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      255 2023-06-19 09:30:44.321124 abi_ds_utils-1.0.1/abi_ds_utils/__init__.py
--rw-r--r--   0        0        0      823 2023-06-19 09:30:44.321124 abi_ds_utils-1.0.1/abi_ds_utils/airflow.py
--rw-r--r--   0        0        0     1737 2023-06-19 09:30:44.321124 abi_ds_utils-1.0.1/abi_ds_utils/aws.py
--rw-r--r--   0        0        0     1356 2023-06-19 09:30:44.321124 abi_ds_utils-1.0.1/abi_ds_utils/spark.py
--rw-r--r--   0        0        0      458 2023-06-19 09:30:44.323124 abi_ds_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-19 09:31:54.281401 abi_ds_utils-1.0.1/setup.py
--rw-r--r--   0        0        0      601 2023-06-19 09:31:54.281677 abi_ds_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-06-19 10:34:08.513948 abi_ds_utils-1.0.2/abi_ds_utils/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/airflow.py
+-rw-r--r--   0        0        0     1737 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/aws.py
+-rw-r--r--   0        0        0     1356 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/spark.py
+-rw-r--r--   0        0        0      433 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      688 2023-06-19 10:34:57.921640 abi_ds_utils-1.0.2/setup.py
+-rw-r--r--   0        0        0      561 2023-06-19 10:34:57.921887 abi_ds_utils-1.0.2/PKG-INFO
```

### Comparing `abi_ds_utils-1.0.1/abi_ds_utils/airflow.py` & `abi_ds_utils-1.0.2/abi_ds_utils/airflow.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-1.0.1/abi_ds_utils/aws.py` & `abi_ds_utils-1.0.2/abi_ds_utils/aws.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-1.0.1/abi_ds_utils/spark.py` & `abi_ds_utils-1.0.2/abi_ds_utils/spark.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-1.0.1/setup.py` & `abi_ds_utils-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 packages = \
 ['abi_ds_utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['apache-airflow==2.4.0',
- 'boto3>=1.21.14,<2.0.0',
- 'pyarrow>=7.0.0,<8.0.0',
- 'pyspark==3.3.2']
+['boto3>=1.21.14,<2.0.0', 'pyarrow>=7.0.0,<8.0.0', 'pyspark==3.3.2']
 
 setup_kwargs = {
     'name': 'abi-ds-utils',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Utility modules for working with spark, containers, aws and more.',
     'long_description': None,
     'author': 'Martin Matousek',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `abi_ds_utils-1.0.1/PKG-INFO` & `abi_ds_utils-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: abi-ds-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utility modules for working with spark, containers, aws and more.
 License: Private
 Author: Martin Matousek
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: apache-airflow (==2.4.0)
 Requires-Dist: boto3 (>=1.21.14,<2.0.0)
 Requires-Dist: pyarrow (>=7.0.0,<8.0.0)
 Requires-Dist: pyspark (==3.3.2)
```

