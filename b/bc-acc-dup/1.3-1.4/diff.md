# Comparing `tmp/bc-acc-dup-1.3.tar.gz` & `tmp/bc-acc-dup-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc-acc-dup-1.3.tar", last modified: Mon Jun 19 02:55:03 2023, max compression
+gzip compressed data, was "bc-acc-dup-1.4.tar", last modified: Mon Jun 19 02:57:31 2023, max compression
```

## Comparing `bc-acc-dup-1.3.tar` & `bc-acc-dup-1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 02:55:04.196230 bc-acc-dup-1.3/
--rw-rw-rw-   0        0        0      189 2023-06-19 02:55:04.194488 bc-acc-dup-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 02:55:04.196599 bc-acc-dup-1.3/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-06-19 02:54:50.000000 bc-acc-dup-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 02:55:04.140668 bc-acc-dup-1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 02:55:04.184763 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/
--rw-rw-rw-   0        0        0      189 2023-06-19 02:55:03.000000 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-06-19 02:55:04.000000 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:55:03.000000 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-19 02:55:03.000000 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:55:03.000000 bc-acc-dup-1.3/src/bc_acc_dup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 02:57:32.157698 bc-acc-dup-1.4/
+-rw-rw-rw-   0        0        0      189 2023-06-19 02:57:32.155521 bc-acc-dup-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:57:32.158262 bc-acc-dup-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-19 02:57:02.000000 bc-acc-dup-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:57:32.093963 bc-acc-dup-1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 02:57:32.141761 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/
+-rw-rw-rw-   0        0        0      189 2023-06-19 02:57:31.000000 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-19 02:57:31.000000 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:57:31.000000 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-19 02:57:31.000000 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:57:31.000000 bc-acc-dup-1.4/src/bc_acc_dup.egg-info/top_level.txt
```

### Comparing `bc-acc-dup-1.3/setup.py` & `bc-acc-dup-1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name="bc-acc-dup",
-    version='1.3',
+    version='1.4',
     author="CintagramABP",
     description="battle cats account duplicator",
     long_description="battle cats account duplicator",
     url="",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
     install_requires=[
         "colored==1.4.4",
         "tk",
         "python-dateutil",
         "requests",
         "pyyaml",
-        "aiohttp"
+        "aiohttp",
+        "bcsfe-discord"
     ],
     include_package_data=True,
-    package_data={"BCSFE_Python_Discord": ["py.typed"]},
+    package_data={"bc_acc_dup": ["py.typed"]},
     flake8={"max-line-length": 160},
 )
```

