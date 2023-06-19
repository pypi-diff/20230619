# Comparing `tmp/hscan-2.5.1.tar.gz` & `tmp/hscan-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscan-2.5.1.tar", last modified: Mon Jun 19 03:34:29 2023, max compression
+gzip compressed data, was "hscan-2.5.2.tar", last modified: Mon Jun 19 03:56:46 2023, max compression
```

## Comparing `hscan-2.5.1.tar` & `hscan-2.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:34:29.377922 hscan-2.5.1/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-19 03:34:29.377579 hscan-2.5.1/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.5.1/README.md
--rw-r--r--   0 jyanghe    (501) staff       (20)     1004 2023-06-19 03:34:07.000000 hscan-2.5.1/Setup.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:34:29.364870 hscan-2.5.1/hscan.egg-info/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-19 03:34:29.000000 hscan-2.5.1/hscan.egg-info/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-06-19 03:34:29.000000 hscan-2.5.1/hscan.egg-info/SOURCES.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-06-19 03:34:29.000000 hscan-2.5.1/hscan.egg-info/dependency_links.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)      210 2023-06-19 03:34:29.000000 hscan-2.5.1/hscan.egg-info/requires.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-06-19 03:34:29.000000 hscan-2.5.1/hscan.egg-info/top_level.txt
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:34:29.371464 hscan-2.5.1/scan/
--rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.5.1/scan/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.5.1/scan/common.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.5.1/scan/config.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      845 2022-05-19 02:18:07.000000 hscan-2.5.1/scan/crawl.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:34:29.376076 hscan-2.5.1/scan/database/
--rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.5.1/scan/database/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.5.1/scan/database/kafka.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.5.1/scan/database/mongodb.py
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.5.1/scan/database/mysql.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.5.1/scan/database/oss.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.5.1/scan/database/pg.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.5.1/scan/database/rabbitmq.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.5.1/scan/database/redis.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:34:29.376963 hscan-2.5.1/scan/downloade/
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.5.1/scan/downloade/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     4685 2022-09-09 07:51:51.000000 hscan-2.5.1/scan/downloade/downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.5.1/scan/log.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.5.1/scan/monitor.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.5.1/scan/response.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.5.1/scan/spider.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1021 2022-03-14 02:23:08.000000 hscan-2.5.1/scan/util.py
--rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-06-19 03:34:29.378034 hscan-2.5.1/setup.cfg
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:56:46.543195 hscan-2.5.2/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-19 03:56:46.542912 hscan-2.5.2/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.5.2/README.md
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1004 2023-06-19 03:55:41.000000 hscan-2.5.2/Setup.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:56:46.533485 hscan-2.5.2/hscan.egg-info/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-19 03:56:46.000000 hscan-2.5.2/hscan.egg-info/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-06-19 03:56:46.000000 hscan-2.5.2/hscan.egg-info/SOURCES.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-06-19 03:56:46.000000 hscan-2.5.2/hscan.egg-info/dependency_links.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)      210 2023-06-19 03:56:46.000000 hscan-2.5.2/hscan.egg-info/requires.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-06-19 03:56:46.000000 hscan-2.5.2/hscan.egg-info/top_level.txt
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:56:46.537963 hscan-2.5.2/scan/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.5.2/scan/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.5.2/scan/common.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.5.2/scan/config.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      845 2022-05-19 02:18:07.000000 hscan-2.5.2/scan/crawl.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:56:46.541692 hscan-2.5.2/scan/database/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.5.2/scan/database/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.5.2/scan/database/kafka.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.5.2/scan/database/mongodb.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.5.2/scan/database/mysql.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.5.2/scan/database/oss.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.5.2/scan/database/pg.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.5.2/scan/database/rabbitmq.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.5.2/scan/database/redis.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-19 03:56:46.542354 hscan-2.5.2/scan/downloade/
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.5.2/scan/downloade/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     4691 2023-06-19 03:55:26.000000 hscan-2.5.2/scan/downloade/downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.5.2/scan/log.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.5.2/scan/monitor.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.5.2/scan/response.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.5.2/scan/spider.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-2.5.2/scan/util.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-06-19 03:56:46.543289 hscan-2.5.2/setup.cfg
```

### Comparing `hscan-2.5.1/Setup.py` & `hscan-2.5.2/Setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hscan",
-    version="2.5.1",
+    version="2.5.2",
     author="jyanghe",
     author_email="jyanghe1023@gmail.com",
     description="A python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jyangHe/hscan",
     packages=setuptools.find_packages(),
```

### Comparing `hscan-2.5.1/hscan.egg-info/SOURCES.txt` & `hscan-2.5.2/hscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/config.py` & `hscan-2.5.2/scan/config.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/crawl.py` & `hscan-2.5.2/scan/crawl.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/database/kafka.py` & `hscan-2.5.2/scan/database/kafka.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/database/mongodb.py` & `hscan-2.5.2/scan/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/database/pg.py` & `hscan-2.5.2/scan/database/pg.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/database/rabbitmq.py` & `hscan-2.5.2/scan/database/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/database/redis.py` & `hscan-2.5.2/scan/database/redis.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/downloade/downloader.py` & `hscan-2.5.2/scan/downloade/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 class Downloader(object):
     def __init__(self):
         self.client = None
 
     @staticmethod
     async def gen_headers():
-        kit = f'{random.randint(490,540)}.{random.randint(10,90)}'
+        kit = f'{random.randint(490, 540)}.{random.randint(10, 90)}'
         return {
-            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;'
+            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;'
                       'q=0.8,application/signed-exchange;v=b3;q=0.9',
-            'accept-encoding': 'gzip, deflate, br',
-            'accept-language': 'en;q=0.9',
-            'user-agent': f'Mozilla/5.0 (Macintosh; Intel Mac OS X {random.randint(6,15)}_{random.randint(2,20)}'
-                          f'_{random.randint(1,9)}) AppleWebKit/{kit} (KHTML, like Gecko) '
-                          f'Chrome/{random.randint(95, 98)}.0.{random.randint(1000,5000)}.{random.randint(100, 200)}'
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Language': 'en;q=0.9',
+            'User-Agent': f'Mozilla/5.0 (Macintosh; Intel Mac OS X {random.randint(6, 15)}_{random.randint(2, 20)}'
+                          f'_{random.randint(1, 9)}) AppleWebKit/{kit} (KHTML, like Gecko) '
+                          f'Chrome/{random.randint(95, 98)}.0.{random.randint(1000, 5000)}.{random.randint(100, 200)}'
                           f' Safari/{kit}'
         }
 
     async def close(self):
         try:
             await self.client.aclose()
         except:
```

### Comparing `hscan-2.5.1/scan/log.py` & `hscan-2.5.2/scan/log.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/monitor.py` & `hscan-2.5.2/scan/monitor.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/response.py` & `hscan-2.5.2/scan/response.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/spider.py` & `hscan-2.5.2/scan/spider.py`

 * *Files identical despite different names*

### Comparing `hscan-2.5.1/scan/util.py` & `hscan-2.5.2/scan/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import hashlib
 
+
 def get_local_ip():
     import socket
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.connect(('8.8.8.8', 80))
         ip = s.getsockname()[0]
     except:
```

