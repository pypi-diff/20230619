# Comparing `tmp/spherecluster2-0.2.0.tar.gz` & `tmp/spherecluster2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherecluster2-0.2.0.tar", last modified: Mon Jun 19 11:05:06 2023, max compression
+gzip compressed data, was "spherecluster2-0.2.1.tar", last modified: Mon Jun 19 12:17:51 2023, max compression
```

## Comparing `spherecluster2-0.2.0.tar` & `spherecluster2-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:06.106345 spherecluster2-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-19 11:05:06.106345 spherecluster2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 11:05:06.110345 spherecluster2-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:06.106345 spherecluster2-0.2.0/spherecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/spherecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/spherecluster/regacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/spherecluster/spherical_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/spherecluster/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    31327 2023-06-19 11:04:57.000000 spherecluster2-0.2.0/spherecluster/von_mises_fisher_mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:05:06.106345 spherecluster2-0.2.0/spherecluster2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-19 11:05:06.000000 spherecluster2-0.2.0/spherecluster2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-19 11:05:06.000000 spherecluster2-0.2.0/spherecluster2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:05:06.000000 spherecluster2-0.2.0/spherecluster2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 11:05:06.000000 spherecluster2-0.2.0/spherecluster2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 11:05:06.000000 spherecluster2-0.2.0/spherecluster2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:17:51.554212 spherecluster2-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-19 12:17:51.554212 spherecluster2-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 12:17:51.558212 spherecluster2-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:17:51.554212 spherecluster2-0.2.1/spherecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/spherecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/spherecluster/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/spherecluster/spherical_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/spherecluster/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31327 2023-06-19 12:17:42.000000 spherecluster2-0.2.1/spherecluster/von_mises_fisher_mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:17:51.554212 spherecluster2-0.2.1/spherecluster2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-06-19 12:17:51.000000 spherecluster2-0.2.1/spherecluster2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-19 12:17:51.000000 spherecluster2-0.2.1/spherecluster2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:17:51.000000 spherecluster2-0.2.1/spherecluster2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 12:17:51.000000 spherecluster2-0.2.1/spherecluster2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 12:17:51.000000 spherecluster2-0.2.1/spherecluster2.egg-info/top_level.txt
```

### Comparing `spherecluster2-0.2.0/LICENSE` & `spherecluster2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spherecluster2-0.2.0/PKG-INFO` & `spherecluster2-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherecluster2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Clustering on the unit hypersphere in scikit-learn.
 Home-page: https://github.com/miquelmassot/spherecluster
 Author: Jason Laska
 Author-email: jason@claralabs.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: MIT
```

### Comparing `spherecluster2-0.2.0/README.md` & `spherecluster2-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spherecluster2-0.2.0/setup.py` & `spherecluster2-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 setup(
     name="spherecluster2",
-    version="0.2.0",
+    version="0.2.1",
     description="Clustering on the unit hypersphere in scikit-learn.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jason Laska",
     author_email="jason@claralabs.com",
     maintainer="Miquel Massot",
     maintainer_email="miquel.massot@gmail.com",
```

### Comparing `spherecluster2-0.2.0/spherecluster/spherical_kmeans.py` & `spherecluster2-0.2.1/spherecluster/spherical_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,17 @@
 
 # from sklearn.cluster import _k_means
 from mlinsights.mlmodel import _kmeans_022 as _k_means
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import normalize
 from sklearn.utils import check_array, check_random_state
 from sklearn.utils.extmath import row_norms, squared_norm
-from sklearn.utils.validation import _num_samples
+from sklearn.utils.validation import _check_sample_weight, _num_samples
 
-from .regacy import (
-    _check_sample_weight,
-    _init_centroids,
-    _labels_inertia,
-    _tolerance,
-    _validate_center_shape,
-)
+from .legacy import _init_centroids, _labels_inertia, _tolerance, _validate_center_shape
 
 
 def _spherical_kmeans_single_lloyd(
     X: np.ndarray,
     n_clusters: int,
     sample_weight=None,
     max_iter=300,
```

### Comparing `spherecluster2-0.2.0/spherecluster/util.py` & `spherecluster2-0.2.1/spherecluster/util.py`

 * *Files identical despite different names*

### Comparing `spherecluster2-0.2.0/spherecluster/von_mises_fisher_mixture.py` & `spherecluster2-0.2.1/spherecluster/von_mises_fisher_mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sklearn.metrics.pairwise import cosine_distances
 from sklearn.preprocessing import normalize
 from sklearn.utils import as_float_array, check_array, check_random_state
 from sklearn.utils.extmath import squared_norm
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted
 
 from . import spherical_kmeans
-from .regacy import _init_centroids, _tolerance, _validate_center_shape
+from .legacy import _init_centroids, _tolerance, _validate_center_shape
 
 MAX_CONTENTRATION = 1e10
 
 
 def _inertia_from_labels(X, centers, labels):
     """Compute inertia with cosine distance using known labels."""
     n_examples, n_features = X.shape
```

### Comparing `spherecluster2-0.2.0/spherecluster2.egg-info/PKG-INFO` & `spherecluster2-0.2.1/spherecluster2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherecluster2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Clustering on the unit hypersphere in scikit-learn.
 Home-page: https://github.com/miquelmassot/spherecluster
 Author: Jason Laska
 Author-email: jason@claralabs.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: MIT
```

