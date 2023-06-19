# Comparing `tmp/chanpackage-0.1.tar.gz` & `tmp/chanpackage-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanpackage-0.1.tar", last modified: Mon Jun 19 05:04:07 2023, max compression
+gzip compressed data, was "chanpackage-0.2.tar", last modified: Mon Jun 19 06:20:27 2023, max compression
```

## Comparing `chanpackage-0.1.tar` & `chanpackage-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:04:07.051238 chanpackage-0.1/
--rw-rw-rw-   0        0        0      188 2023-06-19 05:04:07.050239 chanpackage-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 05:04:07.021235 chanpackage-0.1/chanpackage.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 05:04:06.000000 chanpackage-0.1/chanpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 05:04:07.052238 chanpackage-0.1/setup.cfg
--rw-rw-rw-   0        0        0      374 2023-06-19 05:03:19.000000 chanpackage-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:04:07.048238 chanpackage-0.1/zabbix/
--rw-rw-rw-   0        0        0        0 2023-06-19 05:01:32.000000 chanpackage-0.1/zabbix/__init__.py
--rw-rw-rw-   0        0        0    10362 2023-06-19 05:03:14.000000 chanpackage-0.1/zabbix/get_Availability_report.py
--rw-rw-rw-   0        0        0     1790 2023-06-19 05:03:13.000000 chanpackage-0.1/zabbix/login_zabbix.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.442341 chanpackage-0.2/
+-rw-rw-rw-   0        0        0      188 2023-06-19 06:20:27.441340 chanpackage-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.435342 chanpackage-0.2/chanpackage.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 06:20:27.000000 chanpackage-0.2/chanpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 06:20:27.443339 chanpackage-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-19 06:20:02.000000 chanpackage-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:20:27.439340 chanpackage-0.2/zabbix/
+-rw-rw-rw-   0        0        0        0 2023-06-19 06:16:27.000000 chanpackage-0.2/zabbix/__init__.py
+-rw-rw-rw-   0        0        0    10362 2023-06-19 05:03:14.000000 chanpackage-0.2/zabbix/get_Availability_report.py
+-rw-rw-rw-   0        0        0     1773 2023-06-19 06:19:30.000000 chanpackage-0.2/zabbix/login_zabbix.py
```

### Comparing `chanpackage-0.1/zabbix/get_Availability_report.py` & `chanpackage-0.2/zabbix/get_Availability_report.py`

 * *Files identical despite different names*

### Comparing `chanpackage-0.1/zabbix/login_zabbix.py` & `chanpackage-0.2/zabbix/login_zabbix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 import urllib3
 import time
 from datetime import datetime
-import requests
 import json
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 def login(url,user,password,new_login: bool=False):
     get_cokie = authorization()
     if get_cokie == False or new_login:
```

