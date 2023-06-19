# Comparing `tmp/popv-0.3.1.tar.gz` & `tmp/popv-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popv-0.3.1.tar", max compression
+gzip compressed data, was "popv-0.3.2.tar", max compression
```

## Comparing `popv-0.3.1.tar` & `popv-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-11 09:15:47.360637 popv-0.3.1/LICENSE
--rw-r--r--   0        0        0     6433 2023-06-16 20:33:37.835718 popv-0.3.1/README.md
--rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.3.1/popv/__init__.py
--rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.3.1/popv/_settings.py
--rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.3.1/popv/_utils.py
--rw-r--r--   0        0        0      545 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/__init__.py
--rw-r--r--   0        0        0     3895 2023-06-16 05:47:18.932309 popv-0.3.1/popv/algorithms/_bbknn.py
--rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.3.1/popv/algorithms/_celltypist.py
--rw-r--r--   0        0        0     3659 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_harmony.py
--rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.3.1/popv/algorithms/_onclass.py
--rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.3.1/popv/algorithms/_rf.py
--rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.3.1/popv/algorithms/_scaffold_algorithm.py
--rw-r--r--   0        0        0     3869 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_scanorama.py
--rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.3.1/popv/algorithms/_scanvi.py
--rw-r--r--   0        0        0     7072 2023-06-16 20:34:23.400203 popv-0.3.1/popv/algorithms/_scvi.py
--rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.3.1/popv/algorithms/_svm.py
--rw-r--r--   0        0        0    11096 2023-06-16 20:34:23.400203 popv-0.3.1/popv/annotation.py
--rw-r--r--   0        0        0    16786 2023-06-16 20:34:23.400203 popv-0.3.1/popv/preprocessing.py
--rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.3.1/popv/reproducibility/_accuracy.py
--rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.3.1/popv/reproducibility/_alluvial.py
--rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.3.1/popv/visualization.py
--rw-r--r--   0        0        0     4630 2023-06-16 20:34:53.708526 popv-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8747 1970-01-01 00:00:00.000000 popv-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-11 09:15:47.360637 popv-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6433 2023-06-16 20:33:37.835718 popv-0.3.2/README.md
+-rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.3.2/popv/__init__.py
+-rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.3.2/popv/_settings.py
+-rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.3.2/popv/_utils.py
+-rw-r--r--   0        0        0      545 2023-06-16 20:34:23.400203 popv-0.3.2/popv/algorithms/__init__.py
+-rw-r--r--   0        0        0     3895 2023-06-16 05:47:18.932309 popv-0.3.2/popv/algorithms/_bbknn.py
+-rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.3.2/popv/algorithms/_celltypist.py
+-rw-r--r--   0        0        0     3659 2023-06-16 20:34:23.400203 popv-0.3.2/popv/algorithms/_harmony.py
+-rw-r--r--   0        0        0     7544 2023-06-19 10:46:10.258629 popv-0.3.2/popv/algorithms/_onclass.py
+-rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.3.2/popv/algorithms/_rf.py
+-rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.3.2/popv/algorithms/_scaffold_algorithm.py
+-rw-r--r--   0        0        0     3869 2023-06-16 20:34:23.400203 popv-0.3.2/popv/algorithms/_scanorama.py
+-rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.3.2/popv/algorithms/_scanvi.py
+-rw-r--r--   0        0        0     7072 2023-06-16 20:34:23.400203 popv-0.3.2/popv/algorithms/_scvi.py
+-rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.3.2/popv/algorithms/_svm.py
+-rw-r--r--   0        0        0    11096 2023-06-16 20:34:23.400203 popv-0.3.2/popv/annotation.py
+-rw-r--r--   0        0        0    16786 2023-06-16 20:34:23.400203 popv-0.3.2/popv/preprocessing.py
+-rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.3.2/popv/reproducibility/_accuracy.py
+-rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.3.2/popv/reproducibility/_alluvial.py
+-rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.3.2/popv/visualization.py
+-rw-r--r--   0        0        0     4635 2023-06-19 10:50:10.444801 popv-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8752 1970-01-01 00:00:00.000000 popv-0.3.2/PKG-INFO
```

### Comparing `popv-0.3.1/LICENSE` & `popv-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/README.md` & `popv-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/__init__.py` & `popv-0.3.2/popv/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/_settings.py` & `popv-0.3.2/popv/_settings.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/_utils.py` & `popv-0.3.2/popv/_utils.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/__init__.py` & `popv-0.3.2/popv/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_bbknn.py` & `popv-0.3.2/popv/algorithms/_bbknn.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_celltypist.py` & `popv-0.3.2/popv/algorithms/_celltypist.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_harmony.py` & `popv-0.3.2/popv/algorithms/_harmony.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_onclass.py` & `popv-0.3.2/popv/algorithms/_onclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         """
         ontology_id = []
 
         for label in adata.obs[self.labels_key]:
             if label != adata.uns["unknown_celltype_label"]:
                 if label not in celltype_dict:
                     logging.warning("Following label not in celltype_dict ", label)
+                    ontology_id.append("unknown")
                 ontology_id.append(celltype_dict[label])
             else:
                 ontology_id.append("unknown")
 
         adata.obs[ontology_key] = ontology_id
 
     def compute_integration(self, adata):
```

### Comparing `popv-0.3.1/popv/algorithms/_rf.py` & `popv-0.3.2/popv/algorithms/_rf.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_scaffold_algorithm.py` & `popv-0.3.2/popv/algorithms/_scaffold_algorithm.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_scanorama.py` & `popv-0.3.2/popv/algorithms/_scanorama.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_scanvi.py` & `popv-0.3.2/popv/algorithms/_scanvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_scvi.py` & `popv-0.3.2/popv/algorithms/_scvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/algorithms/_svm.py` & `popv-0.3.2/popv/algorithms/_svm.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/annotation.py` & `popv-0.3.2/popv/annotation.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/preprocessing.py` & `popv-0.3.2/popv/preprocessing.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/reproducibility/_accuracy.py` & `popv-0.3.2/popv/reproducibility/_accuracy.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/reproducibility/_alluvial.py` & `popv-0.3.2/popv/reproducibility/_alluvial.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/popv/visualization.py` & `popv-0.3.2/popv/visualization.py`

 * *Files identical despite different names*

### Comparing `popv-0.3.1/pyproject.toml` & `popv-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 description = "Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods."
 packages = [
   {include = "popv"},
 ]
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anndata = "^0.8"
 bbknn = "^1.5.1"
 black = {version = ">=22.3", optional = true}
@@ -44,15 +44,15 @@
 jupyter = {version = ">=1.0", optional = true}
 Markdown = "3.3.4"
 nbconvert = {version = ">=5.4.0", optional = true}
 nbformat = {version = ">=4.4.0", optional = true}
 nbsphinx = {version = "*", optional = true}
 nbsphinx-link = {version = "*", optional = true}
 onclass = "^1.2"
-pandas = ">=1.4"
+pandas = ">=1.4,<2.0"
 pre-commit = {version = ">=2.7.1", optional = true}
 pytest = {version = ">=4.4", optional = true}
 rich = ">=9.1.0"
 scanorama = "^1.7.3"
 scanpy = "^1.9.1"
 scikit-learn = ">0.21.2,<1.0"
 scikit-misc = ">=0.1"
```

### Comparing `popv-0.3.1/PKG-INFO` & `popv-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popv
-Version: 0.3.1
+Version: 0.3.2
 Summary: Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.
 License: BSD-3-Clause
 Author: Galen Xing
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -36,15 +36,15 @@
 Requires-Dist: jupyter (>=1.0) ; extra == "dev"
 Requires-Dist: nbconvert (>=5.4.0) ; extra == "dev"
 Requires-Dist: nbformat (>=4.4.0) ; extra == "dev"
 Requires-Dist: nbsphinx
 Requires-Dist: nbsphinx-link
 Requires-Dist: obonet (>=1.0,<2.0)
 Requires-Dist: onclass (>=1.2,<2.0)
-Requires-Dist: pandas (>=1.4)
+Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: pre-commit (>=2.7.1) ; extra == "dev"
 Requires-Dist: pytest (>=4.4) ; extra == "dev"
 Requires-Dist: rich (>=9.1.0)
 Requires-Dist: scanorama (>=1.7.3,<2.0.0)
 Requires-Dist: scanpy (>=1.9.1,<2.0.0)
 Requires-Dist: scikit-learn (>0.21.2,<1.0)
 Requires-Dist: scikit-misc (>=0.1)
```

