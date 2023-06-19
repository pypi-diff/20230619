# Comparing `tmp/stepmix-1.1.1.tar.gz` & `tmp/stepmix-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.1.1.tar", last modified: Tue May 16 18:14:27 2023, max compression
+gzip compressed data, was "stepmix-1.2.0.tar", last modified: Mon Jun 19 18:18:43 2023, max compression
```

## Comparing `stepmix-1.1.1.tar` & `stepmix-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.1.1/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.1.1/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.1.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.1.1/README-dev.md
--rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.1.1/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.1.1/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.1.1/docs/make.bat
--rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.1.1/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-05-16 18:04:21.788860 stepmix-1.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.1.1/docs/source/installation.rst
--rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.1.1/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1884 2023-05-16 18:04:21.788860 stepmix-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/README.md
--rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.1.1/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-05-16 18:04:21.788860 stepmix-1.1.1/stepmix/__init__.py
--rw-r--r--   0        0        0    10272 2023-05-16 17:54:29.612732 stepmix-1.1.1/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     6283 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.1.1/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6031 2023-01-11 22:01:14.083040 stepmix-1.1.1/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.1.1/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.1.1/stepmix/emission/nested.py
--rw-r--r--   0        0        0    54258 2023-05-16 18:04:21.788860 stepmix-1.1.1/stepmix/stepmix.py
--rw-r--r--   0        0        0    18715 2023-05-16 17:54:29.616732 stepmix-1.1.1/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.1.1/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.1.1/test/test_benchmarks.py
--rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.1.1/test/test_bootstrap.py
--rw-r--r--   0        0        0     8818 2023-04-30 21:21:22.007846 stepmix-1.1.1/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_fiml.py
--rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.1.1/test/test_inputs.py
--rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.1.1/test/test_progress_bar.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.1.1/test/test_random_state.py
--rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.1.1/test/test_sample_weight.py
--rw-r--r--   0        0        0      795 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.1.1/test/test_steps.py
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.2.0/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.2.0/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.2.0/README-dev.md
+-rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.2.0/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.2.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1016 2023-06-19 18:10:41.385049 stepmix-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.2.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.2.0/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1884 2023-06-19 18:10:41.381049 stepmix-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/README.md
+-rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-06-19 18:10:41.381049 stepmix-1.2.0/stepmix/__init__.py
+-rw-r--r--   0        0        0    10523 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.2.0/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     8129 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.2.0/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6162 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.2.0/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.2.0/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    57865 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/stepmix.py
+-rw-r--r--   0        0        0    19721 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.2.0/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.2.0/test/test_benchmarks.py
+-rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.2.0/test/test_bootstrap.py
+-rw-r--r--   0        0        0      735 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_buffers.py
+-rw-r--r--   0        0        0    10743 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.2.0/test/test_fiml.py
+-rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.2.0/test/test_inputs.py
+-rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.2.0/test/test_progress_bar.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.2.0/test/test_random_state.py
+-rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.2.0/test/test_sample_weight.py
+-rw-r--r--   0        0        0      792 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.2.0/test/test_steps.py
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.2.0/PKG-INFO
```

### Comparing `stepmix-1.1.1/.github/workflows/pytest.yaml` & `stepmix-1.2.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/LICENSE` & `stepmix-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/README-dev.md` & `stepmix-1.2.0/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/README.md` & `stepmix-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/docs/Makefile` & `stepmix-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/docs/make.bat` & `stepmix-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/docs/source/api.rst` & `stepmix-1.2.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/docs/source/conf.py` & `stepmix-1.2.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 project = "StepMix"
 copyright = "2022, Labo-Lacourse"
 author = "Sacha Morin, Robin Legault"
 
 release = "0.0"
-version = "1.1.1"
+version = "1.2.0"
 
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.napoleon",
     # 'numpydoc',
```

### Comparing `stepmix-1.1.1/docs/source/index.rst` & `stepmix-1.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/docs/source/tutorials.rst` & `stepmix-1.2.0/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/pyproject.toml` & `stepmix-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.1.1"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.1.1/scripts/README.md` & `stepmix-1.2.0/scripts/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/scripts/run_bakk_simulation.py` & `stepmix-1.2.0/scripts/run_bakk_simulation.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/scripts/run_bakk_simulation_complete.py` & `stepmix-1.2.0/scripts/run_bakk_simulation_complete.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/bootstrap.py` & `stepmix-1.2.0/stepmix/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,23 @@
 
     base_keys = ["measurement"]
     if "structural" in params[0]:
         base_keys.append("structural")
 
     for key_i in base_keys:
         for key_j in params[0][key_i].keys():
