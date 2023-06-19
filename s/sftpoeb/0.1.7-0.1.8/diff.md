# Comparing `tmp/sftpoeb-0.1.7.tar.gz` & `tmp/sftpoeb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.7.tar", last modified: Mon Jun 19 08:23:35 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.8.tar", last modified: Mon Jun 19 09:01:49 2023, max compression
```

## Comparing `sftpoeb-0.1.7.tar` & `sftpoeb-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.684356 sftpoeb-0.1.7/
--rw-rw-rw-   0        0        0      951 2023-06-19 08:07:18.000000 sftpoeb-0.1.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1373 2023-06-19 08:23:35.682357 sftpoeb-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.393382 sftpoeb-0.1.7/home/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.387374 sftpoeb-0.1.7/home/natthawut.th/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.388373 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.389374 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/bubblelytest/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.390376 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/bubblelytest/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.391374 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/bubblelytest/Outbound/2023-06-19/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.466364 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-19 08:11:51.000000 sftpoeb-0.1.7/home/natthawut.th/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/20230619151151_log.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.394377 sftpoeb-0.1.7/home/sftp/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.395377 sftpoeb-0.1.7/home/sftp/bubblelytest/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.396376 sftpoeb-0.1.7/home/sftp/bubblelytest/bubblelytest/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.397376 sftpoeb-0.1.7/home/sftp/bubblelytest/bubblelytest/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.398378 sftpoeb-0.1.7/home/sftp/bubblelytest/bubblelytest/Outbound/2023-06-19/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.471397 sftpoeb-0.1.7/home/sftp/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-19 08:11:51.000000 sftpoeb-0.1.7/home/sftp/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/20230619151151_log.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 08:23:35.685362 sftpoeb-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-19 08:23:31.000000 sftpoeb-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.474358 sftpoeb-0.1.7/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.7/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.532355 sftpoeb-0.1.7/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.7/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.550360 sftpoeb-0.1.7/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.7/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.7/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.1.7/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.579362 sftpoeb-0.1.7/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.7/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.1.7/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.7/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.7/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.7/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.598359 sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.607358 sftpoeb-0.1.7/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.7/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.615356 sftpoeb-0.1.7/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.7/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.7/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.625357 sftpoeb-0.1.7/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.7/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.7/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.7/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.633356 sftpoeb-0.1.7/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.7/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.7/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.641356 sftpoeb-0.1.7/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.7/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.7/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.657359 sftpoeb-0.1.7/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.7/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.667362 sftpoeb-0.1.7/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.1.7/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.1.7/sftpoeb/subclass/process/s_c_process_package_1.py
--rw-rw-rw-   0        0        0    30584 2023-06-19 07:59:51.000000 sftpoeb-0.1.7/sftpoeb/subclass/process/s_c_process_package_2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.678355 sftpoeb-0.1.7/sftpoeb/subclass/recovery/
--rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.1.7/sftpoeb/subclass/recovery/__init__.py
--rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.7/sftpoeb/subclass/recovery/s_c_recovery.py
--rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.1.7/sftpoeb/subclass/recovery/s_c_recovery2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:23:35.529358 sftpoeb-0.1.7/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1373 2023-06-19 08:23:35.000000 sftpoeb-0.1.7/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2023-06-19 08:23:35.000000 sftpoeb-0.1.7/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:23:35.000000 sftpoeb-0.1.7/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-19 08:23:35.000000 sftpoeb-0.1.7/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 08:23:35.000000 sftpoeb-0.1.7/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.1.7/test.py
--rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.7/test_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.323934 sftpoeb-0.1.8/
+-rw-rw-rw-   0        0        0     1087 2023-06-19 09:01:26.000000 sftpoeb-0.1.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1509 2023-06-19 09:01:49.321936 sftpoeb-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.8/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:01:49.323934 sftpoeb-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-19 09:01:31.000000 sftpoeb-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.151937 sftpoeb-0.1.8/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.8/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.187932 sftpoeb-0.1.8/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.8/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.198930 sftpoeb-0.1.8/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.8/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.8/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.1.8/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.219934 sftpoeb-0.1.8/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.8/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.1.8/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.8/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.8/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.8/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.234934 sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.238931 sftpoeb-0.1.8/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.8/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.247938 sftpoeb-0.1.8/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.8/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-19 08:43:27.000000 sftpoeb-0.1.8/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.259932 sftpoeb-0.1.8/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.8/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.8/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.8/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.267930 sftpoeb-0.1.8/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.8/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.8/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.275931 sftpoeb-0.1.8/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.8/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.8/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.292935 sftpoeb-0.1.8/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.8/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.304931 sftpoeb-0.1.8/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.1.8/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.1.8/sftpoeb/subclass/process/s_c_process_package_1.py
+-rw-rw-rw-   0        0        0    30584 2023-06-19 07:59:51.000000 sftpoeb-0.1.8/sftpoeb/subclass/process/s_c_process_package_2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.317933 sftpoeb-0.1.8/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.1.8/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.8/sftpoeb/subclass/recovery/s_c_recovery.py
+-rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.1.8/sftpoeb/subclass/recovery/s_c_recovery2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:01:49.184930 sftpoeb-0.1.8/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1509 2023-06-19 09:01:48.000000 sftpoeb-0.1.8/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-06-19 09:01:48.000000 sftpoeb-0.1.8/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:01:48.000000 sftpoeb-0.1.8/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-19 09:01:48.000000 sftpoeb-0.1.8/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 09:01:48.000000 sftpoeb-0.1.8/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.1.8/test.py
+-rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.8/test_recovery.py
```

### Comparing `sftpoeb-0.1.7/CHANGELOG.txt` & `sftpoeb-0.1.8/CHANGELOG.txt`

 * *Files 10% similar despite different names*

```diff
@@ -61,8 +61,16 @@
 0.1.5 (16/06/2023)
 ------------------
 - Package-2 S06
 - Recovery S06
 
 0.1.6 (19/06/2023)
 ------------------
