# Comparing `tmp/oathlink-0.8.7.tar.gz` & `tmp/oathlink-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oathlink-0.8.7.tar", last modified: Mon Jun 19 16:54:18 2023, max compression
+gzip compressed data, was "oathlink-0.8.8.tar", last modified: Mon Jun 19 17:18:14 2023, max compression
```

## Comparing `oathlink-0.8.7.tar` & `oathlink-0.8.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803681 oathlink-0.8.7/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.8.7/LICENSE
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 16:54:18.803759 oathlink-0.8.7/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.8.7/README.md
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.8.7/pyproject.toml
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      824 2023-06-19 16:54:18.804050 oathlink-0.8.7/setup.cfg
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.795661 oathlink-0.8.7/src/
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.796812 oathlink-0.8.7/src/oathlink/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.8.7/src/oathlink/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.797888 oathlink-0.8.7/src/oathlink/main/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/main/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     5317 2023-06-19 16:53:04.000000 oathlink-0.8.7/src/oathlink/main/oathlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.798193 oathlink-0.8.7/src/oathlink/services/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.798454 oathlink-0.8.7/src/oathlink/services/agent/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.799325 oathlink-0.8.7/src/oathlink/services/agent/account/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/create.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/link.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/account/unlink.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.800061 oathlink-0.8.7/src/oathlink/services/agent/ip/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/add.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/agent/ip/remove.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/hello.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.801743 oathlink-0.8.7/src/oathlink/services/record/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/record/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/record/archive.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/record/cancel.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      896 2023-06-16 15:22:00.000000 oathlink-0.8.7/src/oathlink/services/record/decrypt.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-06-19 16:51:14.000000 oathlink-0.8.7/src/oathlink/services/record/download.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1261 2023-05-29 20:30:18.000000 oathlink-0.8.7/src/oathlink/services/record/upload.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.802583 oathlink-0.8.7/src/oathlink/services/report/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/services/report/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/history.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/outstanding.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.8.7/src/oathlink/services/report/record.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.802828 oathlink-0.8.7/src/oathlink/util/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803225 oathlink-0.8.7/src/oathlink/util/crypto/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.8.7/src/oathlink/util/crypto/Fernet.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/crypto/__init__.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.803440 oathlink-0.8.7/src/oathlink/util/https/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.7/src/oathlink/util/https/__init__.py
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     2852 2023-06-19 16:46:59.000000 oathlink-0.8.7/src/oathlink/util/https/https.py
-drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 16:54:18.797674 oathlink-0.8.7/src/oathlink.egg-info/
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/PKG-INFO
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/requires.txt
--rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-06-19 16:54:18.000000 oathlink-0.8.7/src/oathlink.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.119721 oathlink-0.8.8/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      714 2023-05-26 19:09:37.000000 oathlink-0.8.8/LICENSE
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 17:18:14.119806 oathlink-0.8.8/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       97 2023-05-26 20:09:28.000000 oathlink-0.8.8/README.md
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      233 2023-05-26 20:26:31.000000 oathlink-0.8.8/pyproject.toml
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      824 2023-06-19 17:18:14.120093 oathlink-0.8.8/setup.cfg
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.111698 oathlink-0.8.8/src/
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.112848 oathlink-0.8.8/src/oathlink/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       38 2023-05-26 20:49:07.000000 oathlink-0.8.8/src/oathlink/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.113750 oathlink-0.8.8/src/oathlink/main/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/main/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     5313 2023-06-19 17:16:33.000000 oathlink-0.8.8/src/oathlink/main/oathlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.114220 oathlink-0.8.8/src/oathlink/services/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.114475 oathlink-0.8.8/src/oathlink/services/agent/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/agent/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.115259 oathlink-0.8.8/src/oathlink/services/agent/account/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/agent/account/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1096 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/agent/account/create.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1079 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/agent/account/link.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1083 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/agent/account/unlink.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.115986 oathlink-0.8.8/src/oathlink/services/agent/ip/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/agent/ip/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1053 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/agent/ip/add.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1059 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/agent/ip/remove.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      911 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/hello.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.117936 oathlink-0.8.8/src/oathlink/services/record/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/record/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1315 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/record/archive.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1182 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/record/cancel.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1022 2023-06-19 17:17:53.000000 oathlink-0.8.8/src/oathlink/services/record/decrypt.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1074 2023-06-19 16:51:14.000000 oathlink-0.8.8/src/oathlink/services/record/download.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1261 2023-05-29 20:30:18.000000 oathlink-0.8.8/src/oathlink/services/record/upload.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.118740 oathlink-0.8.8/src/oathlink/services/report/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/services/report/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1188 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/report/history.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      999 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/report/outstanding.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1318 2023-05-26 20:13:39.000000 oathlink-0.8.8/src/oathlink/services/report/record.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.118990 oathlink-0.8.8/src/oathlink/util/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/util/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.119358 oathlink-0.8.8/src/oathlink/util/crypto/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1019 2023-03-10 12:57:36.000000 oathlink-0.8.8/src/oathlink/util/crypto/Fernet.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/util/crypto/__init__.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.119543 oathlink-0.8.8/src/oathlink/util/https/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-05-26 20:05:39.000000 oathlink-0.8.8/src/oathlink/util/https/__init__.py
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     2834 2023-06-19 17:16:04.000000 oathlink-0.8.8/src/oathlink/util/https/https.py
+drwxr-xr-x   0 benjaminmirandacaballero   (501) staff       (20)        0 2023-06-19 17:18:14.113537 oathlink-0.8.8/src/oathlink.egg-info/
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)      689 2023-06-19 17:18:14.000000 oathlink-0.8.8/src/oathlink.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)     1292 2023-06-19 17:18:14.000000 oathlink-0.8.8/src/oathlink.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        1 2023-06-19 17:18:14.000000 oathlink-0.8.8/src/oathlink.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)       77 2023-06-19 17:18:14.000000 oathlink-0.8.8/src/oathlink.egg-info/requires.txt
+-rw-r--r--   0 benjaminmirandacaballero   (501) staff       (20)        9 2023-06-19 17:18:14.000000 oathlink-0.8.8/src/oathlink.egg-info/top_level.txt
```

### Comparing `oathlink-0.8.7/LICENSE` & `oathlink-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/PKG-INFO` & `oathlink-0.8.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.8.7
+Version: 0.8.8
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.8.7/setup.cfg` & `oathlink-0.8.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oathlink
-version = 0.8.7
+version = 0.8.8
 author = oathlink
 author_email = oathlink@bfi.lat
 description = This repository holds the Oathlink user Python package (client source code).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 project_urls =
