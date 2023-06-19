# Comparing `tmp/stego_lsb-1.4.1.tar.gz` & `tmp/stego_lsb-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stego_lsb-1.4.1.tar", last modified: Wed Feb  8 01:05:12 2023, max compression
+gzip compressed data, was "stego_lsb-1.4.2.tar", last modified: Mon Jun 19 15:34:27 2023, max compression
```

## Comparing `stego_lsb-1.4.1.tar` & `stego_lsb-1.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.992680 stego_lsb-1.4.1/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.988680 stego_lsb-1.4.1/.github/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.988680 stego_lsb-1.4.1/.github/workflows/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1658 2023-02-08 00:44:22.000000 stego_lsb-1.4.1/.github/workflows/python-package.yml
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1344 2023-02-07 01:19:19.000000 stego_lsb-1.4.1/.gitignore
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-05-30 14:29:08.000000 stego_lsb-1.4.1/AUTHORS.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1077 2022-05-25 14:17:00.000000 stego_lsb-1.4.1/LICENSE.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-02-08 01:05:12.992680 stego_lsb-1.4.1/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7968 2022-10-28 01:45:20.000000 stego_lsb-1.4.1/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       41 2023-02-08 00:34:28.000000 stego_lsb-1.4.1/mypy.ini
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:02:06.000000 stego_lsb-1.4.1/py.typed
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    44143 2022-10-28 01:45:20.000000 stego_lsb-1.4.1/readme_illustration.png
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       67 2023-02-08 01:05:12.992680 stego_lsb-1.4.1/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1504 2023-02-08 01:03:16.000000 stego_lsb-1.4.1/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.988680 stego_lsb-1.4.1/stego_lsb/
--rwxrwxr-x   0 ryan      (1000) ryan      (1000)     7671 2023-02-08 00:34:28.000000 stego_lsb-1.4.1/stego_lsb/LSBSteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1504 2023-02-07 01:19:19.000000 stego_lsb-1.4.1/stego_lsb/StegDetect.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3951 2023-02-07 01:19:19.000000 stego_lsb-1.4.1/stego_lsb/WavSteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-05-25 14:17:00.000000 stego_lsb-1.4.1/stego_lsb/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6927 2023-02-07 01:19:19.000000 stego_lsb-1.4.1/stego_lsb/bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4483 2023-02-07 01:19:19.000000 stego_lsb-1.4.1/stego_lsb/cli.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.992680 stego_lsb-1.4.1/stego_lsb.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      600 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/entry_points.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-02-08 00:40:02.000000 stego_lsb-1.4.1/stego_lsb.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      116 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2023-02-08 01:05:12.000000 stego_lsb-1.4.1/stego_lsb.egg-info/top_level.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:12.992680 stego_lsb-1.4.1/tests/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-05-25 14:17:00.000000 stego_lsb-1.4.1/tests/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2215 2023-02-08 00:34:28.000000 stego_lsb-1.4.1/tests/test_bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2890 2023-02-08 00:34:28.000000 stego_lsb-1.4.1/tests/test_lsbsteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3786 2023-02-08 00:34:28.000000 stego_lsb-1.4.1/tests/test_wavsteg.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.162143 stego_lsb-1.4.2/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.158143 stego_lsb-1.4.2/.github/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.158143 stego_lsb-1.4.2/.github/workflows/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1658 2023-02-08 00:44:22.000000 stego_lsb-1.4.2/.github/workflows/python-package.yml
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1344 2023-02-07 01:19:19.000000 stego_lsb-1.4.2/.gitignore
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-05-30 14:29:08.000000 stego_lsb-1.4.2/AUTHORS.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1077 2022-05-25 14:17:00.000000 stego_lsb-1.4.2/LICENSE.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-06-19 15:34:27.162143 stego_lsb-1.4.2/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7968 2022-10-28 01:45:20.000000 stego_lsb-1.4.2/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       41 2023-02-08 00:34:28.000000 stego_lsb-1.4.2/mypy.ini
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-02-08 01:05:40.000000 stego_lsb-1.4.2/py.typed
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    44143 2022-10-28 01:45:20.000000 stego_lsb-1.4.2/readme_illustration.png
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       67 2023-06-19 15:34:27.162143 stego_lsb-1.4.2/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1581 2023-06-19 15:32:11.000000 stego_lsb-1.4.2/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.158143 stego_lsb-1.4.2/stego_lsb/
+-rwxrwxr-x   0 ryan      (1000) ryan      (1000)     7671 2023-02-08 00:34:28.000000 stego_lsb-1.4.2/stego_lsb/LSBSteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1504 2023-02-07 01:19:19.000000 stego_lsb-1.4.2/stego_lsb/StegDetect.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3951 2023-02-07 01:19:19.000000 stego_lsb-1.4.2/stego_lsb/WavSteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-05-25 14:17:00.000000 stego_lsb-1.4.2/stego_lsb/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6927 2023-02-07 01:19:19.000000 stego_lsb-1.4.2/stego_lsb/bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4483 2023-02-07 01:19:19.000000 stego_lsb-1.4.2/stego_lsb/cli.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.162143 stego_lsb-1.4.2/stego_lsb.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      600 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/entry_points.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-02-08 00:40:02.000000 stego_lsb-1.4.2/stego_lsb.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      193 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2023-06-19 15:34:27.000000 stego_lsb-1.4.2/stego_lsb.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-19 15:34:27.162143 stego_lsb-1.4.2/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-05-25 14:17:00.000000 stego_lsb-1.4.2/tests/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2215 2023-02-08 00:34:28.000000 stego_lsb-1.4.2/tests/test_bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2890 2023-02-08 00:34:28.000000 stego_lsb-1.4.2/tests/test_lsbsteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3786 2023-02-08 00:34:28.000000 stego_lsb-1.4.2/tests/test_wavsteg.py
```

### Comparing `stego_lsb-1.4.1/.github/workflows/python-package.yml` & `stego_lsb-1.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/.gitignore` & `stego_lsb-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/LICENSE.md` & `stego_lsb-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/PKG-INFO` & `stego_lsb-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stego_lsb
-Version: 1.4.1
+Version: 1.4.2
 Summary: stego lsb
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryanalexandergibson@gmail.com
 License: MIT
 Keywords: stego lsb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stego_lsb-1.4.1/README.md` & `stego_lsb-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/readme_illustration.png` & `stego_lsb-1.4.2/readme_illustration.png`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/setup.py` & `stego_lsb-1.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 requirements = [
     "Pillow>=5.3.0",
     "numpy>=1.15.4,<1.22.0; python_version<'3.8'",
-    "numpy>=1.15.4; python_version>='3.8'",
+    "numpy>=1.15.4,<1.25.0; python_version>='3.8' and python_version<'3.9'",
+    "numpy>=1.15.4; python_version>='3.9'",
     "Click>=7.0",
 ]
 
 setup(
     author="Ryan Gibson",
     author_email="ryanalexandergibson@gmail.com",
     name="stego_lsb",
-    version="1.4.1",
+    version="1.4.2",
     description="stego lsb",
     keywords="stego lsb",
     license="MIT",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/ragibson/Steganography",
     install_requires=requirements,
```

