# Comparing `tmp/django-pgviews-schema-0.0.2.tar.gz` & `tmp/django-pgviews-schema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-pgviews-schema-0.0.2.tar", last modified: Mon Mar 27 16:51:00 2023, max compression
+gzip compressed data, was "django-pgviews-schema-0.0.3.tar", last modified: Mon Jun 19 14:41:03 2023, max compression
```

## Comparing `django-pgviews-schema-0.0.2.tar` & `django-pgviews-schema-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.743026 django-pgviews-schema-0.0.2/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/MANIFEST.in
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)    18102 2023-03-27 16:51:00.743026 django-pgviews-schema-0.0.2/PKG-INFO
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)    13446 2023-03-27 16:48:54.000000 django-pgviews-schema-0.0.2/README.md
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.739026 django-pgviews-schema-0.0.2/django_pgviews/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/__init__.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)     1418 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/apps.py
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.739026 django-pgviews-schema-0.0.2/django_pgviews/db/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      772 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/db/__init__.py
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.739026 django-pgviews-schema-0.0.2/django_pgviews/db/sql/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/db/sql/__init__.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      687 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/db/sql/compiler.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      720 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/db/sql/query.py
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.739026 django-pgviews-schema-0.0.2/django_pgviews/management/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/management/__init__.py
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.739026 django-pgviews-schema-0.0.2/django_pgviews/management/commands/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/management/commands/__init__.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)     1415 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/management/commands/clear_pgviews.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      828 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/management/commands/refresh_pgviews.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)     2628 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/management/commands/sync_pgviews.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)     5610 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/models.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)       88 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/signals.py
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)    17622 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/django_pgviews/view.py
-drwxrwxr-x   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        0 2023-03-27 16:51:00.743026 django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)    18102 2023-03-27 16:51:00.000000 django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/PKG-INFO
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      730 2023-03-27 16:51:00.000000 django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/SOURCES.txt
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)        1 2023-03-27 16:51:00.000000 django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/dependency_links.txt
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)       15 2023-03-27 16:51:00.000000 django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/top_level.txt
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)      333 2023-03-27 12:30:38.000000 django-pgviews-schema-0.0.2/pyproject.toml
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)       79 2023-03-27 16:51:00.743026 django-pgviews-schema-0.0.2/setup.cfg
--rw-rw-r--   0 pedrobarbosa  (1000) pedrobarbosa  (1000)     1261 2023-03-27 16:50:24.000000 django-pgviews-schema-0.0.2/setup.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.233431 django-pgviews-schema-0.0.3/
+-rw-rw-r--   0 napp      (1000) napp      (1000)        0 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/MANIFEST.in
+-rw-rw-r--   0 napp      (1000) napp      (1000)    18109 2023-06-19 14:41:03.233431 django-pgviews-schema-0.0.3/PKG-INFO
+-rw-rw-r--   0 napp      (1000) napp      (1000)    13446 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/README.md
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.229431 django-pgviews-schema-0.0.3/django_pgviews/
+-rw-rw-r--   0 napp      (1000) napp      (1000)        0 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/__init__.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)     1418 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/apps.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.229431 django-pgviews-schema-0.0.3/django_pgviews/db/
+-rw-rw-r--   0 napp      (1000) napp      (1000)      772 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/db/__init__.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.229431 django-pgviews-schema-0.0.3/django_pgviews/db/sql/
+-rw-rw-r--   0 napp      (1000) napp      (1000)        0 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/db/sql/__init__.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)      687 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/db/sql/compiler.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)      720 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/db/sql/query.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.229431 django-pgviews-schema-0.0.3/django_pgviews/management/
+-rw-rw-r--   0 napp      (1000) napp      (1000)        0 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/management/__init__.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.229431 django-pgviews-schema-0.0.3/django_pgviews/management/commands/
+-rw-rw-r--   0 napp      (1000) napp      (1000)        0 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/management/commands/__init__.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)     1415 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/management/commands/clear_pgviews.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)      828 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/management/commands/refresh_pgviews.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)     2628 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/management/commands/sync_pgviews.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)     5610 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/models.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)       88 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/signals.py
+-rw-rw-r--   0 napp      (1000) napp      (1000)    17622 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/django_pgviews/view.py
+drwxrwxr-x   0 napp      (1000) napp      (1000)        0 2023-06-19 14:41:03.233431 django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/
+-rw-rw-r--   0 napp      (1000) napp      (1000)    18109 2023-06-19 14:41:03.000000 django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/PKG-INFO
+-rw-rw-r--   0 napp      (1000) napp      (1000)      730 2023-06-19 14:41:03.000000 django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/SOURCES.txt
+-rw-rw-r--   0 napp      (1000) napp      (1000)        1 2023-06-19 14:41:03.000000 django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/dependency_links.txt
+-rw-rw-r--   0 napp      (1000) napp      (1000)       15 2023-06-19 14:41:03.000000 django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/top_level.txt
+-rw-rw-r--   0 napp      (1000) napp      (1000)      333 2023-06-19 14:36:51.000000 django-pgviews-schema-0.0.3/pyproject.toml
+-rw-rw-r--   0 napp      (1000) napp      (1000)       79 2023-06-19 14:41:03.233431 django-pgviews-schema-0.0.3/setup.cfg
+-rw-rw-r--   0 napp      (1000) napp      (1000)     1268 2023-06-19 14:38:04.000000 django-pgviews-schema-0.0.3/setup.py
```

### Comparing `django-pgviews-schema-0.0.2/PKG-INFO` & `django-pgviews-schema-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-pgviews-schema
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create and manage Postgres SQL Views in Django
 Home-page: https://github.com/pedrohsbarbosa99/django-pgviews-schema
