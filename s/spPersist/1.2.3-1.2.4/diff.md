# Comparing `tmp/sppersist-1.2.3.tar.gz` & `tmp/sppersist-1.2.4.tar.gz`

## Comparing `sppersist-1.2.3.tar` & `sppersist-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/ph.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.3/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.3/README.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/ph.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 sppersist-1.2.4/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.4/README.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.4/PKG-INFO
```

### Comparing `sppersist-1.2.3/src/spPersist/DTM_filtrations.py` & `sppersist-1.2.4/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/src/spPersist/dp.py` & `sppersist-1.2.4/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/src/spPersist/hc.py` & `sppersist-1.2.4/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/src/spPersist/persistence_statistics.py` & `sppersist-1.2.4/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/src/spPersist/ph.py` & `sppersist-1.2.4/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/src/spPersist/pp.py` & `sppersist-1.2.4/src/spPersist/pp.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,18 +124,32 @@
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     adata = adata[adata.obs["pct_counts_mt"] < p]
     print(f"#cells after MT filter: {adata.n_obs}")
 
 
+def extract_human_brain_reference():
+  '''
+  extract_human_brain_reference returns the median gene expression by
+  cluster from the dataset Allen Institute for Brain Science (2021). 
+  Allen Cell Types Database -- Human Multiple Cortical Areas.
+  '''
+
+  url = 'https://idk-etl-prod-download-bucket.s3.amazonaws.com/aibs_human_ctx_smart-seq/medians.csv'
+  df = pd.read_csv(url,index_col='feature')
+
+  return df
+
+
 def extract_mouse_brain_reference():
   '''
   extract_mouse_brain_reference returns the median gene expression by
-  cluster, as a pandas dataframe, from the Yao Z et al.
+  cluster from the dataset Allen Institute for Brain Science (2020). 
+  Allen Cell Types Database -- Mouse Whole Cortex and Hippocampus-10x Genomics.
   '''
 
   url = 'https://idk-etl-prod-download-bucket.s3.amazonaws.com/aibs_mouse_ctx-hpf_10x/medians.csv'
   df = pd.read_csv(url,index_col='feature')
 
   return df
```

### Comparing `sppersist-1.2.3/LICENSE` & `sppersist-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/README.md` & `sppersist-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.3/pyproject.toml` & `sppersist-1.2.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.2.3/PKG-INFO` & `sppersist-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.2.3
+Version: 1.2.4
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