-            is_nested = not isinstance(base[key_i][key_j], np.ndarray)
+            is_nested = isinstance(base[key_i][key_j], dict)
             if is_nested:
                 # Nested parameters have another level of dictionaries
                 for key_k in params[0][key_i][key_j].keys():
-                    base[key_i][key_j][key_k] = np.stack(
-                        [p[key_i][key_j][key_k] for p in params]
-                    )
-            else:
+                    if isinstance(base[key_i][key_j][key_k], np.ndarray):
+                        base[key_i][key_j][key_k] = np.stack(
+                            [p[key_i][key_j][key_k] for p in params]
+                        )
+            elif isinstance(base[key_i][key_j], np.ndarray):
                 base[key_i][key_j] = np.stack([p[key_i][key_j] for p in params])
 
     base["weights"] = np.stack([p["weights"] for p in params])
 
     return base
 
 
@@ -266,28 +267,30 @@
     # Model parameters
     base_keys = ["measurement"]
     if "structural" in estimator_params_dict:
         base_keys.append("structural")
 
     for key_i in base_keys:
         for key_j in estimator_params_dict[key_i].keys():
-            is_nested = not isinstance(estimator_params_dict[key_i][key_j], np.ndarray)
+            is_nested = isinstance(estimator_params_dict[key_i][key_j], dict)
             if is_nested:
                 # Nested parameters have another level of dictionaries
                 for key_k in estimator_params_dict[key_i][key_j].keys():
                     estimate = estimator_params_dict[key_i][key_j][key_k]
-                    params = bootstrapped_params_dict[key_i][key_j][key_k]
-                    fig = percentiles_and_CI(
-                        estimate, params, key_i + " : " + key_j, key_k, alpha
-                    )
-                    figures.append(fig)
+                    if isinstance(estimate, np.ndarray):
+                        params = bootstrapped_params_dict[key_i][key_j][key_k]
+                        fig = percentiles_and_CI(
+                            estimate, params, key_i + " : " + key_j, key_k, alpha
+                        )
+                        figures.append(fig)
             else:
                 estimate = estimator_params_dict[key_i][key_j]
-                params = bootstrapped_params_dict[key_i][key_j]
-                fig = percentiles_and_CI(estimate, params, key_i, key_j, alpha)
-                figures.append(fig)
+                if isinstance(estimate, np.ndarray):
+                    params = bootstrapped_params_dict[key_i][key_j]
+                    fig = percentiles_and_CI(estimate, params, key_i, key_j, alpha)
+                    figures.append(fig)
 
     # Make sure all figures have enough space for figure title
     for f in figures:
         f.subplots_adjust(top=0.85)
 
     return figures
```

### Comparing `stepmix-1.1.1/stepmix/corrections.py` & `stepmix-1.2.0/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/datasets.py` & `stepmix-1.2.0/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/emission/build_emission.py` & `stepmix-1.2.0/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/emission/categorical.py` & `stepmix-1.2.0/stepmix/emission/categorical.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,45 +73,84 @@
 
 
 class Multinoulli(Emission):
     """Multinoulli (categorical) emission model
 
     Uses one-hot encoded features. Expected data formatting:
     X[n,k*L+l]=1 if l is the observed outcome for the kth attribute of data point n,
-    where n is the number of observations, K=n_features, L=n_outcomes for each multinoulli
+    where n is the number of observations, K=n_features, L=max_n_outcomes for each multinoulli where max_n_outcomes
+    represents the maximum number of outcomes for a given feature.
 
     If integer_codes is set to True, the model will expect integer-encoded categories and will one-hot
-    encode the data itself. The result will be cached and reused across iterations. In this case, n_outcomes
-    is ignored and computed by the model.
+    encode the data itself. In this case, max_n_outcomes and total_outcomes are inferred by the model.
 
-    Parameters:
+    Parameters
+    ----------
+    n_components : int, default=2
+        The number of latent classes.
+    random_state : int, RandomState instance or None, default=None
+        Controls the random seed given to the method chosen to initialize the
+        parameters. Pass an int for reproducible output across multiple function calls.
+    integer_codes : bool, default=True
+        Input X should be integer-encoded zero-indexed categories.
+    max_n_outcomes : int, default=None
+        Maximum number of outcomes for a single categorical feature.
+        Each column in the input will have max_n_outcomes associated columns in the one-hot encoding.
+        If None and integer_codes=True, will be inferred from the data.
+    total_outcomes : int, default=None
+        Total outcomes over all features. E.g., if we provide a categorical variable with two outcomes and another
+        with 4 outcomes, total_outcomes = 6.
+        If None and integer_codes=True, will be inferred from the data.
+
+    Attributes
+    ----------
     pis[k*L+l,c]=P[ X[n,k*L+l]=1 | n belongs to class c]
     """
 
     def __init__(
-        self, n_components=2, random_state=None, n_outcomes=None, integer_codes=True
+        self,
+        n_components=2,
+        random_state=None,
+        integer_codes=True,
+        max_n_outcomes=None,
+        total_outcomes=None,
     ):
         super().__init__(n_components=n_components, random_state=random_state)
