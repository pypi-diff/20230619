# Comparing `tmp/oathlink-0.8.6.tar.gz` & `tmp/oathlink-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oathlink-0.8.6.tar", last modified: Fri Jun 16 21:10:07 2023, max compression
+gzip compressed data, was "oathlink-0.8.7.tar", last modified: Mon Jun 19 16:54:18 2023, max compression
```

## Comparing `oathlink-0.8.6.tar` & `oathlink-0.8.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.163895 oathlink-0.8.6/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.8.6/LICENSE
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-16 21:10:07.163968 oathlink-0.8.6/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.8.6/README.md
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.8.6/pyproject.toml
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      824 2023-06-16 21:10:07.164369 oathlink-0.8.6/setup.cfg
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.156087 oathlink-0.8.6/src/
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.157396 oathlink-0.8.6/src/oathlink/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.8.6/src/oathlink/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.158580 oathlink-0.8.6/src/oathlink/main/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/main/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     4715 2023-06-16 20:06:48.000000 oathlink-0.8.6/src/oathlink/main/oathlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.159020 oathlink-0.8.6/src/oathlink/services/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.159289 oathlink-0.8.6/src/oathlink/services/agent/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/agent/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.160413 oathlink-0.8.6/src/oathlink/services/agent/account/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/agent/account/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/agent/account/create.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/agent/account/link.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/agent/account/unlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.160842 oathlink-0.8.6/src/oathlink/services/agent/ip/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/agent/ip/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/agent/ip/add.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/agent/ip/remove.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/hello.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.162436 oathlink-0.8.6/src/oathlink/services/record/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/record/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/record/archive.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/record/cancel.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      896 2023-06-16 15:22:00.000000 oathlink-0.8.6/src/oathlink/services/record/decrypt.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/record/download.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1261 2023-05-29 20:30:18.000000 oathlink-0.8.6/src/oathlink/services/record/upload.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.162953 oathlink-0.8.6/src/oathlink/services/report/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/services/report/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/report/history.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/report/outstanding.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.8.6/src/oathlink/services/report/record.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.163077 oathlink-0.8.6/src/oathlink/util/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/util/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.163437 oathlink-0.8.6/src/oathlink/util/crypto/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.8.6/src/oathlink/util/crypto/Fernet.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/util/crypto/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.163650 oathlink-0.8.6/src/oathlink/util/https/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.6/src/oathlink/util/https/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     2559 2023-06-16 21:09:46.000000 oathlink-0.8.6/src/oathlink/util/https/https.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-16 21:10:07.158365 oathlink-0.8.6/src/oathlink.egg-info/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-16 21:10:07.000000 oathlink-0.8.6/src/oathlink.egg-info/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-06-16 21:10:07.000000 oathlink-0.8.6/src/oathlink.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-06-16 21:10:07.000000 oathlink-0.8.6/src/oathlink.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-06-16 21:10:07.000000 oathlink-0.8.6/src/oathlink.egg-info/requires.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-06-16 21:10:07.000000 oathlink-0.8.6/src/oathlink.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803681 oathlink-0.8.7/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.8.7/LICENSE
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 16:54:18.803759 oathlink-0.8.7/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.8.7/README.md
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.8.7/pyproject.toml
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      824 2023-06-19 16:54:18.804050 oathlink-0.8.7/setup.cfg
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.795661 oathlink-0.8.7/src/
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.796812 oathlink-0.8.7/src/oathlink/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.8.7/src/oathlink/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.797888 oathlink-0.8.7/src/oathlink/main/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/main/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     5317 2023-06-19 16:53:04.000000 oathlink-0.8.7/src/oathlink/main/oathlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.798193 oathlink-0.8.7/src/oathlink/services/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.798454 oathlink-0.8.7/src/oathlink/services/agent/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.799325 oathlink-0.8.7/src/oathlink/services/agent/account/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/create.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/link.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/unlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.800061 oathlink-0.8.7/src/oathlink/services/agent/ip/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/add.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/remove.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/hello.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.801743 oathlink-0.8.7/src/oathlink/services/record/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/record/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/record/archive.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/record/cancel.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      896 2023-06-16 15:22:00.000000 oathlink-0.8.7/src/oathlink/services/record/decrypt.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-06-19 16:51:14.000000 oathlink-0.8.7/src/oathlink/services/record/download.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1261 2023-05-29 20:30:18.000000 oathlink-0.8.7/src/oathlink/services/record/upload.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.802583 oathlink-0.8.7/src/oathlink/services/report/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/report/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/history.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/outstanding.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/record.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.802828 oathlink-0.8.7/src/oathlink/util/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803225 oathlink-0.8.7/src/oathlink/util/crypto/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.8.7/src/oathlink/util/crypto/Fernet.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/crypto/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803440 oathlink-0.8.7/src/oathlink/util/https/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/https/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     2852 2023-06-19 16:46:59.000000 oathlink-0.8.7/src/oathlink/util/https/https.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.797674 oathlink-0.8.7/src/oathlink.egg-info/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/requires.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/top_level.txt
```

### Comparing `oathlink-0.8.6/LICENSE` & `oathlink-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/PKG-INFO` & `oathlink-0.8.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.8.6
+Version: 0.8.7
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.8.6/setup.cfg` & `oathlink-0.8.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oathlink
-version = 0.8.6
+version = 0.8.7
 author = oathlink
 author_email = oathlink@bfi.lat
 description = This repository holds the Oathlink user Python package (client source code).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 project_urls =
