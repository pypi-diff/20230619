# Comparing `tmp/invoicing-zaidikram-1.0.0.tar.gz` & `tmp/invoicing-zaidikram-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoicing-zaidikram-1.0.0.tar", last modified: Mon Jun 19 19:50:30 2023, max compression
+gzip compressed data, was "invoicing-zaidikram-2.0.0.tar", last modified: Mon Jun 19 20:00:21 2023, max compression
```

## Comparing `invoicing-zaidikram-1.0.0.tar` & `invoicing-zaidikram-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:50:30.769166 invoicing-zaidikram-1.0.0/
--rw-rw-rw-   0        0        0      692 2023-06-19 19:50:30.769166 invoicing-zaidikram-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 19:50:30.721422 invoicing-zaidikram-1.0.0/invoicing-zaidikram/
--rw-rw-rw-   0        0        0        0 2023-06-19 15:48:33.000000 invoicing-zaidikram-1.0.0/invoicing-zaidikram/__init__.py
--rw-rw-rw-   0        0        0     2648 2023-06-19 15:40:55.000000 invoicing-zaidikram-1.0.0/invoicing-zaidikram/invoice.py
-drwxrwxrwx   0        0        0        0 2023-06-19 19:50:30.769166 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/
--rw-rw-rw-   0        0        0      692 2023-06-19 19:50:30.000000 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-19 19:50:30.000000 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:50:30.000000 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-19 19:50:30.000000 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-19 19:50:30.000000 invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 19:50:30.769166 invoicing-zaidikram-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1528 2023-06-19 19:50:18.000000 invoicing-zaidikram-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:00:21.941301 invoicing-zaidikram-2.0.0/
+-rw-rw-rw-   0        0        0      692 2023-06-19 20:00:21.908840 invoicing-zaidikram-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 20:00:21.902859 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/
+-rw-rw-rw-   0        0        0      692 2023-06-19 20:00:21.000000 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-19 20:00:21.000000 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:00:21.000000 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-19 20:00:21.000000 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-19 20:00:21.000000 invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 20:00:21.906884 invoicing-zaidikram-2.0.0/invzaidikram/
+-rw-rw-rw-   0        0        0        0 2023-06-19 15:48:33.000000 invoicing-zaidikram-2.0.0/invzaidikram/__init__.py
+-rw-rw-rw-   0        0        0     2648 2023-06-19 15:40:55.000000 invoicing-zaidikram-2.0.0/invzaidikram/invoice.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:00:21.941301 invoicing-zaidikram-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1521 2023-06-19 20:00:16.000000 invoicing-zaidikram-2.0.0/setup.py
```

### Comparing `invoicing-zaidikram-1.0.0/PKG-INFO` & `invoicing-zaidikram-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoicing-zaidikram
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

### Comparing `invoicing-zaidikram-1.0.0/invoicing-zaidikram/invoice.py` & `invoicing-zaidikram-2.0.0/invzaidikram/invoice.py`

 * *Files identical despite different names*

### Comparing `invoicing-zaidikram-1.0.0/invoicing_zaidikram.egg-info/PKG-INFO` & `invoicing-zaidikram-2.0.0/invoicing_zaidikram.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoicing-zaidikram
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

### Comparing `invoicing-zaidikram-1.0.0/setup.py` & `invoicing-zaidikram-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='invoicing-zaidikram',  # * Your package will have this name
-    packages=['invoicing-zaidikram'],  # * Name the package again
-    version='1.0.0',  # * To be increased every time your change your library
+    packages=['invzaidikram'],  # * Name the package again
+    version='2.0.0',  # * To be increased every time your change your library
     license='MIT',  # Type of license. More here: https://help.github.com/articles/licensing-a-repository
     description='This package can be used to convert Excel invoices to PDF invoices.',
     # Short description of your library
     author='Zaid Ikram Mohammed',  # Your name
     author_email='zaidikram422@gmail.com',  # Your email
     url='https://example.com',  # Homepage of your library (e.g. github or your website)
     keywords=['invoice', 'excel', 'pdf'],  # Keywords users can search on pypi.org
```

