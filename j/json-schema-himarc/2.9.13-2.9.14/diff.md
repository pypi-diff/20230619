# Comparing `tmp/json_schema_himarc-2.9.13.tar.gz` & `tmp/json_schema_himarc-2.9.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_himarc-2.9.13.tar", last modified: Tue May 23 11:44:58 2023, max compression
+gzip compressed data, was "json_schema_himarc-2.9.14.tar", last modified: Mon Jun 19 08:36:47 2023, max compression
```

## Comparing `json_schema_himarc-2.9.13.tar` & `json_schema_himarc-2.9.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/
--rw-rw-rw-   0 root         (0) root         (0)     1049 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      371 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.13/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/json_schema_himarc/
--rw-rw-rw-   0 root         (0) root         (0)      577 2022-04-25 09:21:31.000000 json_schema_himarc-2.9.13/json_schema_himarc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.13/json_schema_himarc/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-23 11:44:58.000000 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-23 11:44:58.000000 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 11:44:58.000000 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-23 11:44:58.000000 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-23 11:44:58.000000 json_schema_himarc-2.9.13/json_schema_himarc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       62 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.13/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 11:44:58.660012 json_schema_himarc-2.9.13/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.13/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.13/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.13/tests/test_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 08:36:47.233583 json_schema_himarc-2.9.14/
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-19 08:36:47.233583 json_schema_himarc-2.9.14/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      371 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.14/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 08:36:47.229583 json_schema_himarc-2.9.14/json_schema_himarc/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2022-04-25 09:21:31.000000 json_schema_himarc-2.9.14/json_schema_himarc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.14/json_schema_himarc/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 08:36:47.229583 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-19 08:36:47.000000 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-19 08:36:47.000000 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 08:36:47.000000 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-19 08:36:47.000000 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-19 08:36:47.000000 json_schema_himarc-2.9.14/json_schema_himarc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-19 08:36:47.233583 json_schema_himarc-2.9.14/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       62 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 08:36:47.229583 json_schema_himarc-2.9.14/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-23 10:38:46.000000 json_schema_himarc-2.9.14/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.14/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-01-12 13:54:15.000000 json_schema_himarc-2.9.14/tests/test_validation.py
```

### Comparing `json_schema_himarc-2.9.13/LICENSE` & `json_schema_himarc-2.9.14/LICENSE`

 * *Files identical despite different names*

### Comparing `json_schema_himarc-2.9.13/PKG-INFO` & `json_schema_himarc-2.9.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_schema_himarc
-Version: 2.9.13
+Version: 2.9.14
 Summary: "Python validator for himarc JSON Schema"
 Home-page: UNKNOWN
 Author: "TROUVERIE Joachim"
 Author-email: "jtrouverie@anybox.fr"
 License: "MIT"
 Keywords: "json-schema"
 Platform: UNKNOWN
```

### Comparing `json_schema_himarc-2.9.13/json_schema_himarc/__init__.py` & `json_schema_himarc-2.9.14/json_schema_himarc/__init__.py`

 * *Files identical despite different names*

### Comparing `json_schema_himarc-2.9.13/json_schema_himarc/validation.py` & `json_schema_himarc-2.9.14/json_schema_himarc/validation.py`

 * *Files identical despite different names*

### Comparing `json_schema_himarc-2.9.13/json_schema_himarc.egg-info/PKG-INFO` & `json_schema_himarc-2.9.14/json_schema_himarc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-himarc
-Version: 2.9.13
+Version: 2.9.14
 Summary: "Python validator for himarc JSON Schema"
 Home-page: UNKNOWN
 Author: "TROUVERIE Joachim"
 Author-email: "jtrouverie@anybox.fr"
 License: "MIT"
 Keywords: "json-schema"
 Platform: UNKNOWN
```

### Comparing `json_schema_himarc-2.9.13/setup.cfg` & `json_schema_himarc-2.9.14/setup.cfg`

 * *Files identical despite different names*

### Comparing `json_schema_himarc-2.9.13/tests/conftest.py` & `json_schema_himarc-2.9.14/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `json_schema_himarc-2.9.13/tests/test_validation.py` & `json_schema_himarc-2.9.14/tests/test_validation.py`

 * *Files identical despite different names*

