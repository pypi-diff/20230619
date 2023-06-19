# Comparing `tmp/upstash_ratelimit_a-0.1.0.tar.gz` & `tmp/upstash_ratelimit_a-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.0.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.1.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.0.tar` & `upstash_ratelimit_a-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.0/LICENSE
--rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.0/README.md
--rw-r--r--   0        0        0      418 2023-06-19 02:34:46.392254 upstash_ratelimit_a-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.0/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    12129 2023-05-24 13:49:29.503974 upstash_ratelimit_a-0.1.0/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.0/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3065 2023-05-25 01:08:06.020349 upstash_ratelimit_a-0.1.0/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.0/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.0/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      355 2023-05-24 13:49:29.504602 upstash_ratelimit_a-0.1.0/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    10427 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.1/README.md
+-rw-r--r--   0        0        0      418 2023-06-19 03:11:52.314867 upstash_ratelimit_a-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.1/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    12130 2023-06-19 03:11:05.920479 upstash_ratelimit_a-0.1.1/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.1/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.1/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.1/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.1/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      355 2023-05-24 13:49:29.504602 upstash_ratelimit_a-0.1.1/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    10427 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.1/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.0/LICENSE` & `upstash_ratelimit_a-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.0/README.md` & `upstash_ratelimit_a-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.0/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.1/upstash_ratelimit/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import ClassVar, Literal
-from upstash_redis.client import Redis
+from upstash_redis.asyncio import Redis
 from upstash_ratelimit.utils.time import to_milliseconds
 from upstash_ratelimit.config import SDK, PREFIX
 from upstash_ratelimit.schema.response import RateLimitResponse
 from time import time_ns, sleep
 from math import floor
```

### Comparing `upstash_ratelimit_a-0.1.0/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.1/upstash_ratelimit/limiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from upstash_ratelimit.algorithm import FixedWindow, SlidingWindow, TokenBucket
 from upstash_ratelimit.config import PREFIX
-from upstash_redis.client import Redis
+from upstash_redis.asyncio import Redis
 from typing import Literal
 
 
 class RateLimit:
     """
     A class that incorporates all the algorithms to provide a smoother initialisation experience.
     """
```

### Comparing `upstash_ratelimit_a-0.1.0/PKG-INFO` & `upstash_ratelimit_a-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