-        self.n_outcomes = n_outcomes
         self.integer_codes = integer_codes
+        self.parameters["max_n_outcomes"] = max_n_outcomes
+        self.parameters["total_outcomes"] = total_outcomes
 
-        if n_outcomes is None and not integer_codes:
+        if max_n_outcomes is None and not integer_codes:
+            raise ValueError(
+                "max_n_outcomes can only be set to None with integer_codes=True."
+            )
+        if total_outcomes is None and not integer_codes:
             raise ValueError(
-                "n_outcomes can only be set to None with integer_codes=True."
+                "total_outcomes can only be set to None with integer_codes=True."
             )
 
     def get_n_features(self):
-        n_features_x_n_outcomes = self.parameters["pis"].shape[1]
-        n_features = int(n_features_x_n_outcomes / self.n_outcomes)
+        n_features_x_max_n_outcomes = self.parameters["pis"].shape[1]
+        n_features = int(
+            n_features_x_max_n_outcomes / self.parameters["max_n_outcomes"]
+        )
         return n_features
 
     def encode_features(self, X):
         if self.integer_codes:
             # Self.n_outcomes will only be updated if it is still None
-            X, self.n_outcomes = max_one_hot(X, max_n_outcomes=self.n_outcomes)
+            (
+                X,
+                self.parameters["max_n_outcomes"],
+                self.parameters["total_outcomes"],
+            ) = max_one_hot(
+                X,
+                max_n_outcomes=self.parameters["max_n_outcomes"],
+                total_outcomes=self.parameters["total_outcomes"],
+            )
 
         return X
 
     def m_step(self, X, resp):
         X = self.encode_features(X)
         pis = X.T @ resp
         pis /= resp.sum(axis=0, keepdims=True)
@@ -124,39 +163,46 @@
         pis = np.clip(self.parameters["pis"].T, 1e-15, 1 - 1e-15)
         log_eps = X @ np.log(pis)
         return log_eps
 
     def sample(self, class_no, n_samples):
         pis = self.parameters["pis"].T
         n_features = self.get_n_features()
-        feature_weights = pis[:, class_no].reshape(n_features, self.n_outcomes)
+        feature_weights = pis[:, class_no].reshape(
+            n_features, self.parameters["max_n_outcomes"]
+        )
         X = np.array(
             [
                 self.random_state.multinomial(1, feature_weights[k], size=n_samples)
                 for k in range(n_features)
             ]
         )
-        X = np.reshape(np.swapaxes(X, 0, 1), (n_samples, n_features * self.n_outcomes))
+        X = np.reshape(
+            np.swapaxes(X, 0, 1),
+            (n_samples, n_features * self.parameters["max_n_outcomes"]),
+        )
         return X
 
     def print_parameters(self, indent=1):
         print_parameters(
             self.parameters["pis"],
             "Multinoulli",
-            n_outcomes=self.n_outcomes,
+            n_outcomes=self.parameters["max_n_outcomes"],
             indent=indent,
             np_precision=4,
         )
 
     @property
     def n_parameters(self):
         n_classes = self.parameters["pis"].shape[0]
 
-        # Only n-1 free parameters per outcome since probabilities sum to 1
-        n_free_parameters_per_class = (self.get_n_features() - 1) * self.n_outcomes
+        # Only n_outcomes - 1 free parameters per feature since probabilities sum to 1
+        n_free_parameters_per_class = (
+            self.parameters["total_outcomes"] - self.get_n_features()
+        )
         return n_classes * n_free_parameters_per_class
 
 
 class MultinoulliNan(Multinoulli):
     """Multinoulli (categorical) emission model supporting missing values (Full Information Maximum Likelihood)."""
 
     def m_step(self, X, resp):
