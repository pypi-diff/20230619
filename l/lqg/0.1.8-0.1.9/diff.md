# Comparing `tmp/lqg-0.1.8.tar.gz` & `tmp/lqg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqg-0.1.8.tar", last modified: Thu Apr 27 11:21:47 2023, max compression
+gzip compressed data, was "lqg-0.1.9.tar", last modified: Mon Jun 19 15:09:48 2023, max compression
```

## Comparing `lqg-0.1.8.tar` & `lqg-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/
--rw-r--r--   0 dominik   (1000) dominik   (1000)    34523 2023-04-05 08:53:51.000000 lqg-0.1.8/LICENSE
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-04-27 11:21:47.694705 lqg-0.1.8/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2384 2023-04-27 11:11:09.000000 lqg-0.1.8/README.md
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/
--rw-r--r--   0 dominik   (1000) dominik   (1000)       49 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2028 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/ccg.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/infer/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      121 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1758 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/map.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1557 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/mle.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3721 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/infer/models.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2158 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/infer/prior.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1542 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/infer/utils.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2968 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/io.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4456 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/kalman.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     6971 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/model.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     7607 2023-04-05 08:53:51.000000 lqg-0.1.8/lqg/optim.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1644 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/riccati.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg/tracking/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      587 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4955 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/basic.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)    11395 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/eye.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)      698 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/kf.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     5517 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/subjective.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3096 2023-04-27 11:11:09.000000 lqg-0.1.8/lqg/tracking/three_dims.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-04-27 11:21:47.694705 lqg-0.1.8/lqg.egg-info/
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)      506 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/SOURCES.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/dependency_links.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)      104 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/requires.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        4 2023-04-27 11:21:47.000000 lqg-0.1.8/lqg.egg-info/top_level.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2023-04-27 11:21:47.694705 lqg-0.1.8/setup.cfg
--rw-r--r--   0 dominik   (1000) dominik   (1000)      919 2023-04-27 11:12:46.000000 lqg-0.1.8/setup.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)    34523 2023-04-27 11:26:54.000000 lqg-0.1.9/LICENSE
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-06-19 15:09:48.101289 lqg-0.1.9/PKG-INFO
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2384 2023-06-19 15:07:19.000000 lqg-0.1.9/README.md
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.097955 lqg-0.1.9/lqg/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       49 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2028 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/ccg.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg/infer/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      121 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1758 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/map.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1557 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/mle.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3721 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/infer/models.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2158 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/infer/prior.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1542 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/utils.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2968 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/io.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     4456 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/kalman.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     6971 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/model.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     7607 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/optim.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     1644 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/riccati.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg/tracking/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      587 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/__init__.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     4955 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/basic.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)    11395 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/eye.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      698 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/kf.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     5517 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/subjective.py
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     3096 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/three_dims.py
+drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg.egg-info/
+-rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/PKG-INFO
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      506 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/SOURCES.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/dependency_links.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      104 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/requires.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)        4 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/top_level.txt
+-rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2023-06-19 15:09:48.101289 lqg-0.1.9/setup.cfg
+-rw-r--r--   0 dominik   (1000) dominik   (1000)      919 2023-06-19 15:09:42.000000 lqg-0.1.9/setup.py
```

### Comparing `lqg-0.1.8/LICENSE` & `lqg-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/PKG-INFO` & `lqg-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.1.8
+Version: 0.1.9
 Summary: (Inverse) optimal control for linear quadratic Gaussian systems
 Home-page: https://github.com/dominikstrb/lqg
 Author: Dominik Straub
 Author-email: dominik.straub@tu-darmstadt.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `lqg-0.1.8/README.md` & `lqg-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/ccg.py` & `lqg-0.1.9/lqg/ccg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/infer/map.py` & `lqg-0.1.9/lqg/infer/map.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/infer/mle.py` & `lqg-0.1.9/lqg/infer/mle.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/infer/models.py` & `lqg-0.1.9/lqg/infer/models.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/infer/prior.py` & `lqg-0.1.9/lqg/infer/prior.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/infer/utils.py` & `lqg-0.1.9/lqg/infer/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/io.py` & `lqg-0.1.9/lqg/io.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/kalman.py` & `lqg-0.1.9/lqg/kalman.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/model.py` & `lqg-0.1.9/lqg/model.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/optim.py` & `lqg-0.1.9/lqg/optim.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/riccati.py` & `lqg-0.1.9/lqg/riccati.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/__init__.py` & `lqg-0.1.9/lqg/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/basic.py` & `lqg-0.1.9/lqg/tracking/basic.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/eye.py` & `lqg-0.1.9/lqg/tracking/eye.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/kf.py` & `lqg-0.1.9/lqg/tracking/kf.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/subjective.py` & `lqg-0.1.9/lqg/tracking/subjective.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg/tracking/three_dims.py` & `lqg-0.1.9/lqg/tracking/three_dims.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.8/lqg.egg-info/PKG-INFO` & `lqg-0.1.9/lqg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.1.8
+Version: 0.1.9
 Summary: (Inverse) optimal control for linear quadratic Gaussian systems
 Home-page: https://github.com/dominikstrb/lqg
 Author: Dominik Straub
 Author-email: dominik.straub@tu-darmstadt.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `lqg-0.1.8/setup.py` & `lqg-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqg",
-    version="0.1.8",
+    version="0.1.9",
     author="Dominik Straub",
     author_email="dominik.straub@tu-darmstadt.de",
     description="(Inverse) optimal control for linear quadratic Gaussian systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dominikstrb/lqg",
     packages=setuptools.find_packages(),
@@ -20,12 +20,12 @@
     ],
     python_requires='>=3.7',
     install_requires=[
         "numpy>=1.20.3",
         "scipy>=1.6.3",
         "matplotlib>=3.2.2",
         "ipywidgets==8.0.1",
-        "numpyro==0.9.2",
+        "numpyro>=0.9.2",
         "jax>=0.3.14",
         "arviz>=0.11.2",
     ],
 )
```

