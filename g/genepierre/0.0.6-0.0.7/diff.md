# Comparing `tmp/genepierre-0.0.6.tar.gz` & `tmp/genepierre-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.0.6.tar", last modified: Mon Jun 19 12:40:24 2023, max compression
+gzip compressed data, was "genepierre-0.0.7.tar", last modified: Mon Jun 19 12:51:54 2023, max compression
```

## Comparing `genepierre-0.0.6.tar` & `genepierre-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:40:24.258724 genepierre-0.0.6/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 12:40:24.258724 genepierre-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 12:40:24.229724 genepierre-0.0.6/genepierre/
--rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.0.6/genepierre/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.6/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:40:24.257730 genepierre-0.0.6/genepierre/polytope_utils/
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:33.000000 genepierre-0.0.6/genepierre/polytope_utils/__init__.py
--rw-rw-rw-   0        0        0     2805 2023-06-19 12:36:22.000000 genepierre-0.0.6/genepierre/polytope_utils/directions.py
--rw-rw-rw-   0        0        0     2431 2023-06-19 12:38:07.000000 genepierre-0.0.6/genepierre/polytope_utils/model_computation.py
--rw-rw-rw-   0        0        0      615 2023-06-19 12:38:36.000000 genepierre-0.0.6/genepierre/polytope_utils/model_perturbation.py
--rw-rw-rw-   0        0        0     1219 2023-06-19 12:37:25.000000 genepierre-0.0.6/genepierre/polytope_utils/points_on_sphere.py
--rw-rw-rw-   0        0        0     3394 2023-06-19 12:37:07.000000 genepierre-0.0.6/genepierre/polytope_utils/polytope_computation.py
--rw-rw-rw-   0        0        0     2343 2023-06-19 12:36:48.000000 genepierre-0.0.6/genepierre/polytope_utils/polytope_discretization.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:40:24.252727 genepierre-0.0.6/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 12:40:24.000000 genepierre-0.0.6/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-06-19 12:40:24.000000 genepierre-0.0.6/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:40:24.000000 genepierre-0.0.6/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-19 12:40:24.000000 genepierre-0.0.6/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 12:40:24.000000 genepierre-0.0.6/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 12:40:24.259724 genepierre-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-06-19 12:40:08.000000 genepierre-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.573871 genepierre-0.0.7/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 12:51:54.574871 genepierre-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.562871 genepierre-0.0.7/genepierre/
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.0.7/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.7/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.569871 genepierre-0.0.7/genepierre/joint_configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:47:34.000000 genepierre-0.0.7/genepierre/joint_configurations/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-06-19 12:49:17.000000 genepierre-0.0.7/genepierre/joint_configurations/combinations.py
+-rw-rw-rw-   0        0        0      323 2023-06-19 12:48:51.000000 genepierre-0.0.7/genepierre/joint_configurations/q_4.py
+-rw-rw-rw-   0        0        0      453 2023-06-19 12:48:44.000000 genepierre-0.0.7/genepierre/joint_configurations/q_6.py
+-rw-rw-rw-   0        0        0      590 2023-06-19 12:48:39.000000 genepierre-0.0.7/genepierre/joint_configurations/q_8.py
+-rw-rw-rw-   0        0        0     1230 2023-06-19 12:48:33.000000 genepierre-0.0.7/genepierre/joint_configurations/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.570874 genepierre-0.0.7/genepierre/models/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:46:30.000000 genepierre-0.0.7/genepierre/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.573871 genepierre-0.0.7/genepierre/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:33.000000 genepierre-0.0.7/genepierre/utils/__init__.py
+-rw-rw-rw-   0        0        0     2805 2023-06-19 12:36:22.000000 genepierre-0.0.7/genepierre/utils/directions.py
+-rw-rw-rw-   0        0        0     2431 2023-06-19 12:38:07.000000 genepierre-0.0.7/genepierre/utils/model_computation.py
+-rw-rw-rw-   0        0        0      615 2023-06-19 12:38:36.000000 genepierre-0.0.7/genepierre/utils/model_perturbation.py
+-rw-rw-rw-   0        0        0     1219 2023-06-19 12:37:25.000000 genepierre-0.0.7/genepierre/utils/points_on_sphere.py
+-rw-rw-rw-   0        0        0     3384 2023-06-19 12:50:14.000000 genepierre-0.0.7/genepierre/utils/polytope_computation.py
+-rw-rw-rw-   0        0        0     2343 2023-06-19 12:36:48.000000 genepierre-0.0.7/genepierre/utils/polytope_discretization.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:51:54.566870 genepierre-0.0.7/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 12:51:54.000000 genepierre-0.0.7/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 12:51:54.575871 genepierre-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2023-06-19 12:51:29.000000 genepierre-0.0.7/setup.py
```

### Comparing `genepierre-0.0.6/LICENSE.txt` & `genepierre-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/PKG-INFO` & `genepierre-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.6
+Version: 0.0.7
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.6/genepierre/genetic.py` & `genepierre-0.0.7/genepierre/genetic.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/directions.py` & `genepierre-0.0.7/genepierre/utils/directions.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/model_computation.py` & `genepierre-0.0.7/genepierre/utils/model_computation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/model_perturbation.py` & `genepierre-0.0.7/genepierre/utils/model_perturbation.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/points_on_sphere.py` & `genepierre-0.0.7/genepierre/utils/points_on_sphere.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/polytope_computation.py` & `genepierre-0.0.7/genepierre/utils/polytope_computation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import biorbd
 import pycapacity.human as capacity
-import identification_study.utils.model_computation as mcomp
+import genepierre.utils.model_computation as mcomp
 from pycapacity.algorithms import iterative_convex_hull_method
 
 def getPolytope(model: biorbd.Model, Q: np.ndarray, bodyName: str, endEffector: list, tol=1, withBias: bool = True, name: str = None) -> dict:
     zeros = np.zeros(model.nbQ())
 
     model.updateMuscles(Q, True)
     model.UpdateKinematicsCustom(Q, zeros, zeros)
```

### Comparing `genepierre-0.0.6/genepierre/polytope_utils/polytope_discretization.py` & `genepierre-0.0.7/genepierre/utils/polytope_discretization.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.6/genepierre.egg-info/PKG-INFO` & `genepierre-0.0.7/genepierre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.6
+Version: 0.0.7
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.6/setup.py` & `genepierre-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
-  packages = ['genepierre', 'genepierre.polytope_utils'],   # Chose the same as "name"
-  version = '0.0.6',      # Start with a small number and increase it with every change you make
+  packages = ['genepierre', 'genepierre.utils', 'genepierre.models', 'genepierre.joint_configurations'],   # Chose the same as "name"
+  version = '0.0.7',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Gautier Laisné',                   # Type in your name
   author_email = 'gautier.laisne@inria.fr',      # Type in your E-Mail
   url = 'https://gitlab.inria.fr/auctus-team/people/gautierlaisne',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Genetic Algorithm'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'scipy',
           'bioviz',
-          'matplotlib'
+          'matplotlib',
+          'pycapacity'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