```

### Comparing `oathlink-0.8.6/src/oathlink/services/agent/account/create.py` & `oathlink-0.8.7/src/oathlink/services/agent/account/create.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/agent/account/link.py` & `oathlink-0.8.7/src/oathlink/services/agent/account/link.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/agent/account/unlink.py` & `oathlink-0.8.7/src/oathlink/services/agent/account/unlink.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/agent/ip/add.py` & `oathlink-0.8.7/src/oathlink/services/agent/ip/add.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/agent/ip/remove.py` & `oathlink-0.8.7/src/oathlink/services/agent/ip/remove.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/hello.py` & `oathlink-0.8.7/src/oathlink/services/hello.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/record/archive.py` & `oathlink-0.8.7/src/oathlink/services/record/archive.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/record/cancel.py` & `oathlink-0.8.7/src/oathlink/services/record/cancel.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/record/decrypt.py` & `oathlink-0.8.7/src/oathlink/services/record/decrypt.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/record/download.py` & `oathlink-0.8.7/src/oathlink/services/record/download.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/record/upload.py` & `oathlink-0.8.7/src/oathlink/services/record/upload.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/report/history.py` & `oathlink-0.8.7/src/oathlink/services/report/history.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/report/outstanding.py` & `oathlink-0.8.7/src/oathlink/services/report/outstanding.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/services/report/record.py` & `oathlink-0.8.7/src/oathlink/services/report/record.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/util/crypto/Fernet.py` & `oathlink-0.8.7/src/oathlink/util/crypto/Fernet.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.6/src/oathlink/util/https/https.py` & `oathlink-0.8.7/src/oathlink/util/https/https.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,40 +18,54 @@
 def _getUrl(extension: str) -> str:
     if len(extension) > 0:
         if extension[0] == '/':
             extension = extension[1:]
     return f'{_getBaseUrl()}/{extension}'
 
 def get(url: str) -> list:
+    filename = 'download.txt'
     response = requests.get(url)
     zipFilename = f'download.zip'
     with open(zipFilename, 'wb') as file:
         file.write(response.content)
     with ZipFile(zipFilename, 'r') as zip:
         zip.extractall()
         info = zip.infolist()[0]
         filename = info.filename
     os.remove(zipFilename)
     return filename
 
-def put(url: str, filename: str, content: str = None) -> bool:
+def put(url: str, data: str) -> bool:
     # Resolving url
+    temporalFilename = 'tmp.txt'
     response = requests.get(url)
     url = response.url
-    # Writing file if contents are handed
-    if content is not None:
+    if not os.path.isfile(data):
+        filename = temporalFilename
+        content = data
+        # Writing file if contents are handed
         with open(filename, 'w') as file:
             file.write(content)
+    else:
+        filename = data
     # Zipping the file
     zipFilename = f'{filename}.zip'
     with ZipFile(zipFilename, 'w') as zip:
         zip.write(filename)
     # Regular putting of a file
     response = requests.put(url, data=open(zipFilename, 'rb')).text
-    os.remove(zipFilename)
+    try:
+        os.remove(zipFilename)
+    except:
+        pass
+    if filename == temporalFilename:
+        try:
+            os.remove(filename)
+        except:
+            pass
     return True
 
 def _post(certificateFilename: str, keyFilename: str, extension: str = None, payload: dict = None):
     if extension is None:
         extension = ''
     if payload is None:
         payload = {}
```

### Comparing `oathlink-0.8.6/src/oathlink.egg-info/PKG-INFO` & `oathlink-0.8.7/src/oathlink.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.8.6
+Version: 0.8.7
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.8.6/src/oathlink.egg-info/SOURCES.txt` & `oathlink-0.8.7/src/oathlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