```

### Comparing `stepmix-1.1.1/stepmix/emission/covariate.py` & `stepmix-1.2.0/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/emission/emission.py` & `stepmix-1.2.0/stepmix/emission/emission.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     All model parameters should be values of the self.parameters dict attribute. See the Bernoulli and GaussianUnit
     implementations for reference.
 
     Model parameters should be ndarrays of shape (n_components, ...).
     In other words, the FIRST AXIS should always correspond to the latent class.
 
+    You can save other things to self.parameters, but they must NOT be ndarrays.
+
     To add an emission model, you must :
         - Inherit from Emission.
         - Implement the m_step, log_likelihood and sample methods.
         - Add a corresponding string in the EMISSION_DICT at the end of emission.py.
         - Update the StepMix docstring for the measurement and structural arguments!
 
     Parameters
@@ -176,8 +178,9 @@
         perm : ndarray of shape  (n_classes,)
             Integer array representing the target permutation. Should be a permutation of np.arange(n_classes).
         axis: int
             Axis to use for permuting the parameters.
 
         """
         for key, item in self.parameters.items():
-            self.parameters[key] = item[perm]
+            if isinstance(item, np.ndarray):
+                self.parameters[key] = item[perm]
```

### Comparing `stepmix-1.1.1/stepmix/emission/gaussian.py` & `stepmix-1.2.0/stepmix/emission/gaussian.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/emission/nested.py` & `stepmix-1.2.0/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/stepmix/stepmix.py` & `stepmix-1.2.0/stepmix/stepmix.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,16 @@
     rel_tol : float, default=0.00
         The convergence threshold. EM iterations will stop when the
         relative lower bound average gain is below this threshold.
     max_iter : int, default=1000
         The number of EM iterations to perform.
     n_init : int, default=1
         The number of initializations to perform. The best results are kept.
+    save_param_init : bool, default=False
+        Save the estimated parameters of all initializations to self.param_buffer_.
     init_params : {'kmeans', 'random'}, default='random'
         The method used to initialize the weights, the means and the
         precisions.
         Must be one of:
 
             - 'kmeans' : responsibilities are initialized using kmeans.
             - 'random' : responsibilities are initialized randomly.
@@ -169,14 +171,19 @@
     converged_ : bool
         True when convergence was reached in fit(), False otherwise.
     n_iter_ : int
         Number of step used by the best fit of EM to reach the convergence.
     lower_bound_ : float
         Lower bound value on the log-likelihood (of the training data with
         respect to the model) of the best fit of EM.
+    lower_bound_buffer_ : float
+        Lower bound values on the log-likelihood (of the training data with
+        respect to the model) of all EM initializations.
+    param_buffer_ : list
+        Final parameters of all initializations. Only updated if save_param_init=True.
 
     Notes
     -----
 
     References
     ----------
 
@@ -221,27 +228,29 @@
         structural="gaussian_unit",
         assignment="modal",
         correction=None,
         abs_tol=1e-10,
         rel_tol=0.00,
         max_iter=1000,
         n_init=1,
+        save_param_init=False,
         init_params="random",
         random_state=None,
         verbose=0,
         progress_bar=1,
         measurement_params=None,
         structural_params=None,
     ):
         # Attributes of the base StepMix class
         self.n_components = n_components
         self.abs_tol = abs_tol
         self.rel_tol = rel_tol
         self.max_iter = max_iter
         self.n_init = n_init
+        self.save_param_init = save_param_init
         self.init_params = init_params
         self.random_state = random_state
         self.verbose = verbose
         self.progress_bar = progress_bar
         self.n_steps = n_steps
 
         # Additional attributes for 3-step estimation
@@ -277,21 +286,23 @@
             verbose=self.verbose,
         )
         utils.check_positive(
             n_components=self.n_components,
             max_iter=self.max_iter,
             n_init=self.n_init,
         )
-        utils.check_nonneg(abs_tol=self.abs_tol, verbose=self.verbose)
-        utils.check_nonneg(rel_tol=self.rel_tol, verbose=self.verbose)
+        utils.check_nonneg(
+            abs_tol=self.abs_tol, rel_tol=self.rel_tol, verbose=self.verbose
+        )
         utils.check_in([1, 2, 3], n_steps=self.n_steps)
         utils.check_in([0, 1, 2], progress_bar=self.progress_bar)
         utils.check_in(["kmeans", "random"], init_params=self.init_params)
-        utils.check_in(["modal", "soft"], init_params=self.assignment)
-        utils.check_in([None, "BCH", "ML"], init_params=self.correction)
+        utils.check_in(["modal", "soft"], assignment=self.assignment)
+        utils.check_in([None, "BCH", "ML"], correction=self.correction)
+        utils.check_in([False, True], save_param_init=self.save_param_init)
         utils.check_descriptor(self.measurement, keys=EMISSION_DICT.keys())
         utils.check_descriptor(self.structural, keys=EMISSION_DICT.keys())
         utils.check_type(
             (dict, type(None)),
             measurement_params=self.measurement_params,
             structural_params=self.structural_params,
         )
@@ -304,14 +315,17 @@
         self._force_all_finite_sm = (
             "allow-nan" if utils.check_descriptor_nan(self.structural) else True
         )
 
         # Buffer to save the likelihoods of different inits for debugging
         self.lower_bound_buffer_ = list()
 
+        # Buffer to save params of different inits
+        self.param_buffer_ = list()
+
         # Covariate models have special constraints. Check them.
         is_covariate = utils.check_covariate(self.measurement, self.structural)
 
         # Covariate models use a different conditional likelihood (See Bakk and Kuha, 2018), which should
         # not include the marginal likelihood over the latent classes in the E-step
         self._class_weight_likelihood = not is_covariate
 
@@ -808,40 +822,49 @@
                 )
 
                 # Likelihood & stopping criterion
                 lower_bound = log_prob_norm
                 change = lower_bound - prev_lower_bound
                 rel_change = change / lower_bound
 
-                # Save lower bound
-                self.lower_bound_buffer_.append(lower_bound)
-
                 # if both an absolute and a relative tolerance threshold are given, the EM algorithm stops
                 # as soon as one of them is respected
                 if abs(change) < self.abs_tol or abs(rel_change) < self.rel_tol:
                     self.converged_ = True
                     break
 
                 # Ask tqdm to display current max lower bound
                 ll = (
                     lower_bound * np.sum(sample_weight)
                     if sample_weight is not None
                     else lower_bound * n_samples
                 )
                 tqdm_iter.set_postfix(avg_LL=lower_bound, LL=ll)
 
+            # Update buffers
+            current_parameters = self.get_parameters()
+
             if (
                 lower_bound > max_lower_bound
                 or max_lower_bound == -np.inf
                 or np.isnan(max_lower_bound)
             ):
                 max_lower_bound = lower_bound
-                best_params = self.get_parameters()
+                best_params = current_parameters
                 best_n_iter = n_iter
 
+            if self.save_param_init:
+                self.param_buffer_.append(copy.deepcopy(current_parameters))
+
+            # Save lower bound
+            ll, _ = self._e_step(
+                X, Y=Y, sample_weight=sample_weight, log_emission_pm=log_emission_pm
+            )
+            self.lower_bound_buffer_.append(ll)
+
             # Ask tqdm to display current max lower bound
             max_ll = (
                 max_lower_bound * np.sum(sample_weight)
                 if sample_weight is not None
                 else max_lower_bound * n_samples
             )
             tqdm_init.set_postfix(max_avg_LL=max_lower_bound, max_LL=max_ll)
@@ -1081,14 +1104,70 @@
         Returns
         -------
         aic : float
             The lower the better.
         """
         return -2 * self.score(X, Y) * X.shape[0] + 2 * self.n_parameters
 
