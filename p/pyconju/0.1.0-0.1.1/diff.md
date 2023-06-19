# Comparing `tmp/pyconju-0.1.0.tar.gz` & `tmp/pyconju-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconju-0.1.0.tar", last modified: Wed Jun 14 21:50:15 2023, max compression
+gzip compressed data, was "pyconju-0.1.1.tar", last modified: Mon Jun 19 15:52:23 2023, max compression
```

## Comparing `pyconju-0.1.0.tar` & `pyconju-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 21:50:15.204211 pyconju-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-06-14 08:43:06.000000 pyconju-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-14 11:07:36.000000 pyconju-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2402 2023-06-14 21:50:15.204211 pyconju-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2023-06-14 21:27:43.000000 pyconju-0.1.0/README.md
--rw-rw-rw-   0        0        0      108 2023-06-14 08:56:44.000000 pyconju-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1115 2023-06-14 21:50:15.212211 pyconju-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 21:50:14.916228 pyconju-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 21:50:15.124216 pyconju-0.1.0/src/pyconju/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:55:38.000000 pyconju-0.1.0/src/pyconju/__init__.py
--rw-rw-rw-   0        0        0      862 2023-06-14 21:23:08.000000 pyconju-0.1.0/src/pyconju/csv.py
--rw-rw-rw-   0        0        0      907 2023-06-14 21:22:28.000000 pyconju-0.1.0/src/pyconju/xls.py
--rw-rw-rw-   0        0        0      835 2023-06-14 21:21:15.000000 pyconju-0.1.0/src/pyconju/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-06-14 21:50:15.188212 pyconju-0.1.0/src/pyconju.egg-info/
--rw-rw-rw-   0        0        0     2402 2023-06-14 21:50:14.000000 pyconju-0.1.0/src/pyconju.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-14 21:50:14.000000 pyconju-0.1.0/src/pyconju.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 21:50:14.000000 pyconju-0.1.0/src/pyconju.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 21:50:14.000000 pyconju-0.1.0/src/pyconju.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 21:50:14.000000 pyconju-0.1.0/src/pyconju.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 21:50:15.196210 pyconju-0.1.0/test/
--rw-rw-rw-   0        0        0      161 2023-06-14 21:16:13.000000 pyconju-0.1.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.317040 pyconju-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-14 08:43:06.000000 pyconju-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-14 11:07:36.000000 pyconju-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2944 2023-06-19 15:52:23.317112 pyconju-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-06-18 07:59:28.000000 pyconju-0.1.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-14 08:56:44.000000 pyconju-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1115 2023-06-19 15:52:23.325221 pyconju-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 15:52:22.709156 pyconju-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.061297 pyconju-0.1.1/src/pyconju/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:55:38.000000 pyconju-0.1.1/src/pyconju/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-06-19 14:06:37.000000 pyconju-0.1.1/src/pyconju/csv.py
+-rw-rw-rw-   0        0        0      906 2023-06-19 14:01:42.000000 pyconju-0.1.1/src/pyconju/xls.py
+-rw-rw-rw-   0        0        0      835 2023-06-19 14:07:21.000000 pyconju-0.1.1/src/pyconju/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.206245 pyconju-0.1.1/src/pyconju.egg-info/
+-rw-rw-rw-   0        0        0     2944 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 15:52:22.000000 pyconju-0.1.1/src/pyconju.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 15:52:23.306859 pyconju-0.1.1/test/
+-rw-rw-rw-   0        0        0      225 2023-06-18 07:34:46.000000 pyconju-0.1.1/test/test_example.py
+-rw-rw-rw-   0        0        0      224 2023-06-19 14:02:59.000000 pyconju-0.1.1/test/test_example2.py
```

### Comparing `pyconju-0.1.0/LICENSE` & `pyconju-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.0/PKG-INFO` & `pyconju-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyconju
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for merging multiple files
 Home-page: https://github.com/dyagee/pyconju
-Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.1.tar.gz
 Author: Agee Aondo
 Author-email: ageeaondo45@gmail.com
 Project-URL: Bugs, https://github.com/dyagee/pyconju/issues
 Project-URL: Docs, https://github.com/dyagee/pyconju/README.md
 Keywords: python3,excel,xls,csv,xlsx,merge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,14 +58,42 @@
 # Initialize object
 merger = Excelx
 path = "path/to/files/to/merge"
 fileList = ["file1.xlsx","file2.xlsx","file3.xlsx"]
 merger.merge_xlsx(fileList,path)
 ```
 
+Out of the box you may encounter this error:
+
+```
+ImportError: Pandas requires version '2.0.1' or newer of 'xlrd' (version '1.2.0' currently installed).
+```
+Don't panic, Uninstall the current version of `xlrd`:
+
+```
+(.venv) $ pip uninstall xlrd
+
+   Found existing installation: xlrd 1.2.0
+   Uninstalling xlrd-1.2.0:
+
+
+   Proceed (Y/n)? y
+   Successfully uninstalled xlrd-1.2.0
+```
+
+Install `xlrd` version `2.0.1`:
+
+```
+(.venv) $ pip install xlrd==2.0.1
+```
+
+**Try the merging process again; it will work**🤩
+
+
+
 ###  Example 2
 ```python
 from pyconju.xls import Excel
 ```
 ```python
 # Initialize object
 merger = Excel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyconju-0.1.0/README.md` & `pyconju-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -35,14 +35,42 @@
 # Initialize object
 merger = Excelx
 path = "path/to/files/to/merge"
 fileList = ["file1.xlsx","file2.xlsx","file3.xlsx"]
 merger.merge_xlsx(fileList,path)
 ```
 
+Out of the box you may encounter this error:
+
+```
+ImportError: Pandas requires version '2.0.1' or newer of 'xlrd' (version '1.2.0' currently installed).
+```
+Don't panic, Uninstall the current version of `xlrd`:
+
+```
+(.venv) $ pip uninstall xlrd
+
+   Found existing installation: xlrd 1.2.0
+   Uninstalling xlrd-1.2.0:
+
+
+   Proceed (Y/n)? y
+   Successfully uninstalled xlrd-1.2.0
+```
+
+Install `xlrd` version `2.0.1`:
+
+```
+(.venv) $ pip install xlrd==2.0.1
+```
+
+**Try the merging process again; it will work**🤩
+
+
+
 ###  Example 2
 ```python
 from pyconju.xls import Excel
 ```
 ```python
 # Initialize object
 merger = Excel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyconju-0.1.0/setup.cfg` & `pyconju-0.1.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f6e 6a75 0d0a 7665 7273   = pyconju..vers
-00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
+00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
 00000030: 686f 7220 3d20 4167 6565 2041 6f6e 646f  hor = Agee Aondo
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2061 6765 6561 6f6e 646f 3435 4067 6d61   ageeaondo45@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5079 7468 6f6e 2070 6163  ion = Python pac
 00000080: 6b61 6765 2066 6f72 206d 6572 6769 6e67  kage for merging
 00000090: 206d 756c 7469 706c 6520 6669 6c65 730d   multiple files.
@@ -16,15 +16,15 @@
 000000f0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
 00000100: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7961  //github.com/dya
 00000110: 6765 652f 7079 636f 6e6a 750d 0a64 6f77  gee/pyconju..dow
 00000120: 6e6c 6f61 645f 7572 6c20 3d20 6874 7470  nload_url = http
 00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
 00000140: 7961 6765 652f 7079 636f 6e6a 752f 6172  yagee/pyconju/ar
 00000150: 6368 6976 652f 7265 6673 2f74 6167 732f  chive/refs/tags/
