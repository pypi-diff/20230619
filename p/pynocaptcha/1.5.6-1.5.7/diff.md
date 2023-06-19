# Comparing `tmp/pynocaptcha-1.5.6.tar.gz` & `tmp/pynocaptcha-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.5.6.tar", last modified: Sat Jun 17 09:04:31 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.7.tar", last modified: Mon Jun 19 07:24:39 2023, max compression
```

## Comparing `pynocaptcha-1.5.6.tar` & `pynocaptcha-1.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-17 09:04:31.000000 pynocaptcha-1.5.6/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-17 09:04:31.000000 pynocaptcha-1.5.6/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-17 09:04:31.000000 pynocaptcha-1.5.6/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.5.6/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-17 09:04:31.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1006 2023-06-14 09:31:37.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4785 2023-06-15 08:58:13.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)   222197 2023-06-17 09:04:20.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.5.6/pynocaptcha/crackers/tls.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-17 09:04:10.000000 pynocaptcha-1.5.6/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-19 07:24:39.000000 pynocaptcha-1.5.7/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-19 07:24:39.000000 pynocaptcha-1.5.7/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-19 07:24:39.000000 pynocaptcha-1.5.7/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      630 2023-06-14 09:34:47.000000 pynocaptcha-1.5.7/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-19 07:24:39.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1006 2023-06-14 09:31:37.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4785 2023-06-15 08:58:13.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)   222296 2023-06-19 07:24:22.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.5.7/pynocaptcha/crackers/tls.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-19 07:24:34.000000 pynocaptcha-1.5.7/setup.py
```

### Comparing `pynocaptcha-1.5.6/PKG-INFO` & `pynocaptcha-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.5.6
+Version: 1.5.7
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.5.6/pynocaptcha/__init__.py` & `pynocaptcha-1.5.7/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/incapsula.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,14 @@
         # proxy=proxy,
         # submit=False
     )
     ret = cracker.crack()
     """
     
     # 必传参数
-    must_check_params = ["script", "cookies"]
+    must_check_params = ["cookies"]
+    # 可选参数
+    option_params = {
+        "href": "",
+        "script": "",
+        "proxy": ""
+    }
```

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.5.7/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.6/setup.py` & `pynocaptcha-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.5.6',
+    version='1.5.7',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

