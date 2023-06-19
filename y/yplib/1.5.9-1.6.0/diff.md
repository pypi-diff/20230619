# Comparing `tmp/yplib-1.5.9.tar.gz` & `tmp/yplib-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.9.tar", last modified: Mon Jun 19 00:52:32 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.0.tar", last modified: Mon Jun 19 00:56:13 2023, max compression
```

## Comparing `yplib-1.5.9.tar` & `yplib-1.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.715611 yplib-1.5.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 00:52:32.715611 yplib-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 00:52:32.715611 yplib-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 00:52:23.000000 yplib-1.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.706293 yplib-1.5.9/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.9/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.9/yplib/html_parser.py
--rw-rw-rw-   0        0        0    24191 2023-06-19 00:51:57.000000 yplib-1.5.9/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 00:52:32.714386 yplib-1.5.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 00:52:32.000000 yplib-1.5.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 00:56:13.949614 yplib-1.6.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:56:13.948614 yplib-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 00:56:13.949851 yplib-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 00:54:48.000000 yplib-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:56:13.945236 yplib-1.6.0/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.6.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.0/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.6.0/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    24344 2023-06-19 00:55:36.000000 yplib-1.6.0/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:56:13.948114 yplib-1.6.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:56:13.000000 yplib-1.6.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-19 00:56:13.000000 yplib-1.6.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:56:13.000000 yplib-1.6.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 00:56:13.000000 yplib-1.6.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.9/LICENSE` & `yplib-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.9/setup.py` & `yplib-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.9",
+  version="1.6.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.9/yplib/chart.py` & `yplib-1.6.0/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.9/yplib/chart_html.py` & `yplib-1.6.0/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.9/yplib/file.py` & `yplib-1.6.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.9/yplib/html_parser.py` & `yplib-1.6.0/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.9/yplib/index.py` & `yplib-1.6.0/yplib/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -487,17 +487,26 @@
                  count=None,
                  sheet_index=1,
                  column_index=None,
                  column_date=None,
                  column_datetime=None,
                  r_json=False,
                  r_str=False):
-    d = to_list(file_name=file_name, separator=separator, separator_all=separator_all, start_index=start_index,
-                start_line=start_line, end_index=end_index, end_line=end_line, count=count, sheet_index=sheet_index,
-                column_index=column_index, column_date=column_date, column_datetime=column_datetime)
+    d = to_list(file_name=file_name,
+                separator=separator,
+                separator_all=separator_all,
+                start_index=start_index,
+                start_line=start_line,
+                end_index=end_index,
+                end_line=end_line,
+                count=count,
+                sheet_index=sheet_index,
+                column_index=column_index,
+                column_date=column_date,
+                column_datetime=column_datetime)
     return ''.join(d) if r_str else json.loads(''.join(d)) if r_json else d
 
 
 def to_excel(data_list, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
```

