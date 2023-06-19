# Comparing `tmp/genepierre-0.0.2.tar.gz` & `tmp/genepierre-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.0.2.tar", last modified: Mon Jun 19 11:45:54 2023, max compression
+gzip compressed data, was "genepierre-0.0.3.tar", last modified: Mon Jun 19 11:54:28 2023, max compression
```

## Comparing `genepierre-0.0.2.tar` & `genepierre-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 11:45:54.827140 genepierre-0.0.2/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      527 2023-06-19 11:45:54.827140 genepierre-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-06-19 11:30:27.000000 genepierre-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      535 2023-06-19 11:45:54.829139 genepierre-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 11:45:54.810892 genepierre-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 11:45:54.826133 genepierre-0.0.2/src/genepierre.egg-info/
--rw-rw-rw-   0        0        0      527 2023-06-19 11:45:54.000000 genepierre-0.0.2/src/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-19 11:45:54.000000 genepierre-0.0.2/src/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 11:45:54.000000 genepierre-0.0.2/src/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 11:45:54.000000 genepierre-0.0.2/src/genepierre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 11:45:54.827140 genepierre-0.0.2/src/genetic/
--rw-rw-rw-   0        0        0        0 2023-06-19 11:26:15.000000 genepierre-0.0.2/src/genetic/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-06-19 11:26:27.000000 genepierre-0.0.2/src/genetic/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:54:28.042561 genepierre-0.0.3/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      527 2023-06-19 11:54:28.042561 genepierre-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-19 11:30:27.000000 genepierre-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      535 2023-06-19 11:54:28.044474 genepierre-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 11:54:28.025116 genepierre-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 11:54:28.042561 genepierre-0.0.3/src/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-06-19 11:54:28.000000 genepierre-0.0.3/src/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-19 11:54:28.000000 genepierre-0.0.3/src/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:54:28.000000 genepierre-0.0.3/src/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:54:28.000000 genepierre-0.0.3/src/genepierre.egg-info/top_level.txt
```

### Comparing `genepierre-0.0.2/LICENSE.txt` & `genepierre-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.2/PKG-INFO` & `genepierre-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.2
+Version: 0.0.3
 Summary: Genetic Algorithm BaseCode
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `genepierre-0.0.2/setup.cfg` & `genepierre-0.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 656e 6570 6965 7272 650d 0a76   = genepierre..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
 00000030: 6175 7468 6f72 203d 2047 6175 7469 6572  author = Gautier
 00000040: 204c 6169 736e c3a9 0d0a 6175 7468 6f72   Laisn....author
 00000050: 5f65 6d61 696c 203d 2067 6175 7469 6572  _email = gautier
 00000060: 2e6c 6169 736e 6540 696e 7269 612e 6672  .laisne@inria.fr
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4765 6e65 7469 6320 416c 676f 7269 7468  Genetic Algorith
 00000090: 6d20 4261 7365 436f 6465 0d0a 6c6f 6e67  m BaseCode..long
```

### Comparing `genepierre-0.0.2/src/genepierre.egg-info/PKG-INFO` & `genepierre-0.0.3/src/genepierre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.2
+Version: 0.0.3
 Summary: Genetic Algorithm BaseCode
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