+    def entropy(self, X, Y=None):
+        """Entropy of the posterior over latent classes.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_columns)
+            List of n_features-dimensional data points, where each column corresponds
+            to a feature for univariate variables (n_features=n_columns) and each group
+            of L columns corresponds to a feature for one-hot encoded variables with L
+            possible outcomes (n_features=n_columns/L). Each row corresponds to a single
+            data point of the measurement model.
+        Y : array-like of shape (n_samples, n_columns_structural), default=None
+            List of n_features-dimensional data points, where each column corresponds
+            to a feature for univariate variables (n_features=n_columns_structural)
+            and each group of L columns corresponds to a feature for one-hot encoded
+            variables with L possible outcomes (n_features=n_columns_structural/L).
+            Each row corresponds to a  single data point of the structural model.
+        Returns
+        -------
+        entropy : float
+        """
+        check_is_fitted(self)
+        resp = self.predict_proba(X, Y)
+
+        return -1 * np.sum(resp * np.log(resp))
+
+    def relative_entropy(self, X, Y=None):
+        """Scaled Relative Entropy of the posterior over latent classes.
+
+        Ramaswamy et al., 1993.
+
+        1 - entropy / (n_samples * log(n_components))
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_columns)
+            List of n_features-dimensional data points, where each column corresponds
+            to a feature for univariate variables (n_features=n_columns) and each group
+            of L columns corresponds to a feature for one-hot encoded variables with L
+            possible outcomes (n_features=n_columns/L). Each row corresponds to a single
+            data point of the measurement model.
+        Y : array-like of shape (n_samples, n_columns_structural), default=None
+            List of n_features-dimensional data points, where each column corresponds
+            to a feature for univariate variables (n_features=n_columns_structural)
+            and each group of L columns corresponds to a feature for one-hot encoded
+            variables with L possible outcomes (n_features=n_columns_structural/L).
+            Each row corresponds to a  single data point of the structural model.
+        Returns
+        -------
+        entropy : float
+        """
+        entropy = self.entropy(X, Y)
+        n_samples = X.shape[0]
+
+        return 1 - entropy / (n_samples * np.log(self.n_components))
+
     def predict(self, X, Y=None):
         """Predict the labels for the data samples in X using the measurement model.
 
         Optionally, an array-like Y can be provided to predict the labels based on both the measurement and structural
         models.
 
         Parameters
```

### Comparing `stepmix-1.1.1/stepmix/utils.py` & `stepmix-1.2.0/stepmix/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,14 +313,16 @@
         if sample_weight is not None
         else avg_ll * n_samples
     )
     minus2ll = -2 * ll
 
     bic = model.bic(X, Y)
     aic = model.aic(X, Y)
+    entropy = model.entropy(X, Y)
+    relative_entropy = model.relative_entropy(X, Y)
 
     print("=" * 80)
     print("MODEL REPORT")
     print("=" * 80)
     print("    " + "=" * 76)
     print(f"    Measurement model parameters")
     print("    " + "=" * 76)
@@ -349,14 +351,16 @@
     print(f"    Number of latent classes      : {n_classes}")
     print(f"    Number of estimated parameters: {n_parameters}")
     print(f"    Log-likelihood (LL)           : {ll:.4f}")
     print(f"    -2LL                          : {minus2ll:.4f}")
     print(f"    Average LL                    : {avg_ll:.4f}")
     print(f"    AIC                           : {aic:.2f}")
     print(f"    BIC                           : {bic:.2f}")
+    print(f"    Entropy                       : {entropy:.4f}")
+    print(f"    Scaled Relative Entropy       : {relative_entropy:.4f}")
 
 
 def print_parameters(
     params,
     model_name,
     indent=1,
     np_precision=2,
@@ -402,15 +406,19 @@
 
     # Title
     print(indent_str + "-" * (80 - indent * 4))
     print(
         indent_str
         + f"{model_name} model with {n_features} feature"
         + ("s" if n_features > 1 else "")
-        + (f", each with {n_outcomes} possible outcomes" if n_outcomes >= 2 else "")
+        + (
+            f", each with up to {n_outcomes} possible outcomes"
+            if n_outcomes >= 2
+            else ""
+        )
         + (" and intercept" if intercept else "")
     )
     print(indent_str + "-" * (80 - indent * 4))
 
     # Clarification message for multinoulli model
     if n_outcomes >= 2 and n_features >= 2:
         print(
@@ -456,15 +464,15 @@
                     print()
                 elif isinstance(p, np.ndarray):
                     print(indent_str + f"Class {i + 1} : {p}")
                 else:
                     print(indent_str + f"Class {i + 1} : {p:.2f}")
 
 
-def max_one_hot(array, max_n_outcomes=None):
+def max_one_hot(array, max_n_outcomes=None, total_outcomes=None):
     """Multiple categorical one-hot encoding.
 
     Takes an n_samples x n_features array of integer-encoded categorical features and returns an
     n_samples x (n_features x max_n_outcomes) array where max_n_outcomes is the number of outcomes in the
     categorical feature with the most categories. Categories are one-hot encoded and categories with
     fewer than max_n_outcomes simply have unused extra columns.
 
