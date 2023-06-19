# Comparing `tmp/sftpoeb-0.1.9.tar.gz` & `tmp/sftpoeb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.9.tar", last modified: Mon Jun 19 09:12:37 2023, max compression
+gzip compressed data, was "sftpoeb-0.2.0.tar", last modified: Mon Jun 19 09:55:56 2023, max compression
```

## Comparing `sftpoeb-0.1.9.tar` & `sftpoeb-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.855103 sftpoeb-0.1.9/
--rw-rw-rw-   0        0        0     1157 2023-06-19 09:10:48.000000 sftpoeb-0.1.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1579 2023-06-19 09:12:37.854079 sftpoeb-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.9/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 09:12:37.856083 sftpoeb-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-19 09:10:52.000000 sftpoeb-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.735087 sftpoeb-0.1.9/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.9/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.759078 sftpoeb-0.1.9/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.9/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.767077 sftpoeb-0.1.9/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.9/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.9/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.1.9/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.789090 sftpoeb-0.1.9/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.9/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.1.9/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      597 2023-06-19 09:09:48.000000 sftpoeb-0.1.9/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.9/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.9/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.799079 sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.801085 sftpoeb-0.1.9/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.9/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.807081 sftpoeb-0.1.9/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.9/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-19 08:43:27.000000 sftpoeb-0.1.9/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.815083 sftpoeb-0.1.9/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.9/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.9/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.9/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.819084 sftpoeb-0.1.9/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.9/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.9/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.825079 sftpoeb-0.1.9/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.9/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.9/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.835093 sftpoeb-0.1.9/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.9/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.844080 sftpoeb-0.1.9/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.1.9/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.1.9/sftpoeb/subclass/process/s_c_process_package_1.py
--rw-rw-rw-   0        0        0    30584 2023-06-19 07:59:51.000000 sftpoeb-0.1.9/sftpoeb/subclass/process/s_c_process_package_2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.851076 sftpoeb-0.1.9/sftpoeb/subclass/recovery/
--rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.1.9/sftpoeb/subclass/recovery/__init__.py
--rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.9/sftpoeb/subclass/recovery/s_c_recovery.py
--rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.1.9/sftpoeb/subclass/recovery/s_c_recovery2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:12:37.756077 sftpoeb-0.1.9/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1579 2023-06-19 09:12:37.000000 sftpoeb-0.1.9/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1464 2023-06-19 09:12:37.000000 sftpoeb-0.1.9/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:12:37.000000 sftpoeb-0.1.9/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-19 09:12:37.000000 sftpoeb-0.1.9/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 09:12:37.000000 sftpoeb-0.1.9/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.1.9/test.py
--rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.9/test_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.301197 sftpoeb-0.2.0/
+-rw-rw-rw-   0        0        0     1157 2023-06-19 09:10:48.000000 sftpoeb-0.2.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1579 2023-06-19 09:55:56.299200 sftpoeb-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.2.0/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:55:56.301197 sftpoeb-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-19 09:55:47.000000 sftpoeb-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.181197 sftpoeb-0.2.0/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.2.0/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.202231 sftpoeb-0.2.0/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.209195 sftpoeb-0.2.0/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.2.0/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.2.0/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.2.0/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.230230 sftpoeb-0.2.0/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.2.0/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.2.0/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      629 2023-06-19 09:40:40.000000 sftpoeb-0.2.0/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.2.0/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.240205 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.242195 sftpoeb-0.2.0/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.2.0/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.246202 sftpoeb-0.2.0/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.2.0/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-19 08:43:27.000000 sftpoeb-0.2.0/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.253198 sftpoeb-0.2.0/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.259197 sftpoeb-0.2.0/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.2.0/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.2.0/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.263198 sftpoeb-0.2.0/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.2.0/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.2.0/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.273197 sftpoeb-0.2.0/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.289198 sftpoeb-0.2.0/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_1.py
+-rw-rw-rw-   0        0        0    30592 2023-06-19 09:55:34.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.296197 sftpoeb-0.2.0/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery.py
+-rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.200199 sftpoeb-0.2.0/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1579 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.2.0/test.py
+-rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.2.0/test_recovery.py
```

### Comparing `sftpoeb-0.1.9/CHANGELOG.txt` & `sftpoeb-0.2.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/LICENSE.txt` & `sftpoeb-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/PKG-INFO` & `sftpoeb-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.9
+Version: 0.2.0
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
```

### Comparing `sftpoeb-0.1.9/setup.py` & `sftpoeb-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.1.9',
+        version='0.2.0',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.1.9/sftpoeb/mainclass/c_recovery.py` & `sftpoeb-0.2.0/sftpoeb/mainclass/c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.2.0/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/method/callservice.py` & `sftpoeb-0.2.0/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/method/checkpath.py` & `sftpoeb-0.2.0/sftpoeb/method/checkpath.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,9 +12,10 @@
     #                 os.mkdir(mix_path)
     #                 print("Create path " + mix_path)
     #         except Exception as e:
     #             print("Check path => "+ str(e))
     if os.path.exists(path):
         return True
     else:
