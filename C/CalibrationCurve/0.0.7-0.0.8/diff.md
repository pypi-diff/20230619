# Comparing `tmp/CalibrationCurve-0.0.7.tar.gz` & `tmp/CalibrationCurve-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.7.tar", last modified: Tue Jun 13 23:06:37 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.8.tar", last modified: Mon Jun 19 08:50:45 2023, max compression
```

## Comparing `CalibrationCurve-0.0.7.tar` & `CalibrationCurve-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.309370 CalibrationCurve-0.0.7/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4137 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3088 2023-06-13 23:06:30.000000 CalibrationCurve-0.0.7/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       67 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 23:06:37.000000 CalibrationCurve-0.0.7/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/LICENSE
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.7/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1003 2023-06-13 23:06:25.000000 CalibrationCurve-0.0.7/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 23:06:37.319370 CalibrationCurve-0.0.7/setup.cfg
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.7/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3423 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3189 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-19 08:50:45.000000 CalibrationCurve-0.0.8/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.8/LICENSE
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.8/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-19 08:49:07.000000 CalibrationCurve-0.0.8/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1002 2023-06-19 08:50:42.000000 CalibrationCurve-0.0.8/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-19 08:50:45.332981 CalibrationCurve-0.0.8/setup.cfg
+-rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.8/setup.py
```

### Comparing `CalibrationCurve-0.0.7/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.8/CalibrationCurve/_modidx.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,27 @@
                 'doc_baseurl': '/CalibrationCurve',
                 'doc_host': 'https://Rhys-McAlister.github.io',
                 'git_url': 'https://github.com/Rhys-McAlister/CalibrationCurve',
                 'lib_path': 'CalibrationCurve'},
   'syms': { 'CalibrationCurve.core': { 'CalibrationCurve.core.CalibrationModel': ('core.html#calibrationmodel', 'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.__init__': ( 'core.html#calibrationmodel.__init__',
                                                                                             'CalibrationCurve/core.py'),
+                                       'CalibrationCurve.core.CalibrationModel.calculate_fitted_values': ( 'core.html#calibrationmodel.calculate_fitted_values',
+                                                                                                           'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.calculate_sse': ( 'core.html#calibrationmodel.calculate_sse',
                                                                                                  'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.calculate_sxhat': ( 'core.html#calibrationmodel.calculate_sxhat',
                                                                                                    'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.calculate_syx': ( 'core.html#calibrationmodel.calculate_syx',
                                                                                                  'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.calculate_uncertainty': ( 'core.html#calibrationmodel.calculate_uncertainty',
                                                                                                          'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.fit_model': ( 'core.html#calibrationmodel.fit_model',
                                                                                              'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.fit_ols': ( 'core.html#calibrationmodel.fit_ols',
                                                                                            'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.get_params': ( 'core.html#calibrationmodel.get_params',
-                                                                                              'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.get_r2': ( 'core.html#calibrationmodel.get_r2',
-                                                                                          'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.get_t_value': ( 'core.html#calibrationmodel.get_t_value',
                                                                                                'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.inverse_prediction': ( 'core.html#calibrationmodel.inverse_prediction',
                                                                                                       'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.load_data': ( 'core.html#calibrationmodel.load_data',
-                                                                                             'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.plot_fit': ( 'core.html#calibrationmodel.plot_fit',
-                                                                                            'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.tabulate_results': ( 'core.html#calibrationmodel.tabulate_results',
                                                                                                     'CalibrationCurve/core.py')}}}
```

### Comparing `CalibrationCurve-0.0.7/LICENSE` & `CalibrationCurve-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.7/settings.ini` & `CalibrationCurve-0.0.8/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = CalibrationCurve
 lib_name = CalibrationCurve
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = CalibrationCurve
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,15 @@
 author_email = mcalisterrhys@gmail.com
 copyright = 2023 onwards, Rhys McAlister
 description = A collection of functions that streamline the process of creating calibration curves using Python.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = Rhys-McAlister
-requirements = fastcore pandas scikit-learn matplotlib numpy seaborn scipy
+requirements = fastcore pandas statsmodels matplotlib numpy seaborn scipy
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `CalibrationCurve-0.0.7/setup.py` & `CalibrationCurve-0.0.8/setup.py`

 * *Files identical despite different names*

