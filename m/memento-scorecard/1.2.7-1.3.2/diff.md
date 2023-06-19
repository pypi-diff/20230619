# Comparing `tmp/memento-scorecard-1.2.7.tar.gz` & `tmp/memento-scorecard-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-1.2.7.tar", last modified: Thu Jun 15 23:33:07 2023, max compression
+gzip compressed data, was "memento-scorecard-1.3.2.tar", last modified: Mon Jun 19 07:37:40 2023, max compression
```

## Comparing `memento-scorecard-1.2.7.tar` & `memento-scorecard-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.924055 memento-scorecard-1.2.7/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-1.2.7/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:33:07.921803 memento-scorecard-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.905454 memento-scorecard-1.2.7/memento/
--rw-rw-rw-   0        0        0     1384 2023-06-15 23:32:58.000000 memento-scorecard-1.2.7/memento/__init__.py
--rw-rw-rw-   0        0        0    28781 2023-06-15 23:32:29.000000 memento-scorecard-1.2.7/memento/bojack.py
--rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-1.2.7/memento/diane.py
--rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-1.2.7/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-1.2.7/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-1.2.7/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.917820 memento-scorecard-1.2.7/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 23:33:07.924055 memento-scorecard-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.680210 memento-scorecard-1.3.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1157 2023-06-19 07:37:40.677219 memento-scorecard-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.649291 memento-scorecard-1.3.2/memento/
+-rw-rw-rw-   0        0        0     1384 2023-06-19 07:35:54.000000 memento-scorecard-1.3.2/memento/__init__.py
+-rw-rw-rw-   0        0        0    28781 2023-06-19 07:35:26.000000 memento-scorecard-1.3.2/memento/bojack.py
+-rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-1.3.2/memento/diane.py
+-rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-1.3.2/memento/mr_peanutbutter.py
+-rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-1.3.2/memento/princess_carolyn.py
+-rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-1.3.2/memento/todd.py
+drwxrwxrwx   0        0        0        0 2023-06-19 07:37:40.673227 memento-scorecard-1.3.2/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 07:37:40.000000 memento-scorecard-1.3.2/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 07:37:40.680210 memento-scorecard-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-1.3.2/setup.py
```

### Comparing `memento-scorecard-1.2.7/LICENSE` & `memento-scorecard-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.2.7/PKG-INFO` & `memento-scorecard-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 1.2.7
+Version: 1.3.2
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-1.2.7/memento/__init__.py` & `memento-scorecard-1.3.2/memento/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from memento.diane import (compute_group_names, compute_table, transform_to_woes,
 calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics)
 from memento.princess_carolyn import (compute_final_breakpoints,
 compute_info, features_selection, display_table_ng, reagrupa_var)
 from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style,
 predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
 save_light_model, load_model, genera_punt_par, proc_freq)
-from memento.bojack import scorecard, autogrouping
+from memento.bojack import Scorecard, Autogrouping
 
-__version__ = '1.2.7'
+__version__ = '1.3.2'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
     compute_info, features_selection, display_table_ng, reagrupa_var,
     pretty_scorecard, parceling, cell_style,
     predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
     save_light_model, load_model, genera_punt_par, proc_freq,
-    scorecard, autogrouping
+    Scorecard, Autogrouping
 )
```

### Comparing `memento-scorecard-1.2.7/memento/bojack.py` & `memento-scorecard-1.3.2/memento/bojack.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .diane import *
 from .mr_peanutbutter import *
 from .princess_carolyn import *
 
 ####################################################################################################
 
 
-class scorecard:
+class Scorecard:
 
 
     def __init__(
         
         self,
         
         test_seed=123,
@@ -172,15 +172,15 @@
                 else: min_pct = self.autogrp_min_pct
 
                 if variable in self.autogrp_dict_manual_types: 
                     manual_type = self.autogrp_dict_manual_types[variable]
                 else: manual_type = ''
 
                 x = X_train[variable].values
-                frenken = autogrouping(max_groups=max_groups, 
+                frenken = Autogrouping(max_groups=max_groups, 
                 min_pct=min_pct, manual_type=manual_type).fit(x, y_train)
 
                 if len(frenken.breakpoints_num) == 0: variables_no_agrupadas_error.append(variable)
                 else: autogroupings[variable] = frenken
                 
             except:
                 variables_no_agrupadas_error.append(variable)
@@ -586,15 +586,15 @@
             venga += 1
 
         for i in X2.columns[venga:]: X1[i] = X2[i]
 
         return X1
         
 
-class autogrouping:
+class Autogrouping:
 
 
     def __init__(self, max_groups=5, min_pct=0.05, manual_type=''):
 
         self.max_groups = max_groups
         self.min_pct = min_pct
         self.manual_type = manual_type
```

### Comparing `memento-scorecard-1.2.7/memento/diane.py` & `memento-scorecard-1.3.2/memento/diane.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.2.7/memento/mr_peanutbutter.py` & `memento-scorecard-1.3.2/memento/mr_peanutbutter.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.2.7/memento/princess_carolyn.py` & `memento-scorecard-1.3.2/memento/princess_carolyn.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.2.7/memento/todd.py` & `memento-scorecard-1.3.2/memento/todd.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-1.2.7/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-1.3.2/memento_scorecard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 1.2.7
+Version: 1.3.2
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-1.2.7/setup.py` & `memento-scorecard-1.3.2/setup.py`

 * *Files identical despite different names*

