# Comparing `tmp/bitcoin_p2p-0.3.1.tar.gz` & `tmp/bitcoin_p2p-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_p2p-0.3.1.tar", last modified: Sun Jun 11 09:03:19 2023, max compression
+gzip compressed data, was "bitcoin_p2p-0.3.2.tar", last modified: Mon Jun 19 16:29:10 2023, max compression
```

## Comparing `bitcoin_p2p-0.3.1.tar` & `bitcoin_p2p-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 09:03:19.651137 bitcoin_p2p-0.3.1/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.3.1/LICENSE
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4627 2023-06-11 09:03:19.651137 bitcoin_p2p-0.3.1/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4131 2023-06-11 06:30:57.000000 bitcoin_p2p-0.3.1/README.md
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 09:03:19.651137 bitcoin_p2p-0.3.1/bitcoin_p2p/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-11 09:03:19.651137 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     4627 2023-06-11 09:03:19.000000 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      260 2023-06-11 09:03:19.000000 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 09:03:19.000000 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-06-11 09:03:19.000000 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-11 09:03:19.000000 bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/top_level.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-11 09:03:19.651137 bitcoin_p2p-0.3.1/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1177 2023-06-11 09:02:39.000000 bitcoin_p2p-0.3.1/setup.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:29:10.765804 bitcoin_p2p-0.3.2/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2023-06-09 17:54:40.000000 bitcoin_p2p-0.3.2/LICENSE
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4627 2023-06-19 16:29:10.761804 bitcoin_p2p-0.3.2/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4131 2023-06-11 06:30:57.000000 bitcoin_p2p-0.3.2/README.md
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:29:10.761804 bitcoin_p2p-0.3.2/bitcoin_p2p/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2023-06-19 16:29:10.761804 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     4627 2023-06-19 16:29:10.000000 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      260 2023-06-19 16:29:10.000000 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-19 16:29:10.000000 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2023-06-19 16:29:10.000000 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2023-06-19 16:29:10.000000 bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/top_level.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2023-06-19 16:29:10.765804 bitcoin_p2p-0.3.2/setup.cfg
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     1177 2023-06-19 16:28:23.000000 bitcoin_p2p-0.3.2/setup.py
```

### Comparing `bitcoin_p2p-0.3.1/LICENSE` & `bitcoin_p2p-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_p2p-0.3.1/PKG-INFO` & `bitcoin_p2p-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin_p2p
-Version: 0.3.1
+Version: 0.3.2
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bitcoin_p2p-0.3.1/README.md` & `bitcoin_p2p-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_p2p-0.3.1/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO` & `bitcoin_p2p-0.3.2/bitcoin_p2p/bitcoin_p2p.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-p2p
-Version: 0.3.1
+Version: 0.3.2
 Summary: Bitcoin p2p communication tools in python
 Home-page: https://github.com/andreasgriffin/bitcoin-p2p
 Author: Andreas Griffin
 Author-email: andreasgriffin@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `bitcoin_p2p-0.3.1/setup.py` & `bitcoin_p2p-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="bitcoin_p2p",
-    version="0.3.1",
+    version="0.3.2",
     author="Andreas Griffin",
     author_email="andreasgriffin@proton.me",
     description="Bitcoin p2p communication tools in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreasgriffin/bitcoin-p2p",
     packages=find_namespace_packages("bitcoin_p2p", include=["bitcoin_p2p.*"]),
```