```

### Comparing `oathlink-0.8.7/src/oathlink/main/oathlink.py` & `oathlink-0.8.8/src/oathlink/main/oathlink.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 def download(certificate_filename_pem: str, certificate_filename_key: str, record_id: str) -> str:
     return getOathlinkDownload(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                                oathId=record_id)
 
 def decrypt(record_id_encrypted: str, secret: str) -> str:
     return decryptOathId(oathIdEncrypted=record_id_encrypted, oathSecret=secret)
 
-def archive(certificate_filename_pem: str, certificate_filename_key: str, record_id: [str, list] = None) -> list:
+def archive(certificate_filename_pem: str, certificate_filename_key: str, record_id: str | list = None) -> list:
     return archiveOathlink(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                            recordId=record_id)
 
-def cancel(certificate_filename_pem: str, certificate_filename_key: str, record_id: [str, list] = None) -> list:
+def cancel(certificate_filename_pem: str, certificate_filename_key: str, record_id: str | list = None) -> list:
     return cancelOathlink(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                           recordId=record_id)
 
 def agent_create(certificate_filename_pem: str, certificate_filename_key: str, serial: str, description: str) -> str:
     return createAgent(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                        serial=serial, description=description)
 
@@ -65,17 +65,17 @@
 
 def agent_link(certificate_filename_pem: str, certificate_filename_key: str, user_id: str) -> str:
     return linkAgents(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key, userId=user_id)
 
 def agent_unlink(certificate_filename_pem: str, certificate_filename_key: str, user_id: str) -> str:
     return unlinkAgents(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key, userId=user_id)
 
-def report_record(certificate_filename_pem: str, certificate_filename_key: str, record_id: [str, list] = None) -> list:
+def report_record(certificate_filename_pem: str, certificate_filename_key: str, record_id: str | list = None) -> list:
     return reportRecord(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                         recordId=record_id)
 
-def report_history(certificate_filename_pem: str, certificate_filename_key: str, record_id: [str, list] = None) -> str:
+def report_history(certificate_filename_pem: str, certificate_filename_key: str, record_id: str | list = None) -> str:
     return reportHistory(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key,
                          recordId=record_id)
 
 def report_outstanding(certificate_filename_pem: str, certificate_filename_key: str) -> str:
     return reportOutstanding(certificateFilename=certificate_filename_pem, keyFilename=certificate_filename_key)