@@ -477,60 +485,72 @@
             [
                 [0, 3],
                 [1, 0],
                 [2, 1],
                 [2, 2],
             ]
         )
-        b, max_n_outcomes = max_one_hot(a)
+        b, max_n_outcomes, total_outcomes = max_one_hot(a)
         print(b)
 
         # Should yield
         # [[1. 0. 0. 0. 0. 0. 0. 1.]
         #  [0. 1. 0. 0. 1. 0. 0. 0.]
         #  [0. 0. 1. 0. 0. 1. 0. 0.]
         #  [0. 0. 1. 0. 0. 0. 1. 0.]]
 
     Parameters
     ----------
     array : ndarray of shape  (n_samples, n_features)
         Integer-encoded categorical data. Will be float due to sklearn casting. We'll cast back to ints.
-    max_n_outcomes : max_n_outcomes, default=None
-        Maximum number of outcomes. Each column will max_n_outcomes associated columns. If None, will be inferred
-        from the data.
+    max_n_outcomes : int, default=None
+        Maximum number of outcomes for a single categorical feature.
+        Each column in the input will have max_n_outcomes associated columns in the output.
+        If None, will be inferred from the data.
+    total_outcomes : int, default=None
+        Total outcomes over all features. E.g., if we provide a categorical variable with two outcomes and another
+        with 4 outcomes, total_outcomes = 6.
+        If None, will be inferred from the data.
 
     Returns
     -------
     one_hot : ndarray of shape (n_samples, n_features * max_n_outcomes)
         One-hot encoded categories.
 
