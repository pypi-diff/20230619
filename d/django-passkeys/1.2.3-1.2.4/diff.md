# Comparing `tmp/django-passkeys-1.2.3.tar.gz` & `tmp/django-passkeys-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-passkeys-1.2.3.tar", last modified: Sat Jun 17 16:35:08 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.4.tar", last modified: Mon Jun 19 14:09:30 2023, max compression
```

## Comparing `django-passkeys-1.2.3.tar` & `django-passkeys-1.2.4.tar`

### file list

```diff
@@ -1,44 +1,40 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-10-28 10:01:16.000000 django-passkeys-1.2.3/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      192 2023-06-17 16:31:58.000000 django-passkeys-1.2.3/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7525 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6148 2023-06-17 16:34:53.000000 django-passkeys-1.2.3/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7525 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      913 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-10-28 13:54:59.000000 django-passkeys-1.2.3/django_passkeys.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       17 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/django_passkeys.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/env/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/env/bin/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1199 2022-10-28 10:01:55.000000 django-passkeys-1.2.3/env/bin/activate_this.py
--rwxrwxr-x   0 mohamed   (1000) mohamed   (1000)      153 2022-10-28 10:02:36.000000 django-passkeys-1.2.3/env/bin/django-admin.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5823 2023-06-17 15:37:35.000000 django-passkeys-1.2.3/passkeys/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2022-10-28 11:16:36.000000 django-passkeys-1.2.3/passkeys/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      790 2023-06-17 11:35:33.000000 django-passkeys-1.2.3/passkeys/backend.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2022-10-28 13:18:42.000000 django-passkeys-1.2.3/passkeys/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2022-10-28 10:29:36.000000 django-passkeys-1.2.3/passkeys/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2022-12-09 11:07:59.000000 django-passkeys-1.2.3/passkeys/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2019-06-20 18:14:15.000000 django-passkeys-1.2.3/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     8981 2022-08-24 16:03:28.000000 django-passkeys-1.2.3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2022-10-23 19:24:16.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/base64url.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2019-06-20 18:14:15.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2022-10-23 19:24:16.000000 django-passkeys-1.2.3/passkeys/static/passkeys/js/helpers.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/passkeys/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-06-17 11:35:33.000000 django-passkeys-1.2.3/passkeys/templates/PassKeys.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2022-10-28 10:53:07.000000 django-passkeys-1.2.3/passkeys/templates/PassKeys_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/templates/check_passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2022-09-09 17:51:05.000000 django-passkeys-1.2.3/passkeys/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2249 2023-06-17 09:46:50.000000 django-passkeys-1.2.3/passkeys/templates/passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2022-12-09 11:08:08.000000 django-passkeys-1.2.3/passkeys/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-17 16:35:08.000000 django-passkeys-1.2.3/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-06-17 16:35:01.000000 django-passkeys-1.2.3/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      192 2023-06-19 06:42:21.000000 django-passkeys-1.2.4/MANIFEST.in
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7691 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6314 2023-06-19 13:56:23.000000 django-passkeys-1.2.4/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/django_passkeys.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7691 2023-06-19 14:09:30.000000 django-passkeys-1.2.4/django_passkeys.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2023-06-19 14:09:30.000000 django-passkeys-1.2.4/django_passkeys.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-19 14:09:30.000000 django-passkeys-1.2.4/django_passkeys.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.2.4/django_passkeys.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-06-19 14:09:30.000000 django-passkeys-1.2.4/django_passkeys.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       17 2023-06-19 14:09:30.000000 django-passkeys-1.2.4/django_passkeys.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5823 2023-06-19 06:42:21.000000 django-passkeys-1.2.4/passkeys/FIDO2.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      790 2023-06-19 06:42:21.000000 django-passkeys-1.2.4/passkeys/backend.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/migrations/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/migrations/0001_initial.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/migrations/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/models.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/static/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/static/passkeys/
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/static/passkeys/css/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/static/passkeys/imgs/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8981 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/static/passkeys/js/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/static/passkeys/js/base64url.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/static/passkeys/js/helpers.js
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/passkeys/templates/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-05-23 13:57:16.000000 django-passkeys-1.2.4/passkeys/templates/PassKeys.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/templates/PassKeys_base.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/templates/check_passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/templates/modal.html
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2249 2023-06-08 06:46:46.000000 django-passkeys-1.2.4/passkeys/templates/passkeys.js
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2023-04-09 08:41:37.000000 django-passkeys-1.2.4/passkeys/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1023 2023-06-19 13:24:31.000000 django-passkeys-1.2.4/passkeys/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-19 14:09:30.716174 django-passkeys-1.2.4/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-06-19 14:09:28.000000 django-passkeys-1.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-passkeys-1.2.3/LICENSE` & `django-passkeys-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/PKG-INFO` & `django-passkeys-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,14 +37,18 @@
 
 [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https://badge.fury.io/py/django-passkeys)
 [![Downloads](https://static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-passkeys)
 [![Downloads / Month ](https://pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-passkeys)
 [![build](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml)
 ![Coverage](https://raw.githubusercontent.com/mkalioby/django-passkeys/main/coverage.svg)
 
+![Django Versions](https://img.shields.io/pypi/frameworkversions/django/django-passkeys)
+![Python Versions](https://img.shields.io/pypi/pyversions/django-passkeys)
+
+
 An extension to Django *ModelBackend* backend to support passkeys.
 
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on
```

### Comparing `django-passkeys-1.2.3/README.md` & `django-passkeys-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https://badge.fury.io/py/django-passkeys)
 [![Downloads](https://static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-passkeys)
 [![Downloads / Month ](https://pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-passkeys)
 [![build](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml)
 ![Coverage](https://raw.githubusercontent.com/mkalioby/django-passkeys/main/coverage.svg)
 
+![Django Versions](https://img.shields.io/pypi/frameworkversions/django/django-passkeys)
+![Python Versions](https://img.shields.io/pypi/pyversions/django-passkeys)
+
+
 An extension to Django *ModelBackend* backend to support passkeys.
 
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on
```

#### html2text {}

```diff
@@ -2,24 +2,26 @@
 passkeys.svg)](https://badge.fury.io/py/django-passkeys) [![Downloads](https://
 static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-
 passkeys) [![Downloads / Month ](https://pepy.tech/badge/django-passkeys/
 month)](https://pepy.tech/project/django-passkeys) [![build](https://
 github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/
 badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/
 basic_checks.yml) ![Coverage](https://raw.githubusercontent.com/mkalioby/
-django-passkeys/main/coverage.svg) An extension to Django *ModelBackend*
-backend to support passkeys. Passkeys is an extension to Web Authentication API
-that will allow the user to login to a service using another device. This app
-is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-
-mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone 16.0+, iPadOS
-16.1, Mac OS X Ventura) * Chromium based browsers (on PC and Laptop) allows
-picking up credentials from Android and iPhone/iPadOS. * Android Credentials
-creation for ResidentKeys is currently in live now. On May 3, 2023, Google
-allowed the use of Passkeys for the users to login, killing the password for
-enrolled users. # Installation `pip install django-passkeys` Currently, it
+django-passkeys/main/coverage.svg) ![Django Versions](https://img.shields.io/
+pypi/frameworkversions/django/django-passkeys) ![Python Versions](https://
+img.shields.io/pypi/pyversions/django-passkeys) An extension to Django
+*ModelBackend* backend to support passkeys. Passkeys is an extension to Web
+Authentication API that will allow the user to login to a service using another
+device. This app is a slim-down version of [django-mfa2](https://github.com/
+mkalioby/django-mfa2) Passkeys are now supported on * Apple Ecosystem (iPhone
+16.0+, iPadOS 16.1, Mac OS X Ventura) * Chromium based browsers (on PC and
+Laptop) allows picking up credentials from Android and iPhone/iPadOS. * Android
+Credentials creation for ResidentKeys is currently in live now. On May 3, 2023,
+Google allowed the use of Passkeys for the users to login, killing the password
+for enrolled users. # Installation `pip install django-passkeys` Currently, it
 support Django 2.0+, Python 3.7+ # Usage 1. in your settings.py add the
 application to your installed apps ```python INSTALLED_APPS=( '......',
 'passkeys', '......') ``` 2. Collect Static Files `python manage.py
 collectstatic` 3. Run migrate `python manage.py migrate` 4. Add the following
 settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
```

### Comparing `django-passkeys-1.2.3/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.4/django_passkeys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,14 +37,18 @@
 
 [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https://badge.fury.io/py/django-passkeys)
 [![Downloads](https://static.pepy.tech/badge/django-passkeys)](https://pepy.tech/project/django-passkeys)
 [![Downloads / Month ](https://pepy.tech/badge/django-passkeys/month)](https://pepy.tech/project/django-passkeys)
 [![build](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml/badge.svg)](https://github.com/mkalioby/django-passkeys/actions/workflows/basic_checks.yml)
 ![Coverage](https://raw.githubusercontent.com/mkalioby/django-passkeys/main/coverage.svg)
 
+![Django Versions](https://img.shields.io/pypi/frameworkversions/django/django-passkeys)
+![Python Versions](https://img.shields.io/pypi/pyversions/django-passkeys)
+
+
 An extension to Django *ModelBackend* backend to support passkeys.
 
 Passkeys is an extension to Web Authentication API that will allow the user to login to a service using another device.
 
 This app is a slim-down version of [django-mfa2](https://github.com/mkalioby/django-mfa2)
 
 Passkeys are now supported on
```

### Comparing `django-passkeys-1.2.3/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.4/django_passkeys.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 setup.py
 django_passkeys.egg-info/PKG-INFO
 django_passkeys.egg-info/SOURCES.txt
 django_passkeys.egg-info/dependency_links.txt
 django_passkeys.egg-info/not-zip-safe
 django_passkeys.egg-info/requires.txt
 django_passkeys.egg-info/top_level.txt
-env/bin/activate_this.py
-env/bin/django-admin.py
 passkeys/FIDO2.py
 passkeys/__init__.py
 passkeys/backend.py
 passkeys/models.py
 passkeys/urls.py
 passkeys/views.py
 passkeys/migrations/0001_initial.py
```

### Comparing `django-passkeys-1.2.3/passkeys/FIDO2.py` & `django-passkeys-1.2.4/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/backend.py` & `django-passkeys-1.2.4/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.4/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/models.py` & `django-passkeys-1.2.4/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.4/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.4/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.4/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.4/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.4/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.4/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.4/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/templates/modal.html` & `django-passkeys-1.2.4/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/templates/passkeys.js` & `django-passkeys-1.2.4/passkeys/templates/passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/urls.py` & `django-passkeys-1.2.4/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.3/passkeys/views.py` & `django-passkeys-1.2.4/passkeys/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from django.contrib.auth.decorators import login_required
 from django.http import HttpResponse
 from django.shortcuts import render
 
 from .models import UserPasskey
 
 @login_required
-def index(request,enroll=False):
-    keys = UserPasskey.objects.filter(user=request.user)
-    return render(request,'PassKeys.html',{"keys":keys,"enroll":enroll})
+def index(request,enroll=False): # noqa
+    keys = UserPasskey.objects.filter(user=request.user) # pragma: no cover
+    return render(request,'PassKeys.html',{"keys":keys,"enroll":enroll}) # pragma: no cover
 
 
 @login_required
 def delKey(request):
     key=UserPasskey.objects.get(id=request.GET["id"])
     if key.user.pk  == request.user.pk:
         key.delete()
         return HttpResponse("Deleted Successfully")
-    return HttpResponse("Error: You own this token so you can't delete it")
+    return HttpResponse("Error: You own this token so you can't delete it", status=403)
 
 @login_required
 def toggleKey(request):
     id=request.GET["id"]
     q=UserPasskey.objects.filter(user=request.user, id=id)
     if q.count()==1:
         key=q[0]
         key.enabled=not key.enabled
         key.save()
         return HttpResponse("OK")
-    return HttpResponse("Error")
+    return HttpResponse("Error: You own this token so you can't toggle it", status=403)
```

### Comparing `django-passkeys-1.2.3/setup.py` & `django-passkeys-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.3',
+    version='1.2.4',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

