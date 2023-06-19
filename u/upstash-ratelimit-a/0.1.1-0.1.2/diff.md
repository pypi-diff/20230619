# Comparing `tmp/upstash_ratelimit_a-0.1.1.tar.gz` & `tmp/upstash_ratelimit_a-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit_a-0.1.1.tar", max compression
+gzip compressed data, was "upstash_ratelimit_a-0.1.2.tar", max compression
```

## Comparing `upstash_ratelimit_a-0.1.1.tar` & `upstash_ratelimit_a-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.1/LICENSE
--rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.1/README.md
--rw-r--r--   0        0        0      418 2023-06-19 03:11:52.314867 upstash_ratelimit_a-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.1/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0    12130 2023-06-19 03:11:05.920479 upstash_ratelimit_a-0.1.1/upstash_ratelimit/algorithm.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.1/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.1/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.1/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.1/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0      355 2023-05-24 13:49:29.504602 upstash_ratelimit_a-0.1.1/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    10427 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit_a-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9798 2023-05-24 13:49:29.502103 upstash_ratelimit_a-0.1.2/README.md
+-rw-r--r--   0        0        0      418 2023-06-19 03:20:11.025009 upstash_ratelimit_a-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.503800 upstash_ratelimit_a-0.1.2/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0    12115 2023-06-19 03:20:03.856569 upstash_ratelimit_a-0.1.2/upstash_ratelimit/algorithm.py
+-rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit_a-0.1.2/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3066 2023-06-19 03:11:10.807977 upstash_ratelimit_a-0.1.2/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit_a-0.1.2/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      474 2023-05-24 13:49:29.504424 upstash_ratelimit_a-0.1.2/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0      355 2023-05-24 13:49:29.504602 upstash_ratelimit_a-0.1.2/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0    10427 1970-01-01 00:00:00.000000 upstash_ratelimit_a-0.1.2/PKG-INFO
```

### Comparing `upstash_ratelimit_a-0.1.1/LICENSE` & `upstash_ratelimit_a-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.1/README.md` & `upstash_ratelimit_a-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.1/upstash_ratelimit/algorithm.py` & `upstash_ratelimit_a-0.1.2/upstash_ratelimit/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         key: str = f'{self.prefix}:{identifier}'
 
         async with self.redis:
             current_requests: int = await self.redis.eval(
                 script=FixedWindow.script,
                 keys=[key],
-                arguments=[self.window]
+                args=[self.window]
             )
 
         return {
             "is_allowed": current_requests <= self.max_number_of_requests,
             "limit": self.max_number_of_requests,
             "remaining": self.max_number_of_requests - current_requests,
             "reset": floor((time_ns() / 1000000) / self.window) * self.window + self.window,
@@ -210,15 +210,15 @@
 
         previous_key: str = f'{self.prefix}:{identifier}:{previous_window}'
 
         async with self.redis:
             remaining_requests: int = await self.redis.eval(
                 script=SlidingWindow.script,
                 keys=[current_key, previous_key],
-                arguments=[self.max_number_of_requests, now, self.window]
+                args=[self.max_number_of_requests, now, self.window]
             )
 
         return {
             "is_allowed": remaining_requests >= 0,
             "limit": self.max_number_of_requests,
             "remaining": remaining_requests,
             "reset": floor((time_ns() / 1000000) / self.window) * self.window + self.window,
@@ -304,15 +304,15 @@
 
         key: str = f'{self.prefix}:{identifier}'
 
         async with self.redis:
             remaining_tokens, next_refill_at = await self.redis.eval(
                 script=TokenBucket.script,
                 keys=[key],
-                arguments=[self.max_number_of_tokens, self.interval, self.refill_rate, now]
+                args=[self.max_number_of_tokens, self.interval, self.refill_rate, now]
             )
 
         return {
             "is_allowed": remaining_tokens >= 0,
             "limit": self.max_number_of_tokens,
             "remaining": remaining_tokens,
             "reset": next_refill_at
```

### Comparing `upstash_ratelimit_a-0.1.1/upstash_ratelimit/limiter.py` & `upstash_ratelimit_a-0.1.2/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit_a-0.1.1/PKG-INFO` & `upstash_ratelimit_a-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit-a
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

