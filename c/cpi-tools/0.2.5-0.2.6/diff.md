# Comparing `tmp/cpi_tools-0.2.5.tar.gz` & `tmp/cpi_tools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi_tools-0.2.5.tar", last modified: Fri Jun 16 14:42:22 2023, max compression
+gzip compressed data, was "cpi_tools-0.2.6.tar", last modified: Mon Jun 19 12:57:25 2023, max compression
```

## Comparing `cpi_tools-0.2.5.tar` & `cpi_tools-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/
--rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      956 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.608431 cpi_tools-0.2.5/cpi_tools/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/__init__.py
--rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/aws_tools.py
--rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/cpi_validation.py
--rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/fuzzy_matching_cpi.py
--rw-rw-rw-   0        0        0    14916 2023-06-16 14:33:00.000000 cpi_tools-0.2.5/cpi_tools/tracking_processing_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/cpi_tools.egg-info/
--rw-rw-rw-   0        0        0      956 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      581 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 12:57:25.152318 cpi_tools-0.2.6/
+-rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-06-19 12:57:25.152814 cpi_tools-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 12:57:25.145612 cpi_tools-0.2.6/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/cpi_tools/aws_tools.py
+-rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/cpi_tools/cpi_validation.py
+-rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/cpi_tools/fuzzy_matching_cpi.py
+-rw-rw-rw-   0        0        0    15807 2023-06-19 12:55:42.000000 cpi_tools-0.2.6/cpi_tools/tracking_processing_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:57:25.151599 cpi_tools-0.2.6/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-06-19 12:57:25.000000 cpi_tools-0.2.6/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-19 12:57:25.000000 cpi_tools-0.2.6/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:57:25.000000 cpi_tools-0.2.6/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 12:57:25.000000 cpi_tools-0.2.6/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0      581 2023-06-19 12:57:25.153385 cpi_tools-0.2.6/setup.cfg
```

### Comparing `cpi_tools-0.2.5/LICENSE` & `cpi_tools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.5/PKG-INFO` & `cpi_tools-0.2.6/cpi_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi_tools
-Version: 0.2.5
+Name: cpi-tools
+Version: 0.2.6
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.5/cpi_tools/aws_tools.py` & `cpi_tools-0.2.6/cpi_tools/aws_tools.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.5/cpi_tools/cpi_validation.py` & `cpi_tools-0.2.6/cpi_tools/cpi_validation.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.5/cpi_tools/fuzzy_matching_cpi.py` & `cpi_tools-0.2.6/cpi_tools/fuzzy_matching_cpi.py`

 * *Files identical despite different names*

### Comparing `cpi_tools-0.2.5/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.2.6/cpi_tools/tracking_processing_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,7 +357,33 @@
     # Data source
     ref_data_source = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_data_source.csv', encoding='utf-8')
 
     # Return all the DataFrames as a tuple
     return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
     ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient, ref_data_source
 
+
+def generate_glcf_id(df:pd.DataFrame, year:int):
+    '''
+    This function generates a unique ID for each entry in the dataset processed. 
+    
+    Parameters:
+    df(pd.DataFrame): the dataset being processed. 
+    Note that it is important that this dataset has already been cleaned and most
+    importantly subset to only the relevant row entries, as the final data ID will
+    include the row number of each observation. 
+    year(int): the year of the GLCF publication (e.g., 2023 for data relating to
+    2021 and 2022).
+    
+    Returns:
+    df(pd.DataFrame): the inputted dataframe, with the addition of the column 'data_source_id'.
+    '''
+    
+    df['data_source_id'] = df.data_source_code.map(lambda x: str(x).zfill(3)) + '-' + \
+                           str(year) + '-' + \
+                           df.index.map(lambda x: str(x).zfill(9))
+
+    return df
+    
+    
+    
+
```

### Comparing `cpi_tools-0.2.5/cpi_tools.egg-info/PKG-INFO` & `cpi_tools-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cpi-tools
-Version: 0.2.5
+Name: cpi_tools
+Version: 0.2.6
 Summary: Repository of functions used across CPI
 Home-page: https://github.com/climatepolicydata/cpi_tools
 Author: Jake Connolly, Nikita Marini
 Author-email: datascience@cpiglobal.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpi_tools-0.2.5/setup.cfg` & `cpi_tools-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7069 5f74 6f6f 6c73 0d0a 7665   = cpi_tools..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 350d 0a61  rsion = 0.2.5..a
+00000020: 7273 696f 6e20 3d20 302e 322e 360d 0a61  rsion = 0.2.6..a
 00000030: 7574 686f 7220 3d20 4a61 6b65 2043 6f6e  uthor = Jake Con
 00000040: 6e6f 6c6c 792c 204e 696b 6974 6120 4d61  nolly, Nikita Ma
 00000050: 7269 6e69 0d0a 6175 7468 6f72 5f65 6d61  rini..author_ema
 00000060: 696c 203d 2064 6174 6173 6369 656e 6365  il = datascience
 00000070: 4063 7069 676c 6f62 616c 2e6f 7267 0d0a  @cpiglobal.org..
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 5265  description = Re
 00000090: 706f 7369 746f 7279 206f 6620 6675 6e63  pository of func
```

