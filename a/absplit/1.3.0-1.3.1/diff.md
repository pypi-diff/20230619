# Comparing `tmp/absplit-1.3.0.tar.gz` & `tmp/absplit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.3.0.tar` & `absplit-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.3.0/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.3.0/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.3.0/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.3.0/MANIFEST.in
--rw-r--r--   0        0        0     7816 2023-06-18 23:20:04.805000 absplit-1.3.0/README.md
--rw-r--r--   0        0        0       93 2023-06-18 23:20:04.840000 absplit-1.3.0/absplit/__init__.py
--rw-r--r--   0        0        0     8940 2023-06-14 19:51:59.610000 absplit-1.3.0/absplit/data.py
--rw-r--r--   0        0        0    25425 2023-06-18 23:15:55.977000 absplit-1.3.0/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.3.0/absplit/param.py
--rw-r--r--   0        0        0     3976 2023-06-18 21:48:19.019000 absplit-1.3.0/absplit/tutorials.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.3.0/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-18 23:20:04.770000 absplit-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.3.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.3.0/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.3.0/tests/test_ga.py
--rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 absplit-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.3.1/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.3.1/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.3.1/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.3.1/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.3.1/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.3.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.3.1/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.3.1/MANIFEST.in
+-rw-r--r--   0        0        0     7816 2023-06-18 23:24:24.991000 absplit-1.3.1/README.md
+-rw-r--r--   0        0        0       93 2023-06-18 23:24:25.025000 absplit-1.3.1/absplit/__init__.py
+-rw-r--r--   0        0        0     8940 2023-06-14 19:51:59.610000 absplit-1.3.1/absplit/data.py
+-rw-r--r--   0        0        0    25425 2023-06-18 23:15:55.977000 absplit-1.3.1/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.3.1/absplit/param.py
+-rw-r--r--   0        0        0     3995 2023-06-18 23:23:52.087000 absplit-1.3.1/absplit/tutorials.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.3.1/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-18 23:24:24.953000 absplit-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.3.1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.3.1/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.3.1/tests/test_ga.py
+-rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 absplit-1.3.1/PKG-INFO
```

### Comparing `absplit-1.3.0/.gitignore` & `absplit-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/LICENSE` & `absplit-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/README.md` & `absplit-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.3.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.3.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.3.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

### Comparing `absplit-1.3.0/absplit/data.py` & `absplit-1.3.1/absplit/data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/absplit/ga.py` & `absplit-1.3.1/absplit/ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/absplit/param.py` & `absplit-1.3.1/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/absplit/tutorials.py` & `absplit-1.3.1/absplit/tutorials.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
     df.loc[:, 'deaths'] = df['deaths'].astype(int)
     if drop_fips:
         df = df.drop('fips', axis=1)
     else:
         df = df[~df['fips'].isna()].reset_index(drop=True)
         df['fips'] = df['fips'].astype('int64').astype(str)
     cols = ['state', 'county', 'date']
-    cols = cols + ['fips'] if not drop_fips else []
+    cols = cols + ['fips'] if not drop_fips else cols
+    print(cols)
     df = df.set_index(cols).sort_index()
     df = df.groupby(level=[0, 1]).diff().fillna(0).clip(lower=0)
     resampler = lambda x: x.set_index('date').resample('w').sum()
     df = df.reset_index(level=2).groupby([x for x in cols if x != 'date']).apply(resampler).reset_index()
     return df
```

### Comparing `absplit-1.3.0/images/logo.jpeg` & `absplit-1.3.1/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/pyproject.toml` & `absplit-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.3.0"
+version = "1.3.1"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.3.0/tests/test_data.py` & `absplit-1.3.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/tests/test_ga.py` & `absplit-1.3.1/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.0/PKG-INFO` & `absplit-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.3.0
+Version: 1.3.1
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.3.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.3.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.3.0 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.3.1 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.3.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.3.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

