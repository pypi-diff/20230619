# Comparing `tmp/scikit-datasets-0.2.2.tar.gz` & `tmp/scikit-datasets-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-datasets-0.2.2.tar", last modified: Thu Dec 29 09:38:32 2022, max compression
+gzip compressed data, was "scikit-datasets-0.2.3.tar", last modified: Mon Jun 19 21:43:22 2023, max compression
```

## Comparing `scikit-datasets-0.2.2.tar` & `scikit-datasets-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:32.182932 scikit-datasets-0.2.2/
--rw-------   0 david     (1000) david     (1000)     1094 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     4251 2022-12-29 09:38:32.183930 scikit-datasets-0.2.2/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1693 2022-12-29 09:34:56.000000 scikit-datasets-0.2.2/README.md
--rw-r--r--   0 david     (1000) david     (1000)     1760 2022-12-29 09:35:52.000000 scikit-datasets-0.2.2/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:29.211409 scikit-datasets-0.2.2/scikit_datasets.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     4251 2022-12-29 09:38:28.000000 scikit-datasets-0.2.2/scikit_datasets.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1596 2022-12-29 09:38:28.000000 scikit-datasets-0.2.2/scikit_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-12-29 09:38:28.000000 scikit-datasets-0.2.2/scikit_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-29 09:38:28.000000 scikit-datasets-0.2.2/scikit_datasets.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       11 2022-12-29 09:38:28.000000 scikit-datasets-0.2.2/scikit_datasets.egg-info/top_level.txt
--rw-------   0 david     (1000) david     (1000)      377 2022-12-29 09:38:32.195935 scikit-datasets-0.2.2/setup.cfg
--rwx------   0 david     (1000) david     (1000)      132 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:29.262307 scikit-datasets-0.2.2/skdatasets/
--rw-------   0 david     (1000) david     (1000)      115 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/skdatasets/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:30.250326 scikit-datasets-0.2.2/skdatasets/repositories/
--rw-------   0 david     (1000) david     (1000)      895 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/skdatasets/repositories/__init__.py
--rw-------   0 david     (1000) david     (1000)     3023 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/skdatasets/repositories/aneurisk.py
--rw-r--r--   0 david     (1000) david     (1000)     9199 2022-12-28 23:06:13.000000 scikit-datasets-0.2.2/skdatasets/repositories/base.py
--rw-------   0 david     (1000) david     (1000)    11900 2022-11-12 23:05:39.000000 scikit-datasets-0.2.2/skdatasets/repositories/cran.py
--rw-------   0 david     (1000) david     (1000)     2773 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/forex.py
--rw-r--r--   0 david     (1000) david     (1000)     9496 2022-12-28 23:06:13.000000 scikit-datasets-0.2.2/skdatasets/repositories/keel.py
--rw-------   0 david     (1000) david     (1000)     2426 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/keras.py
--rw-------   0 david     (1000) david     (1000)     6436 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/libsvm.py
--rw-------   0 david     (1000) david     (1000)     6747 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/physionet.py
--rw-------   0 david     (1000) david     (1000)     4855 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/raetsch.py
--rw-r--r--   0 david     (1000) david     (1000)     3672 2022-12-28 23:06:13.000000 scikit-datasets-0.2.2/skdatasets/repositories/sklearn.py
--rw-------   0 david     (1000) david     (1000)     4991 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/uci.py
--rw-------   0 david     (1000) david     (1000)     4862 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/repositories/ucr.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:30.347322 scikit-datasets-0.2.2/skdatasets/tests/
--rw-------   0 david     (1000) david     (1000)        0 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:31.344641 scikit-datasets-0.2.2/skdatasets/tests/repositories/
--rw-------   0 david     (1000) david     (1000)     1351 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/__init__.py
--rw-------   0 david     (1000) david     (1000)      310 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_cran.py
--rw-------   0 david     (1000) david     (1000)      854 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_forex.py
--rw-------   0 david     (1000) david     (1000)     1655 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_keel.py
--rw-------   0 david     (1000) david     (1000)      898 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_keras.py
--rw-------   0 david     (1000) david     (1000)     2598 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_libsvm.py
--rw-------   0 david     (1000) david     (1000)     1259 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_physionet.py
--rw-------   0 david     (1000) david     (1000)      728 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_raetsch.py
--rw-------   0 david     (1000) david     (1000)      503 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_sklearn.py
--rw-------   0 david     (1000) david     (1000)      647 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_uci.py
--rw-------   0 david     (1000) david     (1000)      754 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/repositories/test_ucr.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:31.938933 scikit-datasets-0.2.2/skdatasets/tests/utils/
--rw-------   0 david     (1000) david     (1000)        0 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/__init__.py
--rw-------   0 david     (1000) david     (1000)      142 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/linear_model.py
--rwx------   0 david     (1000) david     (1000)     1197 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/run.py
--rw-------   0 david     (1000) david     (1000)      607 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/test_estimator.py
--rw-r--r--   0 david     (1000) david     (1000)     4970 2022-12-28 23:06:13.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/test_experiment.py
--rw-------   0 david     (1000) david     (1000)     2073 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/test_run.py
--rw-------   0 david     (1000) david     (1000)     2213 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/tests/utils/test_scores.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-12-29 09:38:32.146935 scikit-datasets-0.2.2/skdatasets/utils/
--rw-------   0 david     (1000) david     (1000)        0 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/utils/__init__.py
--rw-------   0 david     (1000) david     (1000)      760 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/utils/estimator.py
--rwx------   0 david     (1000) david     (1000)    25520 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/utils/experiment.py
--rw-------   0 david     (1000) david     (1000)    19239 2022-11-12 23:05:40.000000 scikit-datasets-0.2.2/skdatasets/utils/scores.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.228542 scikit-datasets-0.2.3/
+-rw-------   0 david     (1000) david     (1000)     1094 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     4060 2023-06-19 21:43:22.229545 scikit-datasets-0.2.3/PKG-INFO
+-rw-------   0 david     (1000) david     (1000)     1451 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/README.md
+-rw-r--r--   0 david     (1000) david     (1000)     1788 2023-06-19 21:40:43.000000 scikit-datasets-0.2.3/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:20.844542 scikit-datasets-0.2.3/scikit_datasets.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     4060 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     1596 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)      391 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       11 2023-06-19 21:43:20.000000 scikit-datasets-0.2.3/scikit_datasets.egg-info/top_level.txt
+-rw-------   0 david     (1000) david     (1000)      377 2023-06-19 21:43:22.236544 scikit-datasets-0.2.3/setup.cfg
+-rwx------   0 david     (1000) david     (1000)      132 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:20.866542 scikit-datasets-0.2.3/skdatasets/
+-rw-------   0 david     (1000) david     (1000)      115 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.233543 scikit-datasets-0.2.3/skdatasets/repositories/
+-rw-------   0 david     (1000) david     (1000)      918 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/__init__.py
+-rw-------   0 david     (1000) david     (1000)     3039 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/aneurisk.py
+-rw-------   0 david     (1000) david     (1000)     9085 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/base.py
+-rw-------   0 david     (1000) david     (1000)    11861 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/cran.py
+-rw-------   0 david     (1000) david     (1000)     2774 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/forex.py
+-rw-------   0 david     (1000) david     (1000)     9579 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/keel.py
+-rw-------   0 david     (1000) david     (1000)     2426 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/keras.py
+-rw-------   0 david     (1000) david     (1000)     6645 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/libsvm.py
+-rw-------   0 david     (1000) david     (1000)     6713 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/physionet.py
+-rw-------   0 david     (1000) david     (1000)     4939 2023-03-23 22:36:09.000000 scikit-datasets-0.2.3/skdatasets/repositories/raetsch.py
+-rw-------   0 david     (1000) david     (1000)     3244 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/repositories/sklearn.py
+-rw-------   0 david     (1000) david     (1000)     4960 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/repositories/uci.py
+-rw-r--r--   0 david     (1000) david     (1000)     4852 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/repositories/ucr.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.261553 scikit-datasets-0.2.3/skdatasets/tests/
+-rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/__init__.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:21.720542 scikit-datasets-0.2.3/skdatasets/tests/repositories/
+-rw-------   0 david     (1000) david     (1000)     1254 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/__init__.py
+-rw-------   0 david     (1000) david     (1000)      310 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_cran.py
+-rw-------   0 david     (1000) david     (1000)      928 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_forex.py
+-rw-------   0 david     (1000) david     (1000)     1655 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keel.py
+-rw-------   0 david     (1000) david     (1000)      867 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keras.py
+-rw-------   0 david     (1000) david     (1000)     2776 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_libsvm.py
+-rw-------   0 david     (1000) david     (1000)     1259 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_physionet.py
+-rw-------   0 david     (1000) david     (1000)      728 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_raetsch.py
+-rw-------   0 david     (1000) david     (1000)      503 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_sklearn.py
+-rw-------   0 david     (1000) david     (1000)      647 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_uci.py
+-rw-------   0 david     (1000) david     (1000)      754 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/repositories/test_ucr.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.049544 scikit-datasets-0.2.3/skdatasets/tests/utils/
+-rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/__init__.py
+-rw-------   0 david     (1000) david     (1000)      142 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/linear_model.py
+-rwx------   0 david     (1000) david     (1000)     1180 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/run.py
+-rw-------   0 david     (1000) david     (1000)      609 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_estimator.py
+-rw-r--r--   0 david     (1000) david     (1000)     6083 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_experiment.py
+-rw-------   0 david     (1000) david     (1000)     2714 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_run.py
+-rw-------   0 david     (1000) david     (1000)     2303 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/tests/utils/test_scores.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-06-19 21:43:22.198543 scikit-datasets-0.2.3/skdatasets/utils/
+-rw-------   0 david     (1000) david     (1000)        0 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/utils/__init__.py
+-rw-------   0 david     (1000) david     (1000)      760 2023-03-23 22:36:10.000000 scikit-datasets-0.2.3/skdatasets/utils/estimator.py
+-rwxr-xr-x   0 david     (1000) david     (1000)    26235 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/utils/experiment.py
+-rw-r--r--   0 david     (1000) david     (1000)    19341 2023-06-19 21:36:27.000000 scikit-datasets-0.2.3/skdatasets/utils/scores.py
```

### Comparing `scikit-datasets-0.2.2/LICENSE` & `scikit-datasets-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.2/PKG-INFO` & `scikit-datasets-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-datasets
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scikit-learn-compatible datasets
 Author-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 Maintainer-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 David Díaz Vico
         
@@ -25,22 +25,23 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/daviddiazvico/scikit-datasets
 Project-URL: documentation, https://daviddiazvico.github.io/scikit-datasets/
 Project-URL: repository, https://github.com/daviddiazvico/scikit-datasets
-Project-URL: download, https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.1.tar.gz
+Project-URL: download, https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.2.tar.gz
 Keywords: scikit-learn,datasets,repository,benchmark,Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cran
 Provides-Extra: forex
 Provides-Extra: keel
 Provides-Extra: keras
 Provides-Extra: physionet
@@ -54,15 +55,14 @@
 # scikit-datasets
 Scikit-learn-compatible datasets
 
 ## Status
 [![Tests](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml/badge.svg)](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/maintainability)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/test_coverage)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/test_coverage)
-[![Build Status](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_apis/build/status/daviddiazvico.scikit-datasets?branchName=master)](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_build/latest?definitionId=1&branchName=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6383047.svg)](https://doi.org/10.5281/zenodo.6383047)
 
 ## Installation
 Available in [PyPI](https://pypi.python.org/pypi?:action=display&name=scikit-datasets)
 ```
 pip install scikit-datasets
 ```
```

### Comparing `scikit-datasets-0.2.2/README.md` & `scikit-datasets-0.2.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # scikit-datasets
 Scikit-learn-compatible datasets
 
 ## Status
 [![Tests](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml/badge.svg)](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/maintainability)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/test_coverage)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/test_coverage)