-    max_n_outcomes : max_n_outcomes
-        Maximum number of outcomes. Each column will max_n_outcomes associated columns.
+    max_n_outcomes : int
+        Maximum number of outcomes for a single categorical feature.
+        Each column in the input will have max_n_outcomes associated columns in the output.
+
+    total_outcomes : int
+        Total outcomes over all features. E.g., if we provide a categorical variable with two outcomes and another
+        with 4 outcomes, total_outcomes = 6.
 
     """
     n_samples = array.shape[0]
     n_features = array.shape[1]
 
     # Get maximal number of outcomes
-    if max_n_outcomes is None:
-        max_n_outcomes = int(np.nanmax(array) + 1)
+    if max_n_outcomes is None or total_outcomes is None:
+        outcomes = np.nanmax(array, axis=0) + 1
+        total_outcomes = int(np.sum(outcomes))
+        max_n_outcomes = int(np.nanmax(outcomes))
 
     # Create one-hot encoding
     one_hot = np.zeros((n_samples, array.shape[1] * max_n_outcomes))
 
     for c in range(n_features):
         integer_codes = array[:, c]
         not_observed = np.isnan(integer_codes)
         integer_codes = np.nan_to_num(integer_codes, nan=0).astype(int)
         one_hot[np.arange(n_samples), integer_codes + c * max_n_outcomes] = 1.0
 
         # Now reapply NaNs
         one_hot[not_observed, c * max_n_outcomes : (c + 1) * max_n_outcomes] = np.nan
 
-    return one_hot, max_n_outcomes
+    return one_hot, max_n_outcomes, total_outcomes
 
 
 def get_mixed_descriptor(dataframe, **kwargs):
     """Simpler API to build the mixed model descriptor from a dataframe.
 
     Mixed models can combine multiple datatypes, such as binary or continuous.
     Please refer to :class:`stepmix.emission.nested.Nested` for details on the output descriptor.
```

### Comparing `stepmix-1.1.1/test/conftest.py` & `stepmix-1.2.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_benchmarks.py` & `stepmix-1.2.0/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_bootstrap.py` & `stepmix-1.2.0/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_emission.py` & `stepmix-1.2.0/test/test_emission.py`

 * *Files 18% similar despite different names*

```diff
@@ -210,17 +210,18 @@
             [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
             [0.0, 1.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 0.0, 0.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
         ]
     )
 
-    onehot, max_n_outcomes = max_one_hot(a)
+    onehot, max_n_outcomes, total_outcomes = max_one_hot(a)
 
     assert max_n_outcomes == 4
