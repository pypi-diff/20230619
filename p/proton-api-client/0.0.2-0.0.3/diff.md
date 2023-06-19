# Comparing `tmp/proton-api-client-0.0.2.tar.gz` & `tmp/proton-api-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.2.tar", last modified: Mon Jun 19 18:26:39 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.3.tar", last modified: Mon Jun 19 18:31:40 2023, max compression
```

## Comparing `proton-api-client-0.0.2.tar` & `proton-api-client-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:26:39.385460 proton-api-client-0.0.2/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.2/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1147 2023-06-19 18:26:39.385460 proton-api-client-0.0.2/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      758 2023-06-19 18:25:19.000000 proton-api-client-0.0.2/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:26:39.385460 proton-api-client-0.0.2/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.2/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.2/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4077 2023-06-19 18:23:32.000000 proton-api-client-0.0.2/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4711 2023-06-19 17:57:55.000000 proton-api-client-0.0.2/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2134 2023-06-19 18:15:31.000000 proton-api-client-0.0.2/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2174 2023-06-19 17:57:18.000000 proton-api-client-0.0.2/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.2/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:26:39.385460 proton-api-client-0.0.2/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1147 2023-06-19 18:26:39.000000 proton-api-client-0.0.2/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-19 18:26:39.000000 proton-api-client-0.0.2/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 18:26:39.000000 proton-api-client-0.0.2/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-19 18:26:39.000000 proton-api-client-0.0.2/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-19 18:26:39.000000 proton-api-client-0.0.2/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 18:26:39.385460 proton-api-client-0.0.2/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1671 2023-06-19 18:25:57.000000 proton-api-client-0.0.2/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.3/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1135 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      747 2023-06-19 18:31:17.000000 proton-api-client-0.0.3/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.3/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.3/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4077 2023-06-19 18:23:32.000000 proton-api-client-0.0.3/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4711 2023-06-19 17:57:55.000000 proton-api-client-0.0.3/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2134 2023-06-19 18:15:31.000000 proton-api-client-0.0.3/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2174 2023-06-19 17:57:18.000000 proton-api-client-0.0.3/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.3/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1135 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1655 2023-06-19 18:31:17.000000 proton-api-client-0.0.3/setup.py
```

### Comparing `proton-api-client-0.0.2/LICENSE` & `proton-api-client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/PKG-INFO` & `proton-api-client-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -16,19 +16,19 @@
 
 #### Examples
 
 ```python
 from proton.client import ProtonMail
 
 username, password = ..., ...
-gpg_passphrase = ...
-proton = ProtonMail(username, password, gpg_passphrase=gpg_passphrase)
+proton = ProtonMail(username, password)
 
-# pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
-# proton.gpg_import(pk)
+passphrase = 'myPass'
+pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+proton.gpg_import(pk, passphrase=passphrase)
 
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
 
@@ -45,8 +45,7 @@
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
 ```
-
```

### Comparing `proton-api-client-0.0.2/README.md` & `proton-api-client-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 #### Examples
 
 ```python
 from proton.client import ProtonMail
 
 username, password = ..., ...
-gpg_passphrase = ...
-proton = ProtonMail(username, password, gpg_passphrase=gpg_passphrase)
+proton = ProtonMail(username, password)
 
-# pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
-# proton.gpg_import(pk)
+passphrase = 'myPass'
+pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+proton.gpg_import(pk, passphrase=passphrase)
 
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
```

### Comparing `proton-api-client-0.0.2/proton/_ctsrp.py` & `proton-api-client-0.0.3/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton/_pysrp.py` & `proton-api-client-0.0.3/proton/_pysrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton/client.py` & `proton-api-client-0.0.3/proton/client.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton/constants.py` & `proton-api-client-0.0.3/proton/constants.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton/helpers.py` & `proton-api-client-0.0.3/proton/helpers.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton/login.py` & `proton-api-client-0.0.3/proton/login.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.2/proton_api_client.egg-info/PKG-INFO` & `proton-api-client-0.0.3/proton_api_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -16,19 +16,19 @@
 
 #### Examples
 
 ```python
 from proton.client import ProtonMail
 
 username, password = ..., ...
-gpg_passphrase = ...
-proton = ProtonMail(username, password, gpg_passphrase=gpg_passphrase)
+proton = ProtonMail(username, password)
 
-# pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
-# proton.gpg_import(pk)
+passphrase = 'myPass'
+pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+proton.gpg_import(pk, passphrase=passphrase)
 
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
 
@@ -45,8 +45,7 @@
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
 ```
-
```

### Comparing `proton-api-client-0.0.2/setup.py` & `proton-api-client-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,32 +10,32 @@
     'orjson',
     'httpx',
     'tqdm',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.2',
+    version='0.0.3',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
     
     ```python
     from proton.client import ProtonMail
     
     username, password = ..., ...
-    gpg_passphrase = ...
-    proton = ProtonMail(username, password, gpg_passphrase=gpg_passphrase)
+    proton = ProtonMail(username, password)
     
-    # pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
-    # proton.gpg_import(pk)
+    passphrase = 'myPass'
+    pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
+    proton.gpg_import(pk, passphrase=passphrase)
     
     salts = proton.salts()
     
     users = proton.users()
     
     inbox = proton.inbox()
     
@@ -52,15 +52,14 @@
     
     timezones = proton.timezones()
     
     addresses = proton.addresses()
     
     info = proton.info()
     ```
-    
     '''),
     long_description_content_type='text/markdown',
     author='Trevor Hobenshield',
     author_email='trevorhobenshield@gmail.com',
     url='https://github.com/trevorhobenshield/proton-api-client',
     install_requires=install_requires,
     keywords='proton api client async search automation bot scrape mail email',
```

