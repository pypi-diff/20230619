# Comparing `tmp/gmm_mi-0.7.0.tar.gz` & `tmp/gmm_mi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmm_mi-0.7.0.tar", last modified: Mon Jun  5 18:05:58 2023, max compression
+gzip compressed data, was "gmm_mi-0.7.1.tar", last modified: Mon Jun 19 13:21:42 2023, max compression
```

## Comparing `gmm_mi-0.7.0.tar` & `gmm_mi-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.167538 gmm_mi-0.7.0/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.7.0/LICENSE.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.7.0/LICENSE_EXT.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-05 18:05:58.165537 gmm_mi-0.7.0/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-30 14:51:38.000000 gmm_mi-0.7.0/README.md
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.061537 gmm_mi-0.7.0/gmm_mi/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.7.0/gmm_mi/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.7.0/gmm_mi/cross_validation.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.092537 gmm_mi-0.7.0/gmm_mi/data/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.7.0/gmm_mi/data/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.7.0/gmm_mi/data/synthetic_data.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    25656 2023-05-30 18:01:00.000000 gmm_mi-0.7.0/gmm_mi/gmm.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.7.0/gmm_mi/initializations.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45449 2023-05-30 15:21:34.000000 gmm_mi-0.7.0/gmm_mi/mi.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.7.0/gmm_mi/param_holders.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.7.0/gmm_mi/single_fit.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.150537 gmm_mi-0.7.0/gmm_mi/utils/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.7.0/gmm_mi/utils/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.7.0/gmm_mi/utils/analytic_MI.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.7.0/gmm_mi/utils/plotting.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.7.0/gmm_mi/utils/transformations.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.081537 gmm_mi-0.7.0/gmm_mi.egg-info/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/requires.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-06-05 18:05:57.000000 gmm_mi-0.7.0/gmm_mi.egg-info/top_level.txt
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-05 18:05:58.162537 gmm_mi-0.7.0/notebooks/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.7.0/notebooks/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-06-05 18:05:58.168537 gmm_mi-0.7.0/setup.cfg
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-06-04 15:25:40.000000 gmm_mi-0.7.0/setup.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.211077 gmm_mi-0.7.1/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.7.1/LICENSE.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.7.1/LICENSE_EXT.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-19 13:21:42.210077 gmm_mi-0.7.1/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-30 14:51:38.000000 gmm_mi-0.7.1/README.md
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.171077 gmm_mi-0.7.1/gmm_mi/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.7.1/gmm_mi/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.7.1/gmm_mi/cross_validation.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.190077 gmm_mi-0.7.1/gmm_mi/data/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.7.1/gmm_mi/data/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.7.1/gmm_mi/data/synthetic_data.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    25656 2023-06-08 14:41:11.000000 gmm_mi-0.7.1/gmm_mi/gmm.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.7.1/gmm_mi/initializations.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45647 2023-06-19 12:54:39.000000 gmm_mi-0.7.1/gmm_mi/mi.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.7.1/gmm_mi/param_holders.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.7.1/gmm_mi/single_fit.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.204077 gmm_mi-0.7.1/gmm_mi/utils/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.7.1/gmm_mi/utils/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.7.1/gmm_mi/utils/analytic_MI.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.7.1/gmm_mi/utils/plotting.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.7.1/gmm_mi/utils/transformations.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.185077 gmm_mi-0.7.1/gmm_mi.egg-info/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/requires.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/top_level.txt
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.208077 gmm_mi-0.7.1/notebooks/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.7.1/notebooks/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-06-19 13:21:42.212077 gmm_mi-0.7.1/setup.cfg
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-06-19 12:55:12.000000 gmm_mi-0.7.1/setup.py
```

### Comparing `gmm_mi-0.7.0/LICENSE.txt` & `gmm_mi-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/LICENSE_EXT.txt` & `gmm_mi-0.7.1/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/PKG-INFO` & `gmm_mi-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm_mi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.7.0/README.md` & `gmm_mi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/cross_validation.py` & `gmm_mi-0.7.1/gmm_mi/cross_validation.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/data/synthetic_data.py` & `gmm_mi-0.7.1/gmm_mi/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/gmm.py` & `gmm_mi-0.7.1/gmm_mi/gmm.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/initializations.py` & `gmm_mi-0.7.1/gmm_mi/initializations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/mi.py` & `gmm_mi-0.7.1/gmm_mi/mi.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,22 +598,24 @@
         See the respective methods for all information.
         """ 
         self.fit(X=X, Y=Y, verbose=verbose)
         MI_mean, MI_std = self.estimate(mi_dist_params=mi_dist_params, include_kl=include_kl, 
                                        kl_order=kl_order, base=base, verbose=verbose)
         return MI_mean, MI_std            
                     
-    def plot_fitted_model(self, ax=None, **kwargs):
+    def plot_fitted_model(self, ax=None, return_gmm=False, **kwargs):
         """Fit model to inout data and plot its contours.
         Only works if the model has been fitted successfully first.
         
         Parameters
         ----------
         ax : instance of the axes.Axes class from pyplot, default=None
             The panel where to plot the samples. 
