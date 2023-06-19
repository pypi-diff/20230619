# Comparing `tmp/pyrestack-0.0.27-py3-none-any.whl.zip` & `tmp/pyrestack-0.0.28-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5407 bytes, number of entries: 11
--rw-r--r--  2.0 unx      140 b- defN 23-Jun-12 19:11 pyrestack/__init__.py
--rw-r--r--  2.0 unx      104 b- defN 23-Jun-12 19:11 pyrestack/const.py
--rw-r--r--  2.0 unx     2732 b- defN 23-Jun-12 19:11 pyrestack/decorator.py
--rw-r--r--  2.0 unx      293 b- defN 23-Jun-12 19:11 pyrestack/exceptions.py
--rw-r--r--  2.0 unx     4245 b- defN 23-Jun-12 19:11 pyrestack/models.py
--rw-r--r--  2.0 unx      848 b- defN 23-Jun-12 19:11 pyrestack/restack.py
--rw-r--r--  2.0 unx     1627 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/zip-safe
--rw-rw-r--  2.0 unx      860 b- defN 23-Jun-12 19:11 pyrestack-0.0.27.dist-info/RECORD
-11 files, 10952 bytes uncompressed, 3953 bytes compressed:  63.9%
+Zip file size: 5405 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-19 10:39 pyrestack/__init__.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-19 10:39 pyrestack/const.py
+-rw-r--r--  2.0 unx     2732 b- defN 23-Jun-19 10:39 pyrestack/decorator.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-19 10:39 pyrestack/exceptions.py
+-rw-r--r--  2.0 unx     4245 b- defN 23-Jun-19 10:39 pyrestack/models.py
+-rw-r--r--  2.0 unx      848 b- defN 23-Jun-19 10:39 pyrestack/restack.py
+-rw-r--r--  2.0 unx     1627 b- defN 23-Jun-19 10:40 pyrestack-0.0.28.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 10:40 pyrestack-0.0.28.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-19 10:40 pyrestack-0.0.28.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-19 10:40 pyrestack-0.0.28.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      860 b- defN 23-Jun-19 10:40 pyrestack-0.0.28.dist-info/RECORD
+11 files, 10952 bytes uncompressed, 3951 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyrestack/models.py
 Comment: 
 
 Filename: pyrestack/restack.py
 Comment: 
 
-Filename: pyrestack-0.0.27.dist-info/METADATA
+Filename: pyrestack-0.0.28.dist-info/METADATA
 Comment: 
 
-Filename: pyrestack-0.0.27.dist-info/WHEEL
+Filename: pyrestack-0.0.28.dist-info/WHEEL
 Comment: 
 
-Filename: pyrestack-0.0.27.dist-info/top_level.txt
+Filename: pyrestack-0.0.28.dist-info/top_level.txt
 Comment: 
 
-Filename: pyrestack-0.0.27.dist-info/zip-safe
+Filename: pyrestack-0.0.28.dist-info/zip-safe
 Comment: 
 
-Filename: pyrestack-0.0.27.dist-info/RECORD
+Filename: pyrestack-0.0.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyrestack/__init__.py

```diff
@@ -1,7 +1,7 @@
 """Python API wrapper for ReStack."""
 from .exceptions import *
 from .models import *
 from .restack import ReStack
 
-__version__ = '0.0.27'
+__version__ = '0.0.28'
```

## Comparing `pyrestack-0.0.27.dist-info/METADATA` & `pyrestack-0.0.28.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestack
-Version: 0.0.27
+Version: 0.0.28
 Summary: Simple Python wrapper for ReStack
 Home-page: https://github.com/elentriek/restack-integration
 Author: Floris Heyvaert
 Author-email: floris.heyvaert@gmail.com
 License: MIT License
 Keywords: pyrestack,setuptools
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyrestack-0.0.27.dist-info/RECORD` & `pyrestack-0.0.28.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyrestack/__init__.py,sha256=5NUFcfPtGZ4KFtwujLNIOSCcKCenVOd2moGLEbb_NsM,140
+pyrestack/__init__.py,sha256=J-69iznAMEqoDoNs87uypFul14YMRQGV6mH5bIKLIlU,140
 pyrestack/const.py,sha256=Azb3PK-Q14OO2gKZKye26wcvYPNh7FOOo199lxOER0I,104
 pyrestack/decorator.py,sha256=m7qlhwAWH8i-UJ_1tuVR2hHx4VMNz4VOt-hRmOY39tg,2732
 pyrestack/exceptions.py,sha256=xgSXiqEV6hkZdyto34O-viuh4fKGtz0jkwtjgOR0iaw,293
 pyrestack/models.py,sha256=HNiPOampZ5jtMwy43UMOzskWvYxvwkSP6f_wIJsE12M,4245
 pyrestack/restack.py,sha256=miJXa4QOaHIoNin9n31gV2M1DWBYsjmAw1ZGZxSelBU,848
-pyrestack-0.0.27.dist-info/METADATA,sha256=7SrGKmEfVKvAPuHb6Gcsv7jXAuus1eqSIZ_bA-N08tg,1627
-pyrestack-0.0.27.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyrestack-0.0.27.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
-pyrestack-0.0.27.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyrestack-0.0.27.dist-info/RECORD,,
+pyrestack-0.0.28.dist-info/METADATA,sha256=2X6odK55xWlLEdORE_4kFwWV3H4Ombf8Zj02pKD3QFA,1627
+pyrestack-0.0.28.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyrestack-0.0.28.dist-info/top_level.txt,sha256=9EZedki-jXfc4k1T9TZf0OmFcf8YN5xHRyCkZj0Xhgo,10
+pyrestack-0.0.28.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyrestack-0.0.28.dist-info/RECORD,,
```

