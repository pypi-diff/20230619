# Comparing `tmp/upstash_redis_a-0.1.1.tar.gz` & `tmp/upstash_redis_a-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis_a-0.1.1.tar", max compression
+gzip compressed data, was "upstash_redis_a-0.1.2.tar", max compression
```

## Comparing `upstash_redis_a-0.1.1.tar` & `upstash_redis_a-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.1/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.1/README.md
--rw-r--r--   0        0        0      388 2023-06-19 01:20:59.479851 upstash_redis_a-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.1/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.1/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0    84480 2023-06-19 01:12:18.616114 upstash_redis_a-0.1.1/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.1/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.1/upstash_redis/exception.py
--rw-r--r--   0        0        0      810 2023-06-18 23:12:23.110853 upstash_redis_a-0.1.1/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     3152 2023-06-19 00:52:08.126910 upstash_redis_a-0.1.1/upstash_redis/http/execute.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.1/upstash_redis/py.typed
--rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.1/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1162 2023-06-19 00:16:53.116217 upstash_redis_a-0.1.1/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      746 2023-06-19 00:53:00.198997 upstash_redis_a-0.1.1/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.1/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.1/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.1/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.1/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     3975 2023-06-19 01:03:54.283305 upstash_redis_a-0.1.1/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9702 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis_a-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis_a-0.1.2/README.md
+-rw-r--r--   0        0        0      388 2023-06-19 01:31:20.512293 upstash_redis_a-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-06-18 23:12:23.109932 upstash_redis_a-0.1.2/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-18 23:12:23.110093 upstash_redis_a-0.1.2/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0    84480 2023-06-19 01:12:18.616114 upstash_redis_a-0.1.2/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis_a-0.1.2/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis_a-0.1.2/upstash_redis/exception.py
+-rw-r--r--   0        0        0      810 2023-06-18 23:12:23.110853 upstash_redis_a-0.1.2/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     3193 2023-06-19 01:31:04.187754 upstash_redis_a-0.1.2/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:37.096890 upstash_redis_a-0.1.2/upstash_redis/py.typed
+-rw-r--r--   0        0        0      431 2023-06-19 00:14:29.039876 upstash_redis_a-0.1.2/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1162 2023-06-19 00:16:53.116217 upstash_redis_a-0.1.2/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      746 2023-06-19 00:53:00.198997 upstash_redis_a-0.1.2/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis_a-0.1.2/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis_a-0.1.2/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis_a-0.1.2/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-19 00:09:55.671307 upstash_redis_a-0.1.2/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     3975 2023-06-19 01:29:27.403905 upstash_redis_a-0.1.2/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9702 1970-01-01 00:00:00.000000 upstash_redis_a-0.1.2/PKG-INFO
```

### Comparing `upstash_redis_a-0.1.1/LICENSE` & `upstash_redis_a-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/README.md` & `upstash_redis_a-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/asyncio/client.py` & `upstash_redis_a-0.1.2/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/http/decode.py` & `upstash_redis_a-0.1.2/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/http/execute.py` & `upstash_redis_a-0.1.2/upstash_redis/http/execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     :param retries: how many times an HTTP request will be retried if it fails
     :param retry_interval: how many seconds will be waited between each retry
     :param allow_telemetry: whether anonymous telemetry can be collected
     """
 
     # Serialize the command; more specifically, write string-incompatible types as JSON strings.
     command = [
-        element if isinstance(element, Union[str, int, float]) else dumps(element)
+        element if (isinstance(element, str) or isinstance(element, int) or isinstance(element, float)) else dumps(element)
         for element in command
     ]
 
     for i in range(retries + 1):
         try:
             headers: dict[str, str] = {"Authorization": f"Bearer {token}"}
```

### Comparing `upstash_redis_a-0.1.1/upstash_redis/schema/commands/returns.py` & `upstash_redis_a-0.1.2/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/schema/http.py` & `upstash_redis_a-0.1.2/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/utils/exception.py` & `upstash_redis_a-0.1.2/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/upstash_redis/utils/format.py` & `upstash_redis_a-0.1.2/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis_a-0.1.1/PKG-INFO` & `upstash_redis_a-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis-a
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

