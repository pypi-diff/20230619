# Comparing `tmp/trytoncalidae_authentication_dummy-6.6.0.tar.gz` & `tmp/trytoncalidae_authentication_dummy-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytoncalidae_authentication_dummy-6.6.0.tar", last modified: Fri Nov  4 09:52:25 2022, max compression
+gzip compressed data, was "trytoncalidae_authentication_dummy-6.8.0.tar", last modified: Mon Jun 19 07:51:39 2023, max compression
```

## Comparing `trytoncalidae_authentication_dummy-6.6.0.tar` & `trytoncalidae_authentication_dummy-6.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.403685 trytoncalidae_authentication_dummy-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-04 09:52:25.403685 trytoncalidae_authentication_dummy-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.399685 trytoncalidae_authentication_dummy-6.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.399685 trytoncalidae_authentication_dummy-6.6.0/icons/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/icons/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 09:52:25.403685 trytoncalidae_authentication_dummy-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3787 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.399685 trytoncalidae_authentication_dummy-6.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.399685 trytoncalidae_authentication_dummy-6.6.0/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/tests/factories/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/tests/test_authentication_dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/tryton.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:52:25.403685 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-04 09:52:25.000000 trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-04 09:52:14.000000 trytoncalidae_authentication_dummy-6.6.0/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/icons/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/tests/factories/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/tests/test_authentication_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/tryton.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:51:39.455870 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 07:51:39.000000 trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 07:51:27.000000 trytoncalidae_authentication_dummy-6.8.0/user.py
```

### Comparing `trytoncalidae_authentication_dummy-6.6.0/COPYRIGHT` & `trytoncalidae_authentication_dummy-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytoncalidae_authentication_dummy-6.6.0/LICENSE` & `trytoncalidae_authentication_dummy-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytoncalidae_authentication_dummy-6.6.0/PKG-INFO` & `trytoncalidae_authentication_dummy-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncalidae_authentication_dummy
-Version: 6.6.0
+Version: 6.8.0
 Summary: Authenticate without password
 Home-page: https://github.com/calidae/
 Download-URL: https://github.com/calidae/authentication_dummy
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPL-3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trytoncalidae_authentication_dummy-6.6.0/README.md` & `trytoncalidae_authentication_dummy-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `trytoncalidae_authentication_dummy-6.6.0/setup.py` & `trytoncalidae_authentication_dummy-6.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `trytoncalidae_authentication_dummy-6.6.0/tests/test_authentication_dummy.py` & `trytoncalidae_authentication_dummy-6.8.0/tests/test_authentication_dummy.py`

 * *Files identical despite different names*

### Comparing `trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/PKG-INFO` & `trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytoncalidae-authentication-dummy
-Version: 6.6.0
+Version: 6.8.0
 Summary: Authenticate without password
 Home-page: https://github.com/calidae/
 Download-URL: https://github.com/calidae/authentication_dummy
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPL-3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trytoncalidae_authentication_dummy-6.6.0/trytoncalidae_authentication_dummy.egg-info/SOURCES.txt` & `trytoncalidae_authentication_dummy-6.8.0/trytoncalidae_authentication_dummy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ./user.py
 ./tests/__init__.py
 ./tests/test_authentication_dummy.py
 ./tests/factories/__init__.py
 ./tests/factories/user.py
 doc/index.rst
 icons/.gitkeep
+tests/test_authentication_dummy.py
 trytoncalidae_authentication_dummy.egg-info/PKG-INFO
 trytoncalidae_authentication_dummy.egg-info/SOURCES.txt
 trytoncalidae_authentication_dummy.egg-info/dependency_links.txt
 trytoncalidae_authentication_dummy.egg-info/entry_points.txt
 trytoncalidae_authentication_dummy.egg-info/not-zip-safe
 trytoncalidae_authentication_dummy.egg-info/requires.txt
 trytoncalidae_authentication_dummy.egg-info/top_level.txt
```