-00000160: 7630 2e31 2e30 2e74 6172 2e67 7a0d 0a6b  v0.1.0.tar.gz..k
+00000160: 7630 2e31 2e31 2e74 6172 2e67 7a0d 0a6b  v0.1.1.tar.gz..k
 00000170: 6579 776f 7264 7320 3d20 7079 7468 6f6e  eywords = python
 00000180: 332c 2065 7863 656c 2c20 786c 732c 2063  3, excel, xls, c
 00000190: 7376 2c20 786c 7378 2c20 6d65 7267 650d  sv, xlsx, merge.
 000001a0: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
 000001b0: 0d0a 0942 7567 7320 3d20 6874 7470 733a  ...Bugs = https:
 000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7961  //github.com/dya
 000001d0: 6765 652f 7079 636f 6e6a 752f 6973 7375  gee/pyconju/issu
```

### Comparing `pyconju-0.1.0/src/pyconju/csv.py` & `pyconju-0.1.1/src/pyconju/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
             if len(data) != 0:
                 df = pd.concat(data)
                 #create a dataFrame
                 dframe =pd.DataFrame(df)
                 dframe = dframe.iloc[:,2:]
                 hashed = r.randint(1000,9999)
                 hashed = str(hashed)
-                merged_file = f"merged_{hashed}.xlsx"
+                merged_file = f"merged_{hashed}.csv"
                 dframe.to_csv(os.path.join(path,merged_file ),index=False)
```

### Comparing `pyconju-0.1.0/src/pyconju/xls.py` & `pyconju-0.1.1/src/pyconju/xls.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
             if len(data) != 0:
                 df = pd.concat(data)
                 #create a dataFrame
                 dframe =pd.DataFrame(df)
                 dframe = dframe.iloc[:,1:]
                 hashed = r.randint(1000,9999)
                 hashed = str(hashed)
-                merged_file = f"merged_{hashed}.xlsx"
+                merged_file = f"merged_{hashed}.xls"
                 dframe.to_excel(os.path.join(path,merged_file ),engine="openpyxl",index=False)
```

### Comparing `pyconju-0.1.0/src/pyconju/xlsx.py` & `pyconju-0.1.1/src/pyconju/xlsx.py`

 * *Files identical despite different names*

### Comparing `pyconju-0.1.0/src/pyconju.egg-info/PKG-INFO` & `pyconju-0.1.1/src/pyconju.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyconju
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for merging multiple files
 Home-page: https://github.com/dyagee/pyconju
-Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/dyagee/pyconju/archive/refs/tags/v0.1.1.tar.gz
 Author: Agee Aondo
 Author-email: ageeaondo45@gmail.com
 Project-URL: Bugs, https://github.com/dyagee/pyconju/issues
 Project-URL: Docs, https://github.com/dyagee/pyconju/README.md
 Keywords: python3,excel,xls,csv,xlsx,merge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -58,14 +58,42 @@
 # Initialize object
 merger = Excelx
 path = "path/to/files/to/merge"
 fileList = ["file1.xlsx","file2.xlsx","file3.xlsx"]
 merger.merge_xlsx(fileList,path)
 ```
 
+Out of the box you may encounter this error:
+
+```
+ImportError: Pandas requires version '2.0.1' or newer of 'xlrd' (version '1.2.0' currently installed).
+```
+Don't panic, Uninstall the current version of `xlrd`:
+
+```
+(.venv) $ pip uninstall xlrd
+
+   Found existing installation: xlrd 1.2.0
+   Uninstalling xlrd-1.2.0:
+
+
+   Proceed (Y/n)? y
+   Successfully uninstalled xlrd-1.2.0
+```
+
+Install `xlrd` version `2.0.1`:
+
+```
+(.venv) $ pip install xlrd==2.0.1
+```
+
+**Try the merging process again; it will work**🤩
+
+
+
 ###  Example 2
 ```python
 from pyconju.xls import Excel
 ```
 ```python
 # Initialize object
 merger = Excel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

