# Comparing `tmp/drf_recaptcha_e2e-1.0-py3-none-any.whl.zip` & `tmp/drf_recaptcha_e2e-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8891 bytes, number of entries: 12
+Zip file size: 8896 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 10:05 drf_recaptcha/__init__.py
 -rw-r--r--  2.0 unx      262 b- defN 23-Jun-19 10:05 drf_recaptcha/apps.py
 -rw-r--r--  2.0 unx     1120 b- defN 23-Jun-19 10:05 drf_recaptcha/checks.py
 -rw-r--r--  2.0 unx     1665 b- defN 23-Jun-19 10:05 drf_recaptcha/client.py
 -rw-r--r--  2.0 unx      697 b- defN 23-Jun-19 10:05 drf_recaptcha/constants.py
 -rw-r--r--  2.0 unx     3216 b- defN 23-Jun-19 10:05 drf_recaptcha/fields.py
 -rw-r--r--  2.0 unx     4932 b- defN 23-Jun-19 10:05 drf_recaptcha/validators.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-19 10:15 drf_recaptcha_e2e-1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5918 b- defN 23-Jun-19 10:15 drf_recaptcha_e2e-1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 10:15 drf_recaptcha_e2e-1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-19 10:15 drf_recaptcha_e2e-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      991 b- defN 23-Jun-19 10:15 drf_recaptcha_e2e-1.0.dist-info/RECORD
-12 files, 19973 bytes uncompressed, 7217 bytes compressed:  63.9%
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-19 10:27 drf_recaptcha_e2e-1.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5929 b- defN 23-Jun-19 10:27 drf_recaptcha_e2e-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 10:27 drf_recaptcha_e2e-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-19 10:27 drf_recaptcha_e2e-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      991 b- defN 23-Jun-19 10:27 drf_recaptcha_e2e-1.1.dist-info/RECORD
+12 files, 19984 bytes uncompressed, 7222 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: drf_recaptcha/fields.py
 Comment: 
 
 Filename: drf_recaptcha/validators.py
 Comment: 
 
-Filename: drf_recaptcha_e2e-1.0.dist-info/LICENSE.md
+Filename: drf_recaptcha_e2e-1.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: drf_recaptcha_e2e-1.0.dist-info/METADATA
+Filename: drf_recaptcha_e2e-1.1.dist-info/METADATA
 Comment: 
 
-Filename: drf_recaptcha_e2e-1.0.dist-info/WHEEL
+Filename: drf_recaptcha_e2e-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: drf_recaptcha_e2e-1.0.dist-info/top_level.txt
+Filename: drf_recaptcha_e2e-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: drf_recaptcha_e2e-1.0.dist-info/RECORD
+Filename: drf_recaptcha_e2e-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `drf_recaptcha_e2e-1.0.dist-info/LICENSE.md` & `drf_recaptcha_e2e-1.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `drf_recaptcha_e2e-1.0.dist-info/METADATA` & `drf_recaptcha_e2e-1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-recaptcha-e2e
-Version: 1.0
+Version: 1.1
 Summary: Django rest framework recaptcha field serializer.
 Home-page: https://github.com/abhay033/drf-recaptcha_e2e.git
 Author: Abhay Bhati
 Author-email: abhaybhati987@gmail.com
 License: MIT
 Keywords: django,drf,rest,django-rest-framework,reCAPTCHA,reCAPTCHA v2,reCAPTCHA v3
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,16 +47,16 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 [![PyPI - License](https://img.shields.io/pypi/l/drf-recaptcha)](https://pypi.org/project/drf-recaptcha/)
 
 ## Requirements
 
-*   Python: 3.7, 3.8, 3.9, 3.10
-*   Django: 3.2, 4.0, 4.1
+*   Python: 3.7, 3.8, 3.9, 3.10, 3.11
+*   Django: 3.2, 4.0, 4.1, 4.2
 *   DRF: 3.11, 3.12, 3.13, 3.14
 
 ## Installation
 
 1.  [Sign up for reCAPTCHA](https://www.google.com/recaptcha/)
 2.  Install with `pip install drf-recaptcha`
 3.  Add `"drf_recaptcha"` to your `INSTALLED_APPS` settings.
```

## Comparing `drf_recaptcha_e2e-1.0.dist-info/RECORD` & `drf_recaptcha_e2e-1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 drf_recaptcha/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 drf_recaptcha/apps.py,sha256=yaXboSMrUJAiy_zFW6Lkxe83-bseipxsArsOsW-hLtg,262
 drf_recaptcha/checks.py,sha256=1HEiMirqMyiHcRTpwuMyBW03DFrpKBV7nS8oI9ZGzQ4,1120
 drf_recaptcha/client.py,sha256=CRokE7Uld18W-3Th0sHrkMVlqGVBtwOCtdq2PfZnnzo,1665
 drf_recaptcha/constants.py,sha256=IrfJZC-wT43iIt-PI04qGQL6AUeKejlyFsYCFl_zk-U,697
 drf_recaptcha/fields.py,sha256=xnHlHbpq763EK1F-A1k7akyHPFE0yig4pkd6umVroHs,3216
 drf_recaptcha/validators.py,sha256=b32S1RJZErufIVXldTuXbYczhiy1-JkY5aNyhxFuVTc,4932
-drf_recaptcha_e2e-1.0.dist-info/LICENSE.md,sha256=llxx7Je1nQxCmPmSNZmtKPVrFRx9IMXEr_W3Tt19qWg,1066
-drf_recaptcha_e2e-1.0.dist-info/METADATA,sha256=xsGMYsV8b_iC194BEe11O-6PXLfzSsjrnYPhxvBvwbg,5918
-drf_recaptcha_e2e-1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-drf_recaptcha_e2e-1.0.dist-info/top_level.txt,sha256=xu-JIpEQhXwP9aNr6ztYf2IBe3QWLoGjmaZW0Lb7V2c,14
-drf_recaptcha_e2e-1.0.dist-info/RECORD,,
+drf_recaptcha_e2e-1.1.dist-info/LICENSE.md,sha256=llxx7Je1nQxCmPmSNZmtKPVrFRx9IMXEr_W3Tt19qWg,1066
+drf_recaptcha_e2e-1.1.dist-info/METADATA,sha256=VcF9O7nfr8xjAaGI5muRzOXR2zuA_XesJ_pmaNPwdBg,5929
+drf_recaptcha_e2e-1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+drf_recaptcha_e2e-1.1.dist-info/top_level.txt,sha256=xu-JIpEQhXwP9aNr6ztYf2IBe3QWLoGjmaZW0Lb7V2c,14
+drf_recaptcha_e2e-1.1.dist-info/RECORD,,
```

