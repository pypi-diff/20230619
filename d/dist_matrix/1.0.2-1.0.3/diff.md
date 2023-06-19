# Comparing `tmp/dist_matrix-1.0.2.tar.gz` & `tmp/dist_matrix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist_matrix-1.0.2.tar", last modified: Sat Oct 30 20:05:21 2021, max compression
+gzip compressed data, was "dist_matrix-1.0.3.tar", last modified: Mon Jun 19 09:57:01 2023, max compression
```

## Comparing `dist_matrix-1.0.2.tar` & `dist_matrix-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1818 2021-10-30 20:05:16.211001 dist_matrix-1.0.2/.gitignore
--rw-r--r--   0        0        0     1090 2021-10-30 11:27:53.497338 dist_matrix-1.0.2/LICENSE
--rw-r--r--   0        0        0      146 2021-10-30 11:27:53.498334 dist_matrix-1.0.2/README.md
--rw-r--r--   0        0        0       99 2021-10-30 19:56:03.645612 dist_matrix-1.0.2/dist_matrix/__init__.py
--rw-r--r--   0        0        0    16710 2021-10-30 16:29:07.652026 dist_matrix-1.0.2/dist_matrix/cuda_dist_matrix.py
--rw-r--r--   0        0        0    23155 2021-10-30 16:29:03.023391 dist_matrix-1.0.2/dist_matrix/cuda_dist_matrix_full.py
--rw-r--r--   0        0        0      852 2021-10-30 20:01:11.602048 dist_matrix-1.0.2/dist_matrix/meta.yaml
--rw-r--r--   0        0        0    18176 2021-10-30 16:29:13.442654 dist_matrix-1.0.2/dist_matrix/njit_dist_matrix.py
--rw-r--r--   0        0        0    20277 2021-10-30 19:55:40.593273 dist_matrix-1.0.2/dist_matrix/njit_dist_matrix_full.py
--rw-r--r--   0        0        0     2410 2021-10-30 16:42:23.832191 dist_matrix-1.0.2/dist_matrix/tests/test_cpu_helper.py
--rw-r--r--   0        0        0    12028 2021-10-30 16:43:07.867967 dist_matrix-1.0.2/dist_matrix/tests/test_dist_matrix.py
--rw-r--r--   0        0        0     2542 2021-10-23 23:13:29.425179 dist_matrix-1.0.2/dist_matrix/tests/test_helper.py
--rw-r--r--   0        0        0     9026 2021-10-30 16:42:14.875693 dist_matrix-1.0.2/dist_matrix/tests/test_njit.py
--rw-r--r--   0        0        0      839 2021-10-30 16:42:50.266489 dist_matrix-1.0.2/dist_matrix/utils/Timer.py
--rw-r--r--   0        0        0     1732 2021-10-23 23:13:29.405231 dist_matrix-1.0.2/dist_matrix/utils/benchmark_njit.py
--rw-r--r--   0        0        0     7587 2021-10-23 23:13:29.406229 dist_matrix-1.0.2/dist_matrix/utils/cpu_helper.py
--rw-r--r--   0        0        0    10158 2021-10-30 17:25:51.668914 dist_matrix-1.0.2/dist_matrix/utils/cpu_metrics.py
--rw-r--r--   0        0        0     7798 2021-10-23 23:13:29.407226 dist_matrix-1.0.2/dist_matrix/utils/helper.py
--rw-r--r--   0        0        0    10775 2021-10-23 23:13:29.412213 dist_matrix-1.0.2/dist_matrix/utils/metrics.py
--rw-r--r--   0        0        0      349 2021-10-30 20:04:58.965258 dist_matrix-1.0.2/fixup_grayskull.py
--rw-r--r--   0        0        0      847 2021-10-30 17:25:59.461944 dist_matrix-1.0.2/meta.yaml
--rw-r--r--   0        0        0      497 2021-10-30 20:03:27.316082 dist_matrix-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2021-10-30 11:57:21.829642 dist_matrix-1.0.2/requirements.txt
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 dist_matrix-1.0.2/setup.py
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 dist_matrix-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1818 2021-10-30 20:05:16.211001 dist_matrix-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1090 2021-10-30 11:27:53.497338 dist_matrix-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2453 2023-06-19 09:53:51.219868 dist_matrix-1.0.3/README.md
+-rw-r--r--   0        0        0       99 2023-06-19 09:56:58.917678 dist_matrix-1.0.3/dist_matrix/__init__.py
+-rw-r--r--   0        0        0    16710 2021-10-30 16:29:07.652026 dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix.py
+-rw-r--r--   0        0        0    23155 2021-10-30 16:29:03.023391 dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix_full.py
+-rw-r--r--   0        0        0      876 2021-10-30 20:06:55.108414 dist_matrix-1.0.3/dist_matrix/meta.yaml
+-rw-r--r--   0        0        0    18176 2021-10-30 16:29:13.442654 dist_matrix-1.0.3/dist_matrix/njit_dist_matrix.py
+-rw-r--r--   0        0        0    20277 2021-10-30 19:55:40.593273 dist_matrix-1.0.3/dist_matrix/njit_dist_matrix_full.py
+-rw-r--r--   0        0        0     2410 2021-10-30 16:42:23.832191 dist_matrix-1.0.3/dist_matrix/tests/test_cpu_helper.py
+-rw-r--r--   0        0        0    12028 2021-10-30 16:43:07.867967 dist_matrix-1.0.3/dist_matrix/tests/test_dist_matrix.py
+-rw-r--r--   0        0        0     2542 2021-10-23 23:13:29.425179 dist_matrix-1.0.3/dist_matrix/tests/test_helper.py
+-rw-r--r--   0        0        0     9026 2021-10-30 16:42:14.875693 dist_matrix-1.0.3/dist_matrix/tests/test_njit.py
+-rw-r--r--   0        0        0      839 2021-10-30 16:42:50.266489 dist_matrix-1.0.3/dist_matrix/utils/Timer.py
+-rw-r--r--   0        0        0     1732 2021-10-23 23:13:29.405231 dist_matrix-1.0.3/dist_matrix/utils/benchmark_njit.py
+-rw-r--r--   0        0        0     7587 2021-10-23 23:13:29.406229 dist_matrix-1.0.3/dist_matrix/utils/cpu_helper.py
+-rw-r--r--   0        0        0    10158 2021-10-30 17:25:51.668914 dist_matrix-1.0.3/dist_matrix/utils/cpu_metrics.py
+-rw-r--r--   0        0        0     7798 2021-10-23 23:13:29.407226 dist_matrix-1.0.3/dist_matrix/utils/helper.py
+-rw-r--r--   0        0        0    10775 2021-10-23 23:13:29.412213 dist_matrix-1.0.3/dist_matrix/utils/metrics.py
+-rw-r--r--   0        0        0      349 2021-10-30 20:10:37.506115 dist_matrix-1.0.3/fixup_grayskull.py
+-rw-r--r--   0        0        0      847 2021-10-30 17:25:59.461944 dist_matrix-1.0.3/meta.yaml
+-rw-r--r--   0        0        0      491 2023-06-19 09:53:51.224867 dist_matrix-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2021-10-30 11:57:21.829642 dist_matrix-1.0.3/requirements.txt
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 dist_matrix-1.0.3/setup.py
+-rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 dist_matrix-1.0.3/PKG-INFO
```

### Comparing `dist_matrix-1.0.2/.gitignore` & `dist_matrix-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/LICENSE` & `dist_matrix-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/cuda_dist_matrix.py` & `dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/cuda_dist_matrix_full.py` & `dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix_full.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/njit_dist_matrix.py` & `dist_matrix-1.0.3/dist_matrix/njit_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/njit_dist_matrix_full.py` & `dist_matrix-1.0.3/dist_matrix/njit_dist_matrix_full.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/tests/test_cpu_helper.py` & `dist_matrix-1.0.3/dist_matrix/tests/test_cpu_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/tests/test_dist_matrix.py` & `dist_matrix-1.0.3/dist_matrix/tests/test_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/tests/test_helper.py` & `dist_matrix-1.0.3/dist_matrix/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/tests/test_njit.py` & `dist_matrix-1.0.3/dist_matrix/tests/test_njit.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/Timer.py` & `dist_matrix-1.0.3/dist_matrix/utils/Timer.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/benchmark_njit.py` & `dist_matrix-1.0.3/dist_matrix/utils/benchmark_njit.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/cpu_helper.py` & `dist_matrix-1.0.3/dist_matrix/utils/cpu_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/cpu_metrics.py` & `dist_matrix-1.0.3/dist_matrix/utils/cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/helper.py` & `dist_matrix-1.0.3/dist_matrix/utils/helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/dist_matrix/utils/metrics.py` & `dist_matrix-1.0.3/dist_matrix/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/meta.yaml` & `dist_matrix-1.0.3/meta.yaml`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.2/setup.py` & `dist_matrix-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 package_data = \
 {'': ['*'], 'dist_matrix': ['tests/*', 'utils/*']}
 
 install_requires = \
 ['numpy', 'scipy', 'numba>=0.53.1']
 
 setup(name='dist_matrix',
-      version='1.0.2',
+      version='1.0.3',
       description='Predict materials properties using only the composition information.',
       author=None,
       author_email='"Sterling G. Baird" <sterling.baird@utah.edu>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
-      python_requires='>=3.7,<3.10',
+      python_requires='>=3.7',
      )
```

