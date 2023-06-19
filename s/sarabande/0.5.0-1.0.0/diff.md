# Comparing `tmp/sarabande-0.5.0.tar.gz` & `tmp/sarabande-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarabande-0.5.0.tar", last modified: Tue Apr  4 14:32:58 2023, max compression
+gzip compressed data, was "sarabande-1.0.0.tar", last modified: Mon Jun 19 01:13:40 2023, max compression
```

## Comparing `sarabande-0.5.0.tar` & `sarabande-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.527683 sarabande-0.5.0/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2023-04-03 19:32:46.000000 sarabande-0.5.0/LICENSE
--rw-r--r--   0 jamessunseri   (501) staff       (20)      106 2023-04-03 19:32:46.000000 sarabande-0.5.0/MANIFEST.in
--rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-04 14:32:58.527764 sarabande-0.5.0/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)     4389 2023-04-03 19:32:46.000000 sarabande-0.5.0/README.md
--rw-r--r--   0 jamessunseri   (501) staff       (20)      116 2023-04-03 19:32:46.000000 sarabande-0.5.0/pyproject.toml
--rw-r--r--   0 jamessunseri   (501) staff       (20)       12 2023-04-03 19:32:46.000000 sarabande-0.5.0/requirements.txt
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.526744 sarabande-0.5.0/sarabande/
--rw-r--r--   0 jamessunseri   (501) staff       (20)  2300096 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/CG_Coeffs.npy
--rw-r--r--   0 jamessunseri   (501) staff       (20)      151 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/__init__.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     3080 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/boot_up.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    22357 2023-04-04 14:30:55.000000 sarabande-0.5.0/sarabande/calc_PCF.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     8432 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/main.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    17256 2023-04-03 19:32:46.000000 sarabande-0.5.0/sarabande/utils.py
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2023-04-04 14:32:58.527565 sarabande-0.5.0/sarabande.egg-info/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     5581 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)      338 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/SOURCES.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/dependency_links.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       10 2023-04-04 14:32:58.000000 sarabande-0.5.0/sarabande.egg-info/top_level.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2023-04-04 14:32:58.527996 sarabande-0.5.0/setup.cfg
--rw-r--r--   0 jamessunseri   (501) staff       (20)     2219 2023-04-04 14:32:07.000000 sarabande-0.5.0/setup.py
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.871656 sarabande-1.0.0/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     1070 2023-06-17 09:16:47.000000 sarabande-1.0.0/LICENSE
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      106 2023-06-17 09:16:47.000000 sarabande-1.0.0/MANIFEST.in
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     5690 2023-06-19 01:13:40.871656 sarabande-1.0.0/PKG-INFO
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     4498 2023-06-19 01:00:32.000000 sarabande-1.0.0/README.md
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      116 2023-06-17 09:16:48.000000 sarabande-1.0.0/pyproject.toml
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       12 2023-06-17 09:16:48.000000 sarabande-1.0.0/requirements.txt
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.868656 sarabande-1.0.0/sarabande/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)  2300096 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/CG_Coeffs.npy
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      151 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/__init__.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     3080 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/boot_up.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    22727 2023-06-19 00:58:19.000000 sarabande-1.0.0/sarabande/calc_PCF.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     8432 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/main.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-18 14:41:44.000000 sarabande-1.0.0/sarabande/untitled.py
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)    17256 2023-06-17 09:16:48.000000 sarabande-1.0.0/sarabande/utils.py
+drwxr-xr-x   0 x-jsunseri (7940660) x-ast140041 (7025636)        0 2023-06-19 01:13:40.870656 sarabande-1.0.0/sarabande.egg-info/
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     5690 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/PKG-INFO
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)      360 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/SOURCES.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)        1 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/dependency_links.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       10 2023-06-19 01:13:40.000000 sarabande-1.0.0/sarabande.egg-info/top_level.txt
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)       98 2023-06-19 01:13:40.872656 sarabande-1.0.0/setup.cfg
+-rw-r--r--   0 x-jsunseri (7940660) x-ast140041 (7025636)     2219 2023-06-19 01:00:35.000000 sarabande-1.0.0/setup.py
```

### Comparing `sarabande-0.5.0/LICENSE` & `sarabande-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sarabande-0.5.0/PKG-INFO` & `sarabande-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 0.5.0
+Version: 1.0.0
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
@@ -79,14 +79,16 @@
 * `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
 * `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
 * `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
 * `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
 
 We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
 
