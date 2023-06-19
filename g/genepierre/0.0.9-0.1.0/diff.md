# Comparing `tmp/genepierre-0.0.9.tar.gz` & `tmp/genepierre-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepierre-0.0.9.tar", last modified: Mon Jun 19 13:20:41 2023, max compression
+gzip compressed data, was "genepierre-0.1.0.tar", last modified: Mon Jun 19 13:42:50 2023, max compression
```

## Comparing `genepierre-0.0.9.tar` & `genepierre-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:20:41.903246 genepierre-0.0.9/
--rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0      767 2023-06-19 13:20:41.903246 genepierre-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:20:41.891232 genepierre-0.0.9/genepierre/
--rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.0.9/genepierre/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-06-19 11:53:16.000000 genepierre-0.0.9/genepierre/genetic.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:20:41.902231 genepierre-0.0.9/genepierre.egg-info/
--rw-rw-rw-   0        0        0      767 2023-06-19 13:20:41.000000 genepierre-0.0.9/genepierre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-19 13:20:41.000000 genepierre-0.0.9/genepierre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:20:41.000000 genepierre-0.0.9/genepierre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-19 13:20:41.000000 genepierre-0.0.9/genepierre.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 13:20:41.000000 genepierre-0.0.9/genepierre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 13:20:41.904233 genepierre-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1745 2023-06-19 13:20:29.000000 genepierre-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:50.268217 genepierre-0.1.0/
+-rw-rw-rw-   0        0        0     1080 2023-06-19 11:31:28.000000 genepierre-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:42:50.268217 genepierre-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-19 11:30:44.000000 genepierre-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:50.255149 genepierre-0.1.0/genepierre/
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:38:21.000000 genepierre-0.1.0/genepierre/__init__.py
+-rw-rw-rw-   0        0        0     3196 2023-06-19 13:42:20.000000 genepierre-0.1.0/genepierre/genetic.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:42:50.268217 genepierre-0.1.0/genepierre.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-06-19 13:42:50.000000 genepierre-0.1.0/genepierre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-19 13:42:50.000000 genepierre-0.1.0/genepierre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:42:50.000000 genepierre-0.1.0/genepierre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-19 13:42:50.000000 genepierre-0.1.0/genepierre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 13:42:50.000000 genepierre-0.1.0/genepierre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 13:42:50.269215 genepierre-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-06-19 13:42:39.000000 genepierre-0.1.0/setup.py
```

### Comparing `genepierre-0.0.9/LICENSE.txt` & `genepierre-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genepierre-0.0.9/PKG-INFO` & `genepierre-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.9
+Version: 0.1.0
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.9/genepierre/genetic.py` & `genepierre-0.1.0/genepierre/genetic.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,41 +19,47 @@
         self,
         functions,
         gene_space: list,
         initial_population: np.ndarray,  # one line = one chromosome !!!
         stop_time: int,  # in seconds
         saving_path: str,
         seed: int,
-        multiprocessing: bool
+        multiprocessing: bool,
+        print_options = { "best_parent": True, "parents_costs": True }
     ):
         self.functions = functions
         self.gene_space = gene_space
         self.initial_population = initial_population
         self.stop_time = stop_time
         self.saving_path = saving_path
         Path(saving_path).mkdir(parents=True, exist_ok=True)
         self.cpt_loop = 0
         self.seed = seed
         np.random.seed(seed)
         self.multiprocessing = multiprocessing
+        self.print_options = print_options
 
     def run(self):
         start_time = time.time()
 
         population = self.initial_population
 
         current_time = time.time()
         while (current_time - start_time) <= self.stop_time:
             print(f"Loop {self.cpt_loop}:")
             loop_start_time = time.time()
 
             costs = self.functions.evaluate(self, population)
             parents, costs_parents = self.functions.select_parents(self, population, costs)
-            print(f"\tBest parent: {list(parents[0])[:5]}")
-            print(f"\tBest 5 parents costs: {costs_parents[0:5]}")
+
+            if "best_parent" in self.print_options:
+                print(f"\tBest parent: {list(parents[0])}")
+            if "parents_costs" in self.print_options:
+                print(f"\tBest {len(parents)} parents costs: {costs_parents}")
+                
             crossover_offspring = self.functions.crossover(self, parents, costs_parents)
             mutations_from_parents, mutations_from_crossover_offspring = self.functions.mutate(
                 self, parents, crossover_offspring
             )
 
             data_to_save = {
                 "cpt_loop": self.cpt_loop,
```

### Comparing `genepierre-0.0.9/genepierre.egg-info/PKG-INFO` & `genepierre-0.1.0/genepierre.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genepierre
-Version: 0.0.9
+Version: 0.1.0
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://gitlab.inria.fr/auctus-team/people/gautierlaisne
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Gautier Laisné
 Author-email: gautier.laisne@inria.fr
 License: MIT
 Keywords: Genetic Algorithm
```

### Comparing `genepierre-0.0.9/setup.py` & `genepierre-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from distutils.core import setup
 setup(
   name = 'genepierre',         # How you named your package folder (MyLib)
   packages = ['genepierre'],   # Chose the same as "name"
-  version = '0.0.9',      # Start with a small number and increase it with every change you make
+  version = '0.1.0',      # Start with a small number and increase it with every change you make
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
           'matplotlib',
-          'pycapacity'
+          'pycapacity',
+          'pillow==9.0.0'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