-        os.makedirs(path)
+        os.umask(0)
+        os.makedirs(path,mode=0o777)
         return False
```

### Comparing `sftpoeb-0.1.9/sftpoeb/method/mail.py` & `sftpoeb-0.2.0/sftpoeb/method/mail.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.2.0/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.2.0/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.2.0/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/process/s_c_process_package_2.py` & `sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
         for filename in dataProcess:
             name = str(filename).split('.')[0]
             serviceCode = 'S06'
             try:
                 ### ทำการ copy file ไปไว้ที่ History และ ย้ายไป path local
 
                 ### CSV
-                shutil.copy(self.destination.destinationInbound + name + '.csv', self.local.getLocalHistory() + name + '.csv')
-                shutil.copy(self.destination.destinationInbound + name + '.csv', self.destination.getDestinationHistory() + name + '.csv')
-                shutil.move(self.destination.destinationInbound + name + '.csv', self.local.getLocalPathNow() + name + '.csv')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
+                shutil.copy(self.destination.destinationPathCSV + name + '.csv', self.local.localCsvArchivePath + name + '.csv')
+                shutil.copy(self.destination.destinationPathCSV + name + '.csv', self.destination.destinationCsvArchivePath + name + '.csv')
+                shutil.move(self.destination.destinationPathCSV + name + '.csv', self.local.getLocalPathNow() + name + '.csv')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
                 
                 ### PDF
-                shutil.copy(self.destination.destinationInbound + name + '.pdf', self.local.getLocalHistory() + name + '.pdf')
-                shutil.copy(self.destination.destinationInbound + name + '.pdf', self.destination.getDestinationHistory() + name + '.pdf')
-                shutil.move(self.destination.destinationInbound + name + '.pdf', self.local.getLocalPathNow() + name + '.pdf')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
+                shutil.copy(self.destination.destinationPathPDF + name + '.pdf', self.local.localPdfArchivePath + name + '.pdf')
+                shutil.copy(self.destination.destinationPathPDF + name + '.pdf', self.destination.destinationPdfArchivePath + name + '.pdf')
+                shutil.move(self.destination.destinationPathPDF + name + '.pdf', self.local.getLocalPathNow() + name + '.pdf')  #### วนหยิบ PDF ตามชื่อ text ที่แตกดป็น 1:1 แล้ว
                 
                 ### นำส่งไฟล์ไปทำ E-Tax Invoice ผ่าน API
                 service = serviceSigningS06(self.payloadData, filename, name+".pdf" ,self.local.getLocalPathNow() , 0, serviceCode,self.SERVICE_SIGNING_URL)
                 if service['status'] == 'OK':
                     self.success = self.success + 1
                     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Service signing success.')
                     
@@ -310,15 +310,15 @@
                 #     print(str(self.dateNow + self.timeNow) + '>> ' + str(name) + ' Copy PDF input to Error_File failed : ' + str(e))
 
     def testprocess(self,var):
         print("var == " + str(var))
 
     def runThreadProcess(self,quantityThread=1):
         try:
-            allCSV = [f for f in listdir(self.destination.destinationInbound) if isfile(join(self.destination.destinationInbound, f))]
+            allCSV = [f for f in listdir(self.destination.destinationPathCSV) if isfile(join(self.destination.destinationPathCSV, f))]
 
             self.countInvoice = len(allCSV)
             divInvoice = (self.countInvoice // quantityThread)
             arrVariable = []
             for i in range(quantityThread):
                 arrVariable.append("ThreadProcess" + str(i))
```

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/recovery/s_c_recovery.py` & `sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb/subclass/recovery/s_c_recovery2.py` & `sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery2.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.2.0/sftpoeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.9
+Version: 0.2.0
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
```

### Comparing `sftpoeb-0.1.9/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.2.0/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/test.py` & `sftpoeb-0.2.0/test.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.9/test_recovery.py` & `sftpoeb-0.2.0/test_recovery.py`

 * *Files identical despite different names*

