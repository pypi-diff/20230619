# Comparing `tmp/pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar.gz` & `tmp/pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar", last modified: Mon Jun 19 09:02:27 2023, max compression
+gzip compressed data, was "pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar", last modified: Mon Jun 19 11:33:02 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.2.2023.6.19.16.57.42.tar` & `pdf-docx-pic-3.1.2.2023.6.19.19.27.30.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/
--rw-rw-rw-   0        0        0     1817 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/README.rst
--rw-rw-rw-   0        0        0     1543 2023-06-19 08:58:12.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.528517 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.536516 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:02:27.556570 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1817 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 09:02:27.000000 pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf_docx_pic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.445795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/
+-rw-rw-rw-   0        0        0     1330 2023-06-19 11:33:02.444795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-19 09:02:11.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.434592 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:33:02.442794 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1330 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-19 11:33:02.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf_docx_pic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:33:02.445795 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.cfg
+-rw-rw-rw-   0        0        0     1644 2023-06-19 11:27:48.000000 pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.py
```

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.16.57.42/pyproject.toml` & `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-[build-system]
-requires = ["setuptools"]
+from setuptools import *
 
-[project]
-name = "pdf-docx-pic"
-version = "3.1.2.2023.6.19.16.57.42"
-requires-python = ">=2.6, <=3.12"
-readme = "README.rst"
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: GPU",
-    "Framework :: Jupyter :: JupyterLab :: 4",
-    "Framework :: Django :: 4.2",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
-    "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows :: Windows 7",
-    "Operating System :: Microsoft :: Windows :: Windows 8",
-    "Operating System :: Microsoft :: Windows :: Windows 8.1",
-    "Operating System :: Microsoft :: Windows :: Windows 10",
-    "Operating System :: Microsoft :: Windows :: Windows 11",
-    "Operating System :: POSIX",
-    "Natural Language :: Chinese (Simplified)",
-    "Programming Language :: Python :: 2.6",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Typing :: Typed",
-]
-dependencies = [
-    "ttkbootstrap>=1.10, <1.11",
-    "pdf2docx!=0.5.4, >=0.5.2", 
-    "docx2pdf>=0.1.8", 
-    "PyMuPDF>=1.22.1", 
-    "Pillow>=9.3.0, <10.0", 
-    "wheel!=0.38.2, >=0.38, <0.41",
-]
+setup(
+    name = "pdf-docx-pic",
+    version = "3.1.2.2023.6.19.19.27.30",
+    packages = find_packages(),
+    classifiers = [
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: GPU",
+        "Framework :: Jupyter :: JupyterLab :: 4",
+        "Framework :: Django :: 4.2",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+        "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows :: Windows 7",
+        "Operating System :: Microsoft :: Windows :: Windows 8",
+        "Operating System :: Microsoft :: Windows :: Windows 8.1",
+        "Operating System :: Microsoft :: Windows :: Windows 10",
+        "Operating System :: Microsoft :: Windows :: Windows 11",
+        "Operating System :: POSIX",
+        "Natural Language :: Chinese (Simplified)",
+        "Programming Language :: Python :: 2.6",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Typing :: Typed",
+    ],
+    install_requires = [
+        "ttkbootstrap>=1.10, <1.11",
+        "pdf2docx!=0.5.4, >=0.5.2", 
+        "docx2pdf>=0.1.8", 
+        "PyMuPDF>=1.22.1", 
+        "Pillow>=9.3.0, <10.0", 
+        "wheel!=0.38.2, >=0.38, <0.41",
+    ]
+)
```

### Comparing `pdf-docx-pic-3.1.2.2023.6.19.16.57.42/src/pdf-docx-pic/main.py` & `pdf-docx-pic-3.1.2.2023.6.19.19.27.30/pdf-docx-pic/main.py`

 * *Files identical despite different names*