+- Edit Path Package S06 
+
+0.1.7 (19/06/2023)
+------------------
+- Edit Path Package S06 
+
+0.1.8 (19/06/2023)
+------------------
 - Edit Path Package S06
```

### Comparing `sftpoeb-0.1.7/LICENSE.txt` & `sftpoeb-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/setup.py` & `sftpoeb-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.1.7',
+        version='0.1.8',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.1.7/sftpoeb/mainclass/c_recovery.py` & `sftpoeb-0.1.8/sftpoeb/mainclass/c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.8/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/method/callservice.py` & `sftpoeb-0.1.8/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.8/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/method/mail.py` & `sftpoeb-0.1.8/sftpoeb/method/mail.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.8/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.1.8/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.8/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.8/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.8/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.8/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.8/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.8/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/process/s_c_process_package_2.py` & `sftpoeb-0.1.8/sftpoeb/subclass/process/s_c_process_package_2.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/recovery/s_c_recovery.py` & `sftpoeb-0.1.8/sftpoeb/subclass/recovery/s_c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb/subclass/recovery/s_c_recovery2.py` & `sftpoeb-0.1.8/sftpoeb/subclass/recovery/s_c_recovery2.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.8/sftpoeb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 LICENSE.txt
 MANIFEST.in
 README.txt
 requirements.txt
 setup.py
 test.py
 test_recovery.py
-home/natthawut.th/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/20230619151151_log.txt
-home/sftp/bubblelytest/bubblelytest/Outbound/2023-06-19/Logfile/20230619151151_log.txt
 sftpoeb/__init__.py
 sftpoeb.egg-info/PKG-INFO
 sftpoeb.egg-info/SOURCES.txt
 sftpoeb.egg-info/dependency_links.txt
 sftpoeb.egg-info/requires.txt
 sftpoeb.egg-info/top_level.txt
 sftpoeb/config/variable.py
```

### Comparing `sftpoeb-0.1.7/test.py` & `sftpoeb-0.1.8/test.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.7/test_recovery.py` & `sftpoeb-0.1.8/test_recovery.py`

 * *Files identical despite different names*

