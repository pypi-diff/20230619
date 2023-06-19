# Comparing `tmp/yplib-1.5.7.tar.gz` & `tmp/yplib-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.7.tar", last modified: Fri Jun 16 09:00:05 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.8.tar", last modified: Mon Jun 19 00:11:30 2023, max compression
```

## Comparing `yplib-1.5.7.tar` & `yplib-1.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 09:00:05.246719 yplib-1.5.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 09:00:05.246573 yplib-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 09:00:05.247657 yplib-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 08:59:39.000000 yplib-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:00:05.243683 yplib-1.5.7/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.7/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.7/yplib/html_parser.py
--rw-rw-rw-   0        0        0    21075 2023-06-16 08:59:35.000000 yplib-1.5.7/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 09:00:05.245582 yplib-1.5.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 09:00:05.000000 yplib-1.5.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 09:00:05.000000 yplib-1.5.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 09:00:05.000000 yplib-1.5.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 09:00:05.000000 yplib-1.5.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.026224 yplib-1.5.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:11:30.026224 yplib-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 00:11:30.026224 yplib-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 00:11:11.000000 yplib-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.023277 yplib-1.5.8/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.5.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.8/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.8/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    21818 2023-06-19 00:09:12.000000 yplib-1.5.8/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 00:11:30.025318 yplib-1.5.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 00:11:29.000000 yplib-1.5.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.7/LICENSE` & `yplib-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.7/setup.py` & `yplib-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.7",
+  version="1.5.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.7/yplib/chart.py` & `yplib-1.5.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.7/yplib/chart_html.py` & `yplib-1.5.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.7/yplib/file.py` & `yplib-1.5.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.7/yplib/html_parser.py` & `yplib-1.5.8/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.7/yplib/index.py` & `yplib-1.5.8/yplib/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -299,33 +299,28 @@
 # sheet : 从 1 开始编号,
 # column_index : 从 1 开始编号, 指定列
 # column_index : 如果是指定值, 这个时候返回的是一个 list, 没有嵌套 list
 # column_index : 如果是 '1,2,3,4'   [1,2,3,4], 返回的是一个嵌套 list[list]
 # column_date : 指定日期格式的列,规则与 column_index 一样
 # column_datetime : 指定日期格式的列,规则与 column_index 一样
 # 返回的数据一定是一个 list
-################################################
-# r_str : 返回的数据是否是一个 字符串, ''.join(list)
-# r_json : 返回的数据是否是一个 json 类型的数据
 def to_list(file_name='a.txt',
             separator=None,
             separator_all=None,
             start_index=None,
             start_line=None,
             end_index=None,
             end_line=None,
             count=None,
             sheet_index=1,
             column_index=None,
             column_date=None,
-            column_datetime=None,
-            r_json=False,
-            r_str=False):
+            column_datetime=None):
     if file_name is None or file_name == '' or os.path.exists(file_name) is False:
-        return '' if r_str else []
+        return []
     data_list = list()
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         list_index = []
         for one_index in [column_index, column_date, column_datetime]:
             list_index_one = None
             if one_index is not None:
@@ -419,15 +414,38 @@
             c += 1
             if separator is not None:
                 data_list.append(line.split(str(separator)))
             else:
                 data_list.append(line)
         if separator_all is not None:
             data_list = ''.join(data_list).split(str(separator_all))
-    return ''.join(data_list) if r_str else json.loads(''.join(data_list)) if r_json else data_list
+    return data_list
+
+
+# 在 to_list 方法上再嵌套一层,
+# r_str : 返回的数据是否是一个 字符串, ''.join(list)
+# r_json : 返回的数据是否是一个 json 类型的数据
+def to_list_data(file_name='a.txt',
+                 separator=None,
+                 separator_all=None,
+                 start_index=None,
+                 start_line=None,
+                 end_index=None,
+                 end_line=None,
+                 count=None,
+                 sheet_index=1,
+                 column_index=None,
+                 column_date=None,
+                 column_datetime=None,
+                 r_json=False,
+                 r_str=False):
+    d = to_list(file_name=file_name, separator=separator, separator_all=separator_all, start_index=start_index,
+                start_line=start_line, end_index=end_index, end_line=end_line, count=count, sheet_index=sheet_index,
+                column_index=column_index, column_date=column_date, column_datetime=column_datetime)
+    return ''.join(d) if r_str else json.loads(''.join(d)) if r_json else d
 
 
 def to_excel(data_list, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
```

