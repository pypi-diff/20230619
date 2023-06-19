# Comparing `tmp/yplib-1.6.6.tar.gz` & `tmp/yplib-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.6.tar", last modified: Mon Jun 19 07:21:13 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.7.tar", last modified: Mon Jun 19 07:59:07 2023, max compression
```

## Comparing `yplib-1.6.6.tar` & `yplib-1.6.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.838218 yplib-1.6.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.6/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 07:21:13.838157 yplib-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 07:21:13.838218 yplib-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 07:18:22.000000 yplib-1.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.834359 yplib-1.6.6/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.6/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.6/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.6/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.6/yplib/http_util.py
--rw-rw-rw-   0        0        0    24707 2023-06-19 07:20:57.000000 yplib-1.6.6/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:21:13.837243 yplib-1.6.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 07:21:13.000000 yplib-1.6.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.428756 yplib-1.6.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 07:59:07.427672 yplib-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:59:07.428756 yplib-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 07:58:52.000000 yplib-1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.425038 yplib-1.6.7/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.7/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.7/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.7/yplib/http_util.py
+-rw-rw-rw-   0        0        0    24804 2023-06-19 07:58:45.000000 yplib-1.6.7/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.427309 yplib-1.6.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.6/LICENSE` & `yplib-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.6/setup.py` & `yplib-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.6",
+  version="1.6.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.6/yplib/chart.py` & `yplib-1.6.7/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.6/yplib/chart_html.py` & `yplib-1.6.7/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.6/yplib/file.py` & `yplib-1.6.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.6/yplib/http_util.py` & `yplib-1.6.7/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.6/yplib/index.py` & `yplib-1.6.7/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,15 @@
                 else:
                     # 指定需要的列
                     if j + 1 in list_index[0]:
                         row_data.append(cell_data)
                         if list_only_one:
                             row_data = cell_data
         data_list.append(row_data)
+    return data_list
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # separator : 是否对每一行进行分割,如果存在这个字段,就分割
 # separator_all : 将文件转化成一个字符串,然后对这个字符串,再次总体分割
 # start_index : 从这个地方开始读取,从1开始标号 , 包含这一行
@@ -695,7 +696,10 @@
 # print(datetime.today())
 # print(datetime.today().strftime('%m%d%H%M_%S_%f'))
 # print(get_file_name('1'))
 #
 # for i in range(100):
 #     print(get_file_name('a'))
 #     # print(random_int(i))
+
+
+# print(json.dumps(to_list(r'C:\Users\yangpu\Desktop\study\12.xls')))
```

