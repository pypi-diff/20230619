# Comparing `tmp/genepierre-0.0.4.tar.gz` & `tmp/genepierre-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.0.4.tar", last modified: Mon Jun 19 12:10:05 2023, max compression
+gzip compressed data, was "genepierre-0.0.5.tar", last modified: Mon Jun 19 12:13:36 2023, max compression
```

## Comparing `genepierre-0.0.4.tar` & `genepierre-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:10:05.073320 genepierre-0.0.4/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 12:10:05.073320 genepierre-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 12:10:05.061330 genepierre-0.0.4/genepierre/
--rw-rw-rw-   0        0        0       33 2023-06-19 12:05:17.000000 genepierre-0.0.4/genepierre/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.4/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:10:05.072329 genepierre-0.0.4/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 12:10:04.000000 genepierre-0.0.4/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-19 12:10:05.000000 genepierre-0.0.4/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:10:04.000000 genepierre-0.0.4/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 12:10:04.000000 genepierre-0.0.4/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 12:10:04.000000 genepierre-0.0.4/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 12:10:05.074322 genepierre-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1654 2023-06-19 12:09:51.000000 genepierre-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:13:36.995781 genepierre-0.0.5/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 12:13:36.995781 genepierre-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 12:13:36.987781 genepierre-0.0.5/genepierre/
+-rw-rw-rw-   0        0        0       40 2023-06-19 12:11:25.000000 genepierre-0.0.5/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.5/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 12:13:36.995781 genepierre-0.0.5/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 12:13:36.000000 genepierre-0.0.5/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-19 12:13:36.000000 genepierre-0.0.5/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 12:13:36.000000 genepierre-0.0.5/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 12:13:36.000000 genepierre-0.0.5/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 12:13:36.000000 genepierre-0.0.5/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 12:13:36.996781 genepierre-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2023-06-19 12:13:31.000000 genepierre-0.0.5/setup.py
```

### Comparing `genepierre-0.0.4/LICENSE.txt` & `genepierre-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.4/PKG-INFO` & `genepierre-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.4
+Version: 0.0.5
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.4/genepierre/genetic.py` & `genepierre-0.0.5/genepierre/genetic.py`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.4/genepierre.egg-info/PKG-INFO` & `genepierre-0.0.5/genepierre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.4
+Version: 0.0.5
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.4/setup.py` & `genepierre-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
   packages = ['genepierre'],   # Chose the same as "name"
-  version = '0.0.4',      # Start with a small number and increase it with every change you make
+  version = '0.0.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'Gautier Laisné',                   # Type in your name
   author_email = 'gautier.laisne@inria.fr',      # Type in your E-Mail
   url = 'https://gitlab.inria.fr/auctus-team/people/gautierlaisne',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Genetic Algorithm'],   # Keywords that define your package best
```

