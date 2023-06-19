# Comparing `tmp/dist_matrix-1.0.3.tar.gz` & `tmp/dist_matrix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist_matrix-1.0.3.tar", last modified: Mon Jun 19 09:57:01 2023, max compression
+gzip compressed data, was "dist_matrix-1.0.4.tar", last modified: Mon Jun 19 10:03:51 2023, max compression
```

## Comparing `dist_matrix-1.0.3.tar` & `dist_matrix-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1818 2021-10-30 20:05:16.211001 dist_matrix-1.0.3/.gitignore
--rw-r--r--   0        0        0     1090 2021-10-30 11:27:53.497338 dist_matrix-1.0.3/LICENSE
--rw-r--r--   0        0        0     2453 2023-06-19 09:53:51.219868 dist_matrix-1.0.3/README.md
--rw-r--r--   0        0        0       99 2023-06-19 09:56:58.917678 dist_matrix-1.0.3/dist_matrix/__init__.py
--rw-r--r--   0        0        0    16710 2021-10-30 16:29:07.652026 dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix.py
--rw-r--r--   0        0        0    23155 2021-10-30 16:29:03.023391 dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix_full.py
--rw-r--r--   0        0        0      876 2021-10-30 20:06:55.108414 dist_matrix-1.0.3/dist_matrix/meta.yaml
--rw-r--r--   0        0        0    18176 2021-10-30 16:29:13.442654 dist_matrix-1.0.3/dist_matrix/njit_dist_matrix.py
--rw-r--r--   0        0        0    20277 2021-10-30 19:55:40.593273 dist_matrix-1.0.3/dist_matrix/njit_dist_matrix_full.py
--rw-r--r--   0        0        0     2410 2021-10-30 16:42:23.832191 dist_matrix-1.0.3/dist_matrix/tests/test_cpu_helper.py
--rw-r--r--   0        0        0    12028 2021-10-30 16:43:07.867967 dist_matrix-1.0.3/dist_matrix/tests/test_dist_matrix.py
--rw-r--r--   0        0        0     2542 2021-10-23 23:13:29.425179 dist_matrix-1.0.3/dist_matrix/tests/test_helper.py
--rw-r--r--   0        0        0     9026 2021-10-30 16:42:14.875693 dist_matrix-1.0.3/dist_matrix/tests/test_njit.py
--rw-r--r--   0        0        0      839 2021-10-30 16:42:50.266489 dist_matrix-1.0.3/dist_matrix/utils/Timer.py
--rw-r--r--   0        0        0     1732 2021-10-23 23:13:29.405231 dist_matrix-1.0.3/dist_matrix/utils/benchmark_njit.py
--rw-r--r--   0        0        0     7587 2021-10-23 23:13:29.406229 dist_matrix-1.0.3/dist_matrix/utils/cpu_helper.py
--rw-r--r--   0        0        0    10158 2021-10-30 17:25:51.668914 dist_matrix-1.0.3/dist_matrix/utils/cpu_metrics.py
--rw-r--r--   0        0        0     7798 2021-10-23 23:13:29.407226 dist_matrix-1.0.3/dist_matrix/utils/helper.py
--rw-r--r--   0        0        0    10775 2021-10-23 23:13:29.412213 dist_matrix-1.0.3/dist_matrix/utils/metrics.py
--rw-r--r--   0        0        0      349 2021-10-30 20:10:37.506115 dist_matrix-1.0.3/fixup_grayskull.py
--rw-r--r--   0        0        0      847 2021-10-30 17:25:59.461944 dist_matrix-1.0.3/meta.yaml
--rw-r--r--   0        0        0      491 2023-06-19 09:53:51.224867 dist_matrix-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       44 2021-10-30 11:57:21.829642 dist_matrix-1.0.3/requirements.txt
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 dist_matrix-1.0.3/setup.py
--rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 dist_matrix-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1818 2021-10-30 20:05:16.211001 dist_matrix-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1090 2021-10-30 11:27:53.497338 dist_matrix-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2453 2023-06-19 09:53:51.219868 dist_matrix-1.0.4/README.md
+-rw-r--r--   0        0        0       99 2023-06-19 10:03:26.351443 dist_matrix-1.0.4/dist_matrix/__init__.py
+-rw-r--r--   0        0        0    16710 2021-10-30 16:29:07.652026 dist_matrix-1.0.4/dist_matrix/cuda_dist_matrix.py
+-rw-r--r--   0        0        0    23155 2021-10-30 16:29:03.023391 dist_matrix-1.0.4/dist_matrix/cuda_dist_matrix_full.py
+-rw-r--r--   0        0        0      876 2023-06-19 10:03:45.880456 dist_matrix-1.0.4/dist_matrix/meta.yaml
+-rw-r--r--   0        0        0    18176 2021-10-30 16:29:13.442654 dist_matrix-1.0.4/dist_matrix/njit_dist_matrix.py
+-rw-r--r--   0        0        0    20277 2021-10-30 19:55:40.593273 dist_matrix-1.0.4/dist_matrix/njit_dist_matrix_full.py
+-rw-r--r--   0        0        0     2410 2021-10-30 16:42:23.832191 dist_matrix-1.0.4/dist_matrix/tests/test_cpu_helper.py
+-rw-r--r--   0        0        0    12028 2021-10-30 16:43:07.867967 dist_matrix-1.0.4/dist_matrix/tests/test_dist_matrix.py
+-rw-r--r--   0        0        0     2542 2021-10-23 23:13:29.425179 dist_matrix-1.0.4/dist_matrix/tests/test_helper.py
+-rw-r--r--   0        0        0     9026 2021-10-30 16:42:14.875693 dist_matrix-1.0.4/dist_matrix/tests/test_njit.py
+-rw-r--r--   0        0        0      839 2021-10-30 16:42:50.266489 dist_matrix-1.0.4/dist_matrix/utils/Timer.py
+-rw-r--r--   0        0        0     1732 2021-10-23 23:13:29.405231 dist_matrix-1.0.4/dist_matrix/utils/benchmark_njit.py
+-rw-r--r--   0        0        0     7587 2021-10-23 23:13:29.406229 dist_matrix-1.0.4/dist_matrix/utils/cpu_helper.py
+-rw-r--r--   0        0        0    10158 2021-10-30 17:25:51.668914 dist_matrix-1.0.4/dist_matrix/utils/cpu_metrics.py
+-rw-r--r--   0        0        0     7798 2021-10-23 23:13:29.407226 dist_matrix-1.0.4/dist_matrix/utils/helper.py
+-rw-r--r--   0        0        0    10775 2021-10-23 23:13:29.412213 dist_matrix-1.0.4/dist_matrix/utils/metrics.py
+-rw-r--r--   0        0        0      349 2021-10-30 20:10:37.506115 dist_matrix-1.0.4/fixup_grayskull.py
+-rw-r--r--   0        0        0      847 2023-06-19 10:00:15.529440 dist_matrix-1.0.4/meta.yaml
+-rw-r--r--   0        0        0      491 2023-06-19 10:02:45.798702 dist_matrix-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       44 2021-10-30 11:57:21.829642 dist_matrix-1.0.4/requirements.txt
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 dist_matrix-1.0.4/setup.py
+-rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 dist_matrix-1.0.4/PKG-INFO
```

### Comparing `dist_matrix-1.0.3/.gitignore` & `dist_matrix-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/LICENSE` & `dist_matrix-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/README.md` & `dist_matrix-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix.py` & `dist_matrix-1.0.4/dist_matrix/cuda_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/cuda_dist_matrix_full.py` & `dist_matrix-1.0.4/dist_matrix/cuda_dist_matrix_full.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/meta.yaml` & `dist_matrix-1.0.4/dist_matrix/meta.yaml`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/njit_dist_matrix.py` & `dist_matrix-1.0.4/dist_matrix/njit_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/njit_dist_matrix_full.py` & `dist_matrix-1.0.4/dist_matrix/njit_dist_matrix_full.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/tests/test_cpu_helper.py` & `dist_matrix-1.0.4/dist_matrix/tests/test_cpu_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/tests/test_dist_matrix.py` & `dist_matrix-1.0.4/dist_matrix/tests/test_dist_matrix.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/tests/test_helper.py` & `dist_matrix-1.0.4/dist_matrix/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/tests/test_njit.py` & `dist_matrix-1.0.4/dist_matrix/tests/test_njit.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/Timer.py` & `dist_matrix-1.0.4/dist_matrix/utils/Timer.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/benchmark_njit.py` & `dist_matrix-1.0.4/dist_matrix/utils/benchmark_njit.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/cpu_helper.py` & `dist_matrix-1.0.4/dist_matrix/utils/cpu_helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/cpu_metrics.py` & `dist_matrix-1.0.4/dist_matrix/utils/cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/helper.py` & `dist_matrix-1.0.4/dist_matrix/utils/helper.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/dist_matrix/utils/metrics.py` & `dist_matrix-1.0.4/dist_matrix/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/meta.yaml` & `dist_matrix-1.0.4/meta.yaml`

 * *Files identical despite different names*

### Comparing `dist_matrix-1.0.3/setup.py` & `dist_matrix-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 package_data = \
 {'': ['*'], 'dist_matrix': ['tests/*', 'utils/*']}
 
 install_requires = \
 ['numpy', 'scipy', 'numba>=0.53.1']
 
 setup(name='dist_matrix',
-      version='1.0.3',
+      version='1.0.4',
       description='Predict materials properties using only the composition information.',
       author=None,
       author_email='"Sterling G. Baird" <sterling.baird@utah.edu>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `dist_matrix-1.0.3/PKG-INFO` & `dist_matrix-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dist_matrix
-Version: 1.0.3
+Version: 1.0.4
 Summary: Predict materials properties using only the composition information.
 Author-email: "Sterling G. Baird" <sterling.baird@utah.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
```