-[![Build Status](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_apis/build/status/daviddiazvico.scikit-datasets?branchName=master)](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_build/latest?definitionId=1&branchName=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6383047.svg)](https://doi.org/10.5281/zenodo.6383047)
 
 ## Installation
 Available in [PyPI](https://pypi.python.org/pypi?:action=display&name=scikit-datasets)
 ```
 pip install scikit-datasets
 ```
```

### Comparing `scikit-datasets-0.2.2/pyproject.toml` & `scikit-datasets-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-datasets"
-version = "0.2.2"
+version = "0.2.3"
 description = "Scikit-learn-compatible datasets"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["scikit-learn", "datasets", "repository", "benchmark", "Python"]
 authors = [
   {name = "David Diaz Vico", email = "david.diaz.vico@outlook.com"},
@@ -17,41 +17,29 @@
 classifiers = [
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
-
-dependencies = [
-  "numpy",
-  "scipy",
-  "scikit-learn",
-]
-
+dependencies = ["numpy", "scipy", "scikit-learn"]
 [project.optional-dependencies]
 cran = ["rdata"]
 forex = ["forex_python>=1.6"]
 keel = ["pandas"]
 keras = ["tensorflow"]
 physionet = ["pandas", "wfdb"]
 utils-estimator = ["jsonpickle"]
 utils-experiments = ["sacred", "incense"]
 utils-scores = ["statsmodels", "jinja2"]
-all = ["scikit-datasets[cran,forex,keel,keras,physionet,utils-estimator,utils-experiments,utils-scores]"]
-test = [
-  "pytest",
-  "pytest-cov[all]",
-  "coverage",
-  "scikit-datasets[all]",
-]
-
+all = ["scikit-datasets[cran, forex, keel, keras, physionet, utils-estimator, utils-experiments, utils-scores]"]
+test = ["pytest", "pytest-cov[all]", "coverage", "scikit-datasets[all]"]
 [project.urls]
 homepage = "https://github.com/daviddiazvico/scikit-datasets"
 documentation = "https://daviddiazvico.github.io/scikit-datasets/"
 repository = "https://github.com/daviddiazvico/scikit-datasets"
-download = "https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.1.tar.gz"
-
+download = "https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.2.tar.gz"
 [build-system]
 # Minimum requirements for the build system to execute.
-requires = ["setuptools", "wheel"]  # PEP 508 specifications.
+requires = ["setuptools", "wheel"]  # PEP 508 specifications.
```

### Comparing `scikit-datasets-0.2.2/scikit_datasets.egg-info/PKG-INFO` & `scikit-datasets-0.2.3/scikit_datasets.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-datasets
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scikit-learn-compatible datasets
 Author-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 Maintainer-email: David Diaz Vico <david.diaz.vico@outlook.com>, Carlos Ramos Carreño <vnmabus@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 David Díaz Vico
         
@@ -25,22 +25,23 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/daviddiazvico/scikit-datasets
 Project-URL: documentation, https://daviddiazvico.github.io/scikit-datasets/
 Project-URL: repository, https://github.com/daviddiazvico/scikit-datasets
-Project-URL: download, https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.1.tar.gz
+Project-URL: download, https://github.com/daviddiazvico/scikit-datasets/archive/v0.2.2.tar.gz
 Keywords: scikit-learn,datasets,repository,benchmark,Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cran
 Provides-Extra: forex
 Provides-Extra: keel
 Provides-Extra: keras
 Provides-Extra: physionet
@@ -54,15 +55,14 @@
 # scikit-datasets
 Scikit-learn-compatible datasets
 
 ## Status
 [![Tests](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml/badge.svg)](https://github.com/daviddiazvico/scikit-datasets/actions/workflows/tests.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/maintainability)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/a37c9ee152b41a0cb577/test_coverage)](https://codeclimate.com/github/daviddiazvico/scikit-datasets/test_coverage)
-[![Build Status](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_apis/build/status/daviddiazvico.scikit-datasets?branchName=master)](https://dev.azure.com/daviddiazvico0337/daviddiazvico/_build/latest?definitionId=1&branchName=master)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6383047.svg)](https://doi.org/10.5281/zenodo.6383047)
 
 ## Installation
 Available in [PyPI](https://pypi.python.org/pypi?:action=display&name=scikit-datasets)
 ```
 pip install scikit-datasets
 ```
```

### Comparing `scikit-datasets-0.2.2/scikit_datasets.egg-info/SOURCES.txt` & `scikit-datasets-0.2.3/scikit_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/__init__.py` & `scikit-datasets-0.2.3/skdatasets/repositories/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 """
 @author: David Diaz Vico
 @license: MIT
 """
 
 from . import aneurisk, libsvm, raetsch, sklearn, uci, ucr
 
-repos = {'libsvm': libsvm, 'raetsch': raetsch, 'sklearn': sklearn, 'uci': uci,
-         'ucr': ucr, 'aneurisk': aneurisk}
+repos = {
+    "libsvm": libsvm,
+    "raetsch": raetsch,
+    "sklearn": sklearn,
+    "uci": uci,
+    "ucr": ucr,
+    "aneurisk": aneurisk,
+}
 try:
     from . import cran
-    repos['cran'] = cran
+
+    repos["cran"] = cran
 except ImportError:
     pass
 try:
     from . import forex
-    repos['forex'] = forex
+
+    repos["forex"] = forex
 except ImportError:
     pass
 try:
     from . import keel
-    repos['keel'] = keel
+
+    repos["keel"] = keel
 except ImportError:
     pass
 try:
     from . import keras
-    repos['keras'] = keras
+
+    repos["keras"] = keras
 except ImportError:
     pass
 try:
     from . import physionet
-    repos['physionet'] = physionet
+
+    repos["physionet"] = physionet
 except ImportError:
     pass
 
 
 def fetch(repository, dataset, collection=None, **kwargs):
     if collection:
         data = repos[repository].fetch(collection, dataset, **kwargs)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/aneurisk.py` & `scikit-datasets-0.2.3/skdatasets/repositories/aneurisk.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,61 +22,63 @@
 def fetch(name="Aneurisk65", *, data_home=None, return_X_y=False):
 
     if name != "Aneurisk65":
         raise ValueError(f"Unknown dataset {name}")
 
     n_samples = 65
 
-    url = "http://ecm2.mathcs.emory.edu/aneuriskdata/files/Carotid-data_MBI_workshop.zip"
+    url = (
+        "http://ecm2.mathcs.emory.edu/aneuriskdata/files/Carotid-data_MBI_workshop.zip"
+    )
 
     dataset_path = fetch_zip(
         dataname=name,
         urlname=url,
         subfolder="aneurisk",
         data_home=data_home,
     )
 
     patient_dtype = [
-        ('patient', np.int_),
-        ('code', 'U8'),
-        ('type', 'U1'),
-        ('aneurysm location', np.float_),
-        ('left_right', 'U2'),
+        ("patient", np.int_),
+        ("code", "U8"),
+        ("type", "U1"),
+        ("aneurysm location", np.float_),
+        ("left_right", "U2"),
     ]
 
     functions_dtype = [
-        ('curvilinear abscissa', np.object_),
-        ('MISR', np.object_),
-        ('X0 observed', np.object_),
-        ('Y0 observed', np.object_),
-        ('Z0 observed', np.object_),
-        ('X0 observed FKS', np.object_),
-        ('Y0 observed FKS', np.object_),
-        ('Z0 observed FKS', np.object_),
-        ('X0 observed FKS reflected', np.object_),
-        ('X1 observed FKS', np.object_),
-        ('Y1 observed FKS', np.object_),
-        ('Z1 observed FKS', np.object_),
-        ('X1 observed FKS reflected', np.object_),
-        ('X2 observed FKS', np.object_),
-        ('Y2 observed FKS', np.object_),
-        ('Z2 observed FKS', np.object_),
-        ('X2 observed FKS reflected', np.object_),
-        ('Curvature FKS', np.object_),
+        ("curvilinear abscissa", np.object_),
+        ("MISR", np.object_),
+        ("X0 observed", np.object_),
+        ("Y0 observed", np.object_),
+        ("Z0 observed", np.object_),
+        ("X0 observed FKS", np.object_),
+        ("Y0 observed FKS", np.object_),
+        ("Z0 observed FKS", np.object_),
+        ("X0 observed FKS reflected", np.object_),
+        ("X1 observed FKS", np.object_),
+        ("Y1 observed FKS", np.object_),
+        ("Z1 observed FKS", np.object_),
+        ("X1 observed FKS reflected", np.object_),
+        ("X2 observed FKS", np.object_),
+        ("Y2 observed FKS", np.object_),
+        ("Z2 observed FKS", np.object_),
+        ("X2 observed FKS reflected", np.object_),
+        ("Curvature FKS", np.object_),
     ]
 
     complete_dtype = patient_dtype + functions_dtype
 
     X = np.zeros(shape=n_samples, dtype=complete_dtype)
 
     X[[p[0] for p in patient_dtype]] = np.genfromtxt(
-        dataset_path / 'Patients.txt',
+        dataset_path / "Patients.txt",
         dtype=patient_dtype,
         skip_header=1,
-        missing_values=('NA',),
+        missing_values=("NA",),
     )
 
     for i in range(n_samples):
         file = f"Rawdata_FKS_{i + 1}.txt"
 
         functions = np.genfromtxt(
             dataset_path / file,
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/base.py` & `scikit-datasets-0.2.3/skdatasets/repositories/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 raise DatasetNotFoundError(dataname) from e
             raise
         if data_url.length == 0:
             raise DatasetNotFoundError(dataname)
 
         # store file
         try:
-            with open(filename, 'w+b') as data_file:
+            with open(filename, "w+b") as data_file:
                 copyfileobj(data_url, data_file)
         except Exception:
             filename.unlink()
             raise
         data_url.close()
     return filename
 
@@ -126,33 +126,31 @@
 ) -> Sequence[Union[zipfile.ZipInfo, tarfile.TarInfo]]:
 
     if isinstance(compressed_file, zipfile.ZipFile):
 
         members_zip = compressed_file.infolist()
 
         return [
-            info for info in members_zip
+            info
+            for info in members_zip
             if not (data_home_path / info.filename).exists()
         ]
 
     members_tar = compressed_file.getmembers()
 
-    return [
-        info for info in members_tar
-        if not (data_home_path / info.name).exists()
-    ]
+    return [info for info in members_tar if not (data_home_path / info.name).exists()]
 
 
 def fetch_compressed(
     dataname: str,
     urlname: str,
     compression_open: OpenMethod,
     subfolder: Optional[str] = None,
     data_home: Optional[str] = None,
-    open_format: str = 'r',
+    open_format: str = "r",
 ) -> pathlib.Path:
     """Fetch compressed dataset.
 
     Fetch a compressed file from a given url, unzips and stores it in a given
     directory.
 
     Parameters
@@ -264,15 +262,15 @@
     """
     return fetch_compressed(
         dataname=dataname,
         urlname=urlname,
         compression_open=tarfile.open,
         subfolder=subfolder,
         data_home=data_home,
-        open_format='r:gz',
+        open_format="r:gz",
     )
 
 
 @overload
 def dataset_from_dataframe(
     frame: DataFrame,
     *,
@@ -354,46 +352,33 @@
 ) -> (
     Bunch
     | Tuple[np.typing.NDArray[float], np.typing.NDArray[int] | None]
     | Tuple[DataFrame, Series | DataFrame | None]
 ):
 
     data_dataframe = (
-        frame
-        if target_column is None
-        else frame.drop(target_column, axis=1)
-    )
-    target_dataframe = (
-        None
-        if target_column is None
-        else frame.loc[:, target_column]
+        frame if target_column is None else frame.drop(target_column, axis=1)
     )
+    target_dataframe = None if target_column is None else frame.loc[:, target_column]
 
-    data = (
-        data_dataframe
-        if as_frame is True
-        else data_dataframe.to_numpy()
-    )
+    data = data_dataframe if as_frame is True else data_dataframe.to_numpy()
 
     target = (
         None
         if target_dataframe is None
-        else target_dataframe if as_frame is True
+        else target_dataframe
+        if as_frame is True
         else target_dataframe.to_numpy()
     )
 
     if return_X_y:
         return data, target
 
     feature_names = list(data_dataframe.keys())
-    target_names = (
-        None
-        if target_dataframe is None
-        else list(target_dataframe.keys())
-    )
+    target_names = None if target_dataframe is None else list(target_dataframe.keys())
 
     bunch = Bunch(
         data=data,
         target=target,
         DESCR=DESCR,
         feature_names=feature_names,
         target_names=target_names,
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/cran.py` & `scikit-datasets-0.2.3/skdatasets/repositories/cran.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """Class for parsing the version in the CRAN package information page."""
 
     def __init__(self, *, convert_charrefs: bool = True) -> None:
         super().__init__(convert_charrefs=convert_charrefs)
 
         self.last_is_version = False
         self.version: str | None = None
-        self.version_regex = re.compile('(?i).*version.*')
+        self.version_regex = re.compile("(?i).*version.*")
         self.handling_td = False
 
     def handle_starttag(
         self,
         tag: str,
         attrs: List[Tuple[str, str | None]],
     ) -> None:
@@ -74,15 +74,15 @@
     parser = _LatestVersionHTMLParser()
 
     url_request = urllib.request.Request(
         url=f"{CRAN_URL}/package={package_name}",
     )
     try:
         with urllib.request.urlopen(url_request) as url_file:
-            url_content = url_file.read().decode('utf-8')
+            url_content = url_file.read().decode("utf-8")
     except urllib.error.HTTPError as e:
         if e.code == 404:
             raise DatasetNotFoundError(f"{package_name}/{dataset_name}") from e
         raise
 
     parser.feed(url_content)
 
@@ -101,15 +101,15 @@
     """
     home = pathlib.Path(get_data_home())  # Should allow providing data home?
 
     downloaded_packages = tuple(home.glob(package_name + "_*.tar.gz"))
 
     if downloaded_packages:
         versions = [
-            LooseVersion(p.name[(len(package_name) + 1):-len(".tar.gz")])
+            LooseVersion(p.name[(len(package_name) + 1) : -len(".tar.gz")])
             for p in downloaded_packages
         ]
 
         versions.sort()
         latest_version = versions[-1]
 
         return str(latest_version)
@@ -149,23 +149,20 @@
 def _get_urls(
     package_name: str,
     *,
     dataset_name: str,
     version: str | None = None,
 ) -> Sequence[str]:
 
-    version = _get_version(
-        package_name, dataset_name=dataset_name, version=version)
+    version = _get_version(package_name, dataset_name=dataset_name, version=version)
 
     filename = f"{package_name}_{version}.tar.gz"
 
     latest_url = f"{CRAN_URL}/src/contrib/{filename}"
-    archive_url = (
-        f"{CRAN_URL}/src/contrib/Archive/{package_name}/{filename}"
-    )
+    archive_url = f"{CRAN_URL}/src/contrib/Archive/{package_name}/{filename}"
     return (latest_url, archive_url)
 
 
 def _download_package_data(
     package_name: str,
     *,
     dataset_name: str = "*",
@@ -187,15 +184,15 @@
         folder_name = os.path.basename(url_list[0])
 
     if subdir is None:
         subdir = "data"
 
     for i, url in enumerate(url_list):
         try:
-            directory = _fetch_tgz(folder_name, url, subfolder='cran')
+            directory = _fetch_tgz(folder_name, url, subfolder="cran")
             break
         except Exception:
             # If it is the last url, reraise
             if i >= len(url_list) - 1:
                 raise
 
     data_path = directory / package_name / subdir
@@ -262,16 +259,15 @@
 
     file_path = data_path / dataset_name
 
     if not file_path.suffix:
         possible_names = list(data_path.glob(dataset_name + ".*"))
         if len(possible_names) != 1:
             raise FileNotFoundError(
-                f"Dataset {dataset_name} not found in "
-                f"package {package_name}",
+                f"Dataset {dataset_name} not found in " f"package {package_name}",
             )
 
         file_path = data_path / possible_names[0]
 
     parsed = rdata.parser.parse_file(file_path)
 
     return converter.convert(parsed)
@@ -337,15 +333,15 @@
     if not data_path.exists():
         return {}
 
     all_datasets = {}
 
     for dataset in data_path.iterdir():
 
-        if dataset.suffix.lower() in ['.rda', '.rdata']:
+        if dataset.suffix.lower() in [".rda", ".rdata"]:
             try:
                 parsed = rdata.parser.parse_file(dataset)
 
                 converted = converter.convert(parsed)
 
                 all_datasets.update(converted)
             except Exception:
@@ -362,17 +358,17 @@
 
 class _DatasetArguments(TypedDict):
     load_args: Tuple[Sequence[Any], Mapping[str, Any]]
     sklearn_args: Tuple[Sequence[Any], Mapping[str, Any]]
 
 
 datasets: Mapping[str, _DatasetArguments] = {
-    'geyser': {
-        'load_args': (['geyser.rda', 'MASS'], {}),
-        'sklearn_args': ([], {'target_name': 'waiting'}),
+    "geyser": {
+        "load_args": (["geyser.rda", "MASS"], {}),
+        "sklearn_args": ([], {"target_name": "waiting"}),
     },
 }
 
 
 def _to_sklearn(
     dataset: Mapping[str, Any],
     *,
@@ -443,17 +439,17 @@
     -------
     data : Bunch
           Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
-    load_args = datasets[name]['load_args']
+    load_args = datasets[name]["load_args"]
     dataset = fetch_dataset(*load_args[0], **load_args[1])
 
-    sklearn_args = datasets[name]['sklearn_args']
+    sklearn_args = datasets[name]["sklearn_args"]
     sklearn_dataset = _to_sklearn(dataset, *sklearn_args[0], **sklearn_args[1])
 
     if return_X_y:
         return sklearn_dataset.data, sklearn_dataset.target
 
     return sklearn_dataset
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/forex.py` & `scikit-datasets-0.2.3/skdatasets/repositories/forex.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,38 +22,44 @@
     for d in range(delta.days + 1):
         day = start + timedelta(days=d)
         rate = get_rate(day)
         data.append(rate)
     return np.asarray(data).reshape((-1, 1))
 
 
-def _load_bitcoin(start=date(2015, 1, 1), end=date.today(), currency='EUR'):
+def _load_bitcoin(start=date(2015, 1, 1), end=date.today(), currency="EUR"):
     """Load bitcoin dataset"""
     btcc = BtcConverter()
 
     def get_rate(day):
         return btcc.get_previous_price(currency, day)
 
     return _fetch(get_rate, start=start, end=end)
 
 
-def _load_forex(start=date(2015, 1, 1), end=date.today(), currency_1='USD',
-                currency_2='EUR'):
+def _load_forex(
+    start=date(2015, 1, 1), end=date.today(), currency_1="USD", currency_2="EUR"
+):
     """Load forex dataset."""
     cr = CurrencyRates()
 
     def get_rate(day):
         time.sleep(0.1)
         return cr.get_rate(currency_1, currency_2, day)
 
     return _fetch(get_rate, start=start, end=end)
 
 
-def fetch(start=date(2015, 1, 1), end=date.today(), currency_1='USD',
-          currency_2='EUR', return_X_y=False):
+def fetch(
+    start=date(2015, 1, 1),
+    end=date.today(),
+    currency_1="USD",
+    currency_2="EUR",
+    return_X_y=False,
+):
     """Fetch Forex datasets.
 
     Fetches the ECB Forex and Coindesk Bitcoin datasets. More info at
     http://forex-python.readthedocs.io.
 
     Parameters
     ----------
@@ -72,25 +78,26 @@
     -------
     data : Bunch
         Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
-    if currency_1 == 'BTC':
+    if currency_1 == "BTC":
         X = _load_bitcoin(start=start, end=end, currency=currency_2)
-        descr = 'BTC-' + str(currency_2)
-    elif currency_2 == 'BTC':
+        descr = "BTC-" + str(currency_2)
+    elif currency_2 == "BTC":
         X = _load_bitcoin(start=start, end=end, currency=currency_1)
-        descr = 'BTC-' + str(currency_1)
+        descr = "BTC-" + str(currency_1)
     else:
-        X = _load_forex(start=start, end=end, currency_1=currency_1,
-                        currency_2=currency_2)
-        descr = str(currency_1) + '-' + str(currency_2)
-    descr = descr + start.strftime('%Y-%m-%d') + '-' + end.strftime('%Y-%m-%d')
+        X = _load_forex(
+            start=start, end=end, currency_1=currency_1, currency_2=currency_2
+        )
+        descr = str(currency_1) + "-" + str(currency_2)
+    descr = descr + start.strftime("%Y-%m-%d") + "-" + end.strftime("%Y-%m-%d")
 
     if return_X_y:
         return X, None
 
     return Bunch(
         data=X,
         target=None,
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/keel.py` & `scikit-datasets-0.2.3/skdatasets/repositories/keel.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 @author: David Diaz Vico
 @license: MIT
 """
 from __future__ import annotations
 
 import io
 import os
-import sys
 from pathlib import Path
 from types import MappingProxyType
 from typing import (
     AbstractSet,
     Any,
     Final,
     Iterator,
@@ -27,52 +26,54 @@
 
 import numpy as np
 import pandas as pd
 from sklearn.utils import Bunch
 
 from .base import fetch_file
 
-BASE_URL = 'http://sci2s.ugr.es/keel'
-COLLECTIONS: Final = frozenset((
-    'classification',
-    'missing',
-    'imbalanced',
-    'multiInstance',
-    'multilabel',
-    'textClassification',
-    'classNoise',
-    'attributeNoise',
-    'semisupervised',
-    'regression',
-    'timeseries',
-    'unsupervised',
-    'lowQuality',
-))
+BASE_URL = "http://sci2s.ugr.es/keel"
+COLLECTIONS: Final = frozenset(
+    (
+        "classification",
+        "missing",
+        "imbalanced",
+        "multiInstance",
+        "multilabel",
+        "textClassification",
+        "classNoise",
+        "attributeNoise",
+        "semisupervised",
+        "regression",
+        "timeseries",
+        "unsupervised",
+        "lowQuality",
+    )
+)
 
 
 # WTFs
 IMBALANCED_URLS: Final = (
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p1',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p2',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p3',
-    'dataset/data/imbalanced',
-    'keel-dataset/datasets/imbalanced/imb_noisyBordExamples',
-    'keel-dataset/datasets/imbalanced/preprocessed',
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p1",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p2",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p3",
+    "dataset/data/imbalanced",
+    "keel-dataset/datasets/imbalanced/imb_noisyBordExamples",
+    "keel-dataset/datasets/imbalanced/preprocessed",
 )
 
 IRREGULAR_DESCR_IMBALANCED_URLS: Final = (
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p1',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p2',
-    'keel-dataset/datasets/imbalanced/imb_IRhigherThan9p3',
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p1",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p2",
+    "keel-dataset/datasets/imbalanced/imb_IRhigherThan9p3",
 )
 
 INCORRECT_DESCR_IMBALANCED_URLS: Final = MappingProxyType(
-    {'semisupervised': 'classification'},
+    {"semisupervised": "classification"},
 )
 
 
 class KeelOuterCV(object):
     """Iterable over already separated CV partitions of the dataset."""
 
     def __init__(
@@ -83,30 +84,34 @@
         ys_test: Sequence[np.typing.NDArray[Union[int, float]]],
     ) -> None:
         self.Xs = Xs
         self.ys = ys
         self.Xs_test = Xs_test
         self.ys_test = ys_test
 
-    def __iter__(self) -> Iterator[Tuple[
-        np.typing.NDArray[float],
-        np.typing.NDArray[Union[int, float]],
-        np.typing.NDArray[float],
-        np.typing.NDArray[Union[int, float]],
-    ]]:
+    def __iter__(
+        self,
+    ) -> Iterator[
+        Tuple[
+            np.typing.NDArray[float],
+            np.typing.NDArray[Union[int, float]],
+            np.typing.NDArray[float],
+            np.typing.NDArray[Union[int, float]],
+        ]
+    ]:
         return zip(self.Xs, self.ys, self.Xs_test, self.ys_test)
 
 
 def _load_Xy(
     zipfile: Path,
     csvfile: str,
-    sep: str = ',',
+    sep: str = ",",
     header: Optional[int] = None,
-    engine: str = 'python',
-    na_values: AbstractSet[str] = frozenset(('?')),
+    engine: str = "python",
+    na_values: AbstractSet[str] = frozenset(("?")),
     **kwargs: Any,
 ) -> Tuple[np.typing.NDArray[float], np.typing.NDArray[Union[int, float]]]:
     """Load a zipped csv file with target in the last column."""
     with ZipFile(zipfile) as z:
         with z.open(csvfile) as c:
             s = io.StringIO(c.read().decode(encoding="utf8"))
             data = pd.read_csv(
@@ -125,22 +130,22 @@
 
 def _load_descr(
     collection: str,
     name: str,
     data_home: Optional[str] = None,
 ) -> Tuple[int, str]:
     """Load a dataset description."""
-    subfolder = os.path.join('keel', collection)
-    filename = name + '-names.txt'
-    if collection == 'imbalanced':
+    subfolder = os.path.join("keel", collection)
+    filename = name + "-names.txt"
+    if collection == "imbalanced":
         for url in IMBALANCED_URLS:
             if url in IRREGULAR_DESCR_IMBALANCED_URLS:
-                url = BASE_URL + '/' + url + '/' + 'names' + '/' + filename
+                url = BASE_URL + "/" + url + "/" + "names" + "/" + filename
             else:
-                url = BASE_URL + '/' + url + '/' + filename
+                url = BASE_URL + "/" + url + "/" + filename
             try:
                 f = fetch_file(
                     dataname=name,
                     urlname=url,
                     subfolder=subfolder,
                     data_home=data_home,
                 )
@@ -169,18 +174,18 @@
 def _fetch_keel_zip(
     collection: str,
     name: str,
     filename: str,
     data_home: Optional[str] = None,
 ) -> Path:
     """Fetch Keel dataset zip file."""
-    subfolder = os.path.join('keel', collection)
-    if collection == 'imbalanced':
+    subfolder = os.path.join("keel", collection)
+    if collection == "imbalanced":
         for url in IMBALANCED_URLS:
-            url = BASE_URL + '/' + url + '/' + filename
+            url = BASE_URL + "/" + url + "/" + filename
             try:
                 return fetch_file(
                     dataname=name,
                     urlname=url,
                     subfolder=subfolder,
                     data_home=data_home,
                 )
@@ -206,37 +211,36 @@
     data_home: Optional[str] = None,
 ) -> Tuple[
     np.typing.NDArray[float],
     np.typing.NDArray[Union[int, float]],
     Optional[KeelOuterCV],
 ]:
     """Load a dataset folds."""
-    filename = name + '.zip'
+    filename = name + ".zip"
     f = _fetch_keel_zip(collection, name, filename, data_home=data_home)
-    X, y = _load_Xy(f, name + '.dat', skiprows=nattrs + 4)
+    X, y = _load_Xy(f, name + ".dat", skiprows=nattrs + 4)
     cv = None
     if nfolds in (5, 10):
-        fold = 'dobscv' if dobscv else 'fold'
-        filename = name + '-' + str(nfolds) + '-' + fold + '.zip'
+        fold = "dobscv" if dobscv else "fold"
+        filename = name + "-" + str(nfolds) + "-" + fold + ".zip"
         f = _fetch_keel_zip(collection, name, filename, data_home=data_home)
         Xs = []
         ys = []
         Xs_test = []
         ys_test = []
         for i in range(nfolds):
             if dobscv:
                 # Zipfiles always use fordward slashes, even in Windows.
                 _name = f"{name}/{name}-{nfolds}dobscv-{i + 1}"
             else:
                 _name = f"{name}-{nfolds}-{i + 1}"
-            X_fold, y_fold = _load_Xy(
-                f, _name + 'tra.dat', skiprows=nattrs + 4)
+            X_fold, y_fold = _load_Xy(f, _name + "tra.dat", skiprows=nattrs + 4)
             X_test_fold, y_test_fold = _load_Xy(
                 f,
-                _name + 'tst.dat',
+                _name + "tst.dat",
                 skiprows=nattrs + 4,
             )
             Xs.append(X_fold)
             ys.append(y_fold)
             Xs_test.append(X_test_fold)
             ys_test.append(y_test_fold)
 
@@ -313,15 +317,15 @@
     data : Bunch
         Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
     if collection not in COLLECTIONS:
-        raise ValueError('Avaliable collections are ' + str(list(COLLECTIONS)))
+        raise ValueError("Avaliable collections are " + str(list(COLLECTIONS)))
     nattrs, DESCR = _load_descr(collection, name, data_home=data_home)
     X, y, cv = _load_folds(
         collection,
         name,
         nfolds,
         dobscv,
         nattrs,
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/keras.py` & `scikit-datasets-0.2.3/skdatasets/repositories/keras.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     fashion_mnist,
     imdb,
     mnist,
     reuters,
 )
 
 DATASETS = {
-    'boston_housing': boston_housing.load_data,
-    'cifar10': cifar10.load_data,
-    'cifar100': cifar100.load_data,
-    'fashion_mnist': fashion_mnist.load_data,
-    'imdb': imdb.load_data,
-    'mnist': mnist.load_data,
-    'reuters': reuters.load_data,
+    "boston_housing": boston_housing.load_data,
+    "cifar10": cifar10.load_data,
+    "cifar100": cifar100.load_data,
+    "fashion_mnist": fashion_mnist.load_data,
+    "imdb": imdb.load_data,
+    "mnist": mnist.load_data,
+    "reuters": reuters.load_data,
 }
 
 
 @overload
 def fetch(
     name: str,
     *,
@@ -79,15 +79,15 @@
         Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
     (X_train, y_train), (X_test, y_test) = DATASETS[name](**kwargs)
     if len(X_train.shape) > 2:
-        name = name + ' ' + str(X_train.shape[1:]) + ' shaped'
+        name = name + " " + str(X_train.shape[1:]) + " shaped"
         X_max = np.iinfo(X_train[0][0].dtype).max
         n_features = np.prod(X_train.shape[1:])
         X_train = X_train.reshape([X_train.shape[0], n_features]) / X_max
         X_test = X_test.reshape([X_test.shape[0], n_features]) / X_max
 
     X = np.concatenate((X_train, X_test))
     y = np.concatenate((y_train, y_test))
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/libsvm.py` & `scikit-datasets-0.2.3/skdatasets/repositories/libsvm.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,43 +3,44 @@
 
 @author: David Diaz Vico
 @license: MIT
 """
 from __future__ import annotations
 
 import os
-import sys
 from typing import Final, Literal, Sequence, Tuple, overload
 
 import numpy as np
 import scipy as sp
 from sklearn.datasets import load_svmlight_file, load_svmlight_files
 from sklearn.model_selection import PredefinedSplit
 from sklearn.utils import Bunch
 
 from .base import DatasetNotFoundError, fetch_file
 
-BASE_URL: Final = 'https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets'
-COLLECTIONS: Final = frozenset((
-    'binary',
-    'multiclass',
-    'regression',
-    'string',
-))
+BASE_URL: Final = "https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/datasets"
+COLLECTIONS: Final = frozenset(
+    (
+        "binary",
+        "multiclass",
+        "regression",
+        "string",
+    )
+)
 
 
 def _fetch_partition(
     collection: str,
     name: str,
     partition: str,
     data_home: str | None = None,
 ) -> str | None:
     """Fetch dataset partition."""
-    subfolder = os.path.join('libsvm', collection)
-    dataname = name.replace('/', '-')
+    subfolder = os.path.join("libsvm", collection)
+    dataname = name.replace("/", "-")
 
     url = f"{BASE_URL}/{collection}/{name}{partition}"
 
     for data_url in (f"{url}.bz2", url):
         try:
             return os.fspath(
                 fetch_file(
@@ -64,90 +65,103 @@
     np.typing.NDArray[int | float],
     Sequence[int],
     Sequence[int],
     Sequence[int],
     PredefinedSplit,
 ]:
     """Load dataset."""
-    filename = _fetch_partition(collection, name, '', data_home)
-    filename_tr = _fetch_partition(collection, name, '.tr', data_home)
-    filename_val = _fetch_partition(collection, name, '.val', data_home)
-    filename_t = _fetch_partition(collection, name, '.t', data_home)
-    filename_r = _fetch_partition(collection, name, '.r', data_home)
-
-    if (filename_tr is not None) and (filename_val is not None) and (filename_t is not None):
-
-        _, _, X_tr, y_tr, X_val, y_val, X_test, y_test = load_svmlight_files([
-            filename,
-            filename_tr,
-            filename_val,
-            filename_t,
-        ])
+    filename = _fetch_partition(collection, name, "", data_home)
+    filename_tr = _fetch_partition(collection, name, ".tr", data_home)
+    filename_val = _fetch_partition(collection, name, ".val", data_home)
+    filename_t = _fetch_partition(collection, name, ".t", data_home)
+    filename_r = _fetch_partition(collection, name, ".r", data_home)
+
+    if (
+        (filename_tr is not None)
+        and (filename_val is not None)
+        and (filename_t is not None)
+    ):
+
+        _, _, X_tr, y_tr, X_val, y_val, X_test, y_test = load_svmlight_files(
+            [
+                filename,
+                filename_tr,
+                filename_val,
+                filename_t,
+            ]
+        )
 
         cv = PredefinedSplit([-1] * X_tr.shape[0] + [0] * X_val.shape[0])
 
         X = sp.sparse.vstack((X_tr, X_val, X_test))
         y = np.hstack((y_tr, y_val, y_test))
 
         # Compute indices
         train_indices = list(range(X_tr.shape[0]))
-        validation_indices = list(range(
-            X_tr.shape[0],
-            X_tr.shape[0] + X_val.shape[0],
-        ))
+        validation_indices = list(
+            range(
+                X_tr.shape[0],
+                X_tr.shape[0] + X_val.shape[0],
+            )
+        )
         test_indices = list(range(X_tr.shape[0] + X_val.shape[0], X.shape[0]))
 
     elif (filename_tr is not None) and (filename_val is not None):
 
-        _, _, X_tr, y_tr, X_val, y_val = load_svmlight_files([
-            filename,
-            filename_tr,
-            filename_val,
-        ])
+        _, _, X_tr, y_tr, X_val, y_val = load_svmlight_files(
+            [
+                filename,
+                filename_tr,
+                filename_val,
+            ]
+        )
 
         cv = PredefinedSplit([-1] * X_tr.shape[0] + [0] * X_val.shape[0])
 
         X = sp.sparse.vstack((X_tr, X_val))
         y = np.hstack((y_tr, y_val))
 
         # Compute indices
         train_indices = list(range(X_tr.shape[0]))
         validation_indices = list(range(X_tr.shape[0], X.shape[0]))
         test_indices = []
 
     elif (filename_t is not None) and (filename_r is not None):
 
-        X_tr, y_tr, X_test, y_test, X_remaining, y_remaining = (
-            load_svmlight_files([
+        X_tr, y_tr, X_test, y_test, X_remaining, y_remaining = load_svmlight_files(
+            [
                 filename,
                 filename_t,
                 filename_r,
-            ])
+            ]
         )
 
         X = sp.sparse.vstack((X_tr, X_test, X_remaining))
         y = np.hstack((y_tr, y_test, y_remaining))
 
         # Compute indices
         train_indices = list(range(X_tr.shape[0]))
         validation_indices = []
         test_indices = list(
             range(
-                X_tr.shape[0], X_tr.shape[0] + X_test.shape[0],
+                X_tr.shape[0],
+                X_tr.shape[0] + X_test.shape[0],
             ),
         )
 
         cv = None
 
     elif filename_t is not None:
 
-        X_tr, y_tr, X_test, y_test = load_svmlight_files([
-            filename,
-            filename_t,
-        ])
+        X_tr, y_tr, X_test, y_test = load_svmlight_files(
+            [
+                filename,
+                filename_t,
+            ]
+        )
 
         X = sp.sparse.vstack((X_tr, X_test))
         y = np.hstack((y_tr, y_test))
 
         # Compute indices
         train_indices = list(range(X_tr.shape[0]))
         validation_indices = []
@@ -221,15 +235,15 @@
     data : Bunch
         Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
     if collection not in COLLECTIONS:
-        raise Exception('Avaliable collections are ' + str(list(COLLECTIONS)))
+        raise Exception("Avaliable collections are " + str(list(COLLECTIONS)))
 
     X, y, train_indices, validation_indices, test_indices, cv = _load(
         collection,
         name,
         data_home=data_home,
     )
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/physionet.py` & `scikit-datasets-0.2.3/skdatasets/repositories/physionet.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from skdatasets.repositories.base import dataset_from_dataframe
 
 from .base import DatasetNotFoundError, fetch_zip
 
 BASE_URL: Final = "https://physionet.org/static/published-projects"
 INFO_STRING_SEMICOLONS_ONE_STR: Final = r"(\S*): (\S*)\s*"
 INFO_STRING_SEMICOLONS_SEVERAL_REGEX: Final = re.compile(
-    fr"(?:{INFO_STRING_SEMICOLONS_ONE_STR})+",
+    rf"(?:{INFO_STRING_SEMICOLONS_ONE_STR})+",
 )
 INFO_STRING_SEMICOLONS_ONE_REGEX: Final = re.compile(
     INFO_STRING_SEMICOLONS_ONE_STR,
 )
 
 
 class _ZipNameHTMLParser(HTMLParser):
@@ -58,15 +58,15 @@
 def _get_zip_name_online(dataset_name: str) -> str:
     """Get the zip name of the dataset."""
     parser = _ZipNameHTMLParser()
 
     url_request = urllib.request.Request(url=f"{BASE_URL}/{dataset_name}")
     try:
         with urllib.request.urlopen(url_request) as url_file:
-            url_content = url_file.read().decode('utf-8')
+            url_content = url_file.read().decode("utf-8")
     except urllib.error.HTTPError as e:
         if e.code == 404:
             raise DatasetNotFoundError(dataset_name) from e
         raise
 
     parser.feed(url_content)
 
@@ -98,30 +98,29 @@
                 for result in re.finditer(
                     INFO_STRING_SEMICOLONS_ONE_REGEX,
                     comment,
                 ):
                     key = result.group(1)
                     if key[0] == "<" and key[-1] == ">":
                         key = key[1:-1]
-                    info_strings_semicolons[key] = (
-                        _parse_info_string_value(result.group(2))
+                    info_strings_semicolons[key] = _parse_info_string_value(
+                        result.group(2)
                     )
             else:
                 split = comment.rsplit(maxsplit=1)
                 if len(split) == 2:
                     key, value = split
                     info_strings_spaces[key] = _parse_info_string_value(value)
 
     if info_strings_semicolons:
         return info_strings_semicolons
 
     # Check for absurd things in spaces
-    if (
-        len(info_strings_spaces) == 1
-        or any(key.count(" ") > 3 for key in info_strings_spaces)
+    if len(info_strings_spaces) == 1 or any(
+        key.count(" ") > 3 for key in info_strings_spaces
     ):
         return {}
 
     return info_strings_spaces
 
 
 def _join_info_dicts(
@@ -240,25 +239,22 @@
 
     subpath = path / Path(zip_name).stem
     if subpath.exists():
         path = subpath
 
     with open(path / "RECORDS") as records_file:
         records = [
-            wfdb.io.rdrecord(str(path / record_name.rstrip('\n')))
+            wfdb.io.rdrecord(str(path / record_name.rstrip("\n")))
             for record_name in records_file
         ]
 
     info_strings = [_get_info_strings(r.comments) for r in records]
     info = _join_info_dicts(info_strings)
 
-    assert all(
-        _constant_attrs(r) == _constant_attrs(records[0])
-        for r in records
-    )
+    assert all(_constant_attrs(r) == _constant_attrs(records[0]) for r in records)
     data = {
         "signal": [r.p_signal for r in records],
     }
 
     dataframe = pd.DataFrame(
         {**info, **data},
         index=[r.record_name for r in records],
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/raetsch.py` & `scikit-datasets-0.2.3/skdatasets/repositories/raetsch.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 @author: David Diaz Vico
 @license: MIT
 """
 from __future__ import annotations
 
 import hashlib
-import sys
 from pathlib import Path
 from typing import (
     Final,
     Iterator,
     Literal,
     Optional,
     Sequence,
@@ -23,29 +22,31 @@
 
 import numpy as np
 from scipy.io import loadmat
 from sklearn.utils import Bunch
 
 from .base import fetch_file
 
-DATASETS: Final = frozenset((
-    'banana',
-    'breast_cancer',
-    'diabetis',
-    'flare_solar',
-    'german',
-    'heart',
-    'image',
-    'ringnorm',
-    'splice',
-    'thyroid',
-    'titanic',
-    'twonorm',
-    'waveform',
-))
+DATASETS: Final = frozenset(
+    (
+        "banana",
+        "breast_cancer",
+        "diabetis",
+        "flare_solar",
+        "german",
+        "heart",
+        "image",
+        "ringnorm",
+        "splice",
+        "thyroid",
+        "titanic",
+        "twonorm",
+        "waveform",
+    )
+)
 
 
 class RaetschOuterCV(object):
     """Iterable over already separated CV partitions of the dataset."""
 
     def __init__(
         self,
@@ -55,20 +56,24 @@
         test_splits: Sequence[np.typing.NDArray[int]],
     ) -> None:
         self.X = X
         self.y = y
         self.train_splits = train_splits
         self.test_splits = test_splits
 
-    def __iter__(self) -> Iterator[Tuple[
-        np.typing.NDArray[float],
-        np.typing.NDArray[Union[int, float]],
-        np.typing.NDArray[float],
-        np.typing.NDArray[Union[int, float]],
-    ]]:
+    def __iter__(
+        self,
+    ) -> Iterator[
+        Tuple[
+            np.typing.NDArray[float],
+            np.typing.NDArray[Union[int, float]],
+            np.typing.NDArray[float],
+            np.typing.NDArray[Union[int, float]],
+        ]
+    ]:
         return (
             (self.X[tr - 1], self.y[tr - 1], self.X[ts - 1], self.y[ts - 1])
             for tr, ts in zip(self.train_splits, self.test_splits)
         )
 
 
 def _fetch_remote(data_home: Optional[str] = None) -> Path:
@@ -85,30 +90,28 @@
 
     Returns
     -------
     file_path: string
         Full path of the created file.
     """
     file_path = fetch_file(
-        'raetsch',
-        'https://github.com/tdiethe/gunnar_raetsch_benchmark_datasets'
-        '/raw/master/benchmarks.mat',
+        "raetsch",
+        "https://github.com/tdiethe/gunnar_raetsch_benchmark_datasets"
+        "/raw/master/benchmarks.mat",
         data_home=data_home,
     )
     sha256hash = hashlib.sha256()
     with open(file_path, "rb") as f:
         while True:
             buffer = f.read(8192)
             if not buffer:
                 break
             sha256hash.update(buffer)
     checksum = sha256hash.hexdigest()
-    remote_checksum = (
-        '47c19e4bc4716edc4077cfa5ea61edf4d02af4ec51a0ecfe035626ae8b561c75'
-    )
+    remote_checksum = "47c19e4bc4716edc4077cfa5ea61edf4d02af4ec51a0ecfe035626ae8b561c75"
     if remote_checksum != checksum:
         raise IOError(
             f"{file_path} has an SHA256 checksum ({checksum}) differing "
             f"from expected ({remote_checksum}), file may be corrupted.",
         )
     return file_path
 
@@ -165,15 +168,15 @@
     data : Bunch
         Dictionary-like object with all the data and metadata.
 
     (data, target) : tuple if ``return_X_y`` is True
 
     """
     if name not in DATASETS:
-        raise Exception('Avaliable datasets are ' + str(list(DATASETS)))
+        raise Exception("Avaliable datasets are " + str(list(DATASETS)))
     filename = _fetch_remote(data_home=data_home)
     X, y, train_splits, test_splits = loadmat(filename)[name][0][0]
     if len(y.shape) == 2 and y.shape[1] == 1:
         y = y.ravel()
 
     cv = RaetschOuterCV(X, y, train_splits, test_splits)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/sklearn.py` & `scikit-datasets-0.2.3/skdatasets/repositories/sklearn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,89 @@
 """
 Scikit-learn datasets (http://scikit-learn.org/stable/datasets/index.html).
 
 @author: David Diaz Vico
 @license: MIT
 """
 
-from sklearn.datasets import (fetch_20newsgroups,
-                              fetch_20newsgroups_vectorized,
-                              fetch_california_housing, fetch_covtype,
-                              fetch_kddcup99, fetch_lfw_pairs,
-                              fetch_lfw_people, fetch_olivetti_faces,
-                              fetch_rcv1, load_breast_cancer, load_diabetes,
-                              load_digits, load_iris, load_linnerud, load_wine,
-                              make_biclusters, make_blobs, make_checkerboard,
-                              make_circles, make_classification,
-                              make_friedman1, make_friedman2, make_friedman3,
-                              make_gaussian_quantiles, make_hastie_10_2,
-                              make_low_rank_matrix, make_moons,
-                              make_multilabel_classification, make_regression,
-                              make_s_curve, make_sparse_coded_signal,
-                              make_sparse_spd_matrix, make_sparse_uncorrelated,
-                              make_spd_matrix, make_swiss_roll)
-
-DATASETS = {'20newsgroups': fetch_20newsgroups,
-            '20newsgroups_vectorized': fetch_20newsgroups_vectorized,
-            'biclusters': make_biclusters, 'blobs': make_blobs,
-            'breast_cancer': load_breast_cancer,
-            'california_housing': fetch_california_housing,
-            'checkerboard': make_checkerboard, 'circles': make_circles,
-            'classification': make_classification, 'covtype': fetch_covtype,
-            'diabetes': load_diabetes, 'digits': load_digits,
-            'friedman1': make_friedman1, 'friedman2': make_friedman2,
-            'friedman3': make_friedman3,
-            'gaussian_quantiles': make_gaussian_quantiles,
-            'hastie_10_2': make_hastie_10_2, 'iris': load_iris,
-            'kddcup99': fetch_kddcup99, 'lfw_people': fetch_lfw_people,
-            'lfw_pairs': fetch_lfw_pairs, 'linnerud': load_linnerud,
-            'low_rank_matrix': make_low_rank_matrix, 'moons': make_moons,
-            'multilabel_classification': make_multilabel_classification,
-            'olivetti_faces': fetch_olivetti_faces, 'rcv1': fetch_rcv1,
-            'regression': make_regression, 's_curve': make_s_curve,
-            'sparse_coded_signal': make_sparse_coded_signal,
-            'sparse_spd_matrix': make_sparse_spd_matrix,
-            'sparse_uncorrelated': make_sparse_uncorrelated,
-            'spd_matrix': make_spd_matrix, 'swiss_roll': make_swiss_roll,
-            'wine': load_wine}
+from sklearn.datasets import (
+    fetch_20newsgroups,
+    fetch_20newsgroups_vectorized,
+    fetch_california_housing,
+    fetch_covtype,
+    fetch_kddcup99,
+    fetch_lfw_pairs,
+    fetch_lfw_people,
+    fetch_olivetti_faces,
+    fetch_rcv1,
+    load_breast_cancer,
+    load_diabetes,
+    load_digits,
+    load_iris,
+    load_linnerud,
+    load_wine,
+    make_biclusters,
+    make_blobs,
+    make_checkerboard,
+    make_circles,
+    make_classification,
+    make_friedman1,
+    make_friedman2,
+    make_friedman3,
+    make_gaussian_quantiles,
+    make_hastie_10_2,
+    make_low_rank_matrix,
+    make_moons,
+    make_multilabel_classification,
+    make_regression,
+    make_s_curve,
+    make_sparse_coded_signal,
+    make_sparse_spd_matrix,
+    make_sparse_uncorrelated,
+    make_spd_matrix,
+    make_swiss_roll,
+)
+
+DATASETS = {
+    "20newsgroups": fetch_20newsgroups,
+    "20newsgroups_vectorized": fetch_20newsgroups_vectorized,
+    "biclusters": make_biclusters,
+    "blobs": make_blobs,
+    "breast_cancer": load_breast_cancer,
+    "california_housing": fetch_california_housing,
+    "checkerboard": make_checkerboard,
+    "circles": make_circles,
+    "classification": make_classification,
+    "covtype": fetch_covtype,
+    "diabetes": load_diabetes,
+    "digits": load_digits,
+    "friedman1": make_friedman1,
+    "friedman2": make_friedman2,
+    "friedman3": make_friedman3,
+    "gaussian_quantiles": make_gaussian_quantiles,
+    "hastie_10_2": make_hastie_10_2,
+    "iris": load_iris,
+    "kddcup99": fetch_kddcup99,
+    "lfw_people": fetch_lfw_people,
+    "lfw_pairs": fetch_lfw_pairs,
+    "linnerud": load_linnerud,
+    "low_rank_matrix": make_low_rank_matrix,
+    "moons": make_moons,
+    "multilabel_classification": make_multilabel_classification,
+    "olivetti_faces": fetch_olivetti_faces,
+    "rcv1": fetch_rcv1,
+    "regression": make_regression,
+    "s_curve": make_s_curve,
+    "sparse_coded_signal": make_sparse_coded_signal,
+    "sparse_spd_matrix": make_sparse_spd_matrix,
+    "sparse_uncorrelated": make_sparse_uncorrelated,
+    "spd_matrix": make_spd_matrix,
+    "swiss_roll": make_swiss_roll,
+    "wine": load_wine,
+}
 
 
 def fetch(name, *, return_X_y=False, **kwargs):
     """Fetch Scikit-learn dataset.
 
     Fetch a Scikit-learn dataset by name. More info at
     http://scikit-learn.org/stable/datasets/index.html.
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/uci.py` & `scikit-datasets-0.2.3/skdatasets/repositories/uci.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,39 +2,35 @@
 UCI datasets (https://archive.ics.uci.edu/ml/datasets.html).
 
 @author: David Diaz Vico
 @license: MIT
 """
 from __future__ import annotations
 
-import sys
 from pathlib import Path
 from typing import Any, Literal, Optional, Tuple, Union, overload
 
 import numpy as np
 from sklearn.preprocessing import OrdinalEncoder
 from sklearn.utils import Bunch
 
 from .base import fetch_file
 
-BASE_URL = 'https://archive.ics.uci.edu/ml/machine-learning-databases'
+BASE_URL = "https://archive.ics.uci.edu/ml/machine-learning-databases"
 
 
 def _load_csv(
     fname: Path,
     **kwargs: Any,
-) -> Tuple[
-    np.typing.NDArray[float],
-    np.typing.NDArray[Union[float, int, str]],
-]:
+) -> Tuple[np.typing.NDArray[float], np.typing.NDArray[Union[float, int, str]],]:
     """Load a csv with targets in the last column and features in the rest."""
     data = np.genfromtxt(
         fname,
         dtype=str,
-        delimiter=',',
+        delimiter=",",
         encoding=None,
         **kwargs,
     )
     X = data[:, :-1]
     try:
         X = X.astype(float)
     except ValueError:
@@ -53,33 +49,33 @@
     np.typing.NDArray[Union[float, int]],
     Optional[np.typing.NDArray[float]],
     Optional[np.typing.NDArray[Union[float, int]]],
     str,
     np.typing.NDArray[str],
 ]:
     """Fetch dataset."""
-    subfolder = 'uci'
-    filename_str = name + '.data'
-    url = BASE_URL + '/' + name + '/' + filename_str
+    subfolder = "uci"
+    filename_str = name + ".data"
+    url = BASE_URL + "/" + name + "/" + filename_str
 
     filename = fetch_file(
         dataname=name,
         urlname=url,
         subfolder=subfolder,
         data_home=data_home,
     )
     X, y = _load_csv(filename)
     target_names = None
     ordinal_encoder = OrdinalEncoder(dtype=np.int64)
     if y.dtype.type is np.str_:
         y = ordinal_encoder.fit_transform(y.reshape(-1, 1))[:, 0]
         target_names = ordinal_encoder.categories_[0]
     try:
-        filename_str = name + '.test'
-        url = BASE_URL + '/' + name + '/' + filename_str
+        filename_str = name + ".test"
+        url = BASE_URL + "/" + name + "/" + filename_str
         filename = fetch_file(
             dataname=name,
             urlname=url,
             subfolder=subfolder,
             data_home=data_home,
         )
         X_test: Optional[np.typing.NDArray[float]]
@@ -89,25 +85,25 @@
         if y.dtype.type is np.str_:
             y_test = ordinal_encoder.transform(y_test.reshape(-1, 1))[:, 0]
 
     except Exception:
         X_test = None
         y_test = None
     try:
-        filename_str = name + '.names'
-        url = BASE_URL + '/' + name + '/' + filename_str
+        filename_str = name + ".names"
+        url = BASE_URL + "/" + name + "/" + filename_str
         filename = fetch_file(
             dataname=name,
             urlname=url,
             subfolder=subfolder,
             data_home=data_home,
         )
     except Exception:
-        filename_str = name + '.info'
-        url = BASE_URL + '/' + name + '/' + filename_str
+        filename_str = name + ".info"
+        url = BASE_URL + "/" + name + "/" + filename_str
         filename = fetch_file(
             dataname=name,
             urlname=url,
             subfolder=subfolder,
             data_home=data_home,
         )
     with open(filename) as rst_file:
@@ -136,18 +132,15 @@
 
 
 def fetch(
     name: str,
     data_home: Optional[str] = None,
     *,
     return_X_y: bool = False,
-) -> Union[
-    Bunch,
-    Tuple[np.typing.NDArray[float], np.typing.NDArray[float]],
-]:
+) -> Union[Bunch, Tuple[np.typing.NDArray[float], np.typing.NDArray[float]],]:
     """
     Fetch UCI dataset.
 
     Fetch a UCI dataset by name. More info at
     https://archive.ics.uci.edu/ml/datasets.html.
 
     Parameters
```

### Comparing `scikit-datasets-0.2.2/skdatasets/repositories/ucr.py` & `scikit-datasets-0.2.3/skdatasets/repositories/ucr.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 Datasets from the UCR time series database.
 
 @author: Carlos Ramos Carreño
 @license: MIT
 """
 from __future__ import annotations
 
-import sys
 from pathlib import Path
 from typing import Final, Literal, Optional, Sequence, Tuple, Union, overload
 
 import numpy as np
 import scipy.io.arff
 from sklearn.utils import Bunch
 
 from .base import fetch_zip as _fetch_zip
 
-BASE_URL: Final = 'http://www.timeseriesclassification.com/Downloads/'
+BASE_URL: Final = "http://www.timeseriesclassification.com/ClassificationDownloads/"
 
 
 def _target_conversion(
     target: np.typing.NDArray[Union[int, str]],
 ) -> Tuple[np.typing.NDArray[int], Sequence[str]]:
     try:
         target_data = target.astype(int)
@@ -33,17 +32,16 @@
 
 
 def data_to_matrix(
     struct_array: np.typing.NDArray[object],
 ) -> np.typing.NDArray[float]:
     fields = struct_array.dtype.fields
     assert fields
-    if(
-        len(fields.items()) == 1
-        and list(fields.items())[0][1][0] == np.dtype(np.object_)
+    if len(fields.items()) == 1 and list(fields.items())[0][1][0] == np.dtype(
+        np.object_
     ):
         attribute = struct_array[list(fields.items())[0][0]]
 
         n_instances = len(attribute)
         n_curves = len(attribute[0])
         n_points = len(attribute[0][0])
 
@@ -85,18 +83,15 @@
 
 
 def fetch(
     name: str,
     *,
     data_home: Optional[str] = None,
     return_X_y: bool = False,
-) -> Union[
-    Bunch,
-    Tuple[np.typing.NDArray[float], np.typing.NDArray[int]],
-]:
+) -> Union[Bunch, Tuple[np.typing.NDArray[float], np.typing.NDArray[int]], ]:
     """
     Fetch UCR dataset.
 
     Fetch a UCR dataset by name. More info at
     http://www.timeseriesclassification.com/.
 
     Parameters
@@ -117,15 +112,15 @@
     (data, target) : tuple if ``return_X_y`` is True
 
     """
     url = BASE_URL + name
 
     data_path = _fetch_zip(
         name,
-        urlname=url + '.zip',
+        urlname=url + ".zip",
         subfolder="ucr",
         data_home=data_home,
     )
 
     description_filenames = [name, name + "Description", name + "_Info"]
 
     path_file_descr: Optional[Path]
@@ -133,20 +128,20 @@
         path_file_descr = (data_path / f).with_suffix(".txt")
         if path_file_descr.exists():
             break
     else:
         # No description is found
         path_file_descr = None
 
-    path_file_train = (data_path / (name + '_TRAIN')).with_suffix(".arff")
-    path_file_test = (data_path / (name + '_TEST')).with_suffix(".arff")
+    path_file_train = (data_path / (name + "_TRAIN")).with_suffix(".arff")
+    path_file_test = (data_path / (name + "_TEST")).with_suffix(".arff")
 
     DESCR = (
-        path_file_descr.read_text(errors='surrogateescape')
-        if path_file_descr else ''
+        path_file_descr.read_text(
+            errors="surrogateescape") if path_file_descr else ""
     )
     train = scipy.io.arff.loadarff(path_file_train)
     test = scipy.io.arff.loadarff(path_file_test)
     dataset_name = train[1].name
     column_names = np.array(train[1].names())
     target_column_name = column_names[-1]
     feature_names = column_names[column_names != target_column_name].tolist()
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/__init__.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 from sklearn.model_selection import GridSearchCV, cross_validate
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler
 
 
 def check_estimator(data):
     """Check that the dataset can be used to cross-validate an estimator."""
-    estimator = GridSearchCV(Pipeline([('tr', StandardScaler(with_mean=False)),
-                                       ('pred', Ridge(max_iter=4))]),
-                             {'pred__alpha': [0.33, 0.66]},
-                             cv=data.inner_cv, error_score=np.nan)
+    estimator = GridSearchCV(
+        Pipeline(
+            [("tr", StandardScaler(with_mean=False)), ("pred", Ridge(max_iter=4))]
+        ),
+        {"pred__alpha": [0.33, 0.66]},
+        cv=data.inner_cv,
+        error_score=np.nan,
+    )
     if data.train_indices and data.test_indices:
 
         train_indices = data.train_indices
 
         train_indices += data.validation_indices
 
         estimator.fit(
             data.data[train_indices],
             y=data.target[train_indices],
         )
-        estimator.score(
-            data.data[data.test_indices],
-            y=data.target[data.test_indices]
-        )
+        estimator.score(data.data[data.test_indices], y=data.target[data.test_indices])
     else:
-        if hasattr(data.outer_cv, '__iter__'):
+        if hasattr(data.outer_cv, "__iter__"):
             for X, y, X_test, y_test in data.outer_cv:
                 estimator.fit(X, y=y)
                 estimator.score(X_test, y=y_test)
         else:
-            cross_validate(estimator, data.data, y=data.target,
-                           cv=data.outer_cv)
+            cross_validate(estimator, data.data, y=data.target, cv=data.outer_cv)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_forex.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_forex.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,38 @@
 from datetime import date
 
 from skdatasets.repositories.forex import fetch
 
 
 def test_forex_usd_eur():
     """Tests forex USD-EUR dataset."""
-    data = fetch(start=date(2015, 1, 1), end=date(2015, 1, 31),
-                 currency_1='USD', currency_2='EUR')
+    data = fetch(
+        start=date(2015, 1, 1),
+        end=date(2015, 1, 31),
+        currency_1="USD",
+        currency_2="EUR",
+    )
     assert data.data.shape == (31, 1)
 
 
 def test_forex_usd_eur_return_X_y():
     """Tests forex USD-EUR dataset."""
-    X, y = fetch(start=date(2015, 1, 1), end=date(2015, 1, 31),
-                 currency_1='USD', currency_2='EUR', return_X_y=True)
+    X, y = fetch(
+        start=date(2015, 1, 1),
+        end=date(2015, 1, 31),
+        currency_1="USD",
+        currency_2="EUR",
+        return_X_y=True,
+    )
     assert X.shape == (31, 1)
     assert y is None
 
 
 def test_forex_btc_eur():
     """Tests forex BTC-EUR dataset."""
-    data = fetch(start=date(2015, 1, 1), end=date(2015, 1, 31),
-                 currency_1='BTC', currency_2='EUR')
+    data = fetch(
+        start=date(2015, 1, 1),
+        end=date(2015, 1, 31),
+        currency_1="BTC",
+        currency_2="EUR",
+    )
     assert data.data.shape == (31, 1)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_keel.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keel.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,40 +23,40 @@
     assert not data.test_indices
     assert data.inner_cv is None
     check_estimator(data)
 
 
 def test_fetch_keel_abalone9_18():
     """Tests Keel abalone9-18 dataset."""
-    data = fetch('imbalanced', 'abalone9-18')
+    data = fetch("imbalanced", "abalone9-18")
     check(data, (731, 10))
 
 
 def test_fetch_keel_abalone9_18_return_X_y():
     """Tests Keel abalone9-18 dataset."""
-    X, y = fetch('imbalanced', 'abalone9-18', return_X_y=True)
+    X, y = fetch("imbalanced", "abalone9-18", return_X_y=True)
     assert X.shape == (731, 10)
     assert y.shape == (731,)
 
 
 def test_fetch_keel_abalone9_18_folds():
     """Tests Keel abalone9-18 dataset with folds."""
-    data = fetch('imbalanced', 'abalone9-18', nfolds=5)
+    data = fetch("imbalanced", "abalone9-18", nfolds=5)
     check(data, (731, 10), splits=5)
 
 
 def test_fetch_keel_banana():
     """Tests Keel banana dataset."""
-    data = fetch('classification', 'banana')
+    data = fetch("classification", "banana")
     check(data, (5300, 2))
 
 
 def test_fetch_keel_banana_folds():
     """Tests Keel banana dataset with folds."""
-    data = fetch('classification', 'banana', nfolds=5)
+    data = fetch("classification", "banana", nfolds=5)
     check(data, (5300, 2), splits=5)
 
 
 def test_fetch_keel_banana_dobscv():
     """Tests Keel banana dataset with dobscv folds."""
-    data = fetch('classification', 'banana', nfolds=5, dobscv=True)
+    data = fetch("classification", "banana", nfolds=5, dobscv=True)
     check(data, (5300, 2), splits=5)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_keras.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_keras.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,28 @@
 
 @author: David Diaz Vico
 @license: MIT
 """
 
 from skdatasets.repositories.keras import fetch
 
-from . import check_estimator
-
 
 def check(data, n_samples_train, n_samples_test, n_features):
     """Check dataset properties."""
     assert data.data.shape == (n_samples_train + n_samples_test, n_features)
     assert data.target.shape[0] == n_samples_train + n_samples_test
     assert len(data.train_indices) == n_samples_train
     assert len(data.test_indices) == n_samples_test
     assert not data.validation_indices
 
 
 def test_keras_mnist():
     """Tests keras MNIST dataset."""
-    data = fetch('mnist')
+    data = fetch("mnist")
     check(data, n_samples_train=60000, n_samples_test=10000, n_features=28 * 28)
 
 
 def test_keras_mnist_return_X_y():
     """Tests keras MNIST dataset."""
-    X, y = fetch('mnist', return_X_y=True)
+    X, y = fetch("mnist", return_X_y=True)
     assert X.shape == (70000, 28 * 28)
     assert y.shape == (70000,)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_libsvm.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_libsvm.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,24 @@
     n_samples_validation=None,
     n_samples_test=None,
     n_samples_remaining=None,
     estimator=True,
 ):
     """Check dataset properties."""
     if n_samples is None:
-        n_samples = sum(n for n in [
-            n_samples_train,
-            n_samples_validation,
-            n_samples_test,
-            n_samples_remaining
-        ] if n is not None)
+        n_samples = sum(
+            n
+            for n in [
+                n_samples_train,
+                n_samples_validation,
+                n_samples_test,
+                n_samples_remaining,
+            ]
+            if n is not None
+        )
 
     assert data.data.shape == (n_samples, n_features)
     assert data.target.shape[0] == n_samples
 
     if n_samples_train is None:
         assert not data.train_indices
     else:
@@ -56,43 +60,58 @@
 
     if estimator:
         check_estimator(data)
 
 
 def test_fetch_libsvm_australian():
     """Tests LIBSVM australian dataset."""
-    data = fetch('binary', 'australian')
+    data = fetch("binary", "australian")
     check(data, n_samples=690, n_features=14)
 
 
 def test_fetch_libsvm_australian_return_X_y():
     """Tests LIBSVM australian dataset."""
-    X, y = fetch('binary', 'australian', return_X_y=True)
+    X, y = fetch("binary", "australian", return_X_y=True)
     assert X.shape == (690, 14)
     assert y.shape == (690,)
 
 
 def test_fetch_libsvm_liver_disorders():
     """Tests LIBSVM liver-disorders dataset."""
-    data = fetch('binary', 'liver-disorders')
+    data = fetch("binary", "liver-disorders")
     check(data, n_samples_train=145, n_samples_test=200, n_features=5)
 
 
 def test_fetch_libsvm_duke():
     """Tests LIBSVM duke dataset."""
-    data = fetch('binary', 'duke')
-    check(data, n_samples_train=38, n_samples_validation=4,
-          n_features=7129, estimator=False)
+    data = fetch("binary", "duke")
+    check(
+        data,
+        n_samples_train=38,
+        n_samples_validation=4,
+        n_features=7129,
+        estimator=False,
+    )
 
 
 def test_fetch_libsvm_cod_rna():
     """Tests LIBSVM cod-rna dataset."""
-    data = fetch('binary', 'cod-rna')
-    check(data, n_samples_train=59535, n_samples_test=271617,
-          n_samples_remaining=157413, n_features=8)
+    data = fetch("binary", "cod-rna")
+    check(
+        data,
+        n_samples_train=59535,
+        n_samples_test=271617,
+        n_samples_remaining=157413,
+        n_features=8,
+    )
 
 
 def test_fetch_libsvm_satimage():
     """Tests LIBSVM satimage dataset."""
-    data = fetch('multiclass', 'satimage.scale')
-    check(data, n_samples_train=3104, n_samples_test=2000,
-          n_samples_validation=1331, n_features=36)
+    data = fetch("multiclass", "satimage.scale")
+    check(
+        data,
+        n_samples_train=3104,
+        n_samples_test=2000,
+        n_samples_validation=1331,
+        n_features=36,
+    )
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_physionet.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_physionet.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 
 from skdatasets.repositories.physionet import fetch
 
 
 def test_fetch_ctu_uhb_ctgdb() -> None:
     """Tests ctu_uhb dataset."""
     X, y = fetch(
-        'ctu-uhb-ctgdb',
+        "ctu-uhb-ctgdb",
         return_X_y=True,
         target_column=["pH", "BDecf", "pCO2", "BE", "Apgar1", "Apgar5"],
     )
     assert X.shape == (552, 30)
     assert y.shape == (552, 6)
 
 
 def test_fetch_ctu_uhb_ctgdb_single_target() -> None:
     """Tests ctu_uhb dataset with one target."""
     X, y = fetch(
-        'ctu-uhb-ctgdb',
+        "ctu-uhb-ctgdb",
         return_X_y=True,
         target_column="pH",
     )
     assert X.shape == (552, 35)
     assert y.shape == (552,)
 
 
 def test_fetch_ctu_uhb_ctgdb_bunch() -> None:
     """Tests ctu_uhb dataset returning Bunch."""
     bunch = fetch(
-        'ctu-uhb-ctgdb',
+        "ctu-uhb-ctgdb",
         as_frame=True,
         target_column=["pH", "BDecf", "pCO2", "BE", "Apgar1", "Apgar5"],
     )
     assert bunch.data.shape == (552, 30)
     assert bunch.target.shape == (552, 6)
     assert bunch.frame.shape == (552, 36)
 
 
 def test_fetch_macecgdb() -> None:
     """Tests macecgdb dataset."""
     bunch = fetch(
-        'macecgdb',
+        "macecgdb",
         as_frame=True,
     )
     assert bunch.data.shape == (27, 5)
     assert bunch.target == None
     assert bunch.frame.shape == (27, 5)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_raetsch.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_raetsch.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     assert data.target.shape[0] == shape[0]
     assert len(list(data.outer_cv)) == splits
     check_estimator(data)
 
 
 def test_fetch_raetsch_banana():
     """Tests Gunnar Raetsch banana dataset."""
-    data = fetch('banana')
+    data = fetch("banana")
     check(data, (5300, 2), splits=100)
 
 
 def test_fetch_raetsch_banana_return_X_y():
     """Tests Gunnar Raetsch banana dataset."""
-    X, y = fetch('banana', return_X_y=True)
+    X, y = fetch("banana", return_X_y=True)
     assert X.shape == (5300, 2)
     assert y.shape == (5300,)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_uci.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_uci.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 """
 
 from skdatasets.repositories.uci import fetch
 
 
 def test_fetch_uci_wine():
     """Tests UCI wine dataset."""
-    data = fetch('wine')
+    data = fetch("wine")
     assert data.data.shape == (178, 13)
     assert data.target.shape[0] == data.data.shape[0]
     assert not data.train_indices
     assert not data.validation_indices
     assert not data.test_indices
     assert data.inner_cv is None
     assert data.outer_cv is None
 
 
 def test_fetch_uci_wine_return_X_y():
     """Tests UCI wine dataset."""
-    X, y = fetch('wine', return_X_y=True)
+    X, y = fetch("wine", return_X_y=True)
     assert X.shape == (178, 13)
     assert y.shape == (178,)
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/repositories/test_ucr.py` & `scikit-datasets-0.2.3/skdatasets/tests/repositories/test_ucr.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 """
 
 from skdatasets.repositories.ucr import fetch
 
 
 def test_fetch_ucr_gunpoint():
     """Tests UCR GunPoint dataset."""
-    data = fetch('GunPoint')
+    data = fetch("GunPoint")
     assert data.data.shape == (200, 150)
     assert len(data.train_indices) == 50
     assert len(data.test_indices) == 150
 
 
 def test_fetch_ucr_gunpoint_return_X_y():
     """Tests UCR GunPoint dataset."""
-    X, y = fetch('GunPoint', return_X_y=True)
+    X, y = fetch("GunPoint", return_X_y=True)
     assert X.shape == (200, 150)
     assert y.shape == (200,)
 
 
 def test_fetch_ucr_basicmotions():
     """Tests UCR GunPoint dataset."""
-    data = fetch('BasicMotions')
+    data = fetch("BasicMotions")
     assert data.data.shape == (80,)
     assert len(data.train_indices) == 40
     assert len(data.test_indices) == 40
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/utils/run.py` & `scikit-datasets-0.2.3/skdatasets/tests/utils/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,32 @@
 from sacred.observers import FileStorageObserver
 
 from skdatasets import fetch
 from skdatasets.utils.estimator import json2estimator
 from skdatasets.utils.experiment import experiment
 
 
-def main(dataset=fetch, estimator=json2estimator,
-         observers=[FileStorageObserver('.results')]):
-    parser = argparse.ArgumentParser(description='Run an experiment.')
-    parser.add_argument('-r', '--repository', type=str, help='repository')
-    parser.add_argument('-c', '--collection', type=str, default=None,
-                        help='collection')
-    parser.add_argument('-d', '--dataset', type=str, help='dataset')
-    parser.add_argument('-e', '--estimator', type=str, help='estimator')
+def main(
+    dataset=fetch, estimator=json2estimator, observers=[FileStorageObserver(".results")]
+):
+    parser = argparse.ArgumentParser(description="Run an experiment.")
+    parser.add_argument("-r", "--repository", type=str, help="repository")
+    parser.add_argument("-c", "--collection", type=str, default=None, help="collection")
+    parser.add_argument("-d", "--dataset", type=str, help="dataset")
+    parser.add_argument("-e", "--estimator", type=str, help="estimator")
     args = parser.parse_args()
     e = experiment(dataset, estimator)
     e.observers.extend(observers)
-    e.run(config_updates={'dataset': {'repository': args.repository,
-                                      'collection': args.collection,
-                                      'dataset': args.dataset},
-                          'estimator': {'estimator': args.estimator}})
+    e.run(
+        config_updates={
+            "dataset": {
+                "repository": args.repository,
+                "collection": args.collection,
+                "dataset": args.dataset,
+            },
+            "estimator": {"estimator": args.estimator},
+        }
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scikit-datasets-0.2.2/skdatasets/tests/utils/test_scores.py` & `scikit-datasets-0.2.3/skdatasets/tests/utils/test_scores.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,31 +3,53 @@
 @license: MIT
 """
 
 import numpy as np
 
 from skdatasets.utils.scores import hypotheses_table, scores_table
 
-datasets = ['a4a', 'a8a', 'combined', 'dna', 'ijcnn1', 'letter', 'pendigits',
-            'satimage', 'shuttle', 'usps', 'w7a', 'w8a']
-estimators = ['LogisticRegression', 'MLPClassifier0', 'MLPClassifier1',
-              'MLPClassifier2', 'MLPClassifier3', 'MLPClassifier4',
-              'MLPClassifier5']
-scores = np.asarray(((89.79, 89.78, 89.76, 89.88, 89.85, 89.91, 89.93),
-                     (90.73, 90.73, 90.73, 90.85, 90.83, 90.81, 90.80),
-                     (92.36, 92.31, 94.58, 94.82, 94.84, 94.92, 94.89),
-                     (99.28, 99.27, 99.28, 99.26, 99.27, 99.25, 99.25),
-                     (91.34, 91.34, 99.29, 99.33, 99.34, 99.53, 99.54),
-                     (98.07, 98.04, 99.94, 99.95, 99.96, 99.96, 99.95),
-                     (99.17, 99.08, 99.87, 99.87, 99.88, 99.90, 99.89),
-                     (96.67, 96.28, 98.84, 98.87, 98.90, 98.87, 98.92),
-                     (95.85, 92.83, 99.88, 99.93, 99.96, 99.98, 99.99),
-                     (99.12, 99.11, 99.65, 99.58, 99.58, 99.65, 99.60),
-                     (95.93, 95.40, 94.58, 96.31, 96.34, 96.58, 96.50),
-                     (95.80, 95.99, 95.35, 96.20, 96.22, 96.36, 96.71)))
+datasets = [
+    "a4a",
+    "a8a",
+    "combined",
+    "dna",
+    "ijcnn1",
+    "letter",
+    "pendigits",
+    "satimage",
+    "shuttle",
+    "usps",
+    "w7a",
+    "w8a",
+]
+estimators = [
+    "LogisticRegression",
+    "MLPClassifier0",
+    "MLPClassifier1",
+    "MLPClassifier2",
+    "MLPClassifier3",
+    "MLPClassifier4",
+    "MLPClassifier5",
+]
+scores = np.asarray(
+    (
+        (89.79, 89.78, 89.76, 89.88, 89.85, 89.91, 89.93),
+        (90.73, 90.73, 90.73, 90.85, 90.83, 90.81, 90.80),
+        (92.36, 92.31, 94.58, 94.82, 94.84, 94.92, 94.89),
+        (99.28, 99.27, 99.28, 99.26, 99.27, 99.25, 99.25),
+        (91.34, 91.34, 99.29, 99.33, 99.34, 99.53, 99.54),
+        (98.07, 98.04, 99.94, 99.95, 99.96, 99.96, 99.95),
+        (99.17, 99.08, 99.87, 99.87, 99.88, 99.90, 99.89),
+        (96.67, 96.28, 98.84, 98.87, 98.90, 98.87, 98.92),
+        (95.85, 92.83, 99.88, 99.93, 99.96, 99.98, 99.99),
+        (99.12, 99.11, 99.65, 99.58, 99.58, 99.65, 99.60),
+        (95.93, 95.40, 94.58, 96.31, 96.34, 96.58, 96.50),
+        (95.80, 95.99, 95.35, 96.20, 96.22, 96.36, 96.71),
+    )
+)
 
 
 def test_scores_table() -> None:
     """Tests scores table."""
     scores_table(scores, datasets=datasets, estimators=estimators)
     scores_table(
         scores,
@@ -35,16 +57,29 @@
         datasets=datasets,
         estimators=estimators,
     )
 
 
 def test_hypotheses_table() -> None:
     """Tests hypotheses table."""
-    for multitest in ('kruskal', 'friedmanchisquare', None):
-        for test in ('mannwhitneyu', 'wilcoxon'):
-            hypotheses_table(scores, estimators,
-                             multitest=multitest, test=test)
-            for correction in ('bonferroni', 'sidak', 'holm-sidak', 'holm',
-                               'simes-hochberg', 'hommel', 'fdr_bh', 'fdr_by',
-                               'fdr_tsbh', 'fdr_tsbky'):
-                hypotheses_table(scores, estimators, multitest=multitest,
-                                 test=test, correction=correction)
+    for multitest in ("kruskal", "friedmanchisquare", None):
+        for test in ("mannwhitneyu", "wilcoxon"):
+            hypotheses_table(scores, estimators, multitest=multitest, test=test)
+            for correction in (
+                "bonferroni",
+                "sidak",
+                "holm-sidak",
+                "holm",
+                "simes-hochberg",
+                "hommel",
+                "fdr_bh",
+                "fdr_by",
+                "fdr_tsbh",
+                "fdr_tsbky",
+            ):
+                hypotheses_table(
+                    scores,
+                    estimators,
+                    multitest=multitest,
+                    test=test,
+                    correction=correction,
+                )
```

### Comparing `scikit-datasets-0.2.2/skdatasets/utils/estimator.py` & `scikit-datasets-0.2.3/skdatasets/utils/estimator.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 
     Returns
     -------
     estimator : Estimator
         Instantiated Scikit-learn estimator.
 
     """
-    with open(estimator, 'r') as definition:
+    with open(estimator, "r") as definition:
         estimator = jsonpickle.decode(definition.read())
         for k, v in kwargs.items():
             setattr(estimator, k, v)
         return estimator
```

### Comparing `scikit-datasets-0.2.2/skdatasets/utils/experiment.py` & `scikit-datasets-0.2.3/skdatasets/utils/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """
 @author: David Diaz Vico
 @license: MIT
 """
 from __future__ import annotations
 
 import itertools
-import os
-import sys
 from contextlib import contextmanager
 from dataclasses import dataclass
-from inspect import signature
-from tempfile import NamedTemporaryFile, mkdtemp
-from time import perf_counter, process_time, sleep
+from time import perf_counter, sleep
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
@@ -25,30 +21,29 @@
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 from warnings import warn
 
-import joblib
 import numpy as np
 from sacred import Experiment, Ingredient
 from sacred.observers import FileStorageObserver, MongoObserver, RunObserver
 from sklearn.base import BaseEstimator, is_classifier
+from sklearn.metrics import check_scoring
 from sklearn.model_selection import check_cv
-from sklearn.utils import Bunch, is_scalar_nan
+from sklearn.utils import Bunch
 
 from incense import ExperimentLoader, FileSystemExperimentLoader
 from incense.experiment import FileSystemExperiment
 
 SelfType = TypeVar("SelfType")
 
 
 class DataLike(Protocol):
-
     def __getitem__(
         self: SelfType,
         key: np.typing.NDArray[int],
     ) -> SelfType:
         pass
 
     def __len__(self) -> int:
@@ -65,27 +60,30 @@
     np.typing.NDArray[Union[float, int]],
 ]
 
 ConfigLike = Union[
     Mapping[str, Any],
     str,
 ]
+ScorerLike = Union[
+    str,
+    Callable[[BaseEstimator, DataType, TargetType], float],
+    None,
+]
 
 
 class EstimatorProtocol(Protocol[DataType, TargetType]):
-
     def fit(self: SelfType, X: DataType, y: TargetType) -> SelfType:
         pass
 
     def predict(self, X: DataType) -> TargetType:
         pass
 
 
 class CVSplitter(Protocol):
-
     def split(
         self,
         X: np.typing.NDArray[float],
         y: None = None,
         groups: None = None,
     ) -> Iterable[IndicesType]:
         pass
@@ -168,45 +166,46 @@
     finally:
         final_time = perf_counter()
         elapsed_time = final_time - initial_time
         _append_info(experiment, name, elapsed_time)
 
 
 def _iterate_outer_cv(
-    outer_cv: CVLike | Iterable[
-        Tuple[DataType, TargetType, DataType, TargetType]
-    ],
+    outer_cv: CVLike | Iterable[Tuple[DataType, TargetType, DataType, TargetType]],
     estimator: EstimatorProtocol[DataType, TargetType],
     X: DataType,
     y: TargetType,
 ) -> Iterable[Tuple[DataType, TargetType, DataType, TargetType]]:
     """Iterate over multiple partitions."""
     if isinstance(outer_cv, Iterable):
         outer_cv, cv_copy = itertools.tee(outer_cv)
         if len(next(cv_copy)) == 4:
             yield from outer_cv
 
     cv = check_cv(outer_cv, y, classifier=is_classifier(estimator))
     yield from (
-        (X[train], y[train], X[test], y[test])
-        for train, test in cv.split(X, y)
+        (X[train], y[train], X[test], y[test]) for train, test in cv.split(X, y)
     )
 
 
 def _benchmark_from_data(
     experiment: Experiment,
     *,
     estimator: BaseEstimator,
     X_train: DataType,
     y_train: TargetType,
     X_test: DataType,
     y_test: TargetType,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
 ) -> None:
+
+    scoring_fun = check_scoring(estimator, scoring)
+
     with _add_timing(experiment, "fit_time"):
         estimator.fit(X_train, y_train)
 
     if save_estimator:
         _append_info(experiment, "fitted_estimator", estimator)
 
     best_params = getattr(estimator, "best_params_", None)
@@ -214,88 +213,79 @@
         _append_info(experiment, "search_best_params", best_params)
 
     best_score = getattr(estimator, "best_score_", None)
     if best_params:
         _append_info(experiment, "search_best_score", best_score)
 
     with _add_timing(experiment, "score_time"):
-        test_score = estimator.score(X_test, y_test)
+        test_score = scoring_fun(estimator, X_test, y_test)
 
     _append_info(experiment, "test_score", float(test_score))
 
     if save_train:
-        train_score = estimator.score(X_train, y_train)
+        train_score = scoring_fun(estimator, X_train, y_train)
         _append_info(experiment, "train_score", float(train_score))
 
     for output in ("transform", "predict"):
         method = getattr(estimator, output, None)
         if method is not None:
             with _add_timing(experiment, f"{output}_time"):
                 _append_info(experiment, f"{output}", method(X_test))
 
 
 def _compute_means(experiment: Experiment) -> None:
 
-    experiment.info["score_mean"] = float(
-        np.nanmean(experiment.info["test_score"])
-    )
-    experiment.info["score_std"] = float(
-        np.nanstd(experiment.info["test_score"])
-    )
+    experiment.info["score_mean"] = float(np.nanmean(experiment.info["test_score"]))
+    experiment.info["score_std"] = float(np.nanstd(experiment.info["test_score"]))
 
 
 def _benchmark_one(
     experiment: Experiment,
     *,
     estimator: BaseEstimator,
     data: Bunch,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
 ) -> None:
     """Use only one predefined partition."""
     X = data.data
     y = data.target
 
     train_indices = getattr(data, "train_indices", [])
     validation_indices = getattr(data, "validation_indices", [])
     test_indices = getattr(data, "test_indices", [])
 
-    X_train_val = (
-        X[train_indices + validation_indices]
-        if train_indices
-        else X
-    )
-    y_train_val = (
-        y[train_indices + validation_indices]
-        if train_indices
-        else y
-    )
+    X_train_val = X[train_indices + validation_indices] if train_indices else X
+    y_train_val = y[train_indices + validation_indices] if train_indices else y
 
     X_test = X[test_indices]
     y_test = y[test_indices]
 
     _benchmark_from_data(
         experiment=experiment,
         estimator=estimator,
         X_train=X_train_val,
         y_train=y_train_val,
         X_test=X_test,
         y_test=y_test,
+        scoring=scoring,
         save_estimator=save_estimator,
         save_train=save_train,
     )
 
     _compute_means(experiment)
 
 
 def _benchmark_partitions(
     experiment: Experiment,
     *,
     estimator: BaseEstimator,
     data: Bunch,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
     outer_cv: CVLike | Literal["dataset"] = None,
 ) -> None:
     """Use several partitions."""
     outer_cv = data.outer_cv if outer_cv == "dataset" else outer_cv
 
@@ -309,54 +299,59 @@
         _benchmark_from_data(
             experiment=experiment,
             estimator=estimator,
             X_train=X_train,
             y_train=y_train,
             X_test=X_test,
             y_test=y_test,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
         )
 
     _compute_means(experiment)
 
 
 def _benchmark(
     experiment: Experiment,
     *,
     estimator: BaseEstimator,
     data: Bunch,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
     outer_cv: CVLike | Literal[False, "dataset"] = None,
 ) -> None:
     """Run the experiment."""
     if outer_cv is False:
         _benchmark_one(
             experiment=experiment,
             estimator=estimator,
             data=data,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
         )
     else:
         _benchmark_partitions(
             experiment=experiment,
             estimator=estimator,
             data=data,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
             outer_cv=outer_cv,
         )
 
 
 def experiment(
     dataset: Callable[..., Bunch],
     estimator: Callable[..., BaseEstimator],
     *,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
 ) -> Experiment:
     """
     Prepare a Scikit-learn experiment as a Sacred experiment.
 
     Prepare a Scikit-learn experiment indicating a dataset and an estimator and
@@ -405,14 +400,15 @@
             e = estimator()
 
         # Model assessment
         _benchmark(
             experiment=experiment,
             estimator=e,
             data=data,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
         )
 
         # Ensure that everything is in the info dict at the end
         # See https://github.com/IDSIA/sacred/issues/830
         sleep(experiment.current_run.beat_interval + 1)
@@ -422,30 +418,33 @@
 
 def _get_estimator_function(
     experiment: Experiment,
     estimator: EstimatorLike,
 ) -> Callable[..., EstimatorProtocol[Any, Any]]:
 
     if hasattr(estimator, "fit"):
+
         def estimator_function() -> EstimatorProtocol:
             return estimator
+
     else:
         estimator_function = estimator
 
     return experiment.capture(estimator_function)
 
 
 def _get_dataset_function(
     experiment: Experiment,
     dataset: DatasetLike,
 ) -> Callable[..., Bunch]:
 
     if callable(dataset):
         dataset_function = dataset
     else:
+
         def dataset_function() -> Bunch:
             return dataset
 
     return experiment.capture(dataset_function)
 
 
 def _create_one_experiment(
@@ -454,14 +453,15 @@
     estimator: EstimatorLike,
     dataset_name: str,
     dataset: DatasetLike,
     storage: RunObserver,
     config: ConfigLike,
     inner_cv: CVLike | Literal[False, "dataset"] = None,
     outer_cv: CVLike | Literal[False, "dataset"] = None,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
 ) -> Experiment:
     experiment = Experiment()
 
     experiment.add_config(config)
 
@@ -493,14 +493,15 @@
             estimator.cv = cv
 
         # Model assessment
         _benchmark(
             experiment=experiment,
             estimator=estimator,
             data=dataset,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
             outer_cv=outer_cv,
         )
 
     return experiment
 
@@ -509,14 +510,15 @@
     *,
     datasets: Mapping[str, DatasetLike],
     estimators: Mapping[str, EstimatorLike],
     storage: RunObserver | str,
     config: ConfigLike | None = None,
     inner_cv: CVLike | Literal[False, "dataset"] = False,
     outer_cv: CVLike | Literal[False, "dataset"] = None,
+    scoring: ScorerLike[DataType, TargetType] = None,
     save_estimator: bool = False,
     save_train: bool = False,
 ) -> Sequence[Experiment]:
     """
     Create several Sacred experiments.
 
     It receives a set of estimators and datasets, and create Sacred experiment
@@ -570,14 +572,18 @@
           partition.
         * If ``"dataset"``, the :external:class:`sklearn.utils.Bunch` objects
           for the datasets must have a ``outer_cv`` attribute, which will
           be the one used.
         * Otherwise, this will be passed to
           :external:func:`sklearn.model_selection.check_cv` and the resulting
           cross validator will be used to define the partitions.
+    scoring : string, callable or ``None``, default ``None``
+        Scoring method used to measure the performance of the estimator.
+        If a callable, it should have the signature `scorer(estimator, X, y)`.
+        If ``None`` it uses the ``scorer`` method of the estimator.
     save_estimator : bool, default ``False``
         Whether to save the fitted estimator. This is useful for debugging
         and for obtaining extra information in some cases, but for some
         estimators it could consume much storage.
     save_train : bool, default ``False``
         If ``True``, compute and store also the score over the train data.
 
@@ -604,14 +610,15 @@
             estimator=estimator,
             dataset_name=dataset_name,
             dataset=dataset,
             storage=storage,
             config=config,
             inner_cv=inner_cv,
             outer_cv=outer_cv,
+            scoring=scoring,
             save_estimator=save_estimator,
             save_train=save_train,
         )
         for estimator_name, estimator in estimators.items()
         for dataset_name, dataset in datasets.items()
     ]
 
@@ -673,37 +680,36 @@
     estimator_names: Sequence[str] | None = None,
 ) -> Sequence[Experiment]:
 
     loader = _loader_from_observer(storage)
 
     if (
         (ids, dataset_names, estimator_names) == (None, None, None)
-        or isinstance(loader, FileSystemExperimentLoader) and ids is None
+        or isinstance(loader, FileSystemExperimentLoader)
+        and ids is None
     ):
         find_all_fun = getattr(
             loader,
             "find_all",
             lambda: [
                 FileSystemExperiment.from_run_dir(run_dir)
                 for run_dir in loader._runs_dir.iterdir()
             ],
         )
 
         experiments = find_all_fun()
 
-    elif (
-        (dataset_names, estimator_names) == (None, None)
-        or isinstance(loader, FileSystemExperimentLoader)
+    elif (dataset_names, estimator_names) == (None, None) or isinstance(
+        loader, FileSystemExperimentLoader
     ):
         load_ids_fun = getattr(
             loader,
             "find_by_ids",
             lambda id_seq: [
-                loader.find_by_id(experiment_id)
-                for experiment_id in id_seq
+                loader.find_by_id(experiment_id) for experiment_id in id_seq
             ],
         )
 
         experiments = load_ids_fun(ids)
 
     else:
 
@@ -714,37 +720,34 @@
             ]
         ] = []
 
         if ids is not None:
             conditions.append({"_id": {"$in": ids}})
 
         if estimator_names is not None:
-            conditions.append(
-                {"config.estimator_name": {"$in": estimator_names}})
+            conditions.append({"config.estimator_name": {"$in": estimator_names}})
 
         if dataset_names is not None:
             conditions.append({"config.dataset_name": {"$in": dataset_names}})
 
         query = {"$and": conditions}
 
         experiments = loader.find(query)
 
     if isinstance(loader, FileSystemExperimentLoader):
         # Filter experiments by dataset and estimator names
         experiments = [
-            e for e in experiments
+            e
+            for e in experiments
             if (
                 (
                     estimator_names is None
                     or e.config["estimator_name"] in estimator_names
                 )
-                and (
-                    dataset_names is None
-                    or e.config["dataset_name"] in dataset_names
-                )
+                and (dataset_names is None or e.config["dataset_name"] in dataset_names)
             )
         ]
 
     return experiments
 
 
 def fetch_scores(
@@ -838,17 +841,15 @@
             score_mean,
             score_std,
         )
 
     estimator_names = (
         tuple(estimator_list) if estimator_names is None else estimator_names
     )
-    dataset_names = (
-        tuple(dataset_list) if dataset_names is None else dataset_names
-    )
+    dataset_names = tuple(dataset_list) if dataset_names is None else dataset_names
     matrix_shape = (len(dataset_names), len(estimator_names))
 
     scores = np.full(matrix_shape + (nobs,), np.nan)
     scores_mean = np.full(matrix_shape, np.nan)
     scores_std = np.full(matrix_shape, np.nan)
 
     for i, dataset_name in enumerate(dataset_names):
```

### Comparing `scikit-datasets-0.2.2/skdatasets/utils/scores.py` & `scikit-datasets-0.2.3/skdatasets/utils/scores.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,15 @@
 @license: MIT
 """
 from __future__ import annotations
 
 import itertools as it
 from dataclasses import dataclass
 from functools import reduce
-from typing import (
-    Any,
-    Callable,
-    Iterable,
-    Literal,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    overload,
-)
+from typing import Any, Callable, Literal, Mapping, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 from scipy.stats import (
     friedmanchisquare,
     kruskal,
     mannwhitneyu,
@@ -29,29 +19,29 @@
     wilcoxon,
 )
 from scipy.stats.stats import ttest_ind_from_stats, ttest_rel
 from statsmodels.sandbox.stats.multicomp import multipletests
 
 CorrectionLike = Literal[
     None,
-    'bonferroni',
-    'sidak',
-    'holm-sidak',
-    'holm',
-    'simes-hochberg',
-    'hommel',
-    'fdr_bh',
-    'fdr_by',
-    'fdr_tsbh',
-    'fdr_tsbky',
+    "bonferroni",
+    "sidak",
+    "holm-sidak",
+    "holm",
+    "simes-hochberg",
+    "hommel",
+    "fdr_bh",
+    "fdr_by",
+    "fdr_tsbh",
+    "fdr_tsbky",
 ]
 
-MultitestLike = Literal['kruskal', 'friedmanchisquare']
+MultitestLike = Literal["kruskal", "friedmanchisquare"]
 
-TestLike = Literal['mannwhitneyu', 'wilcoxon']
+TestLike = Literal["mannwhitneyu", "wilcoxon"]
 
 
 @dataclass
 class SummaryRow:
     values: np.typing.NDArray[Any]
     greater_is_better: bool | None = None
 
@@ -230,30 +220,32 @@
     return styler
 
 
 def _set_style_formatter(
     styler: pd.io.formats.style.Styler,
     *,
     precision: int,
+    show_rank: bool = True,
 ) -> pd.io.formats.style.Styler:
-
     def _formatter(
         data: object,
     ) -> str:
         if isinstance(data, str):
             return data
         elif isinstance(data, int):
             return str(int)
         elif isinstance(data, float):
             return f"{data:.{precision}f}"
         elif isinstance(data, ScoreCell):
-            str_repr = f'{data.mean:.{precision}f}'
+            str_repr = f"{data.mean:.{precision}f}"
             if data.std is not None:
-                str_repr += f' ± {data.std:.{precision}f}'
-            str_repr += f' ({data.rank:.0f})'
+                str_repr += f" ± {data.std:.{precision}f}"
+            if show_rank:
+                precision_rank = 0 if isinstance(data.rank, int) else precision
+                str_repr += f" ({data.rank:.{precision_rank}f})"
             return str_repr
         else:
             return ""
 
     return styler.format(
         _formatter,
     )
@@ -281,15 +273,15 @@
             {
                 "selector": ".rank2",
                 "props": [("text-decoration", "underline")],
             },
             {
                 "selector": ".significant::after",
                 "props": [
-                    ("content", "\"*\""),
+                    ("content", '"*"'),
                     ("width", "0px"),
                     ("display", "inline-block"),
                 ],
             },
             {
                 "selector": ".col_heading",
                 "props": [("font-weight", "bold")],
@@ -341,33 +333,33 @@
 
     last_rows_mask = np.zeros(len(styler.data), dtype=int)
     last_rows_mask[-n_summary_rows:] = 1
 
     styler.set_table_styles(
         [
             {
-                'selector': r'newcommand{\summary}',
-                'props': r':[1]{\textit{#1}};',
+                "selector": r"newcommand{\summary}",
+                "props": r":[1]{\textit{#1}};",
             },
             {
-                'selector': r'newcommand{\significant}',
-                'props': r':[1]{#1*};',
+                "selector": r"newcommand{\significant}",
+                "props": r":[1]{#1*};",
             },
             {
-                'selector': r'newcommand{\rank}',
-                'props': (
-                    r':[2]{\ifnum#1=1 \textbf{#2} \else '
-                    r'\ifnum#1=2 \underline{#2} \fi\fi};'
+                "selector": r"newcommand{\rank}",
+                "props": (
+                    r":[2]{\ifnum#1=1 \textbf{#2} \else "
+                    r"\ifnum#1=2 \underline{#2} \else #2 \fi\fi};"
                 ),
             },
         ],
         overwrite=False,
     )
 
-    for rank in range(styler.data.shape[1]):
+    for rank in range(1, styler.data.shape[1] + 1):
         styler = _set_style_from_class(
             styler,
             f"rank{rank}",
             f"rank{{{rank}}}:--rwrap; ",
         )
 
     for class_name in ("summary", "significant"):
@@ -419,20 +411,21 @@
     scores: np.typing.ArrayLike,
     stds: np.typing.ArrayLike | None = None,
     *,
     datasets: Sequence[str],
     estimators: Sequence[str],
     nobs: int | None = None,
     greater_is_better: bool = True,
-    method: Literal['average', 'min', 'max', 'dense', 'ordinal'] = 'min',
+    method: Literal["average", "min", "max", "dense", "ordinal"] = "min",
     significancy_level: float = 0,
     paired_test: bool = False,
     two_sided: bool = True,
     default_style: Literal["html", "latex", None] = "html",
     precision: int = 2,
+    show_rank: bool = True,
     summary_rows: Sequence[Tuple[str, Callable[..., SummaryRow]]] = (
         ("Average rank", average_rank),
     ),
 ) -> pd.io.formats.style.Styler:
     """
     Scores table.
 
@@ -498,20 +491,22 @@
     means = scores if scores.ndim == 2 else np.mean(scores, axis=-1)
     if scores.ndim == 3:
         assert stds is None
         assert nobs is None
         stds = np.std(scores, axis=-1)
         nobs = scores.shape[-1]
 
-    ranks = np.asarray([
-        rankdata(-m, method=method)
-        if greater_is_better
-        else rankdata(m, method=method)
-        for m in means
-    ])
+    ranks = np.asarray(
+        [
+            rankdata(-m, method=method)
+            if greater_is_better
+            else rankdata(m, method=method)
+            for m in means.round(precision)
+        ]
+    )
 
     significants = _all_significants(
         scores,
         means,
         stds,
         ranks,
         nobs=nobs,
@@ -522,15 +517,15 @@
 
     table = pd.DataFrame(data=means, index=datasets, columns=estimators)
     for i, d in enumerate(datasets):
         for j, e in enumerate(estimators):
             table.loc[d, e] = ScoreCell(
                 mean=means[i, j],
                 std=None if stds is None else stds[i, j],
-                rank=ranks[i, j],
+                rank=int(ranks[i, j]),
                 significant=significants[i, j],
             )
 
     # Create additional summary rows
     additional_ranks = []
     for name, summary_fun in summary_rows:
         row = summary_fun(
@@ -557,14 +552,15 @@
         significants=significants,
         n_summary_rows=len(summary_rows),
     )
 
     styler = _set_style_formatter(
         styler,
         precision=precision,
+        show_rank=show_rank,
     )
 
     return _set_default_style(
         styler,
         n_summary_rows=len(summary_rows),
         default_style=default_style,
     )
@@ -572,15 +568,15 @@
 
 def hypotheses_table(
     samples: np.typing.ArrayLike,
     models: Sequence[str],
     *,
     alpha: float = 0.05,
     multitest: Optional[MultitestLike] = None,
-    test: TestLike = 'wilcoxon',
+    test: TestLike = "wilcoxon",
     correction: CorrectionLike = None,
     multitest_args: Optional[Mapping[str, Any]] = None,
     test_args: Optional[Mapping[str, Any]] = None,
 ) -> Tuple[Optional[pd.DataFrame], Optional[pd.DataFrame]]:
     """
     Hypotheses table.
 
@@ -623,78 +619,67 @@
     if test_args is None:
         test_args = {}
 
     samples = np.asanyarray(samples)
 
     versus = list(it.combinations(range(len(models)), 2))
     comparisons = [
-        f"{models[first]} vs {models[second]}"
-        for first, second in versus
+        f"{models[first]} vs {models[second]}" for first, second in versus
     ]
 
     multitests = {
-        'kruskal': kruskal,
-        'friedmanchisquare': friedmanchisquare,
+        "kruskal": kruskal,
+        "friedmanchisquare": friedmanchisquare,
     }
     tests = {
-        'mannwhitneyu': mannwhitneyu,
-        'wilcoxon': wilcoxon,
+        "mannwhitneyu": mannwhitneyu,
+        "wilcoxon": wilcoxon,
     }
 
     multitest_table = None
     if multitest is not None:
         multitest_table = pd.DataFrame(
             index=[multitest],
-            columns=['p-value', 'Hypothesis'],
+            columns=["p-value", "Hypothesis"],
         )
         _, pvalue = multitests[multitest](
             *samples.T,
             **multitest_args,
         )
-        reject_str = 'Rejected' if pvalue <= alpha else 'Not rejected'
-        multitest_table.loc[multitest] = ['{0:.2f}'.format(pvalue), reject_str]
+        reject_str = "Rejected" if pvalue <= alpha else "Not rejected"
+        multitest_table.loc[multitest] = ["{0:.2f}".format(pvalue), reject_str]
 
         # If the multitest does not detect a significative difference,
         # the individual tests are not meaningful, so skip them.
         if pvalue > alpha:
             return multitest_table, None
 
     pvalues = [
         tests[test](
             samples[:, first],
             samples[:, second],
             **test_args,
-        )[1] for first, second in versus
+        )[1]
+        for first, second in versus
     ]
 
     if correction is not None:
         reject_bool, pvalues, _, _ = multipletests(
             pvalues,
             alpha,
             method=correction,
         )
-        reject = [
-            'Rejected'
-            if r
-            else 'Not rejected'
-            for r in reject_bool
-        ]
+        reject = ["Rejected" if r else "Not rejected" for r in reject_bool]
     else:
         reject = [
-            'Rejected'
-            if pvalue <= alpha
-            else 'Not rejected'
-            for pvalue in pvalues
+            "Rejected" if pvalue <= alpha else "Not rejected" for pvalue in pvalues
         ]
 
-    data = [
-        ('{0:.2f}'.format(p), r)
-        for p, r in zip(pvalues, reject)
-    ]
+    data = [("{0:.2f}".format(p), r) for p, r in zip(pvalues, reject)]
 
     test_table = pd.DataFrame(
         data,
         index=comparisons,
-        columns=['p-value', 'Hypothesis'],
+        columns=["p-value", "Hypothesis"],
     )
 
     return multitest_table, test_table
```