### Comparing `stego_lsb-1.4.1/stego_lsb/LSBSteg.py` & `stego_lsb-1.4.2/stego_lsb/LSBSteg.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/stego_lsb/StegDetect.py` & `stego_lsb-1.4.2/stego_lsb/StegDetect.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/stego_lsb/WavSteg.py` & `stego_lsb-1.4.2/stego_lsb/WavSteg.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/stego_lsb/bit_manipulation.py` & `stego_lsb-1.4.2/stego_lsb/bit_manipulation.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/stego_lsb/cli.py` & `stego_lsb-1.4.2/stego_lsb/cli.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/stego_lsb.egg-info/PKG-INFO` & `stego_lsb-1.4.2/stego_lsb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stego-lsb
-Version: 1.4.1
+Version: 1.4.2
 Summary: stego lsb
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryanalexandergibson@gmail.com
 License: MIT
 Keywords: stego lsb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stego_lsb-1.4.1/stego_lsb.egg-info/SOURCES.txt` & `stego_lsb-1.4.2/stego_lsb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/tests/test_bit_manipulation.py` & `stego_lsb-1.4.2/tests/test_bit_manipulation.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/tests/test_lsbsteg.py` & `stego_lsb-1.4.2/tests/test_lsbsteg.py`

 * *Files identical despite different names*

### Comparing `stego_lsb-1.4.1/tests/test_wavsteg.py` & `stego_lsb-1.4.2/tests/test_wavsteg.py`

 * *Files identical despite different names*

