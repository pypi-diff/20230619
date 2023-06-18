# Comparing `tmp/catencfamily-0.0.76.tar.gz` & `tmp/catencfamily-0.0.77.tar.gz`

## Comparing `catencfamily-0.0.76.tar` & `catencfamily-0.0.77.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    40405 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.76/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.76/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.76/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.76/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.77/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.77/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    40745 2020-02-02 00:00:00.000000 catencfamily-0.0.77/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.77/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.77/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.77/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.77/PKG-INFO
```

### Comparing `catencfamily-0.0.76/src/catencfamily/encoders.py` & `catencfamily-0.0.77/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.76/src/catencfamily/utils.py` & `catencfamily-0.0.77/src/catencfamily/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 15th June, 2023
+# 17th June, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
@@ -537,14 +537,15 @@
     if filePath is None:
         filePath = pathlib.Path.cwd()
         path = filePath / filename
     else:
         path = pathlib.Path(filePath) / filename
     with open(path, 'wb') as outp:
         pickle.dump(pythonObject, outp, pickle.HIGHEST_PROTOCOL)
+    print("Object saved to:", str(path))    
 
      
      
 
  # It restores an earlier saved python object
 def restorePythonObject(filename, filePath = None):
      """
@@ -562,14 +563,15 @@
      -------
      Python-object
 
      """
      if filePath is None:
         filePath = pathlib.Path.cwd()
         path = filePath / filename
+        print(f"Looking for '{filename}' in folder: {str(filePath)}" )
      else:
         path = pathlib.Path(filePath) / filename
 
      with open(path, 'rb') as inp:
          ct = pickle.load(inp)
      return ct    
 
@@ -916,15 +918,15 @@
     
 
     
 # Community visualization
 # Kaggle: https://www.kaggle.com/code/rahulgoel1106/commmunity-detection-using-igraph-and-networkx
 def communityVisualization(filename, pathToFolder, algo = nx.community.greedy_modularity_communities ,
                            ax= None, title = None, withLabels = False, font_size = 8, edgewidth = 0.1,
-                           colorList =  ["orange","yellow","cyan","green","red"]):
+                           colorList =  ["orange","yellow","cyan","green","red", "purple"]):
     """
     Desc
     ----
     Displays communities created by given community algo.
 
     Parameters
     ----------
@@ -936,15 +938,15 @@
                     nx.community.greedy_modularity_communities
                     nx.community.louvain_communities
     ax: Matplotlib axis object
     withLabels : boolean, Should labels be displayed? The default is False.
     font_size : int, Label font size. The default is 8.
     edgewidth: float, Edge line width
     colorList: List of colors for difft communitied. 
-               Default is: ["orange","yellow","cyan","green","red"]
+               Default is: ["orange","yellow","cyan","green","red","purple"]
 
     Returns
     -------
     None.
 
     """
     filepath = pathToFolder / filename
@@ -1057,30 +1059,35 @@
 
     # 2. For every file in the filelist
     map_list = []  # Start with a blank list of dictionaries
     # df will store dataframe train_binned after each bin-col is mapped
     #  
     df = pd.DataFrame()
     for file in filelist:
+      print("Reading file: ", file)
       # 2.1 Load network
       # Get full filename that includes filepath
       filepath = Path(pathToGraphFolder) / file
       # Read the file as a network
       G = nx.read_gml(filepath)
-
+      if (len(G.edges())) == 0: 
+        print("This network has no edges. Moving to next file.")
+        continue 
+       
       # 2.2 Calculate community classes using algo
       #    cm_mod contains as many frozensets of nodes
       #    as there are communities:
           
       if algo == nx.community.girvan_newman:
           cm_mod = algo(G)
           cm_mod = tuple(sorted(c) for c in next(cm_mod))
           cm_mod = [frozenset(i) for i in cm_mod ]
       else:
           cm_mod = algo(G)
+          #print(cm_mod)
 
       # 3.0 We now create dict corresponding to
       #     all communities in cm_mod
       #    Example:
       #                 frozenset1         frozenset2
       #   cm_mod:     [{'434', '435' },    {'23' , '78'}]
       #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
@@ -1104,15 +1111,15 @@
       # Now that map dict for the modularity
       # classes are ready, append it to map_list
       map_list.append(fset_dict)
 
       # Extract column name from file:
       colToProject = file.split('_')[0]
       # Map train_binned column using the dict
-      df[file] = train_binned[colToProject].map(fset_dict)
+      df[file] = (train_binned[colToProject].astype(str)).map(fset_dict)
       # Continue for loop for the next filelist
     return map_list,df
 
 
 
 def transformBinnedDF2CommunitiesAll(pathToGraphFolder, train_binned, algo):
     """
```

### Comparing `catencfamily-0.0.76/LICENSE` & `catencfamily-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.76/README.md` & `catencfamily-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.76/pyproject.toml` & `catencfamily-0.0.77/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.76"
+version = "0.0.77"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.76/PKG-INFO` & `catencfamily-0.0.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.76
+Version: 0.0.77
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

