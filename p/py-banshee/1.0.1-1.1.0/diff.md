# Comparing `tmp/py_banshee-1.0.1.tar.gz` & `tmp/py_banshee-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_banshee-1.0.1.tar", last modified: Thu Nov 11 11:14:15 2021, max compression
+gzip compressed data, was "py_banshee-1.1.0.tar", last modified: Mon Jun 19 08:45:16 2023, max compression
```

## Comparing `py_banshee-1.0.1.tar` & `py_banshee-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-11-11 11:14:15.235924 py_banshee-1.0.1/
--rw-rw-rw-   0        0        0     5313 2021-11-11 11:14:15.235924 py_banshee-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2021-10-23 13:03:23.000000 py_banshee-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2021-11-11 11:14:15.218971 py_banshee-1.0.1/py_banshee/
--rw-rw-rw-   0        0        0      458 2021-10-14 10:15:59.000000 py_banshee-1.0.1/py_banshee/__init__.py
--rw-rw-rw-   0        0        0     2953 2021-10-16 17:12:36.000000 py_banshee-1.0.1/py_banshee/bn_plot.py
--rw-rw-rw-   0        0        0     9094 2021-10-16 17:45:45.000000 py_banshee-1.0.1/py_banshee/copula_test.py
--rw-rw-rw-   0        0        0    12096 2021-10-16 17:24:27.000000 py_banshee-1.0.1/py_banshee/d_cal.py
--rw-rw-rw-   0        0        0    20084 2021-11-11 10:56:10.000000 py_banshee-1.0.1/py_banshee/prediction.py
--rw-rw-rw-   0        0        0    19872 2021-11-11 09:53:01.000000 py_banshee-1.0.1/py_banshee/rankcorr.py
--rw-rw-rw-   0        0        0     3857 2021-11-11 09:38:44.000000 py_banshee-1.0.1/py_banshee/sample_bn.py
-drwxrwxrwx   0        0        0        0 2021-11-11 11:14:15.234927 py_banshee-1.0.1/py_banshee.egg-info/
--rw-rw-rw-   0        0        0     5313 2021-11-11 11:14:15.000000 py_banshee-1.0.1/py_banshee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2021-11-11 11:14:15.000000 py_banshee-1.0.1/py_banshee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-11 11:14:15.000000 py_banshee-1.0.1/py_banshee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2021-11-11 11:14:15.000000 py_banshee-1.0.1/py_banshee.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-11-11 11:14:15.000000 py_banshee-1.0.1/py_banshee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-11-11 11:14:15.236921 py_banshee-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2018 2021-11-11 11:13:23.000000 py_banshee-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:45:16.023545 py_banshee-1.1.0/
+-rw-rw-rw-   0        0        0    35809 2021-08-16 13:01:53.000000 py_banshee-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5429 2023-06-19 08:45:16.024243 py_banshee-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4415 2023-02-24 11:57:18.000000 py_banshee-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:45:16.011544 py_banshee-1.1.0/py_banshee/
+-rw-rw-rw-   0        0        0      458 2021-10-14 10:15:59.000000 py_banshee-1.1.0/py_banshee/__init__.py
+-rw-rw-rw-   0        0        0     3337 2022-10-03 10:04:16.000000 py_banshee-1.1.0/py_banshee/bn_plot.py
+-rw-rw-rw-   0        0        0    10831 2023-05-11 12:36:42.000000 py_banshee-1.1.0/py_banshee/copula_test.py
+-rw-rw-rw-   0        0        0    12381 2023-05-09 12:30:53.000000 py_banshee-1.1.0/py_banshee/d_cal.py
+-rw-rw-rw-   0        0        0    20488 2022-02-03 15:46:44.000000 py_banshee-1.1.0/py_banshee/prediction.py
+-rw-rw-rw-   0        0        0    20428 2022-02-03 15:32:03.000000 py_banshee-1.1.0/py_banshee/rankcorr.py
+-rw-rw-rw-   0        0        0     3857 2021-11-11 09:38:44.000000 py_banshee-1.1.0/py_banshee/sample_bn.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:45:16.021544 py_banshee-1.1.0/py_banshee.egg-info/
+-rw-rw-rw-   0        0        0     5429 2023-06-19 08:45:15.000000 py_banshee-1.1.0/py_banshee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-06-19 08:45:15.000000 py_banshee-1.1.0/py_banshee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:45:15.000000 py_banshee-1.1.0/py_banshee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-19 08:45:15.000000 py_banshee-1.1.0/py_banshee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 08:45:15.000000 py_banshee-1.1.0/py_banshee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 08:45:16.025470 py_banshee-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1971 2023-06-19 08:43:30.000000 py_banshee-1.1.0/setup.py
```

### Comparing `py_banshee-1.0.1/PKG-INFO` & `py_banshee-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,121 @@
 Metadata-Version: 2.1
 Name: py_banshee
-Version: 1.0.1
+Version: 1.1.0
 Summary: Py_Banshee allows for quantifying non-parametric Bayesian Networks
 Home-page: https://github.com/mike-mendoza/py_banshee
+Download-URL: https://github.com/mike-mendoza/py_banshee/archive/refs/tags/v1.1.0.tar.gz
 Author: Paul Koot, Miguel Angel Mendoza Lugo, Oswaldo Morales Napoles
 Author-email: mendozalugo@gmail.com
 License: GNU