+    assert total_outcomes == 7
     assert np.all(onehot == target)
 
 
 def test_max_one_hot_nan(data, kwargs):
     """Test the max_one_hot method in utils with NaNs"""
     a = np.array(
         [
@@ -236,17 +237,18 @@
             [1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
             [0.0, 1.0, 0.0, 0.0, np.nan, np.nan, np.nan, np.nan],
             [np.nan, np.nan, np.nan, np.nan, 0.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
         ]
     )
 
-    onehot, max_n_outcomes = max_one_hot(a)
+    onehot, max_n_outcomes, total_outcomes = max_one_hot(a)
 
     assert max_n_outcomes == 4
+    assert total_outcomes == 7
     assert np.allclose(onehot, target, equal_nan=True)
 
 
 def test_categorical_encoding(kwargs):
     # Ignore base measurement and structural for this step
     kwargs.pop("measurement")
     kwargs.pop("structural")
@@ -267,39 +269,101 @@
             [0.0, 1.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 0.0, 0.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
         ]
     )
 
     # Model on integer codes
+    # In this case, max_n_outcomes and total_outcomes are inferred from the data
     model_1 = StepMix(
         measurement="categorical",
-        measurement_params=dict(integer_codes=True, n_outcomes=None),
+        measurement_params=dict(
+            integer_codes=True, max_n_outcomes=None, total_outcomes=None
+        ),
         **kwargs,
     )
     model_1.fit(data_int)
     param_1 = model_1.get_parameters()["measurement"]["pis"]
 
     # Model on one-hot codes
+    # In this case, we need to specify max_n_outcomes and total_outcomes
     model_2 = StepMix(
         measurement="categorical",
-        measurement_params=dict(integer_codes=False, n_outcomes=2),
+        measurement_params=dict(
+            integer_codes=False, max_n_outcomes=4, total_outcomes=7
+        ),
         **kwargs,
     )
     model_2.fit(data_one_hot)
     param_2 = model_2.get_parameters()["measurement"]["pis"]
 
     # Check if parameters are the same
     assert np.all(param_1 == param_2)
 
+    # Check if n_parameters are the same
+    assert model_1.n_parameters == model_2.n_parameters
+
+    # Check n_parameters
+    n_parameters = (3 - 1) + 3 * (2 + 3)
+    assert model_1.n_parameters == n_parameters
+
 
 def test_categorical_less_categories_in_test():
     train = np.random.choice([0, 1, 2, 3], 100).reshape((-1, 1))
     test = np.random.choice([0, 1, 2], 100).reshape((-1, 1))  # no class 3
 
     model = StepMix(
         n_components=3, measurement="categorical", verbose=1, random_state=123
     )
 
     model.fit(train)
 
     preds = model.predict(test)
+
+
+@pytest.mark.filterwarnings(
+    "ignore::sklearn.exceptions.ConvergenceWarning"
+)  # Ignore convergence warnings
+def test_categorical_n_parameters():
+    """Test number of parameters of a simple categorical mixture."""
+    rng = np.random.default_rng(42)
+    data = rng.choice(a=[0, 1, 2], size=200).reshape(-1, 1)
+
+    model = StepMix(
+        n_components=3,
+        measurement="categorical",
+        random_state=42,
+        verbose=0,
+        max_iter=5000,
+        n_init=1,
+    )
+
+    model.fit(data)
+
+    assert model.n_parameters == 8
+
+
+@pytest.mark.filterwarnings(
+    "ignore::sklearn.exceptions.ConvergenceWarning"
+)  # Ignore convergence warnings
+def test_categorical_n_parameters_max():
+    """Test number of parameters of a categorical mixture where some categorical features have fewer outcomes."""
+    rng = np.random.default_rng(42)
+    data_1 = rng.choice(a=[0, 1, 2, 3], size=300).reshape(-1, 1)
+    data_2 = rng.choice(a=[0, 1, 2], size=300).reshape(-1, 1)
+    data_3 = rng.choice(a=[0, 1], size=300).reshape(-1, 1)
+    data = np.hstack((data_1, data_2, data_3))
+
+    model = StepMix(
+        n_components=4,
+        measurement="categorical",
+        random_state=42,
+        verbose=0,
+        max_iter=5000,
+        n_init=1,
+    )
+
+    model.fit(data)
+
+    n_parameters = (4 - 1) + 4 * (1 + 2 + 3)
+
+    assert model.n_parameters == n_parameters
```

### Comparing `stepmix-1.1.1/test/test_fiml.py` & `stepmix-1.2.0/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_inputs.py` & `stepmix-1.2.0/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_random_state.py` & `stepmix-1.2.0/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_sample_weight.py` & `stepmix-1.2.0/test/test_sample_weight.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/test/test_sklearn.py` & `stepmix-1.2.0/test/test_sklearn.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
 def test_gridsearch(data, kwargs):
     """Quick check with the scikit-learn GridSearchCV object"""
     X, Y = data
 
     # Grid search with cross-validation
     model_1 = StepMix(n_steps=1, **kwargs)
-    gs = GridSearchCV(estimator=model_1, param_grid=dict(n_components=[1, 2, 3, 4, 5]))
+    gs = GridSearchCV(estimator=model_1, param_grid=dict(n_components=[2, 3, 4, 5]))
     gs.fit(X, Y)
```

### Comparing `stepmix-1.1.1/test/test_steps.py` & `stepmix-1.2.0/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.1.1/PKG-INFO` & `stepmix-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.1.1 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.2.0 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
```

