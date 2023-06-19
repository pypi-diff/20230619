# Comparing `tmp/tablepic-0.0.2.tar.gz` & `tmp/tablepic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepic-0.0.2.tar", last modified: Fri Jun 16 07:37:04 2023, max compression
+gzip compressed data, was "tablepic-0.0.3.tar", last modified: Mon Jun 19 02:58:28 2023, max compression
```

## Comparing `tablepic-0.0.2.tar` & `tablepic-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.646560 tablepic-0.0.2/
--rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.2/LICENSE
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-16 07:37:04.646405 tablepic-0.0.2/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)    15511 2023-06-16 07:22:07.000000 tablepic-0.0.2/README.md
--rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-16 07:36:53.000000 tablepic-0.0.2/pyproject.toml
--rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.2/readme_pypi.md
--rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-16 07:37:04.646605 tablepic-0.0.2/setup.cfg
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.644746 tablepic-0.0.2/src/
--rw-r--r--   0 xinyan     (501) staff       (20)     8232 2023-06-16 07:25:04.000000 tablepic-0.0.2/src/demo.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.645419 tablepic-0.0.2/src/tablepic/
--rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.2/src/tablepic/__init__.py
--rw-r--r--   0 xinyan     (501) staff       (20)    15925 2023-06-16 07:20:40.000000 tablepic-0.0.2/src/tablepic/main.py
-drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-16 07:37:04.646201 tablepic-0.0.2/src/tablepic.egg-info/
--rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/PKG-INFO
--rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/SOURCES.txt
--rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/dependency_links.txt
--rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-16 07:37:04.000000 tablepic-0.0.2/src/tablepic.egg-info/top_level.txt
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.147264 tablepic-0.0.3/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1066 2023-06-16 07:22:57.000000 tablepic-0.0.3/LICENSE
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-19 02:58:28.147097 tablepic-0.0.3/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)    15596 2023-06-16 07:44:46.000000 tablepic-0.0.3/README.md
+-rw-r--r--   0 xinyan     (501) staff       (20)      604 2023-06-19 02:56:56.000000 tablepic-0.0.3/pyproject.toml
+-rw-r--r--   0 xinyan     (501) staff       (20)      498 2023-06-16 07:33:42.000000 tablepic-0.0.3/readme_pypi.md
+-rw-r--r--   0 xinyan     (501) staff       (20)       38 2023-06-19 02:58:28.147349 tablepic-0.0.3/setup.cfg
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.145267 tablepic-0.0.3/src/
+-rw-r--r--   0 xinyan     (501) staff       (20)     8232 2023-06-16 07:25:04.000000 tablepic-0.0.3/src/demo.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.146041 tablepic-0.0.3/src/tablepic/
+-rw-r--r--   0 xinyan     (501) staff       (20)      167 2023-06-14 15:44:10.000000 tablepic-0.0.3/src/tablepic/__init__.py
+-rw-r--r--   0 xinyan     (501) staff       (20)    15925 2023-06-16 07:20:40.000000 tablepic-0.0.3/src/tablepic/main.py
+drwxr-xr-x   0 xinyan     (501) staff       (20)        0 2023-06-19 02:58:28.146899 tablepic-0.0.3/src/tablepic.egg-info/
+-rw-r--r--   0 xinyan     (501) staff       (20)     1025 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/PKG-INFO
+-rw-r--r--   0 xinyan     (501) staff       (20)      249 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/SOURCES.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)        1 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/dependency_links.txt
+-rw-r--r--   0 xinyan     (501) staff       (20)       14 2023-06-19 02:58:28.000000 tablepic-0.0.3/src/tablepic.egg-info/top_level.txt
```

### Comparing `tablepic-0.0.2/LICENSE` & `tablepic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.2/PKG-INFO` & `tablepic-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: xinyan
  * @Date: 2023-06-16 15:32:25
  * @LastEditors: xinyan
```

### Comparing `tablepic-0.0.2/README.md` & `tablepic-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 <!--
  * @Author: xinyan
  * @Date: 2023-06-15 15:11:57
  * @LastEditors: xinyan
- * @LastEditTime: 2023-06-16 15:22:05
+ * @LastEditTime: 2023-06-16 15:44:45
  * @Description: file content
 -->
 
 # TablePic
 ## Overview
 This package uses PIL (pillow) to generate a picture that contains a table. It has similar functionality to matplotlib's table, but includes more customization options.
 
+## Installation
+
+Use pip to install the package.
+
+```shell
+pip install tablepic
+```
+
 ## Instruction
 
 ### Basic Table
 
 The following code generate a basic table picture, it contains a title and a 10*8 regular table. The table has 1 header row and 9 data rows.
 
 ```python
```

### Comparing `tablepic-0.0.2/pyproject.toml` & `tablepic-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablepic"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Xin Yan", email="slash.xin@gmail.com" },
 ]
 description = "A package can generate a picture which contains a table."
 readme = "readme_pypi.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `tablepic-0.0.2/src/demo.py` & `tablepic-0.0.3/src/demo.py`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.2/src/tablepic/main.py` & `tablepic-0.0.3/src/tablepic/main.py`

 * *Files identical despite different names*

### Comparing `tablepic-0.0.2/src/tablepic.egg-info/PKG-INFO` & `tablepic-0.0.3/src/tablepic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tablepic
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package can generate a picture which contains a table.
 Author-email: Xin Yan <slash.xin@gmail.com>
 Project-URL: Homepage, https://github.com/slash-xin/tablepic
 Project-URL: Bug Tracker, https://github.com/slash-xin/tablepic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
  * @Author: xinyan
  * @Date: 2023-06-16 15:32:25
  * @LastEditors: xinyan
```

