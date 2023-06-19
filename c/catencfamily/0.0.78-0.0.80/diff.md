# Comparing `tmp/catencfamily-0.0.78.tar.gz` & `tmp/catencfamily-0.0.80.tar.gz`

## Comparing `catencfamily-0.0.78.tar` & `catencfamily-0.0.80.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.78/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.78/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    42443 2020-02-02 00:00:00.000000 catencfamily-0.0.78/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.78/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.78/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.78/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.78/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89201 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    42984 2020-02-02 00:00:00.000000 catencfamily-0.0.80/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.80/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.80/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.80/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.80/PKG-INFO
```

### Comparing `catencfamily-0.0.78/src/catencfamily/encoders.py` & `catencfamily-0.0.80/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 04th June, 2023
+# 19th June, 2023
 """
 References:
 Coding standard:
     https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
     
 Developing sklearn estimators:
     https://scikit-learn.org/stable/developers/develop.html 
@@ -1746,23 +1746,25 @@
         Returns
         -------
         A dictionary with keys as column names in cat_cols. For every key,
         in the dict (say, 'app')', value is a dataframe. The dataframe's
         first column is a cat col (same as the dict key, say, 'app').
         Other columns map each level in this column ('app') to difft 
         derived centrality measures (that, together, we call as vector).
+        It is possible that same level may have different vectors at
+        different row positions.
         """
         # Save target in a sep var
         target = X.pop('target')
         # Remaining cols of X
         datacols = list(X.columns)
         
         # Extract a dict: list_rel_cols.
         # Its keys are cat col names.
-        # For every key, say' app',
+        # For every key, say 'app',
         # value is a list (structure) of relevant
         # col-names
         list_rel_cols = self._getRelCols(datacols)
         
         # We now create another dict, ess where
         # keys remain as cat cols ('app') but
         # each value, instead of being a list struct,
@@ -1845,14 +1847,40 @@
         impute: boolean; Imputes X with median strategy and outputs impute model
                 for future use. If False,           
 
         Returns
         -------
         Outputs two objects: One, a dictionary with keys as cat cols and values as corresponding 
         DataFrames and the other an Impute model (or None).
+        Example: 
+                Our input DataFrame has four rows:
+                   'app'     'ip'     'os'
+                    203       198      4
+                    202       199      3
+                    205       198      4
+                    203       200     10
+        
+        vec_dict['app']
+        
+                 deg_    pr_   clu_
+        row 1   0.05    0.8    0.34 
+        row 2   0.003   0.78   0.45
+        row 3   0.33    0.32   0.17
+        row 4   0.051   0.79   0.34  (very similar to row 1)
+        
+        When take_mean = True then output dataframe has 3-rows
+        and mean of row1 and row4 are taken to represent
+        the corresponding level.
+        
+        In the meta data, 'label' column will store row-wise 'app'
+        values, ie:
+            203
+            202
+            205
+            203
 
         """
         # Check if X has a 'target' column
         j = list(X.columns)
         
         if not 'target' in j:
             raise ValueError("Passed DataFrame does not contain 'target' column even if dummy!")
@@ -1901,14 +1929,19 @@
                 d = normalize(vec_dict[i])  
                 # 'd' being np.array(), convert back to DataFrame
                 vec_dict[i] = pd.DataFrame(d,columns = colnames)
             return vec_dict, si
         
         if filepath is None:
             filepath = self.pathToStoreProgress
+            # If filepath folder does not exist, create one
+            if not (Path.is_dir(filepath)):
+                p = Path(filepath)
+                p.mkdir(parents=True, exist_ok=True)
+                
 
         # DataFrame to hold meta data
         vec_meta = pd.DataFrame(columns=["label","color"])
         
         # For every cat col, i
         for i in vec_dict.keys():
             
@@ -1936,17 +1969,19 @@
             vec_dict[i] = pd.DataFrame(d,columns = colnames)
             # Save our vector file as tab-separated without header and without
             # index
             vec_dict[i].to_csv(p , sep="\t", header = False, index = False)
             # Not sure why the following 'sleep' line was needed!
             time.sleep(0.1)
         
-        # Task over. Print messages:    
-        print("Saved files are named as catcolname.tsv and catcolname_meta.tsv")
-        print(f"Folder is {filepath}" )
+        # Task over. Print messages:   
+        print("=============================================================")    
+        print("Saved files are named as '<catColname>.tsv' and '<catColname_meta>.tsv'")
+        print(f"You will find them in folder: '{filepath}'" )
+        print("=============================================================")    
         print("Load these file-pairs in tensorflow's 'Embedding Projector'")
         print("It helps in visualizing interrelationships among levels of a categorical feature")
         
         # Return the dict, and impute model used
         return vec_dict, si
```

### Comparing `catencfamily-0.0.78/src/catencfamily/utils.py` & `catencfamily-0.0.80/src/catencfamily/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,24 +587,34 @@
     
     Desc
     ----
     Given a dictionray of dataframes, the function performs PCA
     on each dataframe and outputs a concatenated dataframe. 
     This it does for both the dictionaries and outputs two dataframes. 
     
+    Example: 
+        Assume our training data has 5-cat columns. Corresponding
+        to every col the input dict will have 5-dataframes of 
+        unit vectors. No of rows in each dataFrame would be the same
+        that is as many as in train/test data. 
+        Take PCA of each dataframe and reduce the unit vectors to
+        2-cols. Thus, we will have 10 columns in all. Concatenate
+        these 10 columns to make our revised training/test data.
+    
     Parameters
     ----------
     
     vec_train: Dictionary of Dataframes. It would contain unit vectors
-               for each cat col of train data.
+               per-level per-row for each cat col of train data.
                
     vec_test:  Dictionary of Dataframes. It would contain unit vectors
                for each cat col of test data.         
                
-    n_components: No of PCA components. Default is 2.
+    n_components: int, No of PCA components to reduce each DataFrame to.
+                  Default is 2.
     scaleData: boolean; Should data be centered and scaled before PCA?
                Default is True.
     
     Returns
     -------
     
     Concated dataframes and two dictionaries. Each dictionary is of
```

### Comparing `catencfamily-0.0.78/LICENSE` & `catencfamily-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.78/README.md` & `catencfamily-0.0.80/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.78/pyproject.toml` & `catencfamily-0.0.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.78"
+version = "0.0.80"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.78/PKG-INFO` & `catencfamily-0.0.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.78
+Version: 0.0.80
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

