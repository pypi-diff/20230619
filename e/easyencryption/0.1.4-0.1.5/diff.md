# Comparing `tmp/easyencryption-0.1.4.tar.gz` & `tmp/easyencryption-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.4.tar", last modified: Sat Aug 27 21:32:50 2022, max compression
+gzip compressed data, was "easyencryption-0.1.5.tar", last modified: Mon Jun 19 16:41:42 2023, max compression
```

## Comparing `easyencryption-0.1.4.tar` & `easyencryption-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-27 21:32:50.595407 easyencryption-0.1.4/
--rw-rw-rw-   0        0        0     2516 2022-08-27 21:32:50.604415 easyencryption-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1416 2022-07-18 02:45:19.000000 easyencryption-0.1.4/README.md
--rw-rw-rw-   0        0        0      723 2022-08-27 21:32:50.605415 easyencryption-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1839 2022-08-27 21:32:33.000000 easyencryption-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-27 21:32:50.545361 easyencryption-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2022-08-27 21:32:50.581393 easyencryption-0.1.4/src/easyencryption/
--rw-rw-rw-   0        0        0      233 2022-07-17 03:06:12.000000 easyencryption-0.1.4/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1396 2022-07-17 03:00:38.000000 easyencryption-0.1.4/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1087 2022-07-17 03:05:15.000000 easyencryption-0.1.4/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     2034 2022-07-17 03:16:59.000000 easyencryption-0.1.4/src/easyencryption/pubprivate.py
-drwxrwxrwx   0        0        0        0 2022-08-27 21:32:50.594406 easyencryption-0.1.4/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     2516 2022-08-27 21:32:50.000000 easyencryption-0.1.4/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2022-08-27 21:32:50.000000 easyencryption-0.1.4/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-27 21:32:50.000000 easyencryption-0.1.4/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-08-27 21:32:50.000000 easyencryption-0.1.4/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-08-27 21:32:50.000000 easyencryption-0.1.4/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.670299 easyencryption-0.1.5/
+-rw-rw-rw-   0        0        0     2516 2023-06-19 16:41:42.671287 easyencryption-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1416 2023-06-17 21:41:18.000000 easyencryption-0.1.5/README.md
+-rw-rw-rw-   0        0        0      723 2023-06-19 16:41:42.675291 easyencryption-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-06-17 21:41:08.000000 easyencryption-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.579882 easyencryption-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.615286 easyencryption-0.1.5/src/easyencryption/
+-rw-rw-rw-   0        0        0      456 2023-06-19 16:39:25.000000 easyencryption-0.1.5/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-06-17 21:41:40.000000 easyencryption-0.1.5/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1087 2023-06-17 21:41:44.000000 easyencryption-0.1.5/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     2034 2023-06-17 21:41:48.000000 easyencryption-0.1.5/src/easyencryption/pubprivate.py
+-rw-rw-rw-   0        0        0     2057 2023-06-19 16:36:12.000000 easyencryption-0.1.5/src/easyencryption/sha.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:41:42.668280 easyencryption-0.1.5/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     2516 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 16:41:42.000000 easyencryption-0.1.5/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.4/PKG-INFO` & `easyencryption-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.4
+Version: 0.1.5
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

### Comparing `easyencryption-0.1.4/README.md` & `easyencryption-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.4/setup.cfg` & `easyencryption-0.1.5/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6173 7965 6e63 7279 7074 696f   = easyencryptio
-00000020: 6e0d 0a76 6572 7369 6f6e 203d 2030 2e30  n..version = 0.0
-00000030: 2e36 0d0a 6175 7468 6f72 203d 2062 6c61  .6..author = bla
+00000020: 6e0d 0a76 6572 7369 6f6e 203d 2030 2e31  n..version = 0.1
+00000030: 2e35 0d0a 6175 7468 6f72 203d 2062 6c61  .5..author = bla
 00000040: 7a65 6e0d 0a61 7574 686f 725f 656d 6169  zen..author_emai
 00000050: 6c20 3d20 636f 6e74 6163 7440 6669 7265  l = contact@fire
 00000060: 6261 6c6c 626f 742e 636f 6d0d 0a64 6573  ballbot.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 2076 6572  cription = A ver
 00000080: 7920 6561 7379 2077 6179 2074 6f20 656e  y easy way to en
 00000090: 6372 7970 7420 6461 7461 0d0a 6c6f 6e67  crypt data..long
 000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `easyencryption-0.1.4/setup.py` & `easyencryption-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.4"
+version = "0.1.5"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.4/src/easyencryption/aes.py` & `easyencryption-0.1.5/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.4/src/easyencryption/fernet.py` & `easyencryption-0.1.5/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.4/src/easyencryption/pubprivate.py` & `easyencryption-0.1.5/src/easyencryption/pubprivate.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.4/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.5/src/easyencryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.4
+Version: 0.1.5
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
```

