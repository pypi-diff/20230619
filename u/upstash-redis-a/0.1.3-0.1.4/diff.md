# Comparing `tmp/upstash_redis_a-0.1.3.tar.gz` & `tmp/upstash_redis_a-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis_a-0.1.3.tar", max compression
+gzip compressed data, was "upstash_redis_a-0.1.4.tar", max compression
```

## Comparing `upstash_redis_a-0.1.3.tar` & `upstash_redis_a-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.3/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.3/README.md
--rw-r--r--   0        0        0      388 2023-06-19 01:59:41.682445 upstash_redis_a-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.3/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.3/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0    84492 2023-06-19 01:59:04.278103 upstash_redis_a-0.1.3/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.3/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.3/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-06-19 01:44:49.341538 upstash_redis_a-0.1.3/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     3205 2023-06-19 01:48:51.048556 upstash_redis_a-0.1.3/upstash_redis/http/execute.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.3/upstash_redis/py.typed
--rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.3/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1174 2023-06-19 01:49:10.086585 upstash_redis_a-0.1.3/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-06-19 01:44:21.139360 upstash_redis_a-0.1.3/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.3/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.3/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.3/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.3/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     3987 2023-06-19 01:48:34.322720 upstash_redis_a-0.1.3/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9702 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.4/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.4/README.md
+-rw-r--r--   0        0        0      388 2023-06-19 02:20:57.987838 upstash_redis_a-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.4/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.4/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0    84492 2023-06-19 01:59:04.278103 upstash_redis_a-0.1.4/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.4/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.4/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-06-19 01:44:49.341538 upstash_redis_a-0.1.4/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     3205 2023-06-19 01:48:51.048556 upstash_redis_a-0.1.4/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.4/upstash_redis/py.typed
+-rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.4/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1174 2023-06-19 01:49:10.086585 upstash_redis_a-0.1.4/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-06-19 01:44:21.139360 upstash_redis_a-0.1.4/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.4/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.4/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.4/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.4/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     3987 2023-06-19 01:48:34.322720 upstash_redis_a-0.1.4/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9752 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.4/PKG-INFO
```

### Comparing `upstash_redis_a-0.1.3/LICENSE` & `upstash_redis_a-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/README.md` & `upstash_redis_a-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/asyncio/client.py` & `upstash_redis_a-0.1.4/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/http/decode.py` & `upstash_redis_a-0.1.4/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/http/execute.py` & `upstash_redis_a-0.1.4/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/schema/commands/returns.py` & `upstash_redis_a-0.1.4/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/schema/http.py` & `upstash_redis_a-0.1.4/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/utils/exception.py` & `upstash_redis_a-0.1.4/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/upstash_redis/utils/format.py` & `upstash_redis_a-0.1.4/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.3/PKG-INFO` & `upstash_redis_a-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: upstash-redis-a
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
```

