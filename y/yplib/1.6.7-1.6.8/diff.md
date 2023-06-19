# Comparing `tmp/yplib-1.6.7.tar.gz` & `tmp/yplib-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.6.7.tar", last modified: Mon Jun 19 07:59:07 2023, max compression
+gzip compressed data, was "dist\yplib-1.6.8.tar", last modified: Mon Jun 19 09:01:47 2023, max compression
```

## Comparing `yplib-1.6.7.tar` & `yplib-1.6.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.428756 yplib-1.6.7/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.7/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-19 07:59:07.427672 yplib-1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 07:59:07.428756 yplib-1.6.7/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-19 07:58:52.000000 yplib-1.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.425038 yplib-1.6.7/yplib/
--rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.7/yplib/__init__.py
--rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.7/yplib/chart.py
--rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.7/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.7/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.7/yplib/http_util.py
--rw-rw-rw-   0        0        0    24804 2023-06-19 07:58:45.000000 yplib-1.6.7/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:59:07.427309 yplib-1.6.7/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 07:59:07.000000 yplib-1.6.7/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.986600 yplib-1.6.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.6.8/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-19 09:01:47.986115 yplib-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:01:47.986791 yplib-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-19 09:01:42.000000 yplib-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.981691 yplib-1.6.8/yplib/
+-rw-rw-rw-   0        0        0      355 2023-06-19 01:15:00.000000 yplib-1.6.8/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11378 2023-06-16 08:54:15.000000 yplib-1.6.8/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.6.8/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.6.8/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.6.8/yplib/http_util.py
+-rw-rw-rw-   0        0        0    24955 2023-06-19 09:01:29.000000 yplib-1.6.8/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:47.985538 yplib-1.6.8/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 09:01:47.000000 yplib-1.6.8/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.6.7/LICENSE` & `yplib-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.6.7/setup.py` & `yplib-1.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.6.7",
+  version="1.6.8",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.6.7/yplib/chart.py` & `yplib-1.6.8/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.7/yplib/chart_html.py` & `yplib-1.6.8/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.7/yplib/file.py` & `yplib-1.6.8/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.7/yplib/http_util.py` & `yplib-1.6.8/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.6.7/yplib/index.py` & `yplib-1.6.8/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,22 +281,27 @@
     return s
 
 
 # 根据json的key排序,用于签名
 def sort_by_json_key(data_obj):
     return '&'.join(list(map(
         lambda x: f'{x}={data_obj[x]}',
-        sorted(data_obj, key=lambda x: x[0])
+        sorted(data_obj, key=lambda x: x)
     )))
 
 
 # data = {}
 # data['merchantId'] = "merchantId"
 # data['currency'] = "IDR"
+# data['aaccType'] = "payout"
+# data['abccType'] = "payout"
+# data['adcType'] = "payout"
 # data['accType'] = "payout"
+# data['accType1'] = "payout"
+# data['accType2'] = "payout"
 # data['version'] = "1.0"
 # sign = sort_by_json_key(data)
 # print(sign)
 
 
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
```

