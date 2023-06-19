# Comparing `tmp/shapes_recognition-2.1.9.tar.gz` & `tmp/shapes_recognition-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.1.9.tar", last modified: Mon Jun 19 07:09:57 2023, max compression
+gzip compressed data, was "shapes_recognition-2.2.0.tar", last modified: Mon Jun 19 10:52:02 2023, max compression
```

## Comparing `shapes_recognition-2.1.9.tar` & `shapes_recognition-2.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 07:09:57.144300 shapes_recognition-2.1.9/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 07:09:57.143983 shapes_recognition-2.1.9/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.1.9/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-19 07:09:57.144379 shapes_recognition-2.1.9/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-19 07:07:07.000000 shapes_recognition-2.1.9/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 07:09:57.143580 shapes_recognition-2.1.9/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 07:09:57.000000 shapes_recognition-2.1.9/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-19 07:09:57.000000 shapes_recognition-2.1.9/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-19 07:09:57.000000 shapes_recognition-2.1.9/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-19 07:09:57.000000 shapes_recognition-2.1.9/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 10:52:02.218458 shapes_recognition-2.2.0/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 10:52:02.218183 shapes_recognition-2.2.0/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.0/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-19 10:52:02.218534 shapes_recognition-2.2.0/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-19 10:45:01.000000 shapes_recognition-2.2.0/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 10:52:02.217831 shapes_recognition-2.2.0/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 10:52:02.000000 shapes_recognition-2.2.0/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-19 10:52:02.000000 shapes_recognition-2.2.0/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-19 10:52:02.000000 shapes_recognition-2.2.0/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-19 10:52:02.000000 shapes_recognition-2.2.0/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.1.9/PKG-INFO` & `shapes_recognition-2.2.0/shapes_recognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes_recognition
-Version: 2.1.9
+Name: shapes-recognition
+Version: 2.2.0
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shapes_recognition-2.1.9/README.md` & `shapes_recognition-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.1.9/setup.py` & `shapes_recognition-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.1.9",
+    version="2.2.0",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.1.9/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes-recognition
-Version: 2.1.9
+Name: shapes_recognition
+Version: 2.2.0
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

