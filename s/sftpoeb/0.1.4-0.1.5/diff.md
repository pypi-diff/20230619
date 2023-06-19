# Comparing `tmp/sftpoeb-0.1.4.tar.gz` & `tmp/sftpoeb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.1.4.tar", last modified: Fri Jun 16 11:56:59 2023, max compression
+gzip compressed data, was "sftpoeb-0.1.5.tar", last modified: Mon Jun 19 07:43:23 2023, max compression
```

## Comparing `sftpoeb-0.1.4.tar` & `sftpoeb-0.1.5.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.064041 sftpoeb-0.1.4/
--rw-rw-rw-   0        0        0      808 2023-06-16 11:55:05.000000 sftpoeb-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1230 2023-06-16 11:56:59.063040 sftpoeb-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.903136 sftpoeb-0.1.4/home/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.899135 sftpoeb-0.1.4/home/natthawut.th/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.900135 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.900135 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.901138 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.902137 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.941174 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.4/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.903136 sftpoeb-0.1.4/home/sftp/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.904135 sftpoeb-0.1.4/home/sftp/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.905137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.905137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.906137 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.943134 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
--rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.4/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:56:59.065045 sftpoeb-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-16 11:56:43.000000 sftpoeb-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.946137 sftpoeb-0.1.4/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.4/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.970137 sftpoeb-0.1.4/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.978136 sftpoeb-0.1.4/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.4/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.4/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.4/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.991138 sftpoeb-0.1.4/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.4/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     4800 2023-06-16 10:56:05.000000 sftpoeb-0.1.4/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.4/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.4/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.002137 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.004135 sftpoeb-0.1.4/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.4/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.010135 sftpoeb-0.1.4/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.4/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.4/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.018137 sftpoeb-0.1.4/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.024137 sftpoeb-0.1.4/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.4/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.4/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.032139 sftpoeb-0.1.4/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.4/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.4/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.047137 sftpoeb-0.1.4/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5375 2023-06-16 03:46:50.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4154 2023-06-16 11:18:57.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.053138 sftpoeb-0.1.4/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       36 2023-06-14 03:51:39.000000 sftpoeb-0.1.4/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30017 2023-06-16 10:56:17.000000 sftpoeb-0.1.4/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:59.060040 sftpoeb-0.1.4/sftpoeb/subclass/recovery/
--rw-rw-rw-   0        0        0       27 2023-06-16 04:43:48.000000 sftpoeb-0.1.4/sftpoeb/subclass/recovery/__init__.py
--rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.4/sftpoeb/subclass/recovery/s_c_recovery.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:56:58.968137 sftpoeb-0.1.4/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1230 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1533 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-16 11:56:58.000000 sftpoeb-0.1.4/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.4/test.py
--rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.4/test_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.366657 sftpoeb-0.1.5/
+-rw-rw-rw-   0        0        0      883 2023-06-19 07:43:09.000000 sftpoeb-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1305 2023-06-19 07:43:23.364659 sftpoeb-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.083656 sftpoeb-0.1.5/home/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.077660 sftpoeb-0.1.5/home/natthawut.th/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.078656 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.079659 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.080659 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.081659 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.148664 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.5/home/natthawut.th/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.084659 sftpoeb-0.1.5/home/sftp/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.085661 sftpoeb-0.1.5/home/sftp/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.085661 sftpoeb-0.1.5/home/sftp/kpc.prd/kpc.prd/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.086657 sftpoeb-0.1.5/home/sftp/kpc.prd/kpc.prd/Outbound/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.087661 sftpoeb-0.1.5/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.152660 sftpoeb-0.1.5/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/
+-rw-rw-rw-   0        0        0      177 2023-06-15 12:04:47.000000 sftpoeb-0.1.5/home/sftp/kpc.prd/kpc.prd/Outbound/2023-06-15/Logfile/20230615190447_log.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:43:23.366657 sftpoeb-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-19 07:43:13.000000 sftpoeb-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.154664 sftpoeb-0.1.5/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.1.5/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.200662 sftpoeb-0.1.5/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.1.5/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.209658 sftpoeb-0.1.5/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.1.5/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.1.5/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 08:31:33.000000 sftpoeb-0.1.5/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.224657 sftpoeb-0.1.5/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.1.5/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.1.5/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      601 2023-06-14 06:57:02.000000 sftpoeb-0.1.5/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.1.5/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.1.5/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.266661 sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.269656 sftpoeb-0.1.5/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.1.5/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.275676 sftpoeb-0.1.5/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.1.5/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-06-15 11:41:55.000000 sftpoeb-0.1.5/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.285662 sftpoeb-0.1.5/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.1.5/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.1.5/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.1.5/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.290667 sftpoeb-0.1.5/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.1.5/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.1.5/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.299659 sftpoeb-0.1.5/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.1.5/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.1.5/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.334655 sftpoeb-0.1.5/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.1.5/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5375 2023-06-16 03:46:50.000000 sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4154 2023-06-16 11:18:57.000000 sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.343658 sftpoeb-0.1.5/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.1.5/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30017 2023-06-16 10:56:17.000000 sftpoeb-0.1.5/sftpoeb/subclass/process/s_c_process_package_1.py
+-rw-rw-rw-   0        0        0    30583 2023-06-19 07:42:03.000000 sftpoeb-0.1.5/sftpoeb/subclass/process/s_c_process_package_2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.357672 sftpoeb-0.1.5/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.1.5/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.1.5/sftpoeb/subclass/recovery/s_c_recovery.py
+-rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.1.5/sftpoeb/subclass/recovery/s_c_recovery2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:43:23.197655 sftpoeb-0.1.5/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-19 07:43:22.000000 sftpoeb-0.1.5/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1626 2023-06-19 07:43:22.000000 sftpoeb-0.1.5/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:43:22.000000 sftpoeb-0.1.5/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-19 07:43:22.000000 sftpoeb-0.1.5/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 07:43:22.000000 sftpoeb-0.1.5/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1107 2023-06-15 08:22:57.000000 sftpoeb-0.1.5/test.py
+-rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.1.5/test_recovery.py
```

### Comparing `sftpoeb-0.1.4/CHANGELOG.txt` & `sftpoeb-0.1.5/CHANGELOG.txt`

 * *Files 22% similar despite different names*

```diff
@@ -52,8 +52,13 @@
 0.1.3 (16/06/2023)
 ------------------
 - Process Recovery
 
 0.1.4 (16/06/2023)
 ------------------
 - Process Recovery all
