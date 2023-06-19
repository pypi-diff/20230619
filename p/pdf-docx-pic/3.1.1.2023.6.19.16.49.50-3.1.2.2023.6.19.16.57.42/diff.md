# Comparing `tmp/pdf-docx-pic-3.1.1.2023.6.19.16.49.50.tar.gz` & `tmp/pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.19.16.49.50.tar", last modified: Mon Jun 19 08:54:21 2023, max compression
+gzip compressed data, was "pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar", last modified: Mon Jun 19 09:02:27 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.1.2023.6.19.16.49.50.tar` & `pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:54:21.361901 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/
--rw-rw-rw-   0        0        0     2099 2023-06-19 08:54:21.361901 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-06-19 08:53:27.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/README.rst
--rw-rw-rw-   0        0        0     1543 2023-06-19 08:54:05.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 08:54:21.361901 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 08:54:21.337880 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 08:54:21.345903 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:54:21.361901 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-06-19 08:54:21.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-19 08:54:21.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:54:21.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-19 08:54:21.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 08:54:21.000000 pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf_docx_pic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/
+-rw-rw-rw-   0        0        0     1817 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/README.rst
+-rw-rw-rw-   0        0        0     1543 2023-06-19 08:58:12.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.528517 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.536516 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1817 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/top_level.txt
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.19.16.49.50/pyproject.toml` & `pdf-docx-pic-3.1.2.2023.6.19.16.57.42/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "pdf-docx-pic"
-version = "3.1.1.2023.6.19.16.49.50"
+version = "3.1.2.2023.6.19.16.57.42"
 requires-python = ">=2.6, <=3.12"
 readme = "README.rst"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: GPU",
     "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Django :: 4.2",
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.19.16.49.50/src/pdf-docx-pic/main.py` & `pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/main.py`

 * *Files identical despite different names*

