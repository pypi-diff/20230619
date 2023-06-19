# Comparing `tmp/gecs-0.14.1.tar.gz` & `tmp/gecs-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.14.1.tar", max compression
+gzip compressed data, was "gecs-0.14.2.tar", max compression
```

## Comparing `gecs-0.14.1.tar` & `gecs-0.14.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.14.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.14.1/README.md
--rw-r--r--   0        0        0      697 2023-06-18 17:27:33.582283 gecs-0.14.1/pyproject.toml
--rw-r--r--   0        0        0    43030 2023-06-18 17:26:22.404258 gecs-0.14.1/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-18 16:26:28.103885 gecs-0.14.1/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.14.1/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.14.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.14.2/README.md
+-rw-r--r--   0        0        0      697 2023-06-19 09:20:16.050681 gecs-0.14.2/pyproject.toml
+-rw-r--r--   0        0        0    43737 2023-06-19 09:19:34.711173 gecs-0.14.2/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-18 16:26:28.103885 gecs-0.14.2/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.14.2/setup.py
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.14.2/PKG-INFO
```

### Comparing `gecs-0.14.1/LICENSE` & `gecs-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.14.1/pyproject.toml` & `gecs-0.14.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.14.1"
+version = "0.14.2"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.14.1/src/gecs/gec.py` & `gecs-0.14.2/src/gecs/gec.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 np.arange(200, 500, 50),
                 np.arange(500, 100, 100),
                 np.arange(1000, 10001, 1000),
             ]
         )
         self._real_hyperparameters_all = [
             ("learning_rate", (np.logspace(0.001, 2.5, 100)) / 1000),
-            ("num_leaves", np.arange(10, 1001, 5)),
+            ("num_leaves",  np.array(list(range(1, 100))+list(range(100, 1000, 5)))),
             ("n_estimators", ten_to_ten_thousand),
             ("max_bin", ten_to_ten_thousand[:-9]),
             ("lambda_l1", (np.logspace(0.00, 1, 100) - 1) / 9),
             ("lambda_l2", (np.logspace(0.00, 1, 100) - 1) / 9),
             ("min_data_in_leaf", np.arange(2, 50, 1)),
             ("feature_fraction",np.arange(0.1, 1.01, 0.01))
         ]
@@ -290,14 +290,17 @@
         self._real_hyperparameters_map_reverse = {
             name: dict(zip(real_values, linear_values))
             for ((name, linear_values), (_, real_values)) in zip(
                 self._real_hyperparameters_linear, self._real_hyperparameters
             )
         }
 
+        self._validate_parameter_maps()
+
+
         self._real_hyperparameter_names, self._real_hyperparameter_ranges = zip(
             *self._real_hyperparameters_linear
         )
 
         self._real_hypermarameter_types = [
             np.array(s).dtype for _, s in self._real_hyperparameters
         ]
@@ -466,14 +469,29 @@
             "best_score": self.best_score,
             "best_params_gec": self.best_params_gec,
             "best_scores_gec": self.best_scores_gec,
             "gec_iter": self.gec_iter,
         }
         return representation
 
+
+    def _validate_parameter_maps(self):
+        real_to_linear_to_real = [
+            self._real_hyperparameters_map[hp][self._real_hyperparameters_map_reverse[hp][v]] == v
+            for hp, values in self._real_hyperparameters for v in values
+        ]
+
+        assert np.all(real_to_linear_to_real), real_to_linear_to_real
+
+        linear_to_real_to_linear = [
+            self._real_hyperparameters_map_reverse[hp][self._real_hyperparameters_map[hp][v]] == v
+            for hp, values in self._real_hyperparameters_linear for v in values
+        ]
+        assert np.all(linear_to_real_to_linear), linear_to_real_to_linear
+
     def set_gec_hyperparameters(self, gec_hyperparameters):
         """Set the hyperparameters of the GEC optimisation process
 
         Parameters
         ----------
             gec_hyperparameters : dict[str, float]
                 dictionary with values for "l", "l_bagging",
```

### Comparing `gecs-0.14.1/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.14.2/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.14.1/setup.py` & `gecs-0.14.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.14.1',
+    'version': '0.14.2',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
     'long_description': '',
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
```

### Comparing `gecs-0.14.1/PKG-INFO` & `gecs-0.14.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.14.1
+Version: 0.14.2
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
```

