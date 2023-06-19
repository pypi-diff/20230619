# Comparing `tmp/HawaData-0.6.6.tar.gz` & `tmp/HawaData-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.6.6.tar", last modified: Mon Jun 19 09:00:47 2023, max compression
+gzip compressed data, was "HawaData-0.7.0.tar", last modified: Mon Jun 19 09:02:19 2023, max compression
```

## Comparing `HawaData-0.6.6.tar` & `HawaData-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.302327 HawaData-0.6.6/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.291416 HawaData-0.6.6/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:00:47.000000 HawaData-0.6.6/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-19 09:00:47.000000 HawaData-0.6.6/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-19 09:00:47.000000 HawaData-0.6.6/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-19 09:00:47.000000 HawaData-0.6.6/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:00:47.302050 HawaData-0.6.6/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.6.6/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.292131 HawaData-0.6.6/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.6.6/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.294535 HawaData-0.6.6/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.6.6/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.6.6/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.6.6/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.6.6/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.6.6/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.296331 HawaData-0.6.6/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.6.6/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    11184 2023-06-14 03:54:52.000000 HawaData-0.6.6/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.6.6/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.6.6/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.6.6/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.299209 HawaData-0.6.6/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.6.6/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.6.6/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.6.6/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.6.6/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.6.6/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.6.6/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.300858 HawaData-0.6.6/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.6.6/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28118 2023-06-14 03:37:58.000000 HawaData-0.6.6/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.6.6/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-19 09:00:47.302420 HawaData-0.6.6/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.6.6/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:00:47.301421 HawaData-0.6.6/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.6.6/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.252437 HawaData-0.7.0/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.246690 HawaData-0.7.0/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-19 09:02:19.000000 HawaData-0.7.0/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2967 2023-06-19 09:02:19.252207 HawaData-0.7.0/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.0/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.247480 HawaData-0.7.0/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.0/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.248724 HawaData-0.7.0/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.0/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.0/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.0/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.0/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.0/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.249643 HawaData-0.7.0/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.0/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    11184 2023-06-14 03:54:52.000000 HawaData-0.7.0/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.0/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.0/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.7.0/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.250976 HawaData-0.7.0/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.0/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.0/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.0/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.0/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-08 13:01:01.000000 HawaData-0.7.0/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.0/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.251669 HawaData-0.7.0/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.0/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28118 2023-06-14 03:37:58.000000 HawaData-0.7.0/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.0/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-19 09:02:19.252500 HawaData-0.7.0/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.0/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-19 09:02:19.251917 HawaData-0.7.0/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.0/test/test_query.py
```

### Comparing `HawaData-0.6.6/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.0/HawaData.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.6
+Version: 0.7.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -101,8 +101,8 @@
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
-- 0.6.6 use contextmanager to connect db
+- 0.7.0 use contextmanager to connect db
```

### Comparing `HawaData-0.6.6/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.0/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/PKG-INFO` & `HawaData-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.6.6
+Version: 0.7.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -101,8 +101,8 @@
 - 0.5.13 count grade class scores
 - 0.6.0 add student health api data
 - 0.6.1 count dim field scores
 - 0.6.2 count dim field scores 2
 - 0.6.3 count student grade
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
-- 0.6.6 use contextmanager to connect db
+- 0.7.0 use contextmanager to connect db
```

### Comparing `HawaData-0.6.6/README.md` & `HawaData-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/base/db.py` & `HawaData-0.7.0/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/base/init.py` & `HawaData-0.7.0/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/common/data.py` & `HawaData-0.7.0/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/common/query.py` & `HawaData-0.7.0/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/common/utils.py` & `HawaData-0.7.0/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/config.py` & `HawaData-0.7.0/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/data/klass.py` & `HawaData-0.7.0/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/data/school.py` & `HawaData-0.7.0/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/data/student.py` & `HawaData-0.7.0/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/paper/health.py` & `HawaData-0.7.0/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/hawa/paper/mht.py` & `HawaData-0.7.0/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/setup.py` & `HawaData-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.6.6/test/test_query.py` & `HawaData-0.7.0/test/test_query.py`

 * *Files identical despite different names*

