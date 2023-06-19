# Comparing `tmp/mypylib-0.1.76.tar.gz` & `tmp/mypylib-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.76.tar", last modified: Thu Jun 15 13:32:24 2023, max compression
+gzip compressed data, was "mypylib-0.1.77.tar", last modified: Mon Jun 19 13:27:10 2023, max compression
```

## Comparing `mypylib-0.1.76.tar` & `mypylib-0.1.77.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-15 13:32:24.961014 mypylib-0.1.76/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-15 13:32:24.960779 mypylib-0.1.76/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.76/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-15 13:32:24.958324 mypylib-0.1.76/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.76/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47024 2023-06-15 13:30:49.000000 mypylib-0.1.76/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.76/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.76/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.76/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1857 2023-06-15 12:43:45.000000 mypylib-0.1.76/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.76/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.76/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.76/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.76/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.76/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.76/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.76/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.76/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.76/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.76/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.76/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.76/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-15 13:32:24.960079 mypylib-0.1.76/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.76/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.76/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.76/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8624 2023-06-15 12:57:21.000000 mypylib-0.1.76/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.76/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-15 13:32:24.959610 mypylib-0.1.76/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-15 13:32:24.000000 mypylib-0.1.76/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-06-15 13:32:24.000000 mypylib-0.1.76/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-06-15 13:32:24.000000 mypylib-0.1.76/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-06-15 13:32:24.000000 mypylib-0.1.76/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-06-15 13:32:24.961102 mypylib-0.1.76/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.76/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.933024 mypylib-0.1.77/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-19 13:27:10.932757 mypylib-0.1.77/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.77/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.929918 mypylib-0.1.77/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.77/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    47089 2023-06-19 13:26:14.000000 mypylib-0.1.77/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.77/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.77/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.77/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1857 2023-06-15 12:43:45.000000 mypylib-0.1.77/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.77/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.77/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.77/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.77/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.77/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.77/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.77/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.77/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.77/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.77/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.931913 mypylib-0.1.77/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.77/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.77/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.77/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.77/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.77/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-19 13:27:10.931218 mypylib-0.1.77/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-06-19 13:27:10.000000 mypylib-0.1.77/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-06-19 13:27:10.933115 mypylib-0.1.77/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.77/setup.py
```

### Comparing `mypylib-0.1.76/README.md` & `mypylib-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.77/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/__init__.py` & `mypylib-0.1.77/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,19 @@
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
     '2023/05/10: 0.1.72 改用shioaji API',
     '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
     '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說',
     '2023/06/01: 0.1.75 Apply Carey change',
-    '2023/06/15: 0.1.76 Add crawler'
+    '2023/06/15: 0.1.76 Add crawler',
+    '2023/06/19: 0.1.77 Not using stupid Redis connection pool'
 }
 
-__version__ = '0.1.76'
+__version__ = '0.1.77'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.1.76/mypylib/binance_copy_bot.py` & `mypylib-0.1.77/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.77/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/chdbif.py` & `mypylib-0.1.77/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/crawler.py` & `mypylib-0.1.77/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/crypto.py` & `mypylib-0.1.77/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/finmind.py` & `mypylib-0.1.77/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/libexcel.py` & `mypylib-0.1.77/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/mvp.py` & `mypylib-0.1.77/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/mytest.py` & `mypylib-0.1.77/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/option_test.py` & `mypylib-0.1.77/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.77/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/shioaji_kline.py` & `mypylib-0.1.77/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/shioaji_ticks.py` & `mypylib-0.1.77/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/sjtools.py` & `mypylib-0.1.77/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/tLineNotify.py` & `mypylib-0.1.77/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/ti.py` & `mypylib-0.1.77/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.77/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/tplaysound.py` & `mypylib-0.1.77/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib/tredis.py` & `mypylib-0.1.77/mypylib/tredis.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,20 @@
         threading.Thread.__init__(self)
         self.server = server
         self.port = port
         self.db = db
         self.password = password
         self.queue_publish = queue.Queue()
 
-        self.pool = redis.BlockingConnectionPool(host=self.server,
-                                                 port=self.port,
-                                                 db=self.db,
-                                                 password=self.password)
-
-
-        self.r = redis.StrictRedis(connection_pool=self.pool,
+        self.r = redis.StrictRedis(host=self.server,
+                                   port=self.port,
+                                   db=self.db,
                                    charset="utf-8",
                                    decode_responses=True,
-                                   )
-
+                                   password=self.password)
         self.start()
 
     def run(self):
         while True:
             try:
                 channel, message = self.queue_publish.get(timeout=1)
                 self.r.publish(channel, message)
```

### Comparing `mypylib-0.1.76/mypylib/warrant.py` & `mypylib-0.1.77/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.77/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.76/setup.py` & `mypylib-0.1.77/setup.py`

 * *Files identical despite different names*

