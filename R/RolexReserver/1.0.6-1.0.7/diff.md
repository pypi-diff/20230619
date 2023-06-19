# Comparing `tmp/RolexReserver-1.0.6.tar.gz` & `tmp/RolexReserver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RolexReserver-1.0.6.tar", last modified: Sat Jun 17 14:18:39 2023, max compression
+gzip compressed data, was "RolexReserver-1.0.7.tar", last modified: Mon Jun 19 12:26:30 2023, max compression
```

## Comparing `RolexReserver-1.0.6.tar` & `RolexReserver-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.921746 RolexReserver-1.0.6/
--rw-rw-rw-   0        0        0      887 2023-06-17 14:18:39.920747 RolexReserver-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.893747 RolexReserver-1.0.6/RolexReserver/
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.903746 RolexReserver-1.0.6/RolexReserver/Getter/
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.904747 RolexReserver-1.0.6/RolexReserver/Getter/Base/
--rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.6/RolexReserver/Getter/Base/baseGetter.py
--rw-rw-rw-   0        0        0     7479 2023-06-13 13:08:49.000000 RolexReserver-1.0.6/RolexReserver/Getter/getter_rolexReserve.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.915747 RolexReserver-1.0.6/RolexReserver/Library/
--rw-rw-rw-   0        0        0     4820 2023-05-23 13:18:26.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverConfig.py
--rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverConfiger.py
--rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverController.py
--rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverDeclare.py
--rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverException.py
--rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverGlobals.py
--rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.6/RolexReserver/Library/rolexReserverMailer.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.917748 RolexReserver-1.0.6/RolexReserver/Models/
--rw-rw-rw-   0        0        0      669 2023-06-13 13:08:49.000000 RolexReserver-1.0.6/RolexReserver/Models/log_reserve.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.918746 RolexReserver-1.0.6/RolexReserver/Register/
--rw-rw-rw-   0        0        0      446 2023-06-13 13:08:49.000000 RolexReserver-1.0.6/RolexReserver/Register/register_LogReserve.py
--rw-rw-rw-   0        0        0      261 2023-06-17 14:14:05.000000 RolexReserver-1.0.6/RolexReserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:18:39.901746 RolexReserver-1.0.6/RolexReserver.egg-info/
--rw-rw-rw-   0        0        0      887 2023-06-17 14:18:39.000000 RolexReserver-1.0.6/RolexReserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-06-17 14:18:39.000000 RolexReserver-1.0.6/RolexReserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:18:39.000000 RolexReserver-1.0.6/RolexReserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      784 2023-06-17 14:18:39.000000 RolexReserver-1.0.6/RolexReserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0      128 2023-06-17 14:18:39.000000 RolexReserver-1.0.6/RolexReserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 14:18:39.922748 RolexReserver-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2667 2023-06-17 14:14:35.000000 RolexReserver-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.075736 RolexReserver-1.0.7/
+-rw-rw-rw-   0        0        0      887 2023-06-19 12:26:30.075736 RolexReserver-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.050734 RolexReserver-1.0.7/RolexReserver/
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.058736 RolexReserver-1.0.7/RolexReserver/Getter/
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.059731 RolexReserver-1.0.7/RolexReserver/Getter/Base/
+-rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.7/RolexReserver/Getter/Base/baseGetter.py
+-rw-rw-rw-   0        0        0     7479 2023-06-13 13:08:49.000000 RolexReserver-1.0.7/RolexReserver/Getter/getter_rolexReserve.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.069732 RolexReserver-1.0.7/RolexReserver/Library/
+-rw-rw-rw-   0        0        0     4820 2023-05-23 13:18:26.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverConfig.py
+-rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverConfiger.py
+-rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverController.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverDeclare.py
+-rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverException.py
+-rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverGlobals.py
+-rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.7/RolexReserver/Library/rolexReserverMailer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.071734 RolexReserver-1.0.7/RolexReserver/Models/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:08:49.000000 RolexReserver-1.0.7/RolexReserver/Models/log_reserve.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.073732 RolexReserver-1.0.7/RolexReserver/Register/
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.074732 RolexReserver-1.0.7/RolexReserver/Register/Base/
+-rw-rw-rw-   0        0        0     3976 2023-06-13 13:08:49.000000 RolexReserver-1.0.7/RolexReserver/Register/Base/baseRegister.py
+-rw-rw-rw-   0        0        0      446 2023-06-13 13:08:49.000000 RolexReserver-1.0.7/RolexReserver/Register/register_LogReserve.py
+-rw-rw-rw-   0        0        0      261 2023-06-19 12:26:15.000000 RolexReserver-1.0.7/RolexReserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:26:30.057734 RolexReserver-1.0.7/RolexReserver.egg-info/
+-rw-rw-rw-   0        0        0      887 2023-06-19 12:26:29.000000 RolexReserver-1.0.7/RolexReserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-06-19 12:26:29.000000 RolexReserver-1.0.7/RolexReserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:26:29.000000 RolexReserver-1.0.7/RolexReserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      784 2023-06-19 12:26:29.000000 RolexReserver-1.0.7/RolexReserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      156 2023-06-19 12:26:29.000000 RolexReserver-1.0.7/RolexReserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 12:26:30.076734 RolexReserver-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2728 2023-06-19 12:26:08.000000 RolexReserver-1.0.7/setup.py
```

### Comparing `RolexReserver-1.0.6/PKG-INFO` & `RolexReserver-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.6
+Version: 1.0.7
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.6/RolexReserver/Getter/Base/baseGetter.py` & `RolexReserver-1.0.7/RolexReserver/Getter/Base/baseGetter.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Getter/getter_rolexReserve.py` & `RolexReserver-1.0.7/RolexReserver/Getter/getter_rolexReserve.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverConfig.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverConfig.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverConfiger.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverConfiger.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverController.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverController.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverException.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverException.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverGlobals.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverGlobals.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Library/rolexReserverMailer.py` & `RolexReserver-1.0.7/RolexReserver/Library/rolexReserverMailer.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver/Models/log_reserve.py` & `RolexReserver-1.0.7/RolexReserver/Models/log_reserve.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/RolexReserver.egg-info/PKG-INFO` & `RolexReserver-1.0.7/RolexReserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.6
+Version: 1.0.7
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.6/RolexReserver.egg-info/SOURCES.txt` & `RolexReserver-1.0.7/RolexReserver.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 RolexReserver/Library/rolexReserverConfiger.py
 RolexReserver/Library/rolexReserverController.py
 RolexReserver/Library/rolexReserverDeclare.py
 RolexReserver/Library/rolexReserverException.py
 RolexReserver/Library/rolexReserverGlobals.py
 RolexReserver/Library/rolexReserverMailer.py
 RolexReserver/Models/log_reserve.py
-RolexReserver/Register/register_LogReserve.py
+RolexReserver/Register/register_LogReserve.py
+RolexReserver/Register/Base/baseRegister.py
```

### Comparing `RolexReserver-1.0.6/RolexReserver.egg-info/requires.txt` & `RolexReserver-1.0.7/RolexReserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.6/setup.py` & `RolexReserver-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     packages=[
         package_name + '/',
         package_name + '/' + subPackage_name_getter,
         package_name + '/' + subPackage_name_getter_base,
         package_name + '/' + subPackage_name_library,
         package_name + '/' + subPackage_name_models,
         package_name + '/' + subPackage_name_register,
+        package_name + '/' + subPackage_name_register_base,
     ],
 
     version=version,
 
     license=license,
 
     install_requires=_requirements(),
```