-- Fixbux variable
+- Fixbux variable
+
+0.1.5 (16/06/2023)
+------------------
+- Package-2 S06
+- Recovery S06
```

### Comparing `sftpoeb-0.1.4/LICENSE.txt` & `sftpoeb-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/PKG-INFO` & `sftpoeb-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.4
+Version: 0.1.5
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -72,7 +72,12 @@
 - Process Recovery
 
 0.1.4 (16/06/2023)
 ------------------
 - Process Recovery all
 - Fixbux variable
 
+0.1.5 (16/06/2023)
+------------------
+- Package-2 S06
+- Recovery S06
+
```

### Comparing `sftpoeb-0.1.4/sftpoeb/mainclass/c_recovery.py` & `sftpoeb-0.1.5/sftpoeb/mainclass/c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.1.5/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/method/callservice.py` & `sftpoeb-0.1.5/sftpoeb/method/callservice.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,59 @@
         else:
             result = {
                 "status": "ER",
                 "errorCode": "EXC001",
                 "errorMessage": "send_for_getfile : " + str(e)
             }
     return result
+
+def serviceSigningS06(data, fileNameText, fileNamePDF ,  pathFile,round,serviceCode,URL):
+    multipart_data = MultipartEncoder(
+        fields={
+            "SellerTaxId": data['SellerTaxid'],
+            "SellerBranchId": data['SellerBranchId'],
+            "APIKey": data['APIKey'],
+            "UserCode": data['UserCode'],
+            "AccessKey": data['AccessKey'],
+            "ServiceCode": serviceCode,
+            "TextContent": (fileNameText, open(os.path.abspath(os.path.join(pathFile + '/' + fileNameText)), 'rb'), "multipart/form-data"),
+            "PDFContent": (fileNamePDF, open(os.path.abspath(os.path.join(pathFile + '/' + fileNamePDF)), 'rb'), "multipart/form-data"),
+            "SendMail": "YES"
+            # "PdfTemplateId":PdfTemplateId
+        }
+    )
+    headers = {
+        'Content-Type': multipart_data.content_type,
+        'Authorization': data['Authorization']
+    }
+    try:
+        response = requests.post(URL, data=multipart_data, headers=headers, verify=False)
+        if response.status_code == 200:
+            result = response.json()
+        else:
+            if round < 3:
+                time.sleep(0.5)
+                result = serviceSigning(data, fileNameText, pathFile,round+1,serviceCode)
+            else:
+                result = {
+                    "status": "ER",
+                    "errorMessage": "Service Stamp was problem.",
+                    "errorCode": response.status_code
+                }
+    except Exception as e:
+        if round < 3:
+            time.sleep(0.5)
+            result = serviceSigning(data, fileNameText, pathFile,round+1,serviceCode)
+        else:
+            result = {
+                "status": "ER",
+                "errorCode": "EXC001",
+                "errorMessage": "send_for_getfile : " + str(e)
+            }
+    return result
     
 def checkStatus(data,TransactionCode,round,serviceCode,URL):
     multipart_data = MultipartEncoder(
         fields={
             "SellerTaxId":data['SellerTaxid'],
             "SellerBranchId": data['SellerBranchId'],
             "APIKey": data['APIKey'],
```

### Comparing `sftpoeb-0.1.4/sftpoeb/method/checkpath.py` & `sftpoeb-0.1.5/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/method/mail.py` & `sftpoeb-0.1.5/sftpoeb/method/mail.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.5/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.1.5/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.1.5/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.1.5/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.1.5/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.1.5/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.1.5/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.1.5/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb/subclass/recovery/s_c_recovery.py` & `sftpoeb-0.1.5/sftpoeb/subclass/recovery/s_c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.1.5/sftpoeb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.1.4
+Version: 0.1.5
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -72,7 +72,12 @@
 - Process Recovery
 
 0.1.4 (16/06/2023)
 ------------------
 - Process Recovery all
 - Fixbux variable
 
+0.1.5 (16/06/2023)
+------------------
+- Package-2 S06
+- Recovery S06
+
```

### Comparing `sftpoeb-0.1.4/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.1.5/sftpoeb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -39,9 +39,11 @@
 sftpoeb/subclass/output/s_c_output.py
 sftpoeb/subclass/path/__init__.py
 sftpoeb/subclass/path/s_c_setgetdestination.py
 sftpoeb/subclass/path/s_c_setgetlocal.py
 sftpoeb/subclass/path/s_c_setgetrecovery.py
 sftpoeb/subclass/process/__init__.py
 sftpoeb/subclass/process/s_c_process_package_1.py
+sftpoeb/subclass/process/s_c_process_package_2.py
 sftpoeb/subclass/recovery/__init__.py
-sftpoeb/subclass/recovery/s_c_recovery.py
+sftpoeb/subclass/recovery/s_c_recovery.py
+sftpoeb/subclass/recovery/s_c_recovery2.py
```

### Comparing `sftpoeb-0.1.4/test.py` & `sftpoeb-0.1.5/test.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.1.4/test_recovery.py` & `sftpoeb-0.1.5/test_recovery.py`

 * *Files identical despite different names*

