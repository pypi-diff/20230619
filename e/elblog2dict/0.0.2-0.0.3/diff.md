# Comparing `tmp/elblog2dict-0.0.2.tar.gz` & `tmp/elblog2dict-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elblog2dict-0.0.2.tar", last modified: Mon Jun 19 08:29:43 2023, max compression
+gzip compressed data, was "elblog2dict-0.0.3.tar", last modified: Mon Jun 19 08:46:11 2023, max compression
```

## Comparing `elblog2dict-0.0.2.tar` & `elblog2dict-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:29:43.977172 elblog2dict-0.0.2/
--rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.2/LICENSE
--rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:29:43.977060 elblog2dict-0.0.2/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)        0 2023-06-19 06:18:59.000000 elblog2dict-0.0.2/README.md
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:29:43.976296 elblog2dict-0.0.2/elblog2dict/
--rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 08:25:41.000000 elblog2dict-0.0.2/elblog2dict/__init__.py
--rw-r--r--   0 jonghun    (501) staff       (20)     1477 2023-06-19 08:24:25.000000 elblog2dict-0.0.2/elblog2dict/parser.py
-drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:29:43.976916 elblog2dict-0.0.2/elblog2dict.egg-info/
--rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:29:43.000000 elblog2dict-0.0.2/elblog2dict.egg-info/PKG-INFO
--rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 08:29:43.000000 elblog2dict-0.0.2/elblog2dict.egg-info/SOURCES.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:29:43.000000 elblog2dict-0.0.2/elblog2dict.egg-info/dependency_links.txt
--rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:29:43.000000 elblog2dict-0.0.2/elblog2dict.egg-info/not-zip-safe
--rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 08:29:43.000000 elblog2dict-0.0.2/elblog2dict.egg-info/top_level.txt
--rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 08:29:43.977206 elblog2dict-0.0.2/setup.cfg
--rw-r--r--   0 jonghun    (501) staff       (20)      636 2023-06-19 08:25:33.000000 elblog2dict-0.0.2/setup.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.798334 elblog2dict-0.0.3/
+-rw-r--r--   0 jonghun    (501) staff       (20)     1036 2023-06-19 06:50:28.000000 elblog2dict-0.0.3/LICENSE
+-rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:46:11.798231 elblog2dict-0.0.3/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)        0 2023-06-19 06:18:59.000000 elblog2dict-0.0.3/README.md
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.797572 elblog2dict-0.0.3/elblog2dict/
+-rw-r--r--   0 jonghun    (501) staff       (20)       21 2023-06-19 08:45:58.000000 elblog2dict-0.0.3/elblog2dict/__init__.py
+-rw-r--r--   0 jonghun    (501) staff       (20)     1490 2023-06-19 08:45:21.000000 elblog2dict-0.0.3/elblog2dict/parser.py
+drwxr-xr-x   0 jonghun    (501) staff       (20)        0 2023-06-19 08:46:11.798080 elblog2dict-0.0.3/elblog2dict.egg-info/
+-rw-r--r--   0 jonghun    (501) staff       (20)      408 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/PKG-INFO
+-rw-r--r--   0 jonghun    (501) staff       (20)      246 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/SOURCES.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/dependency_links.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)        1 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/not-zip-safe
+-rw-r--r--   0 jonghun    (501) staff       (20)       12 2023-06-19 08:46:11.000000 elblog2dict-0.0.3/elblog2dict.egg-info/top_level.txt
+-rw-r--r--   0 jonghun    (501) staff       (20)       38 2023-06-19 08:46:11.798367 elblog2dict-0.0.3/setup.cfg
+-rw-r--r--   0 jonghun    (501) staff       (20)      636 2023-06-19 08:46:04.000000 elblog2dict-0.0.3/setup.py
```

### Comparing `elblog2dict-0.0.2/LICENSE` & `elblog2dict-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elblog2dict-0.0.2/elblog2dict/parser.py` & `elblog2dict-0.0.3/elblog2dict/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 
-fields = ['type', 'timestamp', 'elb', 'client_ip', 'clent_port', 'target_ip', 'target_port', 'request_processing_time', 'target_processing_time',
+def parse(datas):
+    
+    fields = ['type', 'timestamp', 'elb', 'client_ip', 'clent_port', 'target_ip', 'target_port', 'request_processing_time', 'target_processing_time',
           'response_processing_time', 'elb_status_code', 'target_status_code', 'received_bytes', 'sent_bytes',
           'request_method', 'url', 'http_version', 'user_agent', 'ssl_cipher', 'ssl_protocol', 'target_group_arn', 'trace_id', 'domain_name', 
           'chosen_cert_arn', 'matched_rule_priority', 'request_creation_time', 'actions_executed', 'redirect_url', 'error_reason', 
           'target_port_list', 'target_status_code_list', 'classification', 'classification_reason']
-
-def parse(datas):
+    
     result = []
     if type(datas) == bytes:
         datas = datas.decode('utf-8')
 
     datas = datas.splitlines()
 
     for line in datas:
```

### Comparing `elblog2dict-0.0.2/setup.py` & `elblog2dict-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='elblog2dict',
-    version='0.0.2',
+    version='0.0.3',
     description='temp',
     author='leemhoon00',
     author_email='leemhoon000@gmail.com',
     url='',
     install_requires=[],
     packages=find_packages(exclude=['.git', '.gitignore', '*.gz', 'test.py']),
     keywords=['elb'],
```