-Download-URL: https://github.com/mike-mendoza/py_banshee/archive/refs/tags/0.1.tar.gz
 Project-URL: Bug Tracker, https://github.com/mike-mendoza/py_banshee/issues
-Description: # Py_BANSHEE
-        Bayesian Networks (BNs) are probabilistic, graphical models for representing complex dependency structures. They have many applications in science and engineering. Their particularly powerful variant – Non-Parametric BNs – are  implemented as an open-access scriptable code, in the form of a Python-based package.
-        
-        The package allows for quantifying the BN, validating the underlying assumptions of the model, visualizing the network and its corresponding rank correlation matrix, sampling and finally making inference with a BN based on existing or new evidence. 
-        
-        Py_BANSHEE  is a Python-based open source successor of the MATLAB toolbox [BANSHEE](https://doi.org/10.1016/j.softx.2020.100588). 
-        
-        ## Installation and updating
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Toolbox like below. 
-        Rerun this command to check for and install  updates .
-        ```bash
-        pip install py-banshee
-        ```
-        
-        ## Usage
-        Features:
-        * py_banshee.rankcorr.bn_rankcorr  --> Create a Bayesian Network rank correlation matrix 
-        * py_banshee.bn_plot.bn_visualize    --> Visualize the structure of a defined Bayesian Network
-        * py_banshee.copula_test.cvm_statistic      --> Goodness-of-fit test for copulas
-        * py_banshee.d_cal.gaussian_distance  --> Measure the distance between Gaussian densities
-        * py_banshee.sample_bn.generate_samples  --> Make samples using the defined Bayesian Network
-        * py_banshee.sample_bn.sample_base_conditioning --> Make samples based conditioning on intervals
-        * py_banshee.prediction.inference  --> Make predictions using a non-parametric Bayesian Network
-        * py_banshee.prediction.conditional_margins_hist  --> Visualize the un-conditional and conditional marginal histograms
-        
-        #### Demo of some of the features:
-        
-        ```python
-        from py_banshee.rankcorr import bn_rankcorr
-        from py_banshee.bn_plot import bn_visualize
-        from py_banshee.prediction import inference,conditional_margins_hist
-        
-        #Defining the variables of the BN
-        names = ['V1','V2','V3']  #names of the variables (nodes)
-        N = len(names) 		      #number of nodes
-        
-        #parametric distributions of the nodes
-        distributions = ['norm','genextreme','norm']	
-        parameters = [[100,23],[-0.15,130,50],[500,100]]
-        
-        #Defining the structure of the BN
-        ParentCell = [None]*N
-        ParentCell[0] = []
-        ParentCell[1] = [0]
-        ParentCell[2] = [0,1]
-        
-        #Defining the rank correlation matrix
-        RankCorr = [None]*N
-        RankCorr[0] = []
-        RankCorr[1] = [.1]
-        RankCorr[2] = [.41,-.25]
-        
-        #Conditional rank correlation matrix
-        R = bn_rankcorr(ParentCell,RankCorr,var_names=names,is_data=False, plot=True)
-        
-        #Plot of the Bayesian Network
-        bn_visualize(ParentCell,R,names,fig_name='BN_TEST')
-        
-        # Inference
-        condition_nodes = [0] #conditionalized variables (node V1)
-        condition_values = [181] #conditionalized value (node V1)
-        
-        F = inference(Nodes = condition_nodes,
-                      Values = condition_values,
-                      R=R,
-                      DATA=[],
-                      SampleSize=100000,
-                      empirical_data=False, 
-                      distributions=distributions,
-                      parameters=parameters,
-                      Output='full')
-        
-        #Conditional and un-conditional histograms 
-        conditional_margins_hist(F,[],names,condition_nodes,
-                                 empirical_data = False,
-                                 distributions=distributions,
-                                 parameters=parameters)
-        ```
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        ## License
-        [GNU](https://choosealicense.com/licenses/gpl-3.0/)
 Keywords: pypi,py_banshee,tutorial
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# BANSHEE
+
+Bayesian Networks (BNs) are probabilistic, graphical models for representing complex dependency structures. They have many applications in science and engineering. Their particularly powerful variant – Non-Parametric BNs – are  implemented as a Matlab toolbox and an open-access scriptable code, in the form of a Python-based package.
+
+This repository contains:
+* PyBanshee a Python-based open source of the MATLAB toolbox.
+
+These codes are an update of the original version supporting SoftwareX paper: https://doi.org/10.1016/j.softx.2020.100588. The latest version of MATLAB BANSHEE (v1.3) can be found [here](https://github.com/mike-mendoza/matlab_banshee). 
+
+The supporting SoftwareX paper for PyBanhsee, _PyBanshee version (1.0): A Python implementation of the MATLAB toolbox BANSHEE for Non-Parametric Bayesian Networks with updated features_, can be found at https://doi.org/10.1016/j.softx.2022.101279 
+
+The packages allows for quantifying the BN, validating the underlying assumptions of the model, visualizing the network and its corresponding rank correlation matrix, sampling and finally making inference with a BN based on existing or new evidence. MATLAB BANSHEE v1.3 and Py_BANSHEE have the same features.
+
+# PyBanshee
+
+PyBanshee  is a Python-based open source of the MATLAB toolbox [BANSHEE](https://doi.org/10.1016/j.softx.2020.100588). 
+
+## Installation and updating
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install last stable version of the package. 
+
+```bash
+pip install py-banshee
+```
+However, if you are looking for the latest updates, consider installation directly from sources.
+```
+git clone https://github.com/mike-mendoza/py_banshee.git
+cd py_banshee
+python setup.py install
+```
+
+## Usage
+Features:
+* py_banshee.rankcorr.bn_rankcorr  --> Create a Bayesian Network rank correlation matrix 
+* py_banshee.bn_plot.bn_visualize    --> Visualize the structure of a defined Bayesian Network
+* py_banshee.copula_test.cvm_statistic      --> Goodness-of-fit test for copulas
+* py_banshee.d_cal.gaussian_distance  --> Measure the distance between Gaussian densities
+* py_banshee.sample_bn.generate_samples  --> Make samples using the defined Bayesian Network
+* py_banshee.sample_bn.sample_base_conditioning --> Make samples based conditioning on intervals
+* py_banshee.prediction.inference  --> Make predictions using a non-parametric Bayesian Network
+* py_banshee.prediction.conditional_margins_hist  --> Visualize the un-conditional and conditional marginal histograms
+
+#### Demo of some of the features:
+
+```python
+from py_banshee.rankcorr import bn_rankcorr
+from py_banshee.bn_plot import bn_visualize
+from py_banshee.prediction import inference,conditional_margins_hist
+
+#Defining the variables of the BN
+names = ['V1','V2','V3']  #names of the variables (nodes)
+N = len(names) 		      #number of nodes
+
+#parametric distributions of the nodes
+distributions = ['norm','genextreme','norm']	
+parameters = [[100,23],[-0.15,130,50],[500,100]]
+
+#Defining the structure of the BN
+ParentCell = [None]*N
+ParentCell[0] = []
+ParentCell[1] = [0]
+ParentCell[2] = [0,1]
+
+#Defining the rank correlation matrix
+RankCorr = [None]*N
+RankCorr[0] = []
+RankCorr[1] = [.1]
+RankCorr[2] = [.41,-.25]
+
+#Conditional rank correlation matrix
+R = bn_rankcorr(ParentCell,RankCorr,var_names=names,is_data=False, plot=True)
+
+#Plot of the Bayesian Network
+bn_visualize(ParentCell,R,names,fig_name='BN_TEST')
+
+# Inference
+condition_nodes = [0] #conditionalized variables (node V1)
+condition_values = [181] #conditionalized value (node V1)
+
+F = inference(Nodes = condition_nodes,
+              Values = condition_values,
+              R=R,
+              DATA=[],
+              SampleSize=100000,
+              empirical_data=False, 
+              distributions=distributions,
+              parameters=parameters,
+              Output='full')
+
+#Conditional and un-conditional histograms 
+conditional_margins_hist(F,[],names,condition_nodes,
+                         empirical_data = False,
+                         distributions=distributions,
+                         parameters=parameters)
+```
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[GNU](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `py_banshee-1.0.1/py_banshee/bn_plot.py` & `py_banshee-1.1.0/py_banshee/bn_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,34 +50,46 @@
     """
 
     G = nx.DiGraph()
     if isinstance(data, pd.DataFrame):
         for node in data:
             plt.figure()
             h = sns.histplot(data[node], kde=True)
-            h.set_xlabel('')
+            h.set_xlabel('x')
             h.set_title('{}'.format(node), fontsize=25)
+            plt.xticks(rotation=45)
+            plt.ylabel("Count", fontsize=18)
+            plt.xlabel("x", fontsize=18)
+            plt.xticks(fontsize=14)
+            plt.yticks(fontsize=14)
+            plt.tight_layout()
             plt.savefig('histogram_{}.png'.format(node))
             G.add_node(node, image='histogram_{}.png'.format(node),
                        fontsize=0)
             plt.show()
     else:
         G.add_nodes_from(names, style='filled', fillcolor='red')
         plt.show()
-
+       
+    #edges and labels
+    edgs=[]
+    edglbs=[]
     for i in range(len(names)):
         parents = parent_cell[i]
         for j in parents:
-            G.add_edge(names[j], names[i], label=("%.2f") % R[j, i],
-                       fontsize=18)
-
-    nx.drawing.nx_pydot.write_dot(G, 'BN_visualize_{}'.format(fig_name))
+            edgs.append((names[j], names[i]))
+            edglbs.append(f'{round(R[j, i],2)}')
+    #add edges and labels         
+    for k in range(len(edgs)):
+        G.add_edges_from([edgs[k]], label = edglbs[k])
+    #dot file
+    nx.drawing.nx_pydot.write_dot(G, f'BN_visualize_{fig_name}')
     # Convert dot file to png file
-    gv.render('dot', 'png', 'BN_visualize_{}'.format(fig_name))
+    gv.render('dot', 'pdf', f'BN_visualize_{fig_name}')
+    deleteFile(f'BN_visualize_{fig_name}')
 
-    def deleteFile(filename):
-        if os.path.exists(filename) and not os.path.isdir(filename) and not os.path.islink(filename):
-            os.remove(filename)
+    return f'BN plot saved in : {os.getcwd()}\BN_visualize_{fig_name}.pdf' 
 
-    deleteFile('BN_visualize_{}'.format(fig_name))
 
-    return Image(filename='BN_visualize_{}'.format(fig_name) + '.png')
+def deleteFile(filename):
+    if os.path.exists(filename) and not os.path.isdir(filename) and not os.path.islink(filename):
+        os.remove(filename)
```

### Comparing `py_banshee-1.0.1/py_banshee/copula_test.py` & `py_banshee-1.1.0/py_banshee/copula_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,53 +64,85 @@
     M[:] = np.nan
 
     # Calculate an unconditional rank correlation matrix
     DATA2 = DATA.dropna()  # remove NaN values
     Rd = sc.stats.spearmanr(DATA2)[0]  # compute correlation
     Nk_i = 0  # initiate counter to allocate combination in M
     # Calculating the CvM statistics per each pair and copula type
+    var_nam=[]
     for i in list(indP):
         # Selecting variables for the pair
         var = DATA.iloc[:, [i[0], i[1]]]
+        var_nam.append(var.columns.tolist())
         # Storing the numbers of the variables in the pair
         M[Nk_i, 0] = i[0]
         M[Nk_i, 1] = i[1]
         # Computing rank correlation between variables
         M[Nk_i, 2] = Rd[i[0], i[1]]
         # Computing CvM statistic per pair (auxiliary function 1)
         M[Nk_i, 3] = CVM(var, 'Clayton')
         M[Nk_i, 4] = CVM(var, 'Frank')
         M[Nk_i, 5] = CVM(var, 'Gaussian')
         M[Nk_i, 6] = CVM(var, 'Gumbel')
         Nk_i += 1
+    
 
+    #dataframe 
+    M_df = pd.DataFrame(np.concatenate((var_nam,M[:,2:7]), axis=1))
+    M_df.columns = ['Var1','Var2','r', 'Clayton','Frank','Gaussian','Gumbel']
+    M_df.iloc[:,2:7]=M_df.iloc[:,2:7].astype(float)
+                     
     if plot:
         fig, ax = plt.subplots(figsize=(12, 12), sharex=False, sharey=False, ncols=N - 1, nrows=N - 1)
         x = np.arange(4)
         labels = ['Cla', 'Fra', 'Gau', 'Gum']
         colors = ['#1f77b4', '#1f77b4', '#BFE5D9', '#1f77b4']
         count = 0
-        for i in range(N - 1):
-            for j in range(N - 1):
-                if i > j:
-                    ax[i, j].axis('off')
-                else:
-                    ax[i, j].bar(x, M[count, 3:7], color=colors)
-                    ax[i, j].set_xticks(x)
-                    ax[i, j].set_xticklabels(labels, rotation=90)
-                    if i == 0:
-                        ax[i, j].set_title(names[int(M[count, 1])])
-                    if i == j:
-                        ax[i, j].set_ylabel(names[int(M[count, 0])])
-                    count += 1
+        if N<=12:
+            for i in range(N - 1):
+                for j in range(N - 1):
+                    if i > j:
+                        ax[i, j].axis('off')
+                    else:
+                        ax[i, j].bar(x, M[count, 3:7], color=colors)
+                        ax[i, j].yaxis.set_label_position("right")
+                        ax[i, j].set_xticks(x)
+                        ax[i, j].set_xticklabels(labels, rotation=90)
+                        if i == 0:
+                            ax[i, j].set_title(names[int(M[count, 1])])
+                        ax[i, N-2].set_ylabel(names[int(M[count, 0])],fontsize='large',
+                                              rotation='horizontal',ha='left',va="center")    
+                        count += 1
+                        
+        else:                
+            for i in range(N - 1):
+                for j in range(N - 1):
+                    if i > j:
+                        ax[i, j].axis('off')
+                    else:
+                        ax[i, j].bar(x, M[count, 3:7], color=colors)
+                        ax[i, j].yaxis.set_label_position("right")
+                        ax[i, j].tick_params(axis='x',bottom=False,labelbottom=False)
+                        ax[i, j].tick_params(axis='y',left=False,labelleft=False)
+                        if i == 0:
+                            ax[i, j].set_title(names[int(M[count, 1])],rotation=30)
+                            
+                        if i == j:
+                            ax[i, j].set_xticks(x)
+                            ax[i, j].set_xticklabels(labels, rotation=90)
+                            ax[i, j].tick_params(axis='x',bottom=True,labelbottom=True)
+                        ax[i, N-2].set_ylabel(names[int(M[count, 0])],fontsize='large',
+                                              rotation='horizontal',ha='left',va="center")    
+                        count += 1
+                        
+                        
+        plt.savefig('cvm_statistics_{}.pdf'.format(fig_name))
+        plt.show()
 
-        plt.tight_layout()
-        plt.savefig('cvm_statistics_{}.png'.format(fig_name))
-
-    return M
+    return M_df
 
 
 # -------------------------------------------------------------------------
 # AUXILIARY FUNCTIONS
 # -------------------------------------------------------------------------
 #
 # --------------------------------------------------------------------------
```

### Comparing `py_banshee-1.0.1/py_banshee/d_cal.py` & `py_banshee-1.1.0/py_banshee/d_cal.py`

 * *Files 13% similar despite different names*

```diff
@@ -158,43 +158,48 @@
     B_BNRC = np.quantile(D_BN, q)
 
     # Generate plot
     if Plot:
         # first subplot with the d-calibration and range for the ERC
         f, x = ecdf(pd.Series(D_NR))
 
-        fig, ax = plt.subplots(figsize=(13, 7), sharex=False, sharey=False, ncols=2, nrows=1)
+        fig, ax = plt.subplots(figsize=(12, 6), sharex=False, sharey=False, ncols=2, nrows=1)
         ax[0].step(np.array(x), np.array(f), color='k')
         ax[0].plot([D_ERC, D_ERC], [f[1], 1], 'r', linewidth=2)
         ax[0].set_ylim([f[0], f[-1]])
-        ax[0].set_xlabel('d-calibration score')
-        ax[0].set_ylabel('Cumulative density function')
+        ax[0].set_xlabel('d-calibration score',fontsize=15)
+        ax[0].set_ylabel('Cumulative density function',fontsize=15)
         ax[0].plot(B_ERC, q, 'or', markersize=6)
-        ax[0].title.set_text('d-Cal(ERC,NRC)\n' \
-                             'in the distribution of\n' \
-                             'd-Cal(NRC,NRC)\n' \
-                             '{} samples in {} iterations'.format(str(SampleSize_1), str(M)))
+        ax[0].set_title('d-Cal(ERC,NRC)\n '
+                    'in the distribution of\n '
+                    'd-Cal(NRC,NRC)\n '+
+                    str(SampleSize_1) +' samples in '+ str(M)+'iterations', fontsize=17)
         ax[0].grid(which="both", ls="--", linewidth=.5)
+        ax[0].tick_params(axis ='x', labelsize=14, labelrotation=45)
+        ax[0].tick_params(axis ='y', labelsize=14)
 
+        
         # second subplot with the d-calibration and range for the BNRC
         f1, x1 = ecdf(pd.Series(D_BN))
 
         ax[1].step(np.array(x1), np.array(f1), '-k')
-
         ax[1].plot([D_BNRC, D_BNRC], [f1[1], 1], 'r', linewidth=2)
         ax[1].set_ylim([f1[0], f1[-1]])
-        ax[1].set_xlabel('d-calibration score')
+        ax[1].set_xlabel('d-calibration score', fontsize=16)
         # ax[0,1].set_ylabel('Cumulative density function')    
         ax[1].plot(B_BNRC, q, 'or', markersize=6)
-        ax[1].title.set_text('d-Cal(NRC,BNRC)\n' \
-                             'in the distribution of\n' \
-                             'd-Cal(BNRC,BNRC)\n' \
-                             '{} samples in {} iterations'.format(str(SampleSize_2), str(M)))
+        ax[1].set_title('d-Cal(NRC,BNRC)\n '
+                    'in the distribution of\n '
+                    'd-Cal(BNRC,BNRC)\n '+
+                    str(SampleSize_2) +' samples in '+ str(M)+'iterations', fontsize=17)
         ax[1].grid(which="both", ls="--", linewidth=.5)
-        plt.savefig('gaussian_distance_{}.png'.format(fig_name))
+        ax[1].tick_params(axis ='x', labelsize=14, labelrotation=45)
+        ax[1].tick_params(axis ='y', labelsize=14)
+        plt.tight_layout()
+        plt.savefig('gaussian_distance_{}.pdf'.format(fig_name))
         plt.show()
 
     if D_ERC > B_ERC[0] and D_ERC < B_ERC[1]:
         print(
             'SUCCESS: The d-Cal of the empirical rank correlation matrix (ERC) fall between the confidence intervals of the d-Cal of the normal rank correlation matrix (NRC)\n')
     else:
         print(
@@ -249,20 +254,21 @@
     if Type == 'H':
         # Hellinger distance
         # elements of the distance equation
         a = (np.linalg.det(Sigma1) ** (1 / 4) * np.linalg.det(Sigma2) ** (1 / 4)) / \
             np.linalg.det((1 / 2) * Sigma1 + (1 / 2) * Sigma2) ** (1 / 2)
         b = np.exp(-(1 / 8) * (m1 - m2).reshape(1, -1) @ np.linalg.inv((1 / 2) * Sigma1 + (1 / 2) * Sigma2) @ (m1 - m2))
         # equation proper
-        D = (1 - (a * b)) ** (1 / 2)
+        D = (1 - (np.mul(a,b))) ** (1 / 2)
     elif Type == 'KL':
         # Symmetric Kullback–Leibler divergence
         D = (1 / 2) * (m1 - m2).reshape(1, -1) @ (np.linalg.inv(Sigma1) + np.linalg.inv(Sigma2)) @ (m1 - m2) + \
-            (1 / 2) * np.trace(np.linalg.inv(Sigma1) * Sigma2 + \
-                               Sigma1 * np.linalg.inv(Sigma2) - 2 * np.identity(Sigma1.shape[0]))
+            (1 / 2) * np.trace(np.matmul(np.linalg.inv(Sigma1), Sigma2) + \
+                               np.matmul(Sigma1, np.linalg.inv(Sigma2)) - 2 * np.identity(Sigma1.shape[0]))
+
     elif Type == 'B':
         # Bhattacharyya distance
         D = (1 / 8) * (m1 - m2).reshape(1, -1) @ np.linalg.inv((1 / 2) * Sigma1 + (1 / 2) * Sigma2) @ (m1 - m2) + \
             (1 / 2) * np.log((np.linalg.det((1 / 2) * Sigma1 + (1 / 2) * Sigma2)) / \
                              ((np.linalg.det(Sigma1)) ** (1 / 2) * (np.linalg.det(Sigma2)) ** (1 / 2)))
     elif Type == 'G':
         # G distance (Abou Moustafa et al. 2010)
```

### Comparing `py_banshee-1.0.1/py_banshee/prediction.py` & `py_banshee-1.1.0/py_banshee/prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -425,47 +425,54 @@
 
     if empirical_data:
         try:
             F_uncond = DATA.iloc[:, remaining_nodes].to_numpy()
             F_cond = np.array(F[0]).transpose()
             for i in range(nr_remaining_nodes):
                 F_cond[:, i]
-                plt.figure()
-                plt.hist(F_uncond[:, i], bins=20, edgecolor="black", color='silver',
+                plt.figure(figsize=(7,4))
+                plt.hist(F_uncond[:, i], bins=20, edgecolor="silver", color='silver',
                          label=['un-conditionalized\n mean: ' + str(round(np.mean(F_uncond[:, i]), 1))])
-                plt.hist(F_cond[:, i], bins=20, alpha=0.7, edgecolor="black", color='cornflowerblue',
+                plt.hist(F_cond[:, i], bins=20, edgecolor="cornflowerblue", color='cornflowerblue',
                          label=['conditionalized\n mean: ' + str(round(np.mean(F_cond[:, i]), 1))])
-                plt.legend()
-                plt.ylabel("Count")
-                plt.title(names[remaining_nodes[i]], fontsize=15)
-                plt.savefig(names[remaining_nodes[i]] + '_uncond_cond.png')
+                plt.legend(fontsize=18)
+                plt.ylabel("Count", fontsize=18 )
+                plt.xlabel("x", fontsize=18)
+                plt.title(names[remaining_nodes[i]], fontsize=20, fontweight=550)
+                plt.xticks(fontsize=18)
+                plt.yticks(fontsize=18)
+                plt.tight_layout()
+                plt.savefig(names[remaining_nodes[i]] + '_uncond_cond.pdf')
                 plt.show()
                 
-                    
-                
+        
         except:
             raise Exception('Check if argument Output in inference is equal to full')
     else:
         try:
             # Random unconditional samples of the parametric nodes
             dists, params = make_dist(distributions, parameters)
             random_values = [dists[i].rvs(*params[i], F[0].shape[1]) for i in range(len(dists))]
             random_values = pd.DataFrame(np.array(random_values).transpose(), columns=names)
 
             F_uncond = random_values.iloc[:, remaining_nodes].to_numpy()
             F_cond = np.array(F[0]).transpose()
             for i in range(nr_remaining_nodes):
                 F_cond[:, i]
-                plt.figure()
+                plt.figure(figsize=(7, 4))
                 plt.hist(F_uncond[:, i], bins=20, edgecolor='silver', color='silver',
                          label=['un-conditionalized\n mean: ' + str(round(np.mean(F_uncond[:, i]), 1))])
-                plt.hist(F_cond[:, i], bins=20, alpha=0.7, edgecolor="black", color='cornflowerblue',
+                plt.hist(F_cond[:, i], bins=20, edgecolor="cornflowerblue", color='cornflowerblue',
                          label=['conditionalized\n mean: ' + str(round(np.mean(F_cond[:, i]), 1))])
-                plt.legend()
-                plt.ylabel("Count")
-                plt.title(names[remaining_nodes[i]], fontsize=15)
-                plt.savefig(names[remaining_nodes[i]] + '_uncond_cond.png')
+                plt.legend(fontsize=18)
+                plt.ylabel("Count", fontsize=18 )
+                plt.xlabel("x", fontsize=18)
+                plt.title(names[remaining_nodes[i]], fontsize=20, fontweight=550)
+                plt.xticks(fontsize=18)
+                plt.yticks(fontsize=18)
+                plt.tight_layout()
+                plt.savefig(names[remaining_nodes[i]] + '_uncond_cond.pdf')
                 plt.show()
 				
         except:
             raise Exception('Check if argument Output in inference is equal to full')
     return None
```

### Comparing `py_banshee-1.0.1/py_banshee/rankcorr.py` & `py_banshee-1.1.0/py_banshee/rankcorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,37 +529,48 @@
     elif len(nam) <= 40 and len(nam) > 20:
         nv = int(round(len(nam) / 21, 0))
     elif len(nam) <= 20:
         nv = len(nam)
 
     px = list(range(len(nam)))  # position of the labels
 
-    fig, ax = plt.subplots(figsize=(15, 11))
+    fig, ax = plt.subplots(figsize=(11, 8))
     im = plt.imshow(z, cmap='Blues', interpolation='nearest')
-    plt.colorbar()
+    cbar = plt.colorbar()  #color bar options 
+    for t in cbar.ax.get_yticklabels():
+         t.set_fontsize(14)
+         t.set_fontweight('semibold')
 
     if len(nam) <= 20:
         plt.xticks(px, nam, rotation=45)
         plt.yticks(px, nam)
     else:  # plot the only the reduces names so the plot doesnt look saturated
         plt.xticks(px[::nv], nam[::nv], rotation=45)
         plt.yticks(px[::nv], nam[::nv])
-    plt.setp(ax.get_xticklabels(), fontsize=14)
-    plt.setp(ax.get_yticklabels(), fontsize=14)
+        
+    font_weight = 550  #a numeric value in range 0-1000 
+    plt.setp(ax.get_xticklabels(), fontsize=16,fontweight=font_weight)
+    plt.setp(ax.get_yticklabels(), fontsize=16,fontweight=font_weight)
 
     if len(nam) <= 10:
         zz = np.round(RBN, 4)
         zz = zz.astype(str)
         for i in range(len(nam)):
             for j in range(len(nam)):
                 if zz[i, j] == '0.0':
                     zz[i, j] = ''
-                text = ax.text(j, i, zz[i, j],
+                if zz[i,j] == '1.0':
+                    text = ax.text(j, i, zz[i, j],
                                ha="center", va="center",
-                               color="k", fontsize='xx-large', fontweight='roman')
+                               color="white", fontsize=18, fontweight=font_weight)
+                else:    
+                    text = ax.text(j, i, zz[i, j],
+                               ha="center", va="center",
+                               color="#1E1E1E", fontsize=18, fontweight=font_weight)
+    plt.savefig('rank_corr_matrix.pdf')
     plt.show()
 
     return None
 
 
 # ----------------------------------------------------------------------------
 # 9 - Subtract two lists
```

### Comparing `py_banshee-1.0.1/py_banshee/sample_bn.py` & `py_banshee-1.1.0/py_banshee/sample_bn.py`

 * *Files identical despite different names*

### Comparing `py_banshee-1.0.1/py_banshee.egg-info/PKG-INFO` & `py_banshee-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,99 @@
-Metadata-Version: 2.1
-Name: py-banshee
-Version: 1.0.1
-Summary: Py_Banshee allows for quantifying non-parametric Bayesian Networks
-Home-page: https://github.com/mike-mendoza/py_banshee
-Author: Paul Koot, Miguel Angel Mendoza Lugo, Oswaldo Morales Napoles
-Author-email: mendozalugo@gmail.com
-License: GNU
-Download-URL: https://github.com/mike-mendoza/py_banshee/archive/refs/tags/0.1.tar.gz
-Project-URL: Bug Tracker, https://github.com/mike-mendoza/py_banshee/issues
-Description: # Py_BANSHEE
-        Bayesian Networks (BNs) are probabilistic, graphical models for representing complex dependency structures. They have many applications in science and engineering. Their particularly powerful variant – Non-Parametric BNs – are  implemented as an open-access scriptable code, in the form of a Python-based package.
-        
-        The package allows for quantifying the BN, validating the underlying assumptions of the model, visualizing the network and its corresponding rank correlation matrix, sampling and finally making inference with a BN based on existing or new evidence. 
-        
-        Py_BANSHEE  is a Python-based open source successor of the MATLAB toolbox [BANSHEE](https://doi.org/10.1016/j.softx.2020.100588). 
-        
-        ## Installation and updating
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Toolbox like below. 
-        Rerun this command to check for and install  updates .
-        ```bash
-        pip install py-banshee
-        ```
-        
-        ## Usage
-        Features:
-        * py_banshee.rankcorr.bn_rankcorr  --> Create a Bayesian Network rank correlation matrix 
-        * py_banshee.bn_plot.bn_visualize    --> Visualize the structure of a defined Bayesian Network
-        * py_banshee.copula_test.cvm_statistic      --> Goodness-of-fit test for copulas
-        * py_banshee.d_cal.gaussian_distance  --> Measure the distance between Gaussian densities
-        * py_banshee.sample_bn.generate_samples  --> Make samples using the defined Bayesian Network
-        * py_banshee.sample_bn.sample_base_conditioning --> Make samples based conditioning on intervals
-        * py_banshee.prediction.inference  --> Make predictions using a non-parametric Bayesian Network
-        * py_banshee.prediction.conditional_margins_hist  --> Visualize the un-conditional and conditional marginal histograms
-        
-        #### Demo of some of the features:
-        
-        ```python
-        from py_banshee.rankcorr import bn_rankcorr
-        from py_banshee.bn_plot import bn_visualize
-        from py_banshee.prediction import inference,conditional_margins_hist
-        
-        #Defining the variables of the BN
-        names = ['V1','V2','V3']  #names of the variables (nodes)
-        N = len(names) 		      #number of nodes
-        
-        #parametric distributions of the nodes
-        distributions = ['norm','genextreme','norm']	
-        parameters = [[100,23],[-0.15,130,50],[500,100]]
-        
-        #Defining the structure of the BN
-        ParentCell = [None]*N
-        ParentCell[0] = []
-        ParentCell[1] = [0]
-        ParentCell[2] = [0,1]
-        
-        #Defining the rank correlation matrix
-        RankCorr = [None]*N
-        RankCorr[0] = []
-        RankCorr[1] = [.1]
-        RankCorr[2] = [.41,-.25]
-        
-        #Conditional rank correlation matrix
-        R = bn_rankcorr(ParentCell,RankCorr,var_names=names,is_data=False, plot=True)
-        
-        #Plot of the Bayesian Network
-        bn_visualize(ParentCell,R,names,fig_name='BN_TEST')
-        
-        # Inference
-        condition_nodes = [0] #conditionalized variables (node V1)
-        condition_values = [181] #conditionalized value (node V1)
-        
-        F = inference(Nodes = condition_nodes,
-                      Values = condition_values,
-                      R=R,
-                      DATA=[],
-                      SampleSize=100000,
-                      empirical_data=False, 
-                      distributions=distributions,
-                      parameters=parameters,
-                      Output='full')
-        
-        #Conditional and un-conditional histograms 
-        conditional_margins_hist(F,[],names,condition_nodes,
-                                 empirical_data = False,
-                                 distributions=distributions,
-                                 parameters=parameters)
-        ```
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        ## License
-        [GNU](https://choosealicense.com/licenses/gpl-3.0/)
-Keywords: pypi,py_banshee,tutorial
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Documentation
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+# BANSHEE
+
+Bayesian Networks (BNs) are probabilistic, graphical models for representing complex dependency structures. They have many applications in science and engineering. Their particularly powerful variant – Non-Parametric BNs – are  implemented as a Matlab toolbox and an open-access scriptable code, in the form of a Python-based package.
+
+This repository contains:
+* PyBanshee a Python-based open source of the MATLAB toolbox.
+
+These codes are an update of the original version supporting SoftwareX paper: https://doi.org/10.1016/j.softx.2020.100588. The latest version of MATLAB BANSHEE (v1.3) can be found [here](https://github.com/mike-mendoza/matlab_banshee). 
+
+The supporting SoftwareX paper for PyBanhsee, _PyBanshee version (1.0): A Python implementation of the MATLAB toolbox BANSHEE for Non-Parametric Bayesian Networks with updated features_, can be found at https://doi.org/10.1016/j.softx.2022.101279 
+
+The packages allows for quantifying the BN, validating the underlying assumptions of the model, visualizing the network and its corresponding rank correlation matrix, sampling and finally making inference with a BN based on existing or new evidence. MATLAB BANSHEE v1.3 and Py_BANSHEE have the same features.
+
+# PyBanshee
+
+PyBanshee  is a Python-based open source of the MATLAB toolbox [BANSHEE](https://doi.org/10.1016/j.softx.2020.100588). 
+
+## Installation and updating
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install last stable version of the package. 
+
+```bash
+pip install py-banshee
+```
+However, if you are looking for the latest updates, consider installation directly from sources.
+```
+git clone https://github.com/mike-mendoza/py_banshee.git
+cd py_banshee
+python setup.py install
+```
+
+## Usage
+Features:
+* py_banshee.rankcorr.bn_rankcorr  --> Create a Bayesian Network rank correlation matrix 
+* py_banshee.bn_plot.bn_visualize    --> Visualize the structure of a defined Bayesian Network
+* py_banshee.copula_test.cvm_statistic      --> Goodness-of-fit test for copulas
+* py_banshee.d_cal.gaussian_distance  --> Measure the distance between Gaussian densities
+* py_banshee.sample_bn.generate_samples  --> Make samples using the defined Bayesian Network
+* py_banshee.sample_bn.sample_base_conditioning --> Make samples based conditioning on intervals
+* py_banshee.prediction.inference  --> Make predictions using a non-parametric Bayesian Network
+* py_banshee.prediction.conditional_margins_hist  --> Visualize the un-conditional and conditional marginal histograms
+
+#### Demo of some of the features:
+
+```python
+from py_banshee.rankcorr import bn_rankcorr
+from py_banshee.bn_plot import bn_visualize
+from py_banshee.prediction import inference,conditional_margins_hist
+
+#Defining the variables of the BN
+names = ['V1','V2','V3']  #names of the variables (nodes)
+N = len(names) 		      #number of nodes
+
+#parametric distributions of the nodes
+distributions = ['norm','genextreme','norm']	
+parameters = [[100,23],[-0.15,130,50],[500,100]]
+
+#Defining the structure of the BN
+ParentCell = [None]*N
+ParentCell[0] = []
+ParentCell[1] = [0]
+ParentCell[2] = [0,1]
+
+#Defining the rank correlation matrix
+RankCorr = [None]*N
+RankCorr[0] = []
+RankCorr[1] = [.1]
+RankCorr[2] = [.41,-.25]
+
+#Conditional rank correlation matrix
+R = bn_rankcorr(ParentCell,RankCorr,var_names=names,is_data=False, plot=True)
+
+#Plot of the Bayesian Network
+bn_visualize(ParentCell,R,names,fig_name='BN_TEST')
+
+# Inference
+condition_nodes = [0] #conditionalized variables (node V1)
+condition_values = [181] #conditionalized value (node V1)
+
+F = inference(Nodes = condition_nodes,
+              Values = condition_values,
+              R=R,
+              DATA=[],
+              SampleSize=100000,
+              empirical_data=False, 
+              distributions=distributions,
+              parameters=parameters,
+              Output='full')
+
+#Conditional and un-conditional histograms 
+conditional_margins_hist(F,[],names,condition_nodes,
+                         empirical_data = False,
+                         distributions=distributions,
+                         parameters=parameters)
+```
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[GNU](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `py_banshee-1.0.1/setup.py` & `py_banshee-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='py_banshee',                           # should match the package folder
     packages=['py_banshee'],                   # should match the package folder
-    version='1.0.1',                              # important for updates
+    version='1.1.0',                              # important for updates
     license='GNU',                                  # should match your chosen license
     description='Py_Banshee allows for quantifying non-parametric Bayesian Networks',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Paul Koot, Miguel Angel Mendoza Lugo, Oswaldo Morales Napoles',
     author_email='mendozalugo@gmail.com',
     url='https://github.com/mike-mendoza/py_banshee', 
@@ -25,12 +25,11 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
     ],
     
-    download_url="https://github.com/mike-mendoza/py_banshee/archive/refs/tags/0.1.tar.gz",
+    download_url="https://github.com/mike-mendoza/py_banshee/archive/refs/tags/v1.1.0.tar.gz",
 )
```