+We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
+
 For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
 
  ## Workflow:    
 The map of SARABANDE is as follows:
 
 <p align="center">
   <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
```

### Comparing `sarabande-0.5.0/README.md` & `sarabande-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 * `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
 * `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
 * `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
 * `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
 
 We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
 
+We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
+
 For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
 
  ## Workflow:    
 The map of SARABANDE is as follows:
 
 <p align="center">
   <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
```

### Comparing `sarabande-0.5.0/sarabande/CG_Coeffs.npy` & `sarabande-1.0.0/sarabande/CG_Coeffs.npy`

 * *Files identical despite different names*

### Comparing `sarabande-0.5.0/sarabande/boot_up.py` & `sarabande-1.0.0/sarabande/boot_up.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.5.0/sarabande/calc_PCF.py` & `sarabande-1.0.0/sarabande/calc_PCF.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,22 +300,24 @@
                 a_lmb_3 = np.load(measure_obj.save_dir + measure_obj.save_name+'conv_data_kernel_'+measure_obj.kernel_name+'_'+str(l_3)+
                                                         '_'+str(m_3)+'_bin_'+str(b_3)+'.npy').astype(np.complex128)
 
 
                 
 
                 if calc_disconnected == True:
-                    disconnected_piece = 2 * S(m_3) * coupling_phase * (np.sum(measure_obj.density_field_data * a_lmb_1) * np.sum(a_lmb_2 * a_lmb_3)
-                                                                      + np.sum(measure_obj.density_field_data * a_lmb_2) * np.sum(a_lmb_3 * a_lmb_1) 
-                                                                      + np.sum(measure_obj.density_field_data * a_lmb_3) * np.sum(a_lmb_1 * a_lmb_2))
+                    disconnected_piece = 2 * S(m_3) * coupling_phase * (np.sum(measure_obj.density_field_data * a_lmb_1.conjugate()) * np.sum(a_lmb_2.conjugate() * a_lmb_3.conjugate())
+                                                                      + np.sum(measure_obj.density_field_data * a_lmb_2.conjugate()) * np.sum(a_lmb_3.conjugate() * a_lmb_1.conjugate()) 
+                                                                      + np.sum(measure_obj.density_field_data * a_lmb_3.conjugate()) * np.sum(a_lmb_1.conjugate() * a_lmb_2.conjugate()))
                 else:
                     disconnected_piece = 0
+                    
 
                 if calc_odd_modes == True and (l1 + l2 + l3)%2 != 0:
-                    full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * (a_lmb_1 * a_lmb_2 * a_lmb_3))
+                    full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * np.imag(a_lmb_1 * a_lmb_2 * a_lmb_3))
+                    disconnected_piece = np.imag(disconnected_piece)
                 else:
                     full_piece = 2 * S(m_3) * coupling_phase * np.sum(measure_obj.density_field_data * np.real(a_lmb_1 * a_lmb_2 * a_lmb_3))
                     disconnected_piece = np.real(disconnected_piece)
                                                 
 
                 
                 return [[l_1, l_2, l_3, b_1, b_2, b_3], full_piece, disconnected_piece]
@@ -370,34 +372,37 @@
 
             #----------------
             # Symmetrization
             #----------------
             for l1 in range(0,ell_max+1):
                 for l2 in range(0,ell_max+1):
                     for l3 in range(np.abs(l1 - l2), min(l1 + l2, ell_max)+1):
