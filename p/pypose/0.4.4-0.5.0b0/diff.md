# Comparing `tmp/pypose-0.4.4.tar.gz` & `tmp/pypose-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.4.4.tar", last modified: Sat Jun  3 19:15:29 2023, max compression
+gzip compressed data, was "pypose-0.5.0b0.tar", last modified: Mon Jun 19 06:08:47 2023, max compression
```

## Comparing `pypose-0.4.4.tar` & `pypose-0.5.0b0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.754408 pypose-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-03 19:15:13.000000 pypose-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-03 19:15:29.754408 pypose-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-03 19:15:13.000000 pypose-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose/function/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/checking.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/function/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    43346 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/pnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-03 19:15:13.000000 pypose-0.4.4/pypose/utils/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.746408 pypose-0.4.4/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:15:29.000000 pypose-0.4.4/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:15:29.750408 pypose-0.4.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-03 19:15:13.000000 pypose-0.4.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-03 19:15:13.000000 pypose-0.4.4/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:15:29.754408 pypose-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-03 19:15:13.000000 pypose-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-19 06:08:37.000000 pypose-0.5.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-19 06:08:47.789939 pypose-0.5.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-19 06:08:37.000000 pypose-0.5.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/function/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33855 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43346 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31560 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109672 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24653 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22445 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24664 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-19 06:08:37.000000 pypose-0.5.0b0/pypose/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.785939 pypose-0.5.0b0/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:08:47.000000 pypose-0.5.0b0/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:08:47.789939 pypose-0.5.0b0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 06:08:37.000000 pypose-0.5.0b0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 06:08:37.000000 pypose-0.5.0b0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:08:47.789939 pypose-0.5.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-19 06:08:37.000000 pypose-0.5.0b0/setup.py
```

### Comparing `pypose-0.4.4/LICENSE` & `pypose-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/PKG-INFO` & `pypose-0.5.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.4
+Version: 0.5.0b0
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.4.4/README.md` & `pypose-0.5.0b0/README.md`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/__init__.py` & `pypose-0.5.0b0/pypose/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/basics/ops.py` & `pypose-0.5.0b0/pypose/basics/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/function/checking.py` & `pypose-0.5.0b0/pypose/function/checking.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/function/geometry.py` & `pypose-0.5.0b0/pypose/function/geometry.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/function/linalg.py` & `pypose-0.5.0b0/pypose/function/linalg.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/__init__.py` & `pypose-0.5.0b0/pypose/lietensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/basics.py` & `pypose-0.5.0b0/pypose/lietensor/basics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/convert.py` & `pypose-0.5.0b0/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/lietensor.py` & `pypose-0.5.0b0/pypose/lietensor/lietensor.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/operation.py` & `pypose-0.5.0b0/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/lietensor/utils.py` & `pypose-0.5.0b0/pypose/lietensor/utils.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/dynamics.py` & `pypose-0.5.0b0/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/ekf.py` & `pypose-0.5.0b0/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/icp.py` & `pypose-0.5.0b0/pypose/module/icp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/imu_preintegrator.py` & `pypose-0.5.0b0/pypose/module/imu_preintegrator.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/pf.py` & `pypose-0.5.0b0/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/pnp.py` & `pypose-0.5.0b0/pypose/module/pnp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/module/ukf.py` & `pypose-0.5.0b0/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/corrector.py` & `pypose-0.5.0b0/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/functional.py` & `pypose-0.5.0b0/pypose/optim/functional.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/kernel.py` & `pypose-0.5.0b0/pypose/optim/kernel.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/optimizer.py` & `pypose-0.5.0b0/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/scheduler.py` & `pypose-0.5.0b0/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/solver.py` & `pypose-0.5.0b0/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/optim/strategy.py` & `pypose-0.5.0b0/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/utils/collect_env.py` & `pypose-0.5.0b0/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose/utils/stepper.py` & `pypose-0.5.0b0/pypose/utils/stepper.py`

 * *Files identical despite different names*

### Comparing `pypose-0.4.4/pypose.egg-info/PKG-INFO` & `pypose-0.5.0b0/pypose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.4.4
+Version: 0.5.0b0
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
```

### Comparing `pypose-0.4.4/pypose.egg-info/SOURCES.txt` & `pypose-0.5.0b0/pypose.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pypose/lietensor/utils.py
 pypose/module/__init__.py
 pypose/module/dynamics.py
 pypose/module/ekf.py
 pypose/module/icp.py
 pypose/module/imu_preintegrator.py
 pypose/module/lqr.py
+pypose/module/mpc.py
 pypose/module/pf.py
 pypose/module/pnp.py
 pypose/module/ukf.py
 pypose/optim/__init__.py
 pypose/optim/corrector.py
 pypose/optim/functional.py
 pypose/optim/kernel.py
```

### Comparing `pypose-0.4.4/setup.py` & `pypose-0.5.0b0/setup.py`

 * *Files identical despite different names*