+        return_gmm : bool
+            Whether or not to return also a GMM class instance with the fitted model
         kwargs : dictionary
             The extra keyword arguments to pass to the plotting function.
         
         Returns
         -------
         fig: instance of the figure.Figure class from pyplot
             The output figure.
@@ -627,15 +629,18 @@
                                 )
             
         from gmm_mi.utils.plotting import plot_gmm_contours
         gmm = single_fit(X=self.X, n_components=self.best_components, reg_covar=self.reg_covar, 
                  threshold_fit=self.threshold_fit, random_state=self.best_seed, max_iter=self.max_iter, 
                  w_init=self.w_init, m_init=self.m_init, p_init=self.p_init)
         ax = plot_gmm_contours(gmm, ax=ax, label='Fitted model', **kwargs)
-        return ax
+        if return_gmm:
+            return ax, gmm
+        else:
+            return ax
                
     def _calculate_MI_categorical(self):
         """Calculate mutual information (MI) integral given a Gaussian mixture model in 2D.
         Use only Monte Carlo (MC) method. 
         The complete formula can be found in Appendix B of Piras et al. (2022).
 
         Returns
@@ -847,8 +852,8 @@
         
     def fit_estimate_categorical(self, X, Y, mi_dist_params=None, base=np.exp(1), verbose=False):
         """Combine the `fit_categorical` and `estimate_categorical` methods for easier calculation of MI. 
         See the respective methods for all information.
         """ 
         self.fit_categorical(X=X, Y=Y, verbose=verbose)
         MI_mean, MI_std = self.estimate_categorical(mi_dist_params=mi_dist_params, base=base, verbose=verbose)
-        return MI_mean, MI_std  
+        return MI_mean, MI_std
```

### Comparing `gmm_mi-0.7.0/gmm_mi/param_holders.py` & `gmm_mi-0.7.1/gmm_mi/param_holders.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/single_fit.py` & `gmm_mi-0.7.1/gmm_mi/single_fit.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/utils/analytic_MI.py` & `gmm_mi-0.7.1/gmm_mi/utils/analytic_MI.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/utils/plotting.py` & `gmm_mi-0.7.1/gmm_mi/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi/utils/transformations.py` & `gmm_mi-0.7.1/gmm_mi/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/gmm_mi.egg-info/PKG-INFO` & `gmm_mi-0.7.1/gmm_mi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm-mi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gmm_mi-0.7.0/gmm_mi.egg-info/SOURCES.txt` & `gmm_mi-0.7.1/gmm_mi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.0/setup.py` & `gmm_mi-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 PACKAGENAME = 'gmm_mi'
 
 setup(
     name='gmm_mi',
-    version="0.7.0",
+    version="0.7.1",
     author='Davide Piras',
     author_email='dr.davide.piras@gmail.com',
     description='Estimate mutual information distribution with Gaussian mixture models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dpiras/GMM-MI',
     license='GNU General Public License v3.0 (GPLv3)',
```