-                        if (l1 + l2 + l3)%2 != 0: # we don't assume this to be true for Turbulent ISM
+                        if (l1 + l2 + l3)%2 != 0 and calc_odd_modes==False: # we don't assume this to be true for Turbulent ISM
                             continue
                         for b1 in range(0,nbins):
                             for b2 in range(b1+diag,nbins):
                                 for b3 in range(b2+diag,nbins):
                                     this_4pcf = zeta[l1,l2,l3,b1,b2,b3]
                                     zeta[l3,l1,l2,b3,b1,b2] = this_4pcf
                                     zeta[l2,l3,l1,b2,b3,b1] = this_4pcf
                                     zeta[l1,l3,l2,b1,b3,b2] = this_4pcf
                                     zeta[l2,l1,l3,b2,b1,b3] = this_4pcf
                                     zeta[l3,l2,l1,b3,b2,b1] = this_4pcf
 
                                     if calc_disconnected == True:
-                                        this_4pcf_disconnected = zeta_disconnected[l1,l2,l3,b1,b2,b3]
+                                        this_4pcf_disconnected = zeta_disconnected[l1,l2,l3,b1,b2,b3] 
                                         zeta_disconnected[l3,l1,l2,b3,b1,b2] = this_4pcf_disconnected
                                         zeta_disconnected[l2,l3,l1,b2,b3,b1] = this_4pcf_disconnected
                                         zeta_disconnected[l1,l3,l2,b1,b3,b2] = this_4pcf_disconnected
                                         zeta_disconnected[l2,l1,l3,b2,b1,b3] = this_4pcf_disconnected
                                         zeta_disconnected[l3,l2,l1,b3,b2,b1] = this_4pcf_disconnected
 
+            # additional factor of Nmesh^3 because of the products of two 2PCFs
+            zeta_disconnected /= measure_obj.ld_one_d**3
+
 
 
             #---------------
             # Normalization
             #---------------
             if measure_obj.normalize:  
                 binvolume = measure_obj.boundsandnumber[1,0:nbins]
```

### Comparing `sarabande-0.5.0/sarabande/main.py` & `sarabande-1.0.0/sarabande/main.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.5.0/sarabande/utils.py` & `sarabande-1.0.0/sarabande/utils.py`

 * *Files identical despite different names*

### Comparing `sarabande-0.5.0/sarabande.egg-info/PKG-INFO` & `sarabande-1.0.0/sarabande.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarabande
-Version: 0.5.0
+Version: 1.0.0
 Summary: Tool for measuring 3/4 PCFs on discrete periodic data.
 Home-page: https://github.com/James11222/sarabande/
 Author: James Sunseri
 Author-email: jamessunseri@berkeley.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/sarabande/issues
 Project-URL: Funding, https://donate.pypi.org
@@ -79,14 +79,16 @@
 * `rmin` ([`float`]): minimum calculation distance (determins `bin_min`)
 * `rmax` ([`float`]): maximum calculation distance (determins `bin_max`)
 * `normalize` ([`bool`]): A boolean flag to normalize the 3/4 PCFs. Defaults to True. Can't use normalize without giving a `physical_boxsize`, `rmin`, and `rmax` first.
 * `particles_on_grid` ([`bool`]): An optional boolean flag to modify the normalization scheme slightly. This is recommended if you are working with particles on the grid mesh where a given cell corresponds to a particle. 
 
 We note that the `calc_zeta` method has an optional boolean argument `verbose_flag` which can be turned on and off depending on if the user wants to see the steps of the code printed. We also add an optional boolean argument `parallelized` which can be turned on and off if the user wishes to compute the Full 4PCF serially. This is added due to the instability of `concurrent.futures` and parallel processing in python across different machines. 
 
+We also provide an implementation of the connected 4PCF, this will be further documented in a future paper.
+
 For an example, please visit the demo notebook in the analysis notebooks folder: `notebooks/Application_Example.ipynb`
 
  ## Workflow:    
 The map of SARABANDE is as follows:
 
 <p align="center">
   <img src="notebooks/paper_figures/workflow_dm.png#gh-dark-mode-only" width="100%">
```

### Comparing `sarabande-0.5.0/setup.py` & `sarabande-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='sarabande',  # Required
-    version='0.5.0',  # Required
+    version='1.0.0',  # Required
     description='Tool for measuring 3/4 PCFs on discrete periodic data.',  # Optional
     long_description=(here / 'README.md').read_text(encoding='utf-8'),  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/James11222/sarabande/',  # Optional
 
     author='James Sunseri',  # Optional
```