-Author: Mikuláš Poul
-Author-email: git@mikulaspoul.cz
+Author: Pedro Barbosa
+Author-email: pedrohsbarbosa99@gmail.com
 License: Public Domain
 Description: # SQL Views for Postgres
         
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         Adds first-class support for [PostgreSQL Views][pg-views] in the Django ORM.
         Fork of the [django-pgviews-redux][django-pgviews-redux] by [mypebble][xelixdev] with support for Django 3.2+ and schema postgres.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-pgviews-schema-0.0.2/README.md` & `django-pgviews-schema-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/apps.py` & `django-pgviews-schema-0.0.3/django_pgviews/apps.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/db/__init__.py` & `django-pgviews-schema-0.0.3/django_pgviews/db/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/db/sql/compiler.py` & `django-pgviews-schema-0.0.3/django_pgviews/db/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/db/sql/query.py` & `django-pgviews-schema-0.0.3/django_pgviews/db/sql/query.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/management/commands/clear_pgviews.py` & `django-pgviews-schema-0.0.3/django_pgviews/management/commands/clear_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/management/commands/refresh_pgviews.py` & `django-pgviews-schema-0.0.3/django_pgviews/management/commands/refresh_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/management/commands/sync_pgviews.py` & `django-pgviews-schema-0.0.3/django_pgviews/management/commands/sync_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/models.py` & `django-pgviews-schema-0.0.3/django_pgviews/models.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews/view.py` & `django-pgviews-schema-0.0.3/django_pgviews/view.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/PKG-INFO` & `django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-pgviews-schema
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create and manage Postgres SQL Views in Django
 Home-page: https://github.com/pedrohsbarbosa99/django-pgviews-schema
-Author: Mikuláš Poul
-Author-email: git@mikulaspoul.cz
+Author: Pedro Barbosa
+Author-email: pedrohsbarbosa99@gmail.com
 License: Public Domain
 Description: # SQL Views for Postgres
         
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         Adds first-class support for [PostgreSQL Views][pg-views] in the Django ORM.
         Fork of the [django-pgviews-redux][django-pgviews-redux] by [mypebble][xelixdev] with support for Django 3.2+ and schema postgres.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-pgviews-schema-0.0.2/django_pgviews_schema.egg-info/SOURCES.txt` & `django-pgviews-schema-0.0.3/django_pgviews_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pgviews-schema-0.0.2/setup.py` & `django-pgviews-schema-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     LONG_DESCRIPTION = open("README.md").read()
 else:
     LONG_DESCRIPTION = ""
 
 
 setup(
     name="django-pgviews-schema",
-    version="0.0.2",
+    version="0.0.3",
     description="Create and manage Postgres SQL Views in Django",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    author="Mikuláš Poul",
-    author_email="git@mikulaspoul.cz",
+    author="Pedro Barbosa",
+    author_email="pedrohsbarbosa99@gmail.com",
     license="Public Domain",
     packages=find_packages(),
     url="https://github.com/pedrohsbarbosa99/django-pgviews-schema",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

