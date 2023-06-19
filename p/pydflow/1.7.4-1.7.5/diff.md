# Comparing `tmp/pydflow-1.7.4.tar.gz` & `tmp/pydflow-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.7.4.tar", last modified: Wed Jun 14 08:58:59 2023, max compression
+gzip compressed data, was "pydflow-1.7.5.tar", last modified: Mon Jun 19 08:48:12 2023, max compression
```

## Comparing `pydflow-1.7.4.tar` & `pydflow-1.7.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.613044 pydflow-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-14 08:58:37.000000 pydflow-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 08:58:37.000000 pydflow-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-14 08:58:59.613044 pydflow-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-14 08:58:37.000000 pydflow-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 08:58:37.000000 pydflow-1.7.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:58:59.613044 pydflow-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-14 08:58:37.000000 pydflow-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.601044 pydflow-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.605044 pydflow-1.7.4/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.609044 pydflow-1.7.4/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.609044 pydflow-1.7.4/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/launching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.609044 pydflow-1.7.4/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    31751 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)   102606 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45085 2023-06-14 08:58:37.000000 pydflow-1.7.4/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.613044 pydflow-1.7.4/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 08:58:59.000000 pydflow-1.7.4/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:59.613044 pydflow-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-14 08:58:37.000000 pydflow-1.7.4/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.911081 pydflow-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-19 08:48:03.000000 pydflow-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 08:48:03.000000 pydflow-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-19 08:48:12.911081 pydflow-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-19 08:48:03.000000 pydflow-1.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 08:48:03.000000 pydflow-1.7.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:48:12.911081 pydflow-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-19 08:48:03.000000 pydflow-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.899080 pydflow-1.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.903080 pydflow-1.7.5/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.903080 pydflow-1.7.5/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31751 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102981 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25735 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-06-19 08:48:03.000000 pydflow-1.7.5/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 08:48:12.000000 pydflow-1.7.5/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:48:12.907081 pydflow-1.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-19 08:48:03.000000 pydflow-1.7.5/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.7.4/LICENSE` & `pydflow-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/PKG-INFO` & `pydflow-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.4
+Version: 1.7.5
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.4/README.md` & `pydflow-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/setup.py` & `pydflow-1.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/__init__.py` & `pydflow-1.7.5/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/argo_objects.py` & `pydflow-1.7.5/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.7.5/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.7.5/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.7.5/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.7.5/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.7.5/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/common.py` & `pydflow-1.7.5/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/config.py` & `pydflow-1.7.5/src/dflow/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "register_tasks": boolize(os.environ.get("DFLOW_REGISTER_TASKS", False)),
     "http_headers": split_headers(os.environ.get("DFLOW_HTTP_HEADERS", {})),
     "workflow_annotations": json.loads(os.environ.get(
         "DFLOW_WORKFLOW_ANNOTATIONS", "{}")),
     "overwrite_reused_artifact": boolize(os.environ.get(
         "DFLOW_OVERWRITE_REUSED_ARTIFACT", True)),
     "detach": boolize(os.environ.get("DFLOW_DETACH", False)),
