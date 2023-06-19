# Comparing `tmp/chinese_pdf_divider-1.0.0.tar.gz` & `tmp/chinese_pdf_divider-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinese_pdf_divider-1.0.0.tar", last modified: Mon Jun 19 03:25:16 2023, max compression
+gzip compressed data, was "chinese_pdf_divider-1.1.0.tar", last modified: Mon Jun 19 03:39:20 2023, max compression
```

## Comparing `chinese_pdf_divider-1.0.0.tar` & `chinese_pdf_divider-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:15.995900 chinese_pdf_divider-1.0.0/
--rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 chinese_pdf_divider-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-06-19 03:25:15.994607 chinese_pdf_divider-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-06-18 11:14:18.000000 chinese_pdf_divider-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:15.982496 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/
--rw-rw-rw-   0        0        0      427 2023-06-19 03:25:15.000000 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-19 03:25:15.000000 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:25:15.000000 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-19 03:25:15.000000 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 03:25:15.000000 chinese_pdf_divider-1.0.0/chinese_pdf_divider.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 03:25:15.990511 chinese_pdf_divider-1.0.0/pdf_divider/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 chinese_pdf_divider-1.0.0/pdf_divider/__init__.py
--rw-rw-rw-   0        0        0     8954 2023-06-18 11:19:44.000000 chinese_pdf_divider-1.0.0/pdf_divider/pdf_divider.py
--rw-rw-rw-   0        0        0       42 2023-06-19 03:25:15.995900 chinese_pdf_divider-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-06-19 03:25:09.000000 chinese_pdf_divider-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:39:20.801649 chinese_pdf_divider-1.1.0/
+-rw-rw-rw-   0        0        0     1834 2023-06-18 09:32:09.000000 chinese_pdf_divider-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-06-19 03:39:20.800644 chinese_pdf_divider-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-18 11:14:18.000000 chinese_pdf_divider-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:39:20.782507 chinese_pdf_divider-1.1.0/chinese_pdf_divider/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:37:36.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider/__init__.py
+-rw-rw-rw-   0        0        0     8954 2023-06-18 11:19:44.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider/pdf_divider.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:39:20.797597 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-06-19 03:39:20.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-06-19 03:39:20.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:39:20.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-19 03:39:20.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-19 03:39:20.000000 chinese_pdf_divider-1.1.0/chinese_pdf_divider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:39:20.801649 chinese_pdf_divider-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-06-19 03:37:55.000000 chinese_pdf_divider-1.1.0/setup.py
```

### Comparing `chinese_pdf_divider-1.0.0/LICENSE.txt` & `chinese_pdf_divider-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chinese_pdf_divider-1.0.0/pdf_divider/pdf_divider.py` & `chinese_pdf_divider-1.1.0/chinese_pdf_divider/pdf_divider.py`

 * *Files identical despite different names*

### Comparing `chinese_pdf_divider-1.0.0/setup.py` & `chinese_pdf_divider-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chinese_pdf_divider',
-    version='1.0.0',
+    version='1.1.0',
     author='yunsi lin',
     author_email='yunsi0115@gmail.com',
     description='divide chinese pdf file into blocks within 512',
     packages=find_packages(),
     install_requires=[
         'pymupdf',
         'fitz',
```