```

### Comparing `oathlink-0.8.7/src/oathlink/services/agent/account/create.py` & `oathlink-0.8.8/src/oathlink/services/agent/account/create.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/agent/account/link.py` & `oathlink-0.8.8/src/oathlink/services/agent/account/link.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/agent/account/unlink.py` & `oathlink-0.8.8/src/oathlink/services/agent/account/unlink.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/agent/ip/add.py` & `oathlink-0.8.8/src/oathlink/services/agent/ip/add.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/agent/ip/remove.py` & `oathlink-0.8.8/src/oathlink/services/agent/ip/remove.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/hello.py` & `oathlink-0.8.8/src/oathlink/services/hello.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/record/archive.py` & `oathlink-0.8.8/src/oathlink/services/record/archive.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/record/cancel.py` & `oathlink-0.8.8/src/oathlink/services/record/cancel.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/record/decrypt.py` & `oathlink-0.8.8/src/oathlink/services/record/decrypt.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,11 +3,15 @@
 agreement.
 BFI Software License Agreement: Any User wishing to make a commercial use of the Software must contact BFI
 at jacques.burrus@bfi.lat to arrange an appropriate license. Commercial use includes (1) integrating or incorporating
 all or part of the source code into a product for sale or license by, or on behalf of, User to third parties,
 or (2) distribution of the binary or source code to third parties for use with a commercial product sold or licensed
 by, or on behalf of, User. """
 
+import os
 from oathlink.util.crypto import Fernet
 
 def decryptOathId(oathIdEncrypted: str, oathSecret: str) -> str:
+    if os.path.isfile(oathSecret):
+        with open(oathSecret, 'r') as file:
+            oathSecret = file.read()
     return Fernet.decode(key=oathSecret, encryptedString=oathIdEncrypted)
```

### Comparing `oathlink-0.8.7/src/oathlink/services/record/download.py` & `oathlink-0.8.8/src/oathlink/services/record/download.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/record/upload.py` & `oathlink-0.8.8/src/oathlink/services/record/upload.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/report/history.py` & `oathlink-0.8.8/src/oathlink/services/report/history.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/report/outstanding.py` & `oathlink-0.8.8/src/oathlink/services/report/outstanding.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/services/report/record.py` & `oathlink-0.8.8/src/oathlink/services/report/record.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/util/crypto/Fernet.py` & `oathlink-0.8.8/src/oathlink/util/crypto/Fernet.py`

 * *Files identical despite different names*

### Comparing `oathlink-0.8.7/src/oathlink/util/https/https.py` & `oathlink-0.8.8/src/oathlink/util/https/https.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 by, or on behalf of, User. """
 
 import os
 import json
 import requests
 from zipfile import ZipFile
 
+
 def _getBaseUrl() -> str:
     return 'https://api.oathlink.com'
 
+
 def _getUrl(extension: str) -> str:
     if len(extension) > 0:
         if extension[0] == '/':
             extension = extension[1:]
     return f'{_getBaseUrl()}/{extension}'
 
-def get(url: str) -> list:
-    filename = 'download.txt'
+
+def get(url: str) -> str | list:
     response = requests.get(url)
     zipFilename = f'download.zip'
     with open(zipFilename, 'wb') as file:
         file.write(response.content)
     with ZipFile(zipFilename, 'r') as zip:
         zip.extractall()
         info = zip.infolist()[0]
@@ -60,23 +62,25 @@
     if filename == temporalFilename:
         try:
             os.remove(filename)
         except:
             pass
     return True
 
+
 def _post(certificateFilename: str, keyFilename: str, extension: str = None, payload: dict = None):
     if extension is None:
         extension = ''
     if payload is None:
         payload = {}
     cert = (certificateFilename, keyFilename)
     data = json.dumps(payload)
     response = requests.post(_getUrl(extension), data=data, cert=cert)
     return response.text
 
+
 def _get(certificateFilename: str, keyFilename: str, extension: str = None):
     if extension is None:
         extension = ''
     cert = (certificateFilename, keyFilename)
     response = requests.get(_getUrl(extension), cert=cert)
-    return response.text
+    return response.text
```

### Comparing `oathlink-0.8.7/src/oathlink.egg-info/PKG-INFO` & `oathlink-0.8.8/src/oathlink.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oathlink
-Version: 0.8.7
+Version: 0.8.8
 Summary: This repository holds the Oathlink user Python package (client source code).
 Home-page: https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git
 Author: oathlink
 Author-email: oathlink@bfi.lat
 Project-URL: Bug Tracker, https://github.com/BurrusFinancialIntelligence/Oathlink-Client.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `oathlink-0.8.7/src/oathlink.egg-info/SOURCES.txt` & `oathlink-0.8.8/src/oathlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