+    "debug_copy_method": os.environ.get("DFLOW_DEBUG_COPY_METHOD", "symlink"),
 }
 
 
 def set_config(
     **kwargs,
 ) -> None:
     """
```

### Comparing `pydflow-1.7.4/src/dflow/context_syntax.py` & `pydflow-1.7.5/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/dag.py` & `pydflow-1.7.5/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/executor.py` & `pydflow-1.7.5/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/io.py` & `pydflow-1.7.5/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/main.py` & `pydflow-1.7.5/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/op_template.py` & `pydflow-1.7.5/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/bohrium.py` & `pydflow-1.7.5/src/dflow/plugins/bohrium.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/datasets.py` & `pydflow-1.7.5/src/dflow/plugins/datasets.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/dispatcher.py` & `pydflow-1.7.5/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/launching.py` & `pydflow-1.7.5/src/dflow/plugins/launching.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/lebesgue.py` & `pydflow-1.7.5/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/metadata.py` & `pydflow-1.7.5/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/oss.py` & `pydflow-1.7.5/src/dflow/plugins/oss.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/plugins/ray.py` & `pydflow-1.7.5/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/python/op.py` & `pydflow-1.7.5/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/python/opio.py` & `pydflow-1.7.5/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/python/python_op_template.py` & `pydflow-1.7.5/src/dflow/python/python_op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/python/utils.py` & `pydflow-1.7.5/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/resource.py` & `pydflow-1.7.5/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/slurm.py` & `pydflow-1.7.5/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/step.py` & `pydflow-1.7.5/src/dflow/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 import re
+import shutil
 import sys
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import jsonpickle
 
 from .common import CustomArtifact, HTTPArtifact, LocalArtifact, S3Artifact
@@ -15,16 +16,16 @@
 from .io import (PVC, ArgoVar, Expression, InputArtifact, InputParameter,
                  OutputArtifact, OutputParameter, if_expression, to_expr)
 from .op_template import (OPTemplate, PythonScriptOPTemplate, ScriptOPTemplate,
                           ShellOPTemplate)
 from .python import Slices
 from .resource import Resource
 from .util_ops import CheckNumSuccess, CheckSuccessRatio, InitArtifactForSlices
-from .utils import (add_prefix_to_slice, catalog_of_artifact, flatten,
-                    merge_dir, randstr, upload_artifact)
+from .utils import (add_prefix_to_slice, catalog_of_artifact, copy_file,
+                    flatten, merge_dir, randstr, upload_artifact)
 
 try:
     from argo.workflows.client import (V1alpha1Arguments, V1alpha1ContinueOn,
                                        V1alpha1ResourceTemplate,
                                        V1alpha1WorkflowStep, V1VolumeMount)
 
     from .client import V1alpha1Sequence
@@ -1848,16 +1849,22 @@
             os.makedirs(os.path.dirname(
                 os.path.abspath(path)), exist_ok=True)
             backup(path)
             if isinstance(
                     art.source,
                     InputArtifact) and art.source is None and art.optional:
                 pass
-            else:
+            elif config["debug_copy_method"] == "symlink":
                 os.symlink(art_path, path)
+            elif config["debug_copy_method"] == "link":
+                copy_file(art_path, path)
+            elif config["debug_copy_method"] == "copy":
+                copy_file(art_path, path, func=shutil.copy2)
+            else:
+                raise ValueError("Unsupported copy method for debug mode.")
 
         # render variables in the script
         script = self.template.script
         if not self.template.script_rendered:
             if hasattr(self.template, "tmp_root"):
                 # do not modify self.template
                 template = deepcopy(self.template)
```

### Comparing `pydflow-1.7.4/src/dflow/steps.py` & `pydflow-1.7.5/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/task.py` & `pydflow-1.7.5/src/dflow/task.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/util_ops.py` & `pydflow-1.7.5/src/dflow/util_ops.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/utils.py` & `pydflow-1.7.5/src/dflow/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/src/dflow/workflow.py` & `pydflow-1.7.5/src/dflow/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,18 +337,20 @@
                 outputs["parameters"] = []
                 for name, par in step.outputs.parameters.items():
                     if not hasattr(step.outputs.parameters[name],
                                    "save_as_artifact"):
                         outputs["parameters"].append(par.recover())
             if hasattr(step.outputs, "artifacts"):
                 for name, art in step.outputs.artifacts.items():
-                    if hasattr(step, "inputs") and \
-                        hasattr(step.inputs, "parameters") and \
-                        "dflow_group_key" in step.inputs.parameters \
-                            and name != "main-logs":
+                    group_key = step.get("inputs", {}).get(
+                        "parameters", {}).get("dflow_group_key", {}).get(
+                        "value")
+                    art_key = get_key(art, raise_error=False)
+                    if group_key and art_key and art_key.endswith(
+                            "%s/%s" % (group_key, name)):
                         if config["overwrite_reused_artifact"]:
                             self.handle_reused_artifact(step, name, art)
                         else:
                             self.handle_reused_artifact_with_copy(
                                 step, name, art)
 
         outputs["artifacts"] = [
```

### Comparing `pydflow-1.7.4/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.7.5/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.4
+Version: 1.7.5
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.4/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.7.5/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_big_parameter.py` & `pydflow-1.7.5/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_conditional_outputs.py` & `pydflow-1.7.5/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_dag.py` & `pydflow-1.7.5/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_group_size.py` & `pydflow-1.7.5/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_makevasp.py` & `pydflow-1.7.5/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_python.py` & `pydflow-1.7.5/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_recurse.py` & `pydflow-1.7.5/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_reuse.py` & `pydflow-1.7.5/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_slices.py` & `pydflow-1.7.5/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.4/tests/test_subpath_slices.py` & `pydflow-1.7.5/tests/test_subpath_slices.py`

 * *Files identical despite different names*

