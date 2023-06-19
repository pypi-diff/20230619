# Comparing `tmp/django-navhelper-0.1.tar.gz` & `tmp/django-navhelper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-navhelper-0.1.tar", last modified: Sun Oct 27 10:00:13 2013, max compression
+gzip compressed data, was "django-navhelper-1.0.0.tar", last modified: Mon Jun 19 20:47:47 2023, max compression
```

## Comparing `django-navhelper-0.1.tar` & `django-navhelper-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/
--rw-r--r--   0 gluchet    (501) staff       (20)     1084 2013-10-27 09:44:40.000000 django-navhelper-0.1/LICENSE.txt
--rw-r--r--   0 gluchet    (501) staff       (20)       38 2013-10-27 09:45:15.000000 django-navhelper-0.1/MANIFEST.in
--rw-r--r--   0 gluchet    (501) staff       (20)     1970 2013-10-27 10:00:13.000000 django-navhelper-0.1/PKG-INFO
--rw-r--r--   0 gluchet    (501) staff       (20)     1158 2013-10-27 09:50:34.000000 django-navhelper-0.1/README.md
--rw-r--r--   0 gluchet    (501) staff       (20)      100 2013-10-27 10:00:13.000000 django-navhelper-0.1/setup.cfg
--rw-r--r--   0 gluchet    (501) staff       (20)     1246 2013-10-27 09:49:31.000000 django-navhelper-0.1/setup.py
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/
--rw-r--r--   0 gluchet    (501) staff       (20)        1 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/dependency_links.txt
--rw-r--r--   0 gluchet    (501) staff       (20)       23 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/namespace_packages.txt
--rw-r--r--   0 gluchet    (501) staff       (20)     1970 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/PKG-INFO
--rw-r--r--   0 gluchet    (501) staff       (20)      486 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/SOURCES.txt
--rw-r--r--   0 gluchet    (501) staff       (20)        8 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/django_navhelper.egg-info/top_level.txt
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/geelweb/
--rw-r--r--   0 gluchet    (501) staff       (20)       56 2013-10-27 09:23:04.000000 django-navhelper-0.1/src/geelweb/__init__.py
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/geelweb/django/
--rw-r--r--   0 gluchet    (501) staff       (20)       56 2013-10-27 09:23:22.000000 django-navhelper-0.1/src/geelweb/django/__init__.py
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/geelweb/django/navhelper/
--rw-r--r--   0 gluchet    (501) staff       (20)        0 2013-10-27 09:00:10.000000 django-navhelper-0.1/src/geelweb/django/navhelper/__init__.py
-drwxr-xr-x   0 gluchet    (501) staff       (20)        0 2013-10-27 10:00:13.000000 django-navhelper-0.1/src/geelweb/django/navhelper/templatetags/
--rw-r--r--   0 gluchet    (501) staff       (20)        0 2013-10-27 09:00:18.000000 django-navhelper-0.1/src/geelweb/django/navhelper/templatetags/__init__.py
--rw-r--r--   0 gluchet    (501) staff       (20)      772 2013-10-27 09:20:05.000000 django-navhelper-0.1/src/geelweb/django/navhelper/templatetags/navactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.597791 django-navhelper-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/src/django_navhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-19 20:47:47.000000 django-navhelper-1.0.0/src/django_navhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-19 20:47:47.000000 django-navhelper-1.0.0/src/django_navhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:47:47.000000 django-navhelper-1.0.0/src/django_navhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 20:47:47.000000 django-navhelper-1.0.0/src/django_navhelper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 20:47:47.000000 django-navhelper-1.0.0/src/django_navhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/src/geelweb/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/src/geelweb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/src/geelweb/django/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/src/geelweb/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/src/geelweb/django/navhelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/src/geelweb/django/navhelper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/src/geelweb/django/navhelper/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/src/geelweb/django/navhelper/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/src/geelweb/django/navhelper/templatetags/navactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:47:47.601791 django-navhelper-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-19 20:47:32.000000 django-navhelper-1.0.0/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-navhelper-0.1/LICENSE.txt` & `django-navhelper-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-navhelper-0.1/setup.py` & `django-navhelper-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # vim: set expandtab tabstop=4 shiftwidth=4 softtabstop=4:
 
 """
 django navhelper setup script
 """
 
 __author__ = "Guillaume Luchet <guillaume@geelweb.org>"
-__version__ = "0.1"
+__version__ = "1.0.0"
 
 import os, sys
 from setuptools import setup, find_packages
 
 author_data = __author__.split(" ")
 maintainer = " ".join(author_data[0:-1])
 maintainer_email = author_data[-1]
-README = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
+README = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
 
 if __name__ == "__main__":
     setup(
         name="django-navhelper",
         version=__version__,
         description="Django template tags designed to help the navigation rendering",
         long_description=README,
```

