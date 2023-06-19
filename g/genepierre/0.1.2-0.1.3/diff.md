# Comparing `tmp/genepierre-0.1.2.tar.gz` & `tmp/genepierre-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.1.2.tar", last modified: Mon Jun 19 13:47:04 2023, max compression
+gzip compressed data, was "genepierre-0.1.3.tar", last modified: Mon Jun 19 13:49:16 2023, max compression
```

## Comparing `genepierre-0.1.2.tar` & `genepierre-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.873844 genepierre-0.1.2/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 13:47:04.873844 genepierre-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.863846 genepierre-0.1.2/genepierre/
--rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.1.2/genepierre/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-06-19 13:46:51.000000 genepierre-0.1.2/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.872854 genepierre-0.1.2/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 13:47:04.874844 genepierre-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-19 13:46:59.000000 genepierre-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.124814 genepierre-0.1.3/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:49:16.124814 genepierre-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.108814 genepierre-0.1.3/genepierre/
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.1.3/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-06-19 13:46:51.000000 genepierre-0.1.3/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.119816 genepierre-0.1.3/genepierre/joint_configurations/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:47:34.000000 genepierre-0.1.3/genepierre/joint_configurations/__init__.py
+-rw-rw-rw-   0        0        0      509 2023-06-19 12:49:17.000000 genepierre-0.1.3/genepierre/joint_configurations/combinations.py
+-rw-rw-rw-   0        0        0      323 2023-06-19 12:48:51.000000 genepierre-0.1.3/genepierre/joint_configurations/q_4.py
+-rw-rw-rw-   0        0        0      453 2023-06-19 12:48:44.000000 genepierre-0.1.3/genepierre/joint_configurations/q_6.py
+-rw-rw-rw-   0        0        0      590 2023-06-19 12:48:39.000000 genepierre-0.1.3/genepierre/joint_configurations/q_8.py
+-rw-rw-rw-   0        0        0     1230 2023-06-19 12:48:33.000000 genepierre-0.1.3/genepierre/joint_configurations/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.123815 genepierre-0.1.3/genepierre/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:33.000000 genepierre-0.1.3/genepierre/utils/__init__.py
+-rw-rw-rw-   0        0        0     2805 2023-06-19 12:36:22.000000 genepierre-0.1.3/genepierre/utils/directions.py
+-rw-rw-rw-   0        0        0     2431 2023-06-19 12:38:07.000000 genepierre-0.1.3/genepierre/utils/model_computation.py
+-rw-rw-rw-   0        0        0      615 2023-06-19 12:38:36.000000 genepierre-0.1.3/genepierre/utils/model_perturbation.py
+-rw-rw-rw-   0        0        0     1219 2023-06-19 12:37:25.000000 genepierre-0.1.3/genepierre/utils/points_on_sphere.py
+-rw-rw-rw-   0        0        0     3384 2023-06-19 12:50:14.000000 genepierre-0.1.3/genepierre/utils/polytope_computation.py
+-rw-rw-rw-   0        0        0     2343 2023-06-19 12:36:48.000000 genepierre-0.1.3/genepierre/utils/polytope_discretization.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.124814 genepierre-0.1.3/genepierre/vizualize/
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:35:35.000000 genepierre-0.1.3/genepierre/vizualize/__init__.py
+-rw-rw-rw-   0        0        0     6467 2023-06-19 12:50:44.000000 genepierre-0.1.3/genepierre/vizualize/bioviz_model_polytope.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:49:16.117815 genepierre-0.1.3/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:49:16.000000 genepierre-0.1.3/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-06-19 13:49:16.000000 genepierre-0.1.3/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:49:16.000000 genepierre-0.1.3/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-19 13:49:16.000000 genepierre-0.1.3/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 13:49:16.000000 genepierre-0.1.3/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 13:49:16.125815 genepierre-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-06-19 13:49:13.000000 genepierre-0.1.3/setup.py
```

### Comparing `genepierre-0.1.2/LICENSE.txt` & `genepierre-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.1.2/PKG-INFO` & `genepierre-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.1.2
+Version: 0.1.3
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.1.2/genepierre/genetic.py` & `genepierre-0.1.3/genepierre/genetic.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.1.2/genepierre.egg-info/PKG-INFO` & `genepierre-0.1.3/genepierre.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.1.2
+Version: 0.1.3
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.1.2/setup.py` & `genepierre-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
-  packages = ['genepierre'],   # Chose the same as "name"
-  version = '0.1.2',      # Start with a small number and increase it with every change you make
+  packages = ['genepierre', 'genepierre.utils', 'genepierre.vizualize', 'genepierre.joint_configurations'],   # Chose the same as "name"
+  version = '0.1.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Gautier Laisné',                   # Type in your name
   author_email = 'gautier.laisne@inria.fr',      # Type in your E-Mail
   url = 'https://gitlab.inria.fr/auctus-team/people/gautierlaisne',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Genetic Algorithm'],   # Keywords that define your package best
```

