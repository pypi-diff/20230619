# Comparing `tmp/BLEST-0.0.5.tar.gz` & `tmp/BLEST-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-0.0.5.tar", last modified: Thu Jun 15 16:12:24 2023, max compression
+gzip compressed data, was "BLEST-0.0.6.tar", last modified: Sun Jun 18 23:13:54 2023, max compression
```

## Comparing `BLEST-0.0.5.tar` & `BLEST-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:12:24.430933 BLEST-0.0.5/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-15 16:12:24.430106 BLEST-0.0.5/BLEST.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     3926 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)       29 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-15 16:12:24.000000 BLEST-0.0.5/BLEST.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.5/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     3926 2023-06-15 16:12:24.430576 BLEST-0.0.5/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3333 2023-06-15 16:11:07.000000 BLEST-0.0.5/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-15 16:12:24.431021 BLEST-0.0.5/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)      941 2023-06-15 16:11:50.000000 BLEST-0.0.5/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-18 23:13:54.012050 BLEST-0.0.6/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-18 23:13:54.011259 BLEST-0.0.6/BLEST.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     4101 2023-06-18 23:13:53.000000 BLEST-0.0.6/BLEST.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-18 23:13:53.000000 BLEST-0.0.6/BLEST.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)       34 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.6/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     4101 2023-06-18 23:13:54.011694 BLEST-0.0.6/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3508 2023-06-18 23:10:16.000000 BLEST-0.0.6/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-18 23:13:54.012216 BLEST-0.0.6/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)      957 2023-06-18 23:10:57.000000 BLEST-0.0.6/setup.py
```

### Comparing `BLEST-0.0.5/LICENSE` & `BLEST-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.5/setup.py` & `BLEST-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="BLEST",
-    version="0.0.5",
+    version="0.0.6",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/jhuntdev/blest-py",
     packages=find_packages(),
@@ -19,14 +19,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "asyncio",
         "aiohttp",
+        "uuid",
         "json",
         "copy",
         "os"
     ],
     python_requires=">=3.6",
     platforms="any",
 )
```

