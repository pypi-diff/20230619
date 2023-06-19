# Comparing `tmp/easyencryption-0.1.5.tar.gz` & `tmp/easyencryption-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.5.tar", last modified: Mon Jun 19 16:41:42 2023, max compression
+gzip compressed data, was "easyencryption-0.1.5.1.tar", last modified: Mon Jun 19 16:46:48 2023, max compression
```

## Comparing `easyencryption-0.1.5.tar` & `easyencryption-0.1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.670299 easyencryption-0.1.5/
--rw-rw-rw-   0        0        0     2516 2023-06-19 16:41:42.671287 easyencryption-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1416 2023-06-17 21:41:18.000000 easyencryption-0.1.5/README.md
--rw-rw-rw-   0        0        0      723 2023-06-19 16:41:42.675291 easyencryption-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1839 2023-06-17 21:41:08.000000 easyencryption-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.579882 easyencryption-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.615286 easyencryption-0.1.5/src/easyencryption/
--rw-rw-rw-   0        0        0      456 2023-06-19 16:39:25.000000 easyencryption-0.1.5/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-06-17 21:41:40.000000 easyencryption-0.1.5/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1087 2023-06-17 21:41:44.000000 easyencryption-0.1.5/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2034 2023-06-17 21:41:48.000000 easyencryption-0.1.5/src/easyencryption/pubprivate.py
--rw-rw-rw-   0        0        0     2057 2023-06-19 16:36:12.000000 easyencryption-0.1.5/src/easyencryption/sha.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.668280 easyencryption-0.1.5/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     2516 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.870244 easyencryption-0.1.5.1/
+-rw-rw-rw-   0        0        0     2810 2023-06-19 16:46:48.871286 easyencryption-0.1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1708 2023-06-19 16:45:47.000000 easyencryption-0.1.5.1/README.md
+-rw-rw-rw-   0        0        0      723 2023-06-19 16:46:48.876241 easyencryption-0.1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1841 2023-06-19 16:46:10.000000 easyencryption-0.1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.787706 easyencryption-0.1.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.819240 easyencryption-0.1.5.1/src/easyencryption/
+-rw-rw-rw-   0        0        0      456 2023-06-19 16:39:25.000000 easyencryption-0.1.5.1/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-06-17 21:41:40.000000 easyencryption-0.1.5.1/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1087 2023-06-17 21:41:44.000000 easyencryption-0.1.5.1/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2034 2023-06-17 21:41:48.000000 easyencryption-0.1.5.1/src/easyencryption/pubprivate.py
+-rw-rw-rw-   0        0        0     2057 2023-06-19 16:36:12.000000 easyencryption-0.1.5.1/src/easyencryption/sha.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:46:48.867241 easyencryption-0.1.5.1/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     2810 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 16:46:48.000000 easyencryption-0.1.5.1/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.5/PKG-INFO` & `easyencryption-0.1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,22 +28,23 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
-[![Python](https://img.shields.io/pypi/pyversions/dislash.py.svg)](https://pypi.python.org/pypi/easyencryption)
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
 [![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
 
 # Downloads
 
 [![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
 [![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
 ![Downloads](https://pepy.tech/badge/easyencryption/week)
```

### Comparing `easyencryption-0.1.5/README.md` & `easyencryption-0.1.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
-[![Python](https://img.shields.io/pypi/pyversions/dislash.py.svg)](https://pypi.python.org/pypi/easyencryption)
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
 [![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
 
 # Downloads
 
 [![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
 [![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
 ![Downloads](https://pepy.tech/badge/easyencryption/week)
```

### Comparing `easyencryption-0.1.5/setup.cfg` & `easyencryption-0.1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5/setup.py` & `easyencryption-0.1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.5"
+version = "0.1.5.1"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.5/src/easyencryption/aes.py` & `easyencryption-0.1.5.1/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5/src/easyencryption/fernet.py` & `easyencryption-0.1.5.1/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5/src/easyencryption/pubprivate.py` & `easyencryption-0.1.5.1/src/easyencryption/pubprivate.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5/src/easyencryption/sha.py` & `easyencryption-0.1.5.1/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.5/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.5.1/src/easyencryption.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -28,22 +28,23 @@
 
 
 We offer a simple way to encrypt data. We have 3 different ways of doing this.<br />
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 Public Key - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
+SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes
 
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
-[![Python](https://img.shields.io/pypi/pyversions/dislash.py.svg)](https://pypi.python.org/pypi/easyencryption)
+[![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
 [![PyPi](https://img.shields.io/pypi/v/easyencryption.svg)](https://pypi.org/project/easyencryption)
 
 # Downloads
 
 [![Downloads](https://pepy.tech/badge/easyencryption)](https://pepy.tech/project/easyencryption)
 [![Downloads](https://pepy.tech/badge/easyencryption/month)](https://pepy.tech/project/easyencryption)
 ![Downloads](https://pepy.tech/badge/easyencryption/week)
```

