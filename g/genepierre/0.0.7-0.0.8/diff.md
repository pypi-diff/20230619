# Comparing `tmp/genepierre-0.0.7.tar.gz` & `tmp/genepierre-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.0.7.tar", last modified: Mon Jun 19 12:51:54 2023, max compression
+gzip compressed data, was "genepierre-0.0.8.tar", last modified: Mon Jun 19 13:04:14 2023, max compression
```

## Comparing `genepierre-0.0.7.tar` & `genepierre-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.573871 genepierre-0.0.7/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 12:51:54.574871 genepierre-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.562871 genepierre-0.0.7/genepierre/
--rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.0.7/genepierre/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.7/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.569871 genepierre-0.0.7/genepierre/joint_configurations/
--rw-rw-rw-   0        0        0        0 2023-06-19 12:47:34.000000 genepierre-0.0.7/genepierre/joint_configurations/__init__.py
--rw-rw-rw-   0        0        0      509 2023-06-19 12:49:17.000000 genepierre-0.0.7/genepierre/joint_configurations/combinations.py
--rw-rw-rw-   0        0        0      323 2023-06-19 12:48:51.000000 genepierre-0.0.7/genepierre/joint_configurations/q_4.py
--rw-rw-rw-   0        0        0      453 2023-06-19 12:48:44.000000 genepierre-0.0.7/genepierre/joint_configurations/q_6.py
--rw-rw-rw-   0        0        0      590 2023-06-19 12:48:39.000000 genepierre-0.0.7/genepierre/joint_configurations/q_8.py
--rw-rw-rw-   0        0        0     1230 2023-06-19 12:48:33.000000 genepierre-0.0.7/genepierre/joint_configurations/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.570874 genepierre-0.0.7/genepierre/models/
--rw-rw-rw-   0        0        0        0 2023-06-19 12:46:30.000000 genepierre-0.0.7/genepierre/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.573871 genepierre-0.0.7/genepierre/utils/
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:33.000000 genepierre-0.0.7/genepierre/utils/__init__.py
--rw-rw-rw-   0        0        0     2805 2023-06-19 12:36:22.000000 genepierre-0.0.7/genepierre/utils/directions.py
--rw-rw-rw-   0        0        0     2431 2023-06-19 12:38:07.000000 genepierre-0.0.7/genepierre/utils/model_computation.py
--rw-rw-rw-   0        0        0      615 2023-06-19 12:38:36.000000 genepierre-0.0.7/genepierre/utils/model_perturbation.py
--rw-rw-rw-   0        0        0     1219 2023-06-19 12:37:25.000000 genepierre-0.0.7/genepierre/utils/points_on_sphere.py
--rw-rw-rw-   0        0        0     3384 2023-06-19 12:50:14.000000 genepierre-0.0.7/genepierre/utils/polytope_computation.py
--rw-rw-rw-   0        0        0     2343 2023-06-19 12:36:48.000000 genepierre-0.0.7/genepierre/utils/polytope_discretization.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.566870 genepierre-0.0.7/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 12:51:54.575871 genepierre-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1821 2023-06-19 12:51:29.000000 genepierre-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:04:14.328839 genepierre-0.0.8/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:04:14.328839 genepierre-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 13:04:14.311840 genepierre-0.0.8/genepierre/
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.0.8/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.8/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:04:14.324843 genepierre-0.0.8/genepierre/joint_configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:47:34.000000 genepierre-0.0.8/genepierre/joint_configurations/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-06-19 12:49:17.000000 genepierre-0.0.8/genepierre/joint_configurations/combinations.py
+-rw-rw-rw-   0        0        0      323 2023-06-19 12:48:51.000000 genepierre-0.0.8/genepierre/joint_configurations/q_4.py
+-rw-rw-rw-   0        0        0      453 2023-06-19 12:48:44.000000 genepierre-0.0.8/genepierre/joint_configurations/q_6.py
+-rw-rw-rw-   0        0        0      590 2023-06-19 12:48:39.000000 genepierre-0.0.8/genepierre/joint_configurations/q_8.py
+-rw-rw-rw-   0        0        0     1230 2023-06-19 12:48:33.000000 genepierre-0.0.8/genepierre/joint_configurations/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:04:14.328839 genepierre-0.0.8/genepierre/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:33.000000 genepierre-0.0.8/genepierre/utils/__init__.py
+-rw-rw-rw-   0        0        0     2805 2023-06-19 12:36:22.000000 genepierre-0.0.8/genepierre/utils/directions.py
+-rw-rw-rw-   0        0        0     2431 2023-06-19 12:38:07.000000 genepierre-0.0.8/genepierre/utils/model_computation.py
+-rw-rw-rw-   0        0        0      615 2023-06-19 12:38:36.000000 genepierre-0.0.8/genepierre/utils/model_perturbation.py
+-rw-rw-rw-   0        0        0     1219 2023-06-19 12:37:25.000000 genepierre-0.0.8/genepierre/utils/points_on_sphere.py
+-rw-rw-rw-   0        0        0     3384 2023-06-19 12:50:14.000000 genepierre-0.0.8/genepierre/utils/polytope_computation.py
+-rw-rw-rw-   0        0        0     2343 2023-06-19 12:36:48.000000 genepierre-0.0.8/genepierre/utils/polytope_discretization.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:04:14.321838 genepierre-0.0.8/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:04:14.000000 genepierre-0.0.8/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-06-19 13:04:14.000000 genepierre-0.0.8/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:04:14.000000 genepierre-0.0.8/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-19 13:04:14.000000 genepierre-0.0.8/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 13:04:14.000000 genepierre-0.0.8/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 13:04:14.329839 genepierre-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1800 2023-06-19 13:04:08.000000 genepierre-0.0.8/setup.py
```

### Comparing `genepierre-0.0.7/LICENSE.txt` & `genepierre-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/PKG-INFO` & `genepierre-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.7
+Version: 0.0.8
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.7/genepierre/genetic.py` & `genepierre-0.0.8/genepierre/genetic.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/joint_configurations/q_8.py` & `genepierre-0.0.8/genepierre/joint_configurations/q_8.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/joint_configurations/validation.py` & `genepierre-0.0.8/genepierre/joint_configurations/validation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/directions.py` & `genepierre-0.0.8/genepierre/utils/directions.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/model_computation.py` & `genepierre-0.0.8/genepierre/utils/model_computation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/model_perturbation.py` & `genepierre-0.0.8/genepierre/utils/model_perturbation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/points_on_sphere.py` & `genepierre-0.0.8/genepierre/utils/points_on_sphere.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/polytope_computation.py` & `genepierre-0.0.8/genepierre/utils/polytope_computation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre/utils/polytope_discretization.py` & `genepierre-0.0.8/genepierre/utils/polytope_discretization.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.7/genepierre.egg-info/PKG-INFO` & `genepierre-0.0.8/genepierre.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.7
+Version: 0.0.8
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.7/genepierre.egg-info/SOURCES.txt` & `genepierre-0.0.8/genepierre.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 genepierre.egg-info/top_level.txt
 genepierre/joint_configurations/__init__.py
 genepierre/joint_configurations/combinations.py
 genepierre/joint_configurations/q_4.py
 genepierre/joint_configurations/q_6.py
 genepierre/joint_configurations/q_8.py
 genepierre/joint_configurations/validation.py
-genepierre/models/__init__.py
 genepierre/utils/__init__.py
 genepierre/utils/directions.py
 genepierre/utils/model_computation.py
 genepierre/utils/model_perturbation.py
 genepierre/utils/points_on_sphere.py
 genepierre/utils/polytope_computation.py
 genepierre/utils/polytope_discretization.py
```

### Comparing `genepierre-0.0.7/setup.py` & `genepierre-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
-  packages = ['genepierre', 'genepierre.utils', 'genepierre.models', 'genepierre.joint_configurations'],   # Chose the same as "name"
-  version = '0.0.7',      # Start with a small number and increase it with every change you make
+  packages = ['genepierre', 'genepierre.utils', 'genepierre.joint_configurations'],   # Chose the same as "name"
+  version = '0.0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Gautier Laisné',                   # Type in your name
   author_email = 'gautier.laisne@inria.fr',      # Type in your E-Mail
   url = 'https://gitlab.inria.fr/auctus-team/people/gautierlaisne',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Genetic Algorithm'],   # Keywords that define your package best
```

