# Comparing `tmp/upstash_ratelimit_a-0.1.2.tar.gz` & `tmp/upstash_ratelimit_a-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.2.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.3.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.2.tar` & `upstash_ratelimit_a-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.2/LICENSE
--rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.2/README.md
--rw-r--r--   0        0        0      418 2023-06-19 03:20:11.025009 upstash_ratelimit_a-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.2/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    12115 2023-06-19 03:20:03.856569 upstash_ratelimit_a-0.1.2/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.2/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.2/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.2/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.2/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      355 2023-05-24 13:49:29.504602 upstash_ratelimit_a-0.1.2/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    10427 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.3/README.md
+-rw-r--r--   0        0        0      402 2023-06-19 04:13:19.287224 upstash_ratelimit_a-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.3/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    12115 2023-06-19 03:20:03.856569 upstash_ratelimit_a-0.1.3/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.3/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.3/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.3/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.3/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      392 2023-06-19 04:13:07.829439 upstash_ratelimit_a-0.1.3/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    10390 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.3/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.2/LICENSE` & `upstash_ratelimit_a-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.2/README.md` & `upstash_ratelimit_a-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.2/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.3/upstash_ratelimit/algorithm.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.2/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.3/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.2/PKG-INFO` & `upstash_ratelimit_a-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: mypy (>=1.3.0,<2.0.0)
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: upstash-redis-a (>=0.1.14,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Upstash Rate Limit - python edition
```

