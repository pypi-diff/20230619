# Comparing `tmp/invoicing-zaid-1.0.0.tar.gz` & `tmp/invoicing-zaid-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoicing-zaid-1.0.0.tar", last modified: Mon Jun 19 16:02:17 2023, max compression
+gzip compressed data, was "invoicing-zaid-2.0.0.tar", last modified: Mon Jun 19 19:27:12 2023, max compression
```

## Comparing `invoicing-zaid-1.0.0.tar` & `invoicing-zaid-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:02:17.237956 invoicing-zaid-1.0.0/
--rw-rw-rw-   0        0        0      687 2023-06-19 16:02:17.234964 invoicing-zaid-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 16:02:17.100520 invoicing-zaid-1.0.0/invoicing/
--rw-rw-rw-   0        0        0        0 2023-06-19 15:48:33.000000 invoicing-zaid-1.0.0/invoicing/__init__.py
--rw-rw-rw-   0        0        0     2648 2023-06-19 15:40:55.000000 invoicing-zaid-1.0.0/invoicing/invoice.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:02:17.228984 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/
--rw-rw-rw-   0        0        0      687 2023-06-19 16:02:16.000000 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-06-19 16:02:16.000000 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:02:16.000000 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-19 16:02:16.000000 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 16:02:16.000000 invoicing-zaid-1.0.0/invoicing_zaid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 16:02:17.238957 invoicing-zaid-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1513 2023-06-19 16:00:50.000000 invoicing-zaid-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:27:11.988323 invoicing-zaid-2.0.0/
+-rw-rw-rw-   0        0        0      687 2023-06-19 19:27:11.987329 invoicing-zaid-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 19:27:11.845294 invoicing-zaid-2.0.0/invoicing-zaid/
+-rw-rw-rw-   0        0        0        0 2023-06-19 15:48:33.000000 invoicing-zaid-2.0.0/invoicing-zaid/__init__.py
+-rw-rw-rw-   0        0        0     2648 2023-06-19 15:40:55.000000 invoicing-zaid-2.0.0/invoicing-zaid/invoice.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:27:11.984332 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/
+-rw-rw-rw-   0        0        0      687 2023-06-19 19:27:10.000000 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-06-19 19:27:10.000000 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:27:10.000000 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-19 19:27:10.000000 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 19:27:10.000000 invoicing-zaid-2.0.0/invoicing_zaid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 19:27:11.989361 invoicing-zaid-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2023-06-19 19:26:32.000000 invoicing-zaid-2.0.0/setup.py
```

### Comparing `invoicing-zaid-1.0.0/PKG-INFO` & `invoicing-zaid-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoicing-zaid
-Version: 1.0.0
+Version: 2.0.0
 Summary: This package can be used to convert Excel invoices to PDF invoices.
 Home-page: https://example.com
 Author: Zaid Ikram Mohammed
 Author-email: zaidikram422@gmail.com
 License: MIT
 Keywords: invoice,excel,pdf
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `invoicing-zaid-1.0.0/invoicing/invoice.py` & `invoicing-zaid-2.0.0/invoicing-zaid/invoice.py`

 * *Files identical despite different names*

### Comparing `invoicing-zaid-1.0.0/invoicing_zaid.egg-info/PKG-INFO` & `invoicing-zaid-2.0.0/invoicing_zaid.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoicing-zaid
-Version: 1.0.0
+Version: 2.0.0
 Summary: This package can be used to convert Excel invoices to PDF invoices.
 Home-page: https://example.com
 Author: Zaid Ikram Mohammed
 Author-email: zaidikram422@gmail.com
 License: MIT
 Keywords: invoice,excel,pdf
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `invoicing-zaid-1.0.0/setup.py` & `invoicing-zaid-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='invoicing-zaid',  # * Your package will have this name
-    packages=['invoicing'],  # * Name the package again
-    version='1.0.0',  # * To be increased every time your change your library
+    packages=['invoicing-zaid'],  # * Name the package again
+    version='2.0.0',  # * To be increased every time your change your library
     license='MIT',  # Type of license. More here: https://help.github.com/articles/licensing-a-repository
     description='This package can be used to convert Excel invoices to PDF invoices.',
     # Short description of your library
     author='Zaid Ikram Mohammed',  # Your name
     author_email='zaidikram422@gmail.com',  # Your email
     url='https://example.com',  # Homepage of your library (e.g. github or your website)
     keywords=['invoice', 'excel', 'pdf'],  # Keywords users can search on pypi.org
```

