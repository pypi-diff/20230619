# Comparing `tmp/genepierre-0.1.1.tar.gz` & `tmp/genepierre-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.1.1.tar", last modified: Mon Jun 19 13:44:09 2023, max compression
+gzip compressed data, was "genepierre-0.1.2.tar", last modified: Mon Jun 19 13:47:04 2023, max compression
```

## Comparing `genepierre-0.1.1.tar` & `genepierre-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:44:09.093547 genepierre-0.1.1/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 13:44:09.093547 genepierre-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:44:09.085554 genepierre-0.1.1/genepierre/
--rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.1.1/genepierre/__init__.py
--rw-rw-rw-   0        0        0     3196 2023-06-19 13:42:20.000000 genepierre-0.1.1/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:44:09.093547 genepierre-0.1.1/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 13:44:09.000000 genepierre-0.1.1/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-19 13:44:09.000000 genepierre-0.1.1/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:44:09.000000 genepierre-0.1.1/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-19 13:44:09.000000 genepierre-0.1.1/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 13:44:09.000000 genepierre-0.1.1/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 13:44:09.094547 genepierre-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-19 13:44:01.000000 genepierre-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.873844 genepierre-0.1.2/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:47:04.873844 genepierre-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.863846 genepierre-0.1.2/genepierre/
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.1.2/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-06-19 13:46:51.000000 genepierre-0.1.2/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:47:04.872854 genepierre-0.1.2/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 13:47:04.000000 genepierre-0.1.2/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 13:47:04.874844 genepierre-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-06-19 13:46:59.000000 genepierre-0.1.2/setup.py
```

### Comparing `genepierre-0.1.1/LICENSE.txt` & `genepierre-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.1.1/PKG-INFO` & `genepierre-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.1.1
+Version: 0.1.2
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.1.1/genepierre/genetic.py` & `genepierre-0.1.2/genepierre/genetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
         "functions",
         "gene_space",
         "initial_population",
         "stop_time",
         "saving_path",
         "cpt_loop",
         "seed",
-        "multiprocessing"
+        "multiprocessing",
+        "print_options"
     ]
 
     def __init__(
         self,
         functions,
         gene_space: list,
         initial_population: np.ndarray,  # one line = one chromosome !!!
```

### Comparing `genepierre-0.1.1/genepierre.egg-info/PKG-INFO` & `genepierre-0.1.2/genepierre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.1.1
+Version: 0.1.2
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.1.1/setup.py` & `genepierre-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
   packages = ['genepierre'],   # Chose the same as "name"
-  version = '0.1.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Gautier Laisné',                   # Type in your name
   author_email = 'gautier.laisne@inria.fr',      # Type in your E-Mail
   url = 'https://gitlab.inria.fr/auctus-team/people/gautierlaisne',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Genetic Algorithm'],   # Keywords that define your package best
```

