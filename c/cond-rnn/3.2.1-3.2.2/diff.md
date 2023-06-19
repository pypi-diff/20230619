# Comparing `tmp/cond-rnn-3.2.1.tar.gz` & `tmp/cond-rnn-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cond-rnn-3.2.1.tar", last modified: Tue Dec 20 12:16:39 2022, max compression
+gzip compressed data, was "cond-rnn-3.2.2.tar", last modified: Mon Jun 19 08:32:57 2023, max compression
```

## Comparing `cond-rnn-3.2.1.tar` & `cond-rnn-3.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 philipperemy   (501) staff       (20)        0 2022-12-20 12:16:39.196496 cond-rnn-3.2.1/
--rw-r--r--   0 philipperemy   (501) staff       (20)     1071 2022-04-15 23:43:22.000000 cond-rnn-3.2.1/LICENSE
--rw-r--r--   0 philipperemy   (501) staff       (20)     8743 2022-12-20 12:16:39.196337 cond-rnn-3.2.1/PKG-INFO
--rw-r--r--   0 philipperemy   (501) staff       (20)     8568 2022-12-19 11:46:58.000000 cond-rnn-3.2.1/README.md
-drwxr-xr-x   0 philipperemy   (501) staff       (20)        0 2022-12-20 12:16:39.195524 cond-rnn-3.2.1/cond_rnn/
--rw-r--r--   0 philipperemy   (501) staff       (20)       59 2022-04-15 23:43:22.000000 cond-rnn-3.2.1/cond_rnn/__init__.py
--rw-r--r--   0 philipperemy   (501) staff       (20)     4051 2022-12-19 12:30:44.000000 cond-rnn-3.2.1/cond_rnn/cond_rnn.py
-drwxr-xr-x   0 philipperemy   (501) staff       (20)        0 2022-12-20 12:16:39.196169 cond-rnn-3.2.1/cond_rnn.egg-info/
--rw-r--r--   0 philipperemy   (501) staff       (20)     8743 2022-12-20 12:16:39.000000 cond-rnn-3.2.1/cond_rnn.egg-info/PKG-INFO
--rw-r--r--   0 philipperemy   (501) staff       (20)      227 2022-12-20 12:16:39.000000 cond-rnn-3.2.1/cond_rnn.egg-info/SOURCES.txt
--rw-r--r--   0 philipperemy   (501) staff       (20)        1 2022-12-20 12:16:39.000000 cond-rnn-3.2.1/cond_rnn.egg-info/dependency_links.txt
--rw-r--r--   0 philipperemy   (501) staff       (20)       56 2022-12-20 12:16:39.000000 cond-rnn-3.2.1/cond_rnn.egg-info/requires.txt
--rw-r--r--   0 philipperemy   (501) staff       (20)        9 2022-12-20 12:16:39.000000 cond-rnn-3.2.1/cond_rnn.egg-info/top_level.txt
--rw-r--r--   0 philipperemy   (501) staff       (20)       38 2022-12-20 12:16:39.196536 cond-rnn-3.2.1/setup.cfg
--rw-r--r--   0 philipperemy   (501) staff       (20)      724 2022-12-20 12:16:14.000000 cond-rnn-3.2.1/setup.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-06-19 08:32:57.621756 cond-rnn-3.2.2/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     1071 2023-06-19 08:27:58.000000 cond-rnn-3.2.2/LICENSE
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     8743 2023-06-19 08:32:57.621756 cond-rnn-3.2.2/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     8568 2023-06-19 08:27:58.000000 cond-rnn-3.2.2/README.md
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-06-19 08:32:57.617756 cond-rnn-3.2.2/cond_rnn/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       59 2023-06-19 08:27:58.000000 cond-rnn-3.2.2/cond_rnn/__init__.py
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     4051 2023-06-19 08:27:58.000000 cond-rnn-3.2.2/cond_rnn/cond_rnn.py
+drwxrwxr-x   0 philippe  (1000) philippe  (1000)        0 2023-06-19 08:32:57.621756 cond-rnn-3.2.2/cond_rnn.egg-info/
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)     8743 2023-06-19 08:32:57.000000 cond-rnn-3.2.2/cond_rnn.egg-info/PKG-INFO
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      227 2023-06-19 08:32:57.000000 cond-rnn-3.2.2/cond_rnn.egg-info/SOURCES.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        1 2023-06-19 08:32:57.000000 cond-rnn-3.2.2/cond_rnn.egg-info/dependency_links.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       50 2023-06-19 08:32:57.000000 cond-rnn-3.2.2/cond_rnn.egg-info/requires.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)        9 2023-06-19 08:32:57.000000 cond-rnn-3.2.2/cond_rnn.egg-info/top_level.txt
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)       38 2023-06-19 08:32:57.621756 cond-rnn-3.2.2/setup.cfg
+-rw-rw-r--   0 philippe  (1000) philippe  (1000)      742 2023-06-19 08:32:55.000000 cond-rnn-3.2.2/setup.py
```

### Comparing `cond-rnn-3.2.1/LICENSE` & `cond-rnn-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cond-rnn-3.2.1/PKG-INFO` & `cond-rnn-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cond-rnn
-Version: 3.2.1
+Version: 3.2.2
 Summary: Conditional RNN
 Author: Philippe Remy
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Recurrent for Tensorflow/Keras
```

### Comparing `cond-rnn-3.2.1/README.md` & `cond-rnn-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cond-rnn-3.2.1/cond_rnn/cond_rnn.py` & `cond-rnn-3.2.2/cond_rnn/cond_rnn.py`

 * *Files identical despite different names*

### Comparing `cond-rnn-3.2.1/cond_rnn.egg-info/PKG-INFO` & `cond-rnn-3.2.2/cond_rnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cond-rnn
-Version: 3.2.1
+Version: 3.2.2
 Summary: Conditional RNN
 Author: Philippe Remy
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Recurrent for Tensorflow/Keras
```

### Comparing `cond-rnn-3.2.1/setup.py` & `cond-rnn-3.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     os.environ['GRPC_PYTHON_BUILD_SYSTEM_OPENSSL'] = '1'
     os.environ['GRPC_PYTHON_BUILD_SYSTEM_ZLIB'] = '1'
 
 install_requires = ['numpy', tensorflow, 'tensorflow_addons', "protobuf<=3.20"]
 
 setup(
     name='cond-rnn',
-    version='3.2.1',
+    version='3.2.2',
     description='Conditional RNN',
     author='Philippe Remy',
     license='MIT',
     long_description_content_type='text/markdown',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     packages=['cond_rnn'],
     install_requires=install_requires
 )
```

