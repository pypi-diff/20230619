# Comparing `tmp/sarus_data_spec_public-3.5.1.tar.gz` & `tmp/sarus_data_spec_public-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.5.1.tar", last modified: Thu Jun  8 13:27:13 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.5.5.tar", last modified: Mon Jun 19 12:32:44 2023, max compression
```

## Comparing `sarus_data_spec_public-3.5.1.tar` & `sarus_data_spec_public-3.5.5.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.609702 sarus_data_spec_public-3.5.1/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      825 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.611702 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6445 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10508 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4702 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.611702 sarus_data_spec_public-3.5.1/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.612702 sarus_data_spec_public-3.5.1/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18991 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.612702 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    11349 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.613702 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    27034 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.614702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30163 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.614702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8793 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.615702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.615702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.616702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5988 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.616702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.618702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12912 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.618702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7902 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    73600 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    34273 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.622702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38501 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     6872 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5997 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    24500 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6094 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    11092 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.623702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16286 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12002 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11186 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     9205 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.624702 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10475 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.635702 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    74241 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29134 2023-06-08 13:27:05.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10848 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4640 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    16874 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.635702 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 13:26:57.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12136 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     4969 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30852 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   137075 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    36553 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:27:13.636702 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7841 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 13:27:13.000000 sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-08 13:27:13.637702 sarus_data_spec_public-3.5.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-08 13:26:56.000000 sarus_data_spec_public-3.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.764302 sarus_data_spec_public-3.5.5/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-19 12:32:44.764302 sarus_data_spec_public-3.5.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.731302 sarus_data_spec_public-3.5.5/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      825 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.732302 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6445 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10508 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4702 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.732302 sarus_data_spec_public-3.5.5/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3770 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.733302 sarus_data_spec_public-3.5.5/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18990 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.734302 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11349 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.735302 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15008 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    27058 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3593 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4514 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.736302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7507 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30163 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.737302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8793 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.737302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.737302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.738302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5988 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.738302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.740302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13227 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.741302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7902 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    73410 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    34273 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.744302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38501 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6872 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5997 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    24500 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6094 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.746302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16286 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12002 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11186 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     8671 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11609 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27450 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.747302 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.761302 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3672 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8843 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5793 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    13978 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39597 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2023-06-19 12:32:36.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10848 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4640 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16874 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.762302 sarus_data_spec_public-3.5.5/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13776 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5448 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32463 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   137075 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    36553 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 12:32:44.764302 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7841 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-19 12:32:44.000000 sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-19 12:32:44.765302 sarus_data_spec_public-3.5.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-19 12:32:23.000000 sarus_data_spec_public-3.5.5/setup.py
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.5.1'
+VERSION: Final[str] = '3.5.5'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,30 @@
 
 
 async def async_arrow_batches_to_series(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the first columns of the DataFrame."""
     df = await async_arrow_batches_to_dataframe(batches_async_iterator)
-    first_col = df.columns[0]
-    series = df[first_col]
-    if first_col == NO_SERIES_NAME:
-        # This is a default value for a column.
-        # The series actually has no name.
-        series.name = None
+    n_rows, n_cols = df.shape
+    if n_rows == 1:
+        series = df.iloc[0]
+    elif n_cols == 1:
+        first_col = df.columns[0]
+        series = df[first_col]
+        if first_col == NO_SERIES_NAME:
+            # This is a default value for a column.
+            # The series actually has no name.
+            series.name = None
+    else:
+        raise ValueError(
+            "Trying to convert to series Arrow batches "
+            "with more than 1 line and 1 column."
+        )
+
     return series
 
 
 def to_pyarrow_table(data: t.Any) -> pa.Table:
     """Convert the result of an external transform to a Pyarrow Table."""
     if not type(data) in t.get_args(st.DatasetCastable):
         raise TypeError(f"Cannot convert {type(data)} to Arrow batches.")
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.5.5/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 SYNTHETIC_TASK = 'synthetic'
 
 
 # Privacy
 PEP_TOKEN = "pep_token"
 NO_TOKEN = "no_token"
 IS_PUBLIC = "is_public"
+IS_SYNTHETIC = "is_synthetic"
 PRIVACY_LIMIT = "privacy_limit"
 CONSTRAINT_KIND = "constraint_kind"
 BEST_ALTERNATIVE = "best_alternative"
 
 # QUERYBUILDER
 QUERIES = 'queries'
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         with a random uuid so that even if they are submitted multiple times to
         an account, they are only accounted once (ask @cgastaud for more on
         accounting).
         """
         return self.manager().dataspec_validator().private_queries(self)
 
     def spec(self) -> str:
-        return cast(str, self.protobuf().spec.WhichOneof('spec'))
+        return cast(str, self._protobuf.spec.WhichOneof('spec'))
 
     def __iter__(self) -> Iterator[pa.RecordBatch]:
         return self.to_arrow(batch_size=1)
 
     def to_pandas(self) -> pd.DataFrame:
         return self.manager().to_pandas(self)
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from typing import Collection, List, Optional, cast
 import json
 import logging
 
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import (
-    IS_PUBLIC,
     IS_VALID,
     NO_TOKEN,
     PEP_TOKEN,
     PRIVATE_QUERY,
     PUBLIC,
 )
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
@@ -66,15 +65,15 @@
 
     def verifies(
         self,
         variant_constraint: st.VariantConstraint,
         kind: st.ConstraintKind,
         public_context: Collection[str],
         privacy_limit: Optional[st.PrivacyLimit],
-    ) -> bool:
+    ) -> Optional[bool]:
         """Check if the constraint attached to a Dataspec meets requirements.
 
         This function is useful because comparisons are not straightforwards.
         For instance, a Dataspec might have the variant constraint SYNTHETIC
         attached to it. This synthetic dataspec also verifies the DP constraint
         and the PUBLIC constraint.
 
@@ -124,18 +123,22 @@
         the SYNTHETIC constraint.
         """
         # TODO fetch real context and epsilon
         public_context: Collection[str] = []
         privacy_limit = None
         kind = st.ConstraintKind.SYNTHETIC
 
-        # Does any saved constraint yet verifies that the Dataspec is synthetic
+        self.is_public(dataspec)
+
         for constraint in self.verified_constraints(dataspec):
-            if self.verifies(constraint, kind, public_context, privacy_limit):
-                return True
+            check_constraint = self.verifies(
+                constraint, kind, public_context, privacy_limit
+            )
+            if check_constraint is not None:
+                return check_constraint
 
         # Determine is the Dataspec is synthetic
         if dataspec.is_transformed():
             transform = dataspec.transform()
             if transform.protobuf().spec.HasField("synthetic"):
                 is_synthetic = True
             else:
@@ -153,16 +156,15 @@
                         if isinstance(ds, st.DataSpec)
                     ]
                 )
         else:
             is_synthetic = False
 
         # save variant constraint
-        if is_synthetic:
-            syn_constraint(dataspec)
+        syn_constraint(dataspec, is_synthetic=is_synthetic)
 
         return is_synthetic
 
     def is_public(self, dataspec: st.DataSpec) -> bool:
         """Return True if the dataspec is public.
 
         Some DataSpecs are intrinsically Public, this is the case if they are
@@ -177,18 +179,20 @@
         PUBLIC constraint.
         """
         # TODO fetch real context and epsilon
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
         kind = st.ConstraintKind.PUBLIC
 
-        # Does any saved constraint yet verifies that the Dataspec is public
         for constraint in self.verified_constraints(dataspec):
-            if self.verifies(constraint, kind, public_context, privacy_limit):
-                return constraint.properties()[IS_PUBLIC] == str(True)
+            check_constraint = self.verifies(
+                constraint, kind, public_context, privacy_limit
+            )
+            if check_constraint is not None:
+                return check_constraint
 
         # Determine is the Dataspec is public
         if dataspec.is_transformed():
             # Returns true if the DataSpec derives only from public
             if (
                 dataspec.transform().is_external()
                 or dataspec.prototype() == sp.Scalar
@@ -256,19 +260,23 @@
         dataset = cast(st.Dataset, dataspec)
 
         # TODO fetch real context and budget
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
         kind = st.ConstraintKind.PEP
 
-        # Does any constraint yet verifies that the Dataset is PEP
-        for constraint in self.verified_constraints(dataset):
-            if self.verifies(constraint, kind, public_context, privacy_limit):
-                stored_token = constraint.properties()[PEP_TOKEN]
-                return None if stored_token == NO_TOKEN else stored_token
+        for constraint in self.verified_constraints(dataspec):
+            check_constraint = self.verifies(
+                constraint, kind, public_context, privacy_limit
+            )
+            if check_constraint is not None:
+                if check_constraint:
+                    return constraint.properties()[PEP_TOKEN]
+                else:
+                    return None
 
         # Compute the PEP token
         if not dataset.is_transformed():
             return None
 
         transform = dataset.transform()
         _, StaticChecker = routing.get_dataset_op(transform)
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,18 +417,18 @@
             if ds.prototype() == sp.Dataset:
                 dataset = t.cast(st.Dataset, self.static_value())
                 if self.kind is None:
                     raise ValueError(
                         f"Parameter {self.name()} is a Dataset, but no type "
                         "to cast to is defined."
                     )
-                return dataset.to(self.dataset_types[self.kind])
+                return await dataset.async_to(self.dataset_types[self.kind])
             else:
                 scalar = t.cast(st.Scalar, ds)
-                return scalar.value()
+                return await scalar.async_value()
         elif isinstance(self.static_value(), st.Transform):
             transform = t.cast(st.Transform, self.static_value())
             return transform.composed_callable()
         else:
             return self.static_value()
 
     def callable(self) -> t.Callable[..., SarusArgumentValue]:
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from typing import Collection, List, Optional, Tuple, cast
 import logging
 
-from sarus_data_spec.constants import IS_PUBLIC
+from sarus_data_spec.constants import (
+    IS_PUBLIC,
+    IS_SYNTHETIC,
+    NO_TOKEN,
+    PEP_TOKEN,
+)
 import sarus_data_spec.typing as st
 
 ArgStruct = Tuple[List[int], List[str]]
 logger = logging.getLogger(__name__)
 
 
 def verifies(
     variant_constraint: st.VariantConstraint,
     kind: st.ConstraintKind,
     public_context: Collection[str],
     privacy_limit: Optional[st.PrivacyLimit],
-) -> bool:
+) -> Optional[bool]:
     if kind == st.ConstraintKind.PUBLIC:
         return verifies_public(variant_constraint=variant_constraint)
 
     elif kind == st.ConstraintKind.SYNTHETIC:
         return verifies_synthetic(variant_constraint=variant_constraint)
 
     elif kind == st.ConstraintKind.MOCK:
@@ -29,64 +34,83 @@
             privacy_limit=privacy_limit,
         )
 
     else:  # kind == st.ConstraintKind.PEP:
         return verifies_pep(variant_constraint=variant_constraint)
 
 
-def verifies_public(variant_constraint: st.VariantConstraint) -> bool:
-    return variant_constraint.constraint_kind() == st.ConstraintKind.PUBLIC
+def verifies_public(
+    variant_constraint: st.VariantConstraint,
+) -> Optional[bool]:
+    kind = variant_constraint.constraint_kind()
+    if kind == st.ConstraintKind.PUBLIC:
+        return variant_constraint.properties()[IS_PUBLIC] == str(True)
+    else:
+        return None
 
 
-def verifies_synthetic(variant_constraint: st.VariantConstraint) -> bool:
+def verifies_synthetic(
+    variant_constraint: st.VariantConstraint,
+) -> Optional[bool]:
     kind = variant_constraint.constraint_kind()
     if kind == st.ConstraintKind.SYNTHETIC:
-        return True
+        return variant_constraint.properties()[IS_SYNTHETIC] == str(True)
     elif kind == st.ConstraintKind.PUBLIC:
-        return variant_constraint.properties()[IS_PUBLIC] == str(True)
+        if variant_constraint.properties()[IS_PUBLIC] == str(True):
+            return True
+        else:
+            return None
     else:
-        return False
+        return None
 
 
-def verifies_mock(variant_constraint: st.VariantConstraint) -> bool:
+def verifies_mock(variant_constraint: st.VariantConstraint) -> Optional[bool]:
     kind = variant_constraint.constraint_kind()
     if kind == st.ConstraintKind.MOCK:
         return True
     elif kind == st.ConstraintKind.PUBLIC:
-        return variant_constraint.properties()[IS_PUBLIC] == str(True)
+        if variant_constraint.properties()[IS_PUBLIC] == str(True):
+            return True
+        else:
+            return None
     else:
-        return False
+        return None
 
 
 def verifies_pep(
     variant_constraint: st.VariantConstraint,
-) -> bool:
+) -> Optional[bool]:
     """If we attached a PEP constraint to a dataspec then it is PEP.
 
     NB: for now we don't check the context nor the privacy limit
     """
-    return variant_constraint.constraint_kind() == st.ConstraintKind.PEP
+    kind = variant_constraint.constraint_kind()
+    if kind == st.ConstraintKind.PEP:
+        stored_token = variant_constraint.properties()[PEP_TOKEN]
+        return False if stored_token == NO_TOKEN else True
+    else:
+        return None
 
 
 def verifies_dp(
     variant_constraint: st.VariantConstraint,
     privacy_limit: Optional[st.PrivacyLimit],
-) -> bool:
+) -> Optional[bool]:
     """Check if a variant constraint satisfies a DP profile.
 
     For now, return True only for strict equality.
     """
     if privacy_limit is None:
         raise ValueError(
             "Input privacy limit required when checking against DP."
         )
 
     kind = variant_constraint.constraint_kind()
     if kind != st.ConstraintKind.DP:
-        return False
+        return None
 
     constraint_privacy_limit = variant_constraint.privacy_limit()
     if constraint_privacy_limit is None:
         raise ValueError(
             "Found a DP constraint without a privacy limit "
             "when checking against DP."
         )
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/dataspec_validator/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,28 @@
     PUBLIC = "Public"
 
 
 class PEPKind(Enum):
     NOT_PEP = 0
     PEP = 1
     TOKEN_PRESERVING = 2
+    ROW = 3
 
 
 class DataspecValidator(Protocol):
     def storage(self) -> Storage:
         ...
 
     def verifies(
         self,
         variant_constraint: st.VariantConstraint,
         kind: st.ConstraintKind,
         public_context: Collection[str],
         privacy_limit: Optional[st.PrivacyLimit],
-    ) -> bool:
+    ) -> Optional[bool]:
         """Check if the constraint attached to a Dataspec meets requirements.
 
         This function is useful because comparisons are not straightforwards.
         For instance, a Dataspec might have the variant constraint SYNTHETIC
         attached to it. This synthetic dataspec also verifies the DP constraint
         and the PUBLIC constraint.
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/async_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,31 +131,41 @@
             arrays=[el.combine_chunks() for el in table.flatten()],
             names=table.column_names,
         )
         for table_path, table in output.items()
     }
     batches = []
     names = list(struct_arrays.keys())
-    names.append('field_selected')
 
     for current_table, arr_array in struct_arrays.items():
         # iterate over tables
         arrays_list = [
             pa.array(
                 [None] * len(arr_array),
                 type=struct.type,
             )
             if current_table != table
             else arr_array
             for table, struct in struct_arrays.items()
         ]
+        fields = [
+            pa.field(name=name, type=arr.type)
+            for name, arr in zip(names, arrays_list)
+        ]
+        fields.append(
+            pa.field(name='field_selected', type=pa.string(), nullable=False)
+        )
         arrays_list.append(
             pa.array([current_table] * len(arr_array), type=pa.string())
         )
-        batches.append(pa.RecordBatch.from_arrays(arrays_list, names=names))
+        batches.append(
+            pa.RecordBatch.from_arrays(
+                arrays_list, schema=pa.schema(fields=fields)
+            )
+        )
     return async_iter(batches)
 
 
 def standardize_sql_query(
     parent_schema_name: str,
     query: t.Union[str, t.Mapping[t.Union[str, t.Tuple[str, ...]], str]],
 ) -> t.Mapping[str, str]:
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import hashlib
 import typing as t
 
+import pandas as pd
 import pyarrow as pa
 
 from sarus_data_spec.arrow.admin_utils import (
     compute_admin_data,
     create_admin_columns,
     merge_data_and_admin,
 )
@@ -121,15 +122,15 @@
             return None
 
         pep_kind = implementation.pep_kind(bound_signature)
         if pep_kind == PEPKind.NOT_PEP:
             return None
         elif pep_kind == PEPKind.TOKEN_PRESERVING:
             return input_token
-        else:
+        else:  # PEP or ROW
             h = hashlib.md5()
             h.update(input_token.encode("ascii"))
             h.update(transform.protobuf().SerializeToString())
             new_token = h.hexdigest()
             return new_token
 
     async def schema(self) -> st.Schema:
@@ -166,14 +167,21 @@
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
         bound_signature.static_validation()
 
         if self.dataset.is_pep():
             result = await implementation.compute(bound_signature)
+            if (
+                isinstance(result, pd.Series)
+                and implementation.pep_kind(bound_signature) == PEPKind.ROW
+            ):
+                # Reformat the series as a dataframe with a single row
+                result = result.to_frame().transpose()
+
             ds_result = t.cast(st.DatasetCastable, result)
             admin_data = await bound_signature.admin_data()
             output_admin_data = compute_admin_data(admin_data, ds_result)
             data_table = to_pyarrow_table(ds_result)
             table = merge_data_and_admin(data_table, output_admin_data)
 
         else:
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,31 +161,29 @@
     def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
         (this, key) = signature.collect_args()
         return this.loc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """Token preserving if the key is a tuple or a slice that
         selects all the rows (e.g. loc[:, "col"], loc[:]).
-        Not PEP if the key is a single int.
         PEP in the other cases.
         """
         key_arg = signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, tuple) and len(key_value) == 2:
                 row_key, _ = key_value
                 if row_key == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
             elif isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
-            elif isinstance(key_value, int):
-                # a int changes the index, we are not able to compute
-                # the output PE
-                return PEPKind.NOT_PEP
+            elif isinstance(key_value, (int, str)):
+                # a scalar selects a single row
+                return PEPKind.ROW
 
         return PEPKind.PEP
 
 
 class pd_set_loc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_LOC"
     _signature = SarusSignature(
@@ -229,27 +227,25 @@
     def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
         (this, key) = signature.collect_args()
         return this.iloc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
         """Token preserving the alignment if the key is a slice that
         selects all the rows (e.g. iloc[:]).
-        Not PEP if the key is a single int.
         PEP in the other cases.
         """
         key_arg = signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
-            elif isinstance(key_value, int):
-                # a int changes the index, we are not able to compute
-                # the output PE
-                return PEPKind.NOT_PEP
+            elif isinstance(key_value, (int, str)):
+                # a scalar selects a single row
+                return PEPKind.ROW
 
         return PEPKind.PEP
 
 
 class pd_set_iloc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_ILOC"
     _signature = SarusSignature(
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,25 @@
         SelectSQLStaticChecker,
     )
 
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: SelectSQL not available.")
 
+try:
+    from sarus_data_spec.manager.ops.processor.standard.dp_select_sql import (
+        DPSelectSQL,
+        DPSelectSQLStaticChecker,
+    )
+
+except ModuleNotFoundError:
+    logger = logging.getLogger(__name__)
+    logger.info("Transforms: SelectSQL not available.")
+
+
 from sarus_data_spec.manager.ops.processor.standard.shuffle import (
     Shuffle,
     ShuffleStaticChecker,
 )
 
 try:
     from sarus_data_spec.manager.ops.processor.standard.protection_utils.protected_paths import (  # noqa: E501
@@ -176,46 +187,46 @@
 
 
 def get_dataset_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[DatasetImplementation], t.Type[DatasetStaticChecker]]:
     if transform.is_external():
         return ExternalDatasetOp, ExternalDatasetStaticChecker
-    elif transform.protobuf().spec.HasField('sample'):
+    elif transform.spec() == 'sample':
         return Sample, SampleStaticChecker
-    elif transform.protobuf().spec.HasField('differentiated_sample'):
+    elif transform.spec() == 'differentiated_sample':
         return DifferentiatedSample, DifferentiatedSampleStaticChecker
-    elif transform.protobuf().spec.HasField('protect_dataset'):
+    elif transform.spec() == 'protect_dataset':
         return ProtectedDataset, ProtectedDatasetStaticChecker
-    elif transform.protobuf().spec.HasField('user_settings'):
+    elif transform.spec() == 'user_settings':
         return UserSettingsDataset, UserSettingsStaticChecker
-    elif transform.protobuf().spec.HasField('filter'):
+    elif transform.spec() == 'filter':
         return Filter, FilterStaticChecker
-    elif transform.protobuf().spec.HasField('project'):
+    elif transform.spec() == 'project':
         return Project, ProjectStaticChecker
-    elif transform.protobuf().spec.HasField('shuffle'):
+    elif transform.spec() == 'shuffle':
         return Shuffle, ShuffleStaticChecker
-    elif transform.protobuf().spec.HasField('synthetic'):
+    elif transform.spec() == 'synthetic':
         return Synthetic, SyntheticStaticChecker
-    elif transform.protobuf().spec.HasField('get_item'):
+    elif transform.spec() == 'get_item':
         return GetItem, GetItemStaticChecker
-    elif transform.protobuf().spec.HasField('assign_budget'):
+    elif transform.spec() == 'assign_budget':
         return AssignBudget, AssignBudgetStaticChecker
-    elif transform.protobuf().spec.HasField('group_by_pe'):
+    elif transform.spec() == 'group_by_pe':
         return GroupByPE, GroupByPEStaticChecker
     elif transform.name() == 'Transcode':
         return Transcode, TranscodeStaticChecker
-    elif transform.protobuf().spec.HasField('select_sql'):
+    elif transform.spec() == 'select_sql':
         return SelectSQL, SelectSQLStaticChecker
-    elif transform.protobuf().spec.HasField('extract'):
+    elif transform.spec() == 'dp_select_sql':
+        return DPSelectSQL, DPSelectSQLStaticChecker
+    elif transform.spec() == 'extract':
         return Extract, ExtractStaticChecker
     else:
-        raise NotImplementedError(
-            f"{transform.protobuf().spec.WhichOneof('spec')}"
-        )
+        raise NotImplementedError(transform.spec())
 
 
 def get_scalar_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[ScalarImplementation], t.Type[DataspecStaticChecker]]:
     if transform.is_external():
         return ExternalScalarOp, ExternalScalarStaticChecker
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,17 +75,26 @@
         def Union(
             self,
             fields: t.Mapping[str, st.Type],
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             names = list(fields.keys())
-            names.append("field_selected")
+            arrs = arrow_data.flatten()
+            schema = pa.schema(
+                [
+                    pa.field(name, type=arr.type)
+                    for arr, name in zip(arrs[:-1], names)
+                ]
+            )
+            schema = schema.append(
+                pa.field('field_selected', type=pa.string(), nullable=False)
+            )
             self.result = pa.Table.from_arrays(
-                arrays=arrow_data.flatten(), names=names
+                arrays=arrow_data.flatten(), schema=schema
             )
 
         def Null(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             raise NotImplementedError
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,24 +319,33 @@
             else:
                 index_nulls = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
                 self.filter_indices = pa.compute.and_(
                     final_filter, index_nulls
                 )
+
             fields_name = list(fields.keys())
-            fields_name.append('field_selected')
             # here we need to take arrays modified from low level
             selected_arrays = [
                 array_index[0] for array_index in arrays_indices
             ]
+            struct_fields = [
+                pa.field(name=field_name, type=arr.type)
+                for arr, field_name in zip(selected_arrays, fields_name)
+            ]
+            struct_fields.append(
+                pa.field(
+                    name='field_selected', type=pa.string(), nullable=False
+                )
+            )
             selected_arrays.append(self.batch_array.field('field_selected'))
             self.batch_array = pa.StructArray.from_arrays(
                 selected_arrays,
-                names=fields_name,
+                fields=struct_fields,
             )
 
         def Array(
             self,
             type: st.Type,
             shape: t.Tuple[int, ...],
             name: t.Optional[str] = None,
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/path.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     OBJECT_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
     """General attribute about an object"""
@@ -44,9 +44,9 @@
     def __init__(self,
         *,
         uuid : typing.Text = ...,
         object : typing.Text = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         name : typing.Text = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"object",b"object",u"properties",b"properties",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["name",b"name","object",b"object","properties",b"properties","uuid",b"uuid"]) -> None: ...
 global___Attribute = Attribute
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 import google.protobuf.message
 import sarus_data_spec.protobuf.statistics_pb2
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class Bounds(google.protobuf.message.Message):
+class Size(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     STATISTICS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -45,10 +45,10 @@
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         statistics : typing.Optional[sarus_data_spec.protobuf.statistics_pb2.Statistics] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"statistics",b"statistics",u"uuid",b"uuid"]) -> None: ...
-global___Bounds = Bounds
+    def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","statistics",b"statistics","uuid",b"uuid"]) -> None: ...
+global___Size = Size
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class ConstraintKind(_ConstraintKind, metaclass=_ConstraintKindEnumTypeWrapper):
-    pass
 class _ConstraintKind:
-    V = typing.NewType('V', builtins.int)
-class _ConstraintKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ConstraintKind.V], builtins.type):
+    ValueType = typing.NewType('ValueType', builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+class _ConstraintKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ConstraintKind.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-    SYNTHETIC = ConstraintKind.V(0)
-    DP = ConstraintKind.V(1)
-    PUBLIC = ConstraintKind.V(2)
-    PEP = ConstraintKind.V(3)
-    MOCK = ConstraintKind.V(4)
-
-SYNTHETIC = ConstraintKind.V(0)
-DP = ConstraintKind.V(1)
-PUBLIC = ConstraintKind.V(2)
-PEP = ConstraintKind.V(3)
-MOCK = ConstraintKind.V(4)
+    SYNTHETIC: ConstraintKind.ValueType = ...  # 0
+    DP: ConstraintKind.ValueType = ...  # 1
+    PUBLIC: ConstraintKind.ValueType = ...  # 2
+    PEP: ConstraintKind.ValueType = ...  # 3
+    MOCK: ConstraintKind.ValueType = ...  # 4
+class ConstraintKind(_ConstraintKind, metaclass=_ConstraintKindEnumTypeWrapper):
+    pass
+
+SYNTHETIC: ConstraintKind.ValueType = ...  # 0
+DP: ConstraintKind.ValueType = ...  # 1
+PUBLIC: ConstraintKind.ValueType = ...  # 2
+PEP: ConstraintKind.ValueType = ...  # 3
+MOCK: ConstraintKind.ValueType = ...  # 4
 global___ConstraintKind = ConstraintKind
 
 
 class VariantConstraint(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
@@ -41,31 +42,31 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASPEC_FIELD_NUMBER: builtins.int
     CONSTRAINT_KIND_FIELD_NUMBER: builtins.int
     REQUIRED_CONTEXT_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
     dataspec: typing.Text = ...
-    constraint_kind: global___ConstraintKind.V = ...
+    constraint_kind: global___ConstraintKind.ValueType = ...
     @property
     def required_context(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]: ...
     @property
     def properties(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
     def __init__(self,
         *,
         uuid : typing.Text = ...,
         dataspec : typing.Text = ...,
-        constraint_kind : global___ConstraintKind.V = ...,
+        constraint_kind : global___ConstraintKind.ValueType = ...,
         required_context : typing.Optional[typing.Iterable[typing.Text]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"constraint_kind",b"constraint_kind",u"dataspec",b"dataspec",u"properties",b"properties",u"required_context",b"required_context",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["constraint_kind",b"constraint_kind","dataspec",b"dataspec","properties",b"properties","required_context",b"required_context","uuid",b"uuid"]) -> None: ...
 global___VariantConstraint = VariantConstraint
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Spec(google.protobuf.message.Message):
         """Definitions
         How to obtain the dataset
         """
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         TRANSFORMED_FIELD_NUMBER: builtins.int
@@ -50,32 +50,32 @@
             *,
             transformed : typing.Optional[global___Dataset.Transformed] = ...,
             file : typing.Optional[global___Dataset.File] = ...,
             files : typing.Optional[global___Dataset.Files] = ...,
             archive : typing.Optional[global___Dataset.Archive] = ...,
             sql : typing.Optional[global___Dataset.Sql] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"archive",b"archive",u"file",b"file",u"files",b"files",u"spec",b"spec",u"sql",b"sql",u"transformed",b"transformed"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"archive",b"archive",u"file",b"file",u"files",b"files",u"spec",b"spec",u"sql",b"sql",u"transformed",b"transformed"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["transformed","file","files","archive","sql"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["archive",b"archive","file",b"file","files",b"files","spec",b"spec","sql",b"sql","transformed",b"transformed"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["archive",b"archive","file",b"file","files",b"files","spec",b"spec","sql",b"sql","transformed",b"transformed"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["transformed","file","files","archive","sql"]]: ...
 
     class Transformed(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class NamedArgumentsEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         TRANSFORM_FIELD_NUMBER: builtins.int
         ARGUMENTS_FIELD_NUMBER: builtins.int
         NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
         transform: typing.Text = ...
         """Transform id"""
 
@@ -87,45 +87,45 @@
         def named_arguments(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
         def __init__(self,
             *,
             transform : typing.Text = ...,
             arguments : typing.Optional[typing.Iterable[typing.Text]] = ...,
             named_arguments : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"named_arguments",b"named_arguments",u"transform",b"transform"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","named_arguments",b"named_arguments","transform",b"transform"]) -> None: ...
 
     class File(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         FORMAT_FIELD_NUMBER: builtins.int
         URI_FIELD_NUMBER: builtins.int
         format: typing.Text = ...
         uri: typing.Text = ...
         """File URI"""
 
         def __init__(self,
             *,
             format : typing.Text = ...,
             uri : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"format",b"format",u"uri",b"uri"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["format",b"format","uri",b"uri"]) -> None: ...
 
     class Files(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         FORMAT_FIELD_NUMBER: builtins.int
         URI_PATTERN_FIELD_NUMBER: builtins.int
         format: typing.Text = ...
         uri_pattern: typing.Text = ...
         """Pattern of files"""
 
         def __init__(self,
             *,
             format : typing.Text = ...,
             uri_pattern : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"format",b"format",u"uri_pattern",b"uri_pattern"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["format",b"format","uri_pattern",b"uri_pattern"]) -> None: ...
 
     class Archive(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         FORMAT_FIELD_NUMBER: builtins.int
         ARCHIVE_FORMAT_FIELD_NUMBER: builtins.int
         URI_FIELD_NUMBER: builtins.int
         format: typing.Text = ...
@@ -135,30 +135,30 @@
 
         def __init__(self,
             *,
             format : typing.Text = ...,
             archive_format : typing.Text = ...,
             uri : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"archive_format",b"archive_format",u"format",b"format",u"uri",b"uri"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["archive_format",b"archive_format","format",b"format","uri",b"uri"]) -> None: ...
 
     class Sql(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Table(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             SCHEMA_FIELD_NUMBER: builtins.int
             TABLE_FIELD_NUMBER: builtins.int
             schema: typing.Text = ...
             table: typing.Text = ...
             def __init__(self,
                 *,
                 schema : typing.Text = ...,
                 table : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"schema",b"schema",u"table",b"table"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["schema",b"schema","table",b"table"]) -> None: ...
 
         URI_FIELD_NUMBER: builtins.int
         TABLES_FIELD_NUMBER: builtins.int
         uri: typing.Text = ...
         """As in https://docs.sqlalchemy.org/en/14/core/engines.html"""
 
         @property
@@ -166,15 +166,15 @@
             """the sql schemas from which the data can be downloaded"""
             pass
         def __init__(self,
             *,
             uri : typing.Text = ...,
             tables : typing.Optional[typing.Iterable[global___Dataset.Sql.Table]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"tables",b"tables",u"uri",b"uri"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["tables",b"tables","uri",b"uri"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DOC_FIELD_NUMBER: builtins.int
     SPEC_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -194,10 +194,10 @@
         *,
         uuid : typing.Text = ...,
         name : typing.Text = ...,
         doc : typing.Text = ...,
         spec : typing.Optional[global___Dataset.Spec] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"spec",b"spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"doc",b"doc",u"name",b"name",u"properties",b"properties",u"spec",b"spec",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["spec",b"spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["doc",b"doc","name",b"name","properties",b"properties","spec",b"spec","uuid",b"uuid"]) -> None: ...
 global___Dataset = Dataset
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class LinkStat(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class PropertiesEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         POINTING_FIELD_NUMBER: builtins.int
         POINTED_FIELD_NUMBER: builtins.int
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         PROPERTIES_FIELD_NUMBER: builtins.int
         @property
         def pointing(self) -> sarus_data_spec.protobuf.path_pb2.Path: ...
@@ -60,16 +60,16 @@
         def __init__(self,
             *,
             pointing : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
             pointed : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
             distribution : typing.Optional[sarus_data_spec.protobuf.statistics_pb2.Distribution] = ...,
             properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"pointed",b"pointed",u"pointing",b"pointing"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"pointed",b"pointed",u"pointing",b"pointing",u"properties",b"properties"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution","pointed",b"pointed","pointing",b"pointing"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","pointed",b"pointed","pointing",b"pointing","properties",b"properties"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     LINKS_STATISTICS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
     dataset: typing.Text = ...
@@ -82,9 +82,9 @@
     def __init__(self,
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         links_statistics : typing.Optional[typing.Iterable[global___Links.LinkStat]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"links_statistics",b"links_statistics",u"properties",b"properties",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","links_statistics",b"links_statistics","properties",b"properties","uuid",b"uuid"]) -> None: ...
 global___Links = Links
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
     """A mnager must register itself
     e.g. RFC 4122 id used to refer to the dataset (content linked?)
     """
@@ -38,9 +38,9 @@
         """Other properties"""
         pass
     def __init__(self,
         *,
         uuid : typing.Text = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"properties",b"properties",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["properties",b"properties","uuid",b"uuid"]) -> None: ...
 global___Manager = Manager
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     STATISTICS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -45,10 +45,10 @@
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         statistics : typing.Optional[sarus_data_spec.protobuf.statistics_pb2.Statistics] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"statistics",b"statistics",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","statistics",b"statistics","uuid",b"uuid"]) -> None: ...
 global___Marginals = Marginals
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     STATISTICS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -45,10 +45,10 @@
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         statistics : typing.Optional[sarus_data_spec.protobuf.statistics_pb2.Statistics] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"statistics",b"statistics",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","statistics",b"statistics","uuid",b"uuid"]) -> None: ...
 global___Multiplicity = Multiplicity
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     LABEL_FIELD_NUMBER: builtins.int
     PATHS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     label: typing.Text = ...
     @property
     def paths(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Path]: ...
@@ -36,9 +36,9 @@
     def properties(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
     def __init__(self,
         *,
         label : typing.Text = ...,
         paths : typing.Optional[typing.Iterable[global___Path]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"label",b"label",u"paths",b"paths",u"properties",b"properties"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["label",b"label","paths",b"paths","properties",b"properties"]) -> None: ...
 global___Path = Path
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -20,64 +20,64 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Simple(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         OPERATOR_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         operator: typing.Text = ...
         """==, <, <=, in, etc."""
 
         value: typing.Text = ...
         def __init__(self,
             *,
             operator : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"operator",b"operator",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["operator",b"operator","value",b"value"]) -> None: ...
 
     class Inter(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         PREDICATES_FIELD_NUMBER: builtins.int
         @property
         def predicates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Predicate]: ...
         def __init__(self,
             *,
             predicates : typing.Optional[typing.Iterable[global___Predicate]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"predicates",b"predicates"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["predicates",b"predicates"]) -> None: ...
 
     class Union(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         PREDICATES_FIELD_NUMBER: builtins.int
         @property
         def predicates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Predicate]: ...
         def __init__(self,
             *,
             predicates : typing.Optional[typing.Iterable[global___Predicate]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"predicates",b"predicates"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["predicates",b"predicates"]) -> None: ...
 
     class Comp(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         PREDICATE_FIELD_NUMBER: builtins.int
         @property
         def predicate(self) -> global___Predicate: ...
         def __init__(self,
             *,
             predicate : typing.Optional[global___Predicate] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"predicate",b"predicate"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"predicate",b"predicate"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["predicate",b"predicate"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["predicate",b"predicate"]) -> None: ...
 
     SIMPLE_FIELD_NUMBER: builtins.int
     INTER_FIELD_NUMBER: builtins.int
     UNION_FIELD_NUMBER: builtins.int
     COMP_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     @property
@@ -96,11 +96,11 @@
         *,
         simple : typing.Optional[global___Predicate.Simple] = ...,
         inter : typing.Optional[global___Predicate.Inter] = ...,
         union : typing.Optional[global___Predicate.Union] = ...,
         comp : typing.Optional[global___Predicate.Comp] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"comp",b"comp",u"inter",b"inter",u"predicate",b"predicate",u"simple",b"simple",u"union",b"union"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"comp",b"comp",u"inter",b"inter",u"predicate",b"predicate",u"properties",b"properties",u"simple",b"simple",u"union",b"union"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"predicate",b"predicate"]) -> typing.Optional[typing_extensions.Literal["simple","inter","union","comp"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["comp",b"comp","inter",b"inter","predicate",b"predicate","simple",b"simple","union",b"union"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["comp",b"comp","inter",b"inter","predicate",b"predicate","properties",b"properties","simple",b"simple","union",b"union"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["predicate",b"predicate"]) -> typing.Optional[typing_extensions.Literal["simple","inter","union","comp"]]: ...
 global___Predicate = Predicate
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     PROTOS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     @property
     def protos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]:
         """General container to store list of protos
 
@@ -40,9 +40,9 @@
         """Other properties"""
         pass
     def __init__(self,
         *,
         protos : typing.Optional[typing.Iterable[google.protobuf.any_pb2.Any]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"properties",b"properties",u"protos",b"protos"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["properties",b"properties","protos",b"protos"]) -> None: ...
 global___ProtoContainer = ProtoContainer
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     ARGUMENTS_FIELD_NUMBER: builtins.int
     NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -54,9 +54,9 @@
         *,
         uuid : typing.Text = ...,
         name : typing.Text = ...,
         arguments : typing.Optional[typing.Iterable[typing.Text]] = ...,
         named_arguments : typing.Optional[typing.Iterable[typing.Text]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"name",b"name",u"named_arguments",b"named_arguments",u"properties",b"properties",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","name",b"name","named_arguments",b"named_arguments","properties",b"properties","uuid",b"uuid"]) -> None: ...
 global___Relation = Relation
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Spec(google.protobuf.message.Message):
         """Definitions
         How to obtain the dataset
         """
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         TRANSFORMED_FIELD_NUMBER: builtins.int
@@ -55,32 +55,32 @@
             *,
             transformed : typing.Optional[global___Scalar.Transformed] = ...,
             model : typing.Optional[global___Scalar.Model] = ...,
             privacy_params : typing.Optional[global___Scalar.PrivacyParameters] = ...,
             random_seed : typing.Optional[global___Scalar.RandomSeed] = ...,
             synthetic_model : typing.Optional[global___Scalar.SyntheticModel] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"model",b"model",u"privacy_params",b"privacy_params",u"random_seed",b"random_seed",u"spec",b"spec",u"synthetic_model",b"synthetic_model",u"transformed",b"transformed"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"model",b"model",u"privacy_params",b"privacy_params",u"random_seed",b"random_seed",u"spec",b"spec",u"synthetic_model",b"synthetic_model",u"transformed",b"transformed"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["transformed","model","privacy_params","random_seed","synthetic_model"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["model",b"model","privacy_params",b"privacy_params","random_seed",b"random_seed","spec",b"spec","synthetic_model",b"synthetic_model","transformed",b"transformed"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["model",b"model","privacy_params",b"privacy_params","random_seed",b"random_seed","spec",b"spec","synthetic_model",b"synthetic_model","transformed",b"transformed"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["transformed","model","privacy_params","random_seed","synthetic_model"]]: ...
 
     class Transformed(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class NamedArgumentsEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         TRANSFORM_FIELD_NUMBER: builtins.int
         ARGUMENTS_FIELD_NUMBER: builtins.int
         NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
         transform: typing.Text = ...
         """Transform id"""
 
@@ -92,165 +92,166 @@
         def named_arguments(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
         def __init__(self,
             *,
             transform : typing.Text = ...,
             arguments : typing.Optional[typing.Iterable[typing.Text]] = ...,
             named_arguments : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"named_arguments",b"named_arguments",u"transform",b"transform"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","named_arguments",b"named_arguments","transform",b"transform"]) -> None: ...
 
     class Model(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        class ModelClass(_ModelClass, metaclass=_ModelClassEnumTypeWrapper):
-            pass
         class _ModelClass:
-            V = typing.NewType('V', builtins.int)
-        class _ModelClassEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ModelClass.V], builtins.type):
+            ValueType = typing.NewType('ValueType', builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+        class _ModelClassEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ModelClass.ValueType], builtins.type):
             DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-            TF_KERAS = Scalar.Model.ModelClass.V(0)
-            SK_SVC = Scalar.Model.ModelClass.V(1)
-            SK_ONEHOT = Scalar.Model.ModelClass.V(2)
-            SK_PCA = Scalar.Model.ModelClass.V(3)
-            SK_AFFINITY_PROPAGATION = Scalar.Model.ModelClass.V(4)
+            TF_KERAS: Scalar.Model.ModelClass.ValueType = ...  # 0
+            SK_SVC: Scalar.Model.ModelClass.ValueType = ...  # 1
+            SK_ONEHOT: Scalar.Model.ModelClass.ValueType = ...  # 2
+            SK_PCA: Scalar.Model.ModelClass.ValueType = ...  # 3
+            SK_AFFINITY_PROPAGATION: Scalar.Model.ModelClass.ValueType = ...  # 4
             """Cluster"""
 
-            SK_AGGLOMERATIVE_CLUSTERING = Scalar.Model.ModelClass.V(5)
-            SK_BIRCH = Scalar.Model.ModelClass.V(6)
-            SK_DBSCAN = Scalar.Model.ModelClass.V(7)
-            SK_FEATURE_AGGLOMERATION = Scalar.Model.ModelClass.V(8)
-            SK_KMEANS = Scalar.Model.ModelClass.V(9)
-            SK_MINIBATCH_KMEANS = Scalar.Model.ModelClass.V(10)
-            SK_MEAN_SHIFT = Scalar.Model.ModelClass.V(11)
-            SK_OPTICS = Scalar.Model.ModelClass.V(12)
-            SK_SPECTRAL_CLUSTERING = Scalar.Model.ModelClass.V(13)
-            SK_SPECTRAL_BICLUSTERING = Scalar.Model.ModelClass.V(14)
-            SK_SPECTRAL_COCLUSTERING = Scalar.Model.ModelClass.V(15)
-            SK_ADABOOST_CLASSIFIER = Scalar.Model.ModelClass.V(60)
+            SK_AGGLOMERATIVE_CLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 5
+            SK_BIRCH: Scalar.Model.ModelClass.ValueType = ...  # 6
+            SK_DBSCAN: Scalar.Model.ModelClass.ValueType = ...  # 7
+            SK_FEATURE_AGGLOMERATION: Scalar.Model.ModelClass.ValueType = ...  # 8
+            SK_KMEANS: Scalar.Model.ModelClass.ValueType = ...  # 9
+            SK_MINIBATCH_KMEANS: Scalar.Model.ModelClass.ValueType = ...  # 10
+            SK_MEAN_SHIFT: Scalar.Model.ModelClass.ValueType = ...  # 11
+            SK_OPTICS: Scalar.Model.ModelClass.ValueType = ...  # 12
+            SK_SPECTRAL_CLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 13
+            SK_SPECTRAL_BICLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 14
+            SK_SPECTRAL_COCLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 15
+            SK_ADABOOST_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 60
             """ensemble"""
 
-            SK_ADABOOST_REGRESSOR = Scalar.Model.ModelClass.V(61)
-            SK_BAGGING_CLASSIFIER = Scalar.Model.ModelClass.V(62)
-            SK_BAGGING_REGRESSOR = Scalar.Model.ModelClass.V(63)
-            SK_EXTRA_TREES_REGRESSOR = Scalar.Model.ModelClass.V(64)
-            SK_EXTRA_TREES_CLASSIFIER = Scalar.Model.ModelClass.V(65)
-            SK_GRADIENT_BOOSTING_CLASSIFIER = Scalar.Model.ModelClass.V(66)
-            SK_GRADIENT_BOOSTING_REGRESSOR = Scalar.Model.ModelClass.V(67)
-            SK_ISOLATION_FOREST = Scalar.Model.ModelClass.V(68)
-            SK_RANDOM_FOREST_CLASSIFIER = Scalar.Model.ModelClass.V(69)
-            SK_RANDOM_FOREST_REGRESSOR = Scalar.Model.ModelClass.V(70)
-            SK_RANDOM_TREES_EMBEDDING = Scalar.Model.ModelClass.V(71)
-            SK_STACKING_CLASSIFIER = Scalar.Model.ModelClass.V(72)
-            SK_STACKING_REGRESSOR = Scalar.Model.ModelClass.V(73)
-            SK_VOTING_CLASSIFIER = Scalar.Model.ModelClass.V(74)
-            SK_VOTING_REGRESSOR = Scalar.Model.ModelClass.V(75)
-            SK_HIST_GRADIENT_BOOSTING_REGRESSOR = Scalar.Model.ModelClass.V(76)
-            SK_HIST_GRADIENT_BOOSTING_CLASSIFIER = Scalar.Model.ModelClass.V(77)
-            SK_REPEATED_STRATIFIED_KFOLD = Scalar.Model.ModelClass.V(80)
+            SK_ADABOOST_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 61
+            SK_BAGGING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 62
+            SK_BAGGING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 63
+            SK_EXTRA_TREES_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 64
+            SK_EXTRA_TREES_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 65
+            SK_GRADIENT_BOOSTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 66
+            SK_GRADIENT_BOOSTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 67
+            SK_ISOLATION_FOREST: Scalar.Model.ModelClass.ValueType = ...  # 68
+            SK_RANDOM_FOREST_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 69
+            SK_RANDOM_FOREST_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 70
+            SK_RANDOM_TREES_EMBEDDING: Scalar.Model.ModelClass.ValueType = ...  # 71
+            SK_STACKING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 72
+            SK_STACKING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 73
+            SK_VOTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 74
+            SK_VOTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 75
+            SK_HIST_GRADIENT_BOOSTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 76
+            SK_HIST_GRADIENT_BOOSTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 77
+            SK_REPEATED_STRATIFIED_KFOLD: Scalar.Model.ModelClass.ValueType = ...  # 80
             """Model selection"""
 
-            XGB_CLASSIFIER = Scalar.Model.ModelClass.V(92)
+            XGB_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 92
             """XGB"""
 
-            SK_LABEL_ENCODER = Scalar.Model.ModelClass.V(98)
-            SK_KFOLD = Scalar.Model.ModelClass.V(99)
+            SK_LABEL_ENCODER: Scalar.Model.ModelClass.ValueType = ...  # 98
+            SK_KFOLD: Scalar.Model.ModelClass.ValueType = ...  # 99
+        class ModelClass(_ModelClass, metaclass=_ModelClassEnumTypeWrapper):
+            pass
 
-        TF_KERAS = Scalar.Model.ModelClass.V(0)
-        SK_SVC = Scalar.Model.ModelClass.V(1)
-        SK_ONEHOT = Scalar.Model.ModelClass.V(2)
-        SK_PCA = Scalar.Model.ModelClass.V(3)
-        SK_AFFINITY_PROPAGATION = Scalar.Model.ModelClass.V(4)
+        TF_KERAS: Scalar.Model.ModelClass.ValueType = ...  # 0
+        SK_SVC: Scalar.Model.ModelClass.ValueType = ...  # 1
+        SK_ONEHOT: Scalar.Model.ModelClass.ValueType = ...  # 2
+        SK_PCA: Scalar.Model.ModelClass.ValueType = ...  # 3
+        SK_AFFINITY_PROPAGATION: Scalar.Model.ModelClass.ValueType = ...  # 4
         """Cluster"""
 
-        SK_AGGLOMERATIVE_CLUSTERING = Scalar.Model.ModelClass.V(5)
-        SK_BIRCH = Scalar.Model.ModelClass.V(6)
-        SK_DBSCAN = Scalar.Model.ModelClass.V(7)
-        SK_FEATURE_AGGLOMERATION = Scalar.Model.ModelClass.V(8)
-        SK_KMEANS = Scalar.Model.ModelClass.V(9)
-        SK_MINIBATCH_KMEANS = Scalar.Model.ModelClass.V(10)
-        SK_MEAN_SHIFT = Scalar.Model.ModelClass.V(11)
-        SK_OPTICS = Scalar.Model.ModelClass.V(12)
-        SK_SPECTRAL_CLUSTERING = Scalar.Model.ModelClass.V(13)
-        SK_SPECTRAL_BICLUSTERING = Scalar.Model.ModelClass.V(14)
-        SK_SPECTRAL_COCLUSTERING = Scalar.Model.ModelClass.V(15)
-        SK_ADABOOST_CLASSIFIER = Scalar.Model.ModelClass.V(60)
+        SK_AGGLOMERATIVE_CLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 5
+        SK_BIRCH: Scalar.Model.ModelClass.ValueType = ...  # 6
+        SK_DBSCAN: Scalar.Model.ModelClass.ValueType = ...  # 7
+        SK_FEATURE_AGGLOMERATION: Scalar.Model.ModelClass.ValueType = ...  # 8
+        SK_KMEANS: Scalar.Model.ModelClass.ValueType = ...  # 9
+        SK_MINIBATCH_KMEANS: Scalar.Model.ModelClass.ValueType = ...  # 10
+        SK_MEAN_SHIFT: Scalar.Model.ModelClass.ValueType = ...  # 11
+        SK_OPTICS: Scalar.Model.ModelClass.ValueType = ...  # 12
+        SK_SPECTRAL_CLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 13
+        SK_SPECTRAL_BICLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 14
+        SK_SPECTRAL_COCLUSTERING: Scalar.Model.ModelClass.ValueType = ...  # 15
+        SK_ADABOOST_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 60
         """ensemble"""
 
-        SK_ADABOOST_REGRESSOR = Scalar.Model.ModelClass.V(61)
-        SK_BAGGING_CLASSIFIER = Scalar.Model.ModelClass.V(62)
-        SK_BAGGING_REGRESSOR = Scalar.Model.ModelClass.V(63)
-        SK_EXTRA_TREES_REGRESSOR = Scalar.Model.ModelClass.V(64)
-        SK_EXTRA_TREES_CLASSIFIER = Scalar.Model.ModelClass.V(65)
-        SK_GRADIENT_BOOSTING_CLASSIFIER = Scalar.Model.ModelClass.V(66)
-        SK_GRADIENT_BOOSTING_REGRESSOR = Scalar.Model.ModelClass.V(67)
-        SK_ISOLATION_FOREST = Scalar.Model.ModelClass.V(68)
-        SK_RANDOM_FOREST_CLASSIFIER = Scalar.Model.ModelClass.V(69)
-        SK_RANDOM_FOREST_REGRESSOR = Scalar.Model.ModelClass.V(70)
-        SK_RANDOM_TREES_EMBEDDING = Scalar.Model.ModelClass.V(71)
-        SK_STACKING_CLASSIFIER = Scalar.Model.ModelClass.V(72)
-        SK_STACKING_REGRESSOR = Scalar.Model.ModelClass.V(73)
-        SK_VOTING_CLASSIFIER = Scalar.Model.ModelClass.V(74)
-        SK_VOTING_REGRESSOR = Scalar.Model.ModelClass.V(75)
-        SK_HIST_GRADIENT_BOOSTING_REGRESSOR = Scalar.Model.ModelClass.V(76)
-        SK_HIST_GRADIENT_BOOSTING_CLASSIFIER = Scalar.Model.ModelClass.V(77)
-        SK_REPEATED_STRATIFIED_KFOLD = Scalar.Model.ModelClass.V(80)
+        SK_ADABOOST_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 61
+        SK_BAGGING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 62
+        SK_BAGGING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 63
+        SK_EXTRA_TREES_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 64
+        SK_EXTRA_TREES_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 65
+        SK_GRADIENT_BOOSTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 66
+        SK_GRADIENT_BOOSTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 67
+        SK_ISOLATION_FOREST: Scalar.Model.ModelClass.ValueType = ...  # 68
+        SK_RANDOM_FOREST_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 69
+        SK_RANDOM_FOREST_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 70
+        SK_RANDOM_TREES_EMBEDDING: Scalar.Model.ModelClass.ValueType = ...  # 71
+        SK_STACKING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 72
+        SK_STACKING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 73
+        SK_VOTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 74
+        SK_VOTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 75
+        SK_HIST_GRADIENT_BOOSTING_REGRESSOR: Scalar.Model.ModelClass.ValueType = ...  # 76
+        SK_HIST_GRADIENT_BOOSTING_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 77
+        SK_REPEATED_STRATIFIED_KFOLD: Scalar.Model.ModelClass.ValueType = ...  # 80
         """Model selection"""
 
-        XGB_CLASSIFIER = Scalar.Model.ModelClass.V(92)
+        XGB_CLASSIFIER: Scalar.Model.ModelClass.ValueType = ...  # 92
         """XGB"""
 
-        SK_LABEL_ENCODER = Scalar.Model.ModelClass.V(98)
-        SK_KFOLD = Scalar.Model.ModelClass.V(99)
+        SK_LABEL_ENCODER: Scalar.Model.ModelClass.ValueType = ...  # 98
+        SK_KFOLD: Scalar.Model.ModelClass.ValueType = ...  # 99
 
         ARGUMENTS_FIELD_NUMBER: builtins.int
         NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
         MODEL_CLASS_FIELD_NUMBER: builtins.int
         arguments: builtins.bytes = ...
         named_arguments: builtins.bytes = ...
-        model_class: global___Scalar.Model.ModelClass.V = ...
+        model_class: global___Scalar.Model.ModelClass.ValueType = ...
         def __init__(self,
             *,
             arguments : builtins.bytes = ...,
             named_arguments : builtins.bytes = ...,
-            model_class : global___Scalar.Model.ModelClass.V = ...,
+            model_class : global___Scalar.Model.ModelClass.ValueType = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"model_class",b"model_class",u"named_arguments",b"named_arguments"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","model_class",b"model_class","named_arguments",b"named_arguments"]) -> None: ...
 
     class PrivacyParameters(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Point(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             EPSILON_FIELD_NUMBER: builtins.int
             DELTA_FIELD_NUMBER: builtins.int
             epsilon: builtins.float = ...
             delta: builtins.float = ...
             def __init__(self,
                 *,
                 epsilon : builtins.float = ...,
                 delta : builtins.float = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"delta",b"delta",u"epsilon",b"epsilon"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["delta",b"delta","epsilon",b"epsilon"]) -> None: ...
 
         POINTS_FIELD_NUMBER: builtins.int
         @property
         def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Scalar.PrivacyParameters.Point]: ...
         def __init__(self,
             *,
             points : typing.Optional[typing.Iterable[global___Scalar.PrivacyParameters.Point]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"points",b"points"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["points",b"points"]) -> None: ...
 
     class RandomSeed(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         VALUE_FIELD_NUMBER: builtins.int
         value: builtins.int = ...
         def __init__(self,
             *,
             value : builtins.int = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["value",b"value"]) -> None: ...
 
     class SyntheticModel(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
@@ -283,10 +284,10 @@
         *,
         uuid : typing.Text = ...,
         name : typing.Text = ...,
         doc : typing.Text = ...,
         spec : typing.Optional[global___Scalar.Spec] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"spec",b"spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"doc",b"doc",u"name",b"name",u"properties",b"properties",u"spec",b"spec",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["spec",b"spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["doc",b"doc","name",b"name","properties",b"properties","spec",b"spec","uuid",b"uuid"]) -> None: ...
 global___Scalar = Scalar
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Hypothesis(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class PropertiesEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         UUID_FIELD_NUMBER: builtins.int
         DATASET_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         TYPE_FIELD_NUMBER: builtins.int
         PROPERTIES_FIELD_NUMBER: builtins.int
         uuid: typing.Text = ...
@@ -65,16 +65,16 @@
             *,
             uuid : typing.Text = ...,
             dataset : typing.Text = ...,
             name : typing.Text = ...,
             type : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
             properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"type",b"type"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"type",b"type",u"uuid",b"uuid"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["type",b"type"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","type",b"type","uuid",b"uuid"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     PROTECTED_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
@@ -100,10 +100,10 @@
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         type : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
         protected : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"protected",b"protected",u"type",b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"protected",b"protected",u"type",b"type",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["protected",b"protected","type",b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","protected",b"protected","type",b"type","uuid",b"uuid"]) -> None: ...
 global___Schema = Schema
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 import google.protobuf.message
 import sarus_data_spec.protobuf.statistics_pb2
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class Size(google.protobuf.message.Message):
+class Bounds(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     STATISTICS_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
@@ -45,10 +45,10 @@
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         statistics : typing.Optional[sarus_data_spec.protobuf.statistics_pb2.Statistics] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataset",b"dataset",u"name",b"name",u"properties",b"properties",u"statistics",b"statistics",u"uuid",b"uuid"]) -> None: ...
-global___Size = Size
+    def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","statistics",b"statistics","uuid",b"uuid"]) -> None: ...
+global___Bounds = Bounds
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -20,41 +20,41 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Null(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         size: builtins.int = ...
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Unit(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         size: builtins.int = ...
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Boolean(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -63,29 +63,29 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Id(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         size: builtins.int = ...
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Integer(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -94,16 +94,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Enum(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -112,16 +112,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Float(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -130,16 +130,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Text(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         EXAMPLE_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
@@ -151,29 +151,29 @@
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             example : typing.Text = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"example",b"example",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","example",b"example","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Bytes(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         size: builtins.int = ...
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Struct(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Field(google.protobuf.message.Message):
             """A single field"""
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
@@ -182,16 +182,16 @@
             @property
             def statistics(self) -> global___Statistics: ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 statistics : typing.Optional[global___Statistics] = ...,
                 ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"statistics",b"statistics"]) -> None: ...
+            def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name","statistics",b"statistics"]) -> None: ...
 
         FIELDS_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
         def fields(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Statistics.Struct.Field]:
@@ -203,15 +203,15 @@
         def __init__(self,
             *,
             fields : typing.Optional[typing.Iterable[global___Statistics.Struct.Field]] = ...,
             size : builtins.int = ...,
             name : typing.Text = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"fields",b"fields",u"multiplicity",b"multiplicity",u"name",b"name",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fields",b"fields","multiplicity",b"multiplicity","name",b"name","size",b"size"]) -> None: ...
 
     class Union(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Field(google.protobuf.message.Message):
             """A single field"""
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
@@ -220,16 +220,16 @@
             @property
             def statistics(self) -> global___Statistics: ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 statistics : typing.Optional[global___Statistics] = ...,
                 ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"statistics",b"statistics"]) -> None: ...
+            def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name","statistics",b"statistics"]) -> None: ...
 
         FIELDS_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
         def fields(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Statistics.Union.Field]: ...
@@ -239,15 +239,15 @@
         def __init__(self,
             *,
             fields : typing.Optional[typing.Iterable[global___Statistics.Union.Field]] = ...,
             size : builtins.int = ...,
             name : typing.Text = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"fields",b"fields",u"multiplicity",b"multiplicity",u"name",b"name",u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fields",b"fields","multiplicity",b"multiplicity","name",b"name","size",b"size"]) -> None: ...
 
     class Optional(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         STATISTICS_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
@@ -259,16 +259,16 @@
         def __init__(self,
             *,
             statistics : typing.Optional[global___Statistics] = ...,
             size : builtins.int = ...,
             name : typing.Text = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"name",b"name",u"size",b"size",u"statistics",b"statistics"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","name",b"name","size",b"size","statistics",b"statistics"]) -> None: ...
 
     class List(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         STATISTICS_FIELD_NUMBER: builtins.int
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
@@ -281,16 +281,16 @@
         def __init__(self,
             *,
             statistics : typing.Optional[global___Statistics] = ...,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"statistics",b"statistics"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size",u"statistics",b"statistics"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution","statistics",b"statistics"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size","statistics",b"statistics"]) -> None: ...
 
     class Array(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         STATISTICS_FIELD_NUMBER: builtins.int
         DISTRIBUTIONS_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
@@ -305,16 +305,16 @@
         def __init__(self,
             *,
             statistics : typing.Optional[global___Statistics] = ...,
             distributions : typing.Optional[typing.Iterable[global___Distribution]] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distributions",b"distributions",u"multiplicity",b"multiplicity",u"size",b"size",u"statistics",b"statistics"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distributions",b"distributions","multiplicity",b"multiplicity","size",b"size","statistics",b"statistics"]) -> None: ...
 
     class Datetime(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -325,16 +325,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Date(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -345,16 +345,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Time(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -365,16 +365,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Duration(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         DISTRIBUTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -385,16 +385,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             distribution : typing.Optional[global___Distribution] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"distribution",b"distribution",u"multiplicity",b"multiplicity",u"size",b"size"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["distribution",b"distribution"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["distribution",b"distribution","multiplicity",b"multiplicity","size",b"size"]) -> None: ...
 
     class Constrained(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         STATISTICS_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         MULTIPLICITY_FIELD_NUMBER: builtins.int
         @property
@@ -403,16 +403,16 @@
         multiplicity: builtins.float = ...
         def __init__(self,
             *,
             statistics : typing.Optional[global___Statistics] = ...,
             size : builtins.int = ...,
             multiplicity : builtins.float = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"statistics",b"statistics"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"multiplicity",b"multiplicity",u"size",b"size",u"statistics",b"statistics"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["statistics",b"statistics"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["multiplicity",b"multiplicity","size",b"size","statistics",b"statistics"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     NULL_FIELD_NUMBER: builtins.int
     UNIT_FIELD_NUMBER: builtins.int
     BOOLEAN_FIELD_NUMBER: builtins.int
     INTEGER_FIELD_NUMBER: builtins.int
     ENUM_FIELD_NUMBER: builtins.int
@@ -494,17 +494,17 @@
         id : typing.Optional[global___Statistics.Id] = ...,
         constrained : typing.Optional[global___Statistics.Constrained] = ...,
         date : typing.Optional[global___Statistics.Date] = ...,
         time : typing.Optional[global___Statistics.Time] = ...,
         duration : typing.Optional[global___Statistics.Duration] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"array",b"array",u"boolean",b"boolean",u"bytes",b"bytes",u"constrained",b"constrained",u"date",b"date",u"datetime",b"datetime",u"duration",b"duration",u"enum",b"enum",u"float",b"float",u"id",b"id",u"integer",b"integer",u"list",b"list",u"null",b"null",u"optional",b"optional",u"statistics",b"statistics",u"struct",b"struct",u"text",b"text",u"time",b"time",u"union",b"union",u"unit",b"unit"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"array",b"array",u"boolean",b"boolean",u"bytes",b"bytes",u"constrained",b"constrained",u"date",b"date",u"datetime",b"datetime",u"duration",b"duration",u"enum",b"enum",u"float",b"float",u"id",b"id",u"integer",b"integer",u"list",b"list",u"name",b"name",u"null",b"null",u"optional",b"optional",u"properties",b"properties",u"statistics",b"statistics",u"struct",b"struct",u"text",b"text",u"time",b"time",u"union",b"union",u"unit",b"unit"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"statistics",b"statistics"]) -> typing.Optional[typing_extensions.Literal["null","unit","boolean","integer","enum","float","text","bytes","struct","union","optional","list","array","datetime","id","constrained","date","time","duration"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["array",b"array","boolean",b"boolean","bytes",b"bytes","constrained",b"constrained","date",b"date","datetime",b"datetime","duration",b"duration","enum",b"enum","float",b"float","id",b"id","integer",b"integer","list",b"list","null",b"null","optional",b"optional","statistics",b"statistics","struct",b"struct","text",b"text","time",b"time","union",b"union","unit",b"unit"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["array",b"array","boolean",b"boolean","bytes",b"bytes","constrained",b"constrained","date",b"date","datetime",b"datetime","duration",b"duration","enum",b"enum","float",b"float","id",b"id","integer",b"integer","list",b"list","name",b"name","null",b"null","optional",b"optional","properties",b"properties","statistics",b"statistics","struct",b"struct","text",b"text","time",b"time","union",b"union","unit",b"unit"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["statistics",b"statistics"]) -> typing.Optional[typing_extensions.Literal["null","unit","boolean","integer","enum","float","text","bytes","struct","union","optional","list","array","datetime","id","constrained","date","time","duration"]]: ...
 global___Statistics = Statistics
 
 class Distribution(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
@@ -512,75 +512,75 @@
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Double(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Point(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             VALUE_FIELD_NUMBER: builtins.int
             PROBABILITY_FIELD_NUMBER: builtins.int
             value: builtins.float = ...
             probability: builtins.float = ...
             def __init__(self,
                 *,
                 value : builtins.float = ...,
                 probability : builtins.float = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"probability",b"probability",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["probability",b"probability","value",b"value"]) -> None: ...
 
         POINTS_FIELD_NUMBER: builtins.int
         MIN_FIELD_NUMBER: builtins.int
         MAX_FIELD_NUMBER: builtins.int
         @property
         def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Distribution.Double.Point]: ...
         min: builtins.float = ...
         max: builtins.float = ...
         def __init__(self,
             *,
             points : typing.Optional[typing.Iterable[global___Distribution.Double.Point]] = ...,
             min : builtins.float = ...,
             max : builtins.float = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"max",b"max",u"min",b"min",u"points",b"points"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["max",b"max","min",b"min","points",b"points"]) -> None: ...
 
     class Integer(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Point(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             VALUE_FIELD_NUMBER: builtins.int
             PROBABILITY_FIELD_NUMBER: builtins.int
             value: builtins.int = ...
             probability: builtins.float = ...
             def __init__(self,
                 *,
                 value : builtins.int = ...,
                 probability : builtins.float = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"probability",b"probability",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["probability",b"probability","value",b"value"]) -> None: ...
 
         POINTS_FIELD_NUMBER: builtins.int
         MIN_FIELD_NUMBER: builtins.int
         MAX_FIELD_NUMBER: builtins.int
         @property
         def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Distribution.Integer.Point]: ...
         min: builtins.int = ...
         max: builtins.int = ...
         def __init__(self,
             *,
             points : typing.Optional[typing.Iterable[global___Distribution.Integer.Point]] = ...,
             min : builtins.int = ...,
             max : builtins.int = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"max",b"max",u"min",b"min",u"points",b"points"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["max",b"max","min",b"min","points",b"points"]) -> None: ...
 
     class Boolean(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Point(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
@@ -590,24 +590,24 @@
             probability: builtins.float = ...
             def __init__(self,
                 *,
                 name : builtins.bool = ...,
                 value : builtins.int = ...,
                 probability : builtins.float = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"probability",b"probability",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name","probability",b"probability","value",b"value"]) -> None: ...
 
         POINTS_FIELD_NUMBER: builtins.int
         @property
         def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Distribution.Boolean.Point]: ...
         def __init__(self,
             *,
             points : typing.Optional[typing.Iterable[global___Distribution.Boolean.Point]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"points",b"points"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["points",b"points"]) -> None: ...
 
     class Enum(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class Point(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
@@ -617,24 +617,24 @@
             probability: builtins.float = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 value : builtins.float = ...,
                 probability : builtins.float = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"probability",b"probability",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name","probability",b"probability","value",b"value"]) -> None: ...
 
         POINTS_FIELD_NUMBER: builtins.int
         @property
         def points(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Distribution.Enum.Point]: ...
         def __init__(self,
             *,
             points : typing.Optional[typing.Iterable[global___Distribution.Enum.Point]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"points",b"points"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["points",b"points"]) -> None: ...
 
     DOUBLE_FIELD_NUMBER: builtins.int
     INTEGER_FIELD_NUMBER: builtins.int
     BOOLEAN_FIELD_NUMBER: builtins.int
     ENUM_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     @property
@@ -653,11 +653,11 @@
         *,
         double : typing.Optional[global___Distribution.Double] = ...,
         integer : typing.Optional[global___Distribution.Integer] = ...,
         boolean : typing.Optional[global___Distribution.Boolean] = ...,
         enum : typing.Optional[global___Distribution.Enum] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"boolean",b"boolean",u"distribution",b"distribution",u"double",b"double",u"enum",b"enum",u"integer",b"integer"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"boolean",b"boolean",u"distribution",b"distribution",u"double",b"double",u"enum",b"enum",u"integer",b"integer",u"properties",b"properties"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"distribution",b"distribution"]) -> typing.Optional[typing_extensions.Literal["double","integer","boolean","enum"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["boolean",b"boolean","distribution",b"distribution","double",b"double","enum",b"enum","integer",b"integer"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["boolean",b"boolean","distribution",b"distribution","double",b"double","enum",b"enum","integer",b"integer","properties",b"properties"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["distribution",b"distribution"]) -> typing.Optional[typing_extensions.Literal["double","integer","boolean","enum"]]: ...
 global___Distribution = Distribution
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -22,44 +22,44 @@
         @property
         def value(self) -> global___Status.Stage: ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Optional[global___Status.Stage] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Stage(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class PropertiesEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         class Pending(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             def __init__(self,
                 ) -> None: ...
 
         class Processing(google.protobuf.message.Message):
@@ -96,17 +96,17 @@
             *,
             pending : typing.Optional[global___Status.Stage.Pending] = ...,
             processing : typing.Optional[global___Status.Stage.Processing] = ...,
             ready : typing.Optional[global___Status.Stage.Ready] = ...,
             error : typing.Optional[global___Status.Stage.Error] = ...,
             properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"error",b"error",u"pending",b"pending",u"processing",b"processing",u"ready",b"ready",u"stage",b"stage"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"error",b"error",u"pending",b"pending",u"processing",b"processing",u"properties",b"properties",u"ready",b"ready",u"stage",b"stage"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"stage",b"stage"]) -> typing.Optional[typing_extensions.Literal["pending","processing","ready","error"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["error",b"error","pending",b"pending","processing",b"processing","ready",b"ready","stage",b"stage"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["error",b"error","pending",b"pending","processing",b"processing","properties",b"properties","ready",b"ready","stage",b"stage"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["stage",b"stage"]) -> typing.Optional[typing_extensions.Literal["pending","processing","ready","error"]]: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASPEC_FIELD_NUMBER: builtins.int
     MANAGER_FIELD_NUMBER: builtins.int
     DATETIME_FIELD_NUMBER: builtins.int
     TASK_STAGES_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
@@ -129,9 +129,9 @@
         uuid : typing.Text = ...,
         dataspec : typing.Text = ...,
         manager : typing.Text = ...,
         datetime : typing.Text = ...,
         task_stages : typing.Optional[typing.Mapping[typing.Text, global___Status.Stage]] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dataspec",b"dataspec",u"datetime",b"datetime",u"manager",b"manager",u"properties",b"properties",u"task_stages",b"task_stages",u"uuid",b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataspec",b"dataspec","datetime",b"datetime","manager",b"manager","properties",b"properties","task_stages",b"task_stages","uuid",b"uuid"]) -> None: ...
 global___Status = Status
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/transform.proto`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
       GroupByPE group_by_pe = 25;
       SamplingRatios sampling_ratios = 26;
       SelectSql select_sql = 27;
       Extract extract = 28;
       RelationshipSpec relationship_spec = 29;
       DifferentiatedSample differentiated_sample = 30;
       ValidatedUserType validated_user_type=31;
+      DPSelectSql dp_select_sql = 32;
     }
   }
 
   message External {
     bytes arguments = 1;
     bytes named_arguments = 2;
     OpIdentifier op_identifier = 3;
@@ -230,36 +231,43 @@
 
   message SelectSql {
     oneof select {
       string query = 1;
       AliasedQueries aliased_queries = 2;
     }
     SQLDialect sql_dialect = 3;
+  }
 
-    enum SQLDialect {
-      NONE = 0;
-      POSTGRES = 1;
-      SQL_SERVER = 2;
-      MY_SQL = 3;
-      SQLLITE = 4;
-      ORACLE = 5;
-      BIG_QUERY = 6;
-      REDSHIFT = 7;
-      HIVE = 8;
+  message DPSelectSql {
+    oneof select {
+      string query = 1;
+      AliasedQueries aliased_queries = 2;
     }
+    SQLDialect sql_dialect = 3;
+  }
+  enum SQLDialect {
+    NONE = 0;
+    POSTGRES = 1;
+    SQL_SERVER = 2;
+    MY_SQL = 3;
+    SQLLITE = 4;
+    ORACLE = 5;
+    BIG_QUERY = 6;
+    REDSHIFT = 7;
+    HIVE = 8;
+  }
 
 
-    message AliasedQueries {
-      repeated AliasedQuery aliased_query = 1;
-    }
+  message AliasedQueries {
+    repeated AliasedQuery aliased_query = 1;
+  }
 
-    message AliasedQuery {
-      sarus_data_spec.Path path = 1;
-      string query = 2;
-    }
+  message AliasedQuery {
+    sarus_data_spec.Path path = 1;
+    string query = 2;
   }
 
   message Extract {
     int32 size = 1;
   }
    message ValidatedUserType {
   }
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,53 @@
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
 class Transform(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    class _SQLDialect:
+        ValueType = typing.NewType('ValueType', builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+    class _SQLDialectEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SQLDialect.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
+        NONE: Transform.SQLDialect.ValueType = ...  # 0
+        POSTGRES: Transform.SQLDialect.ValueType = ...  # 1
+        SQL_SERVER: Transform.SQLDialect.ValueType = ...  # 2
+        MY_SQL: Transform.SQLDialect.ValueType = ...  # 3
+        SQLLITE: Transform.SQLDialect.ValueType = ...  # 4
+        ORACLE: Transform.SQLDialect.ValueType = ...  # 5
+        BIG_QUERY: Transform.SQLDialect.ValueType = ...  # 6
+        REDSHIFT: Transform.SQLDialect.ValueType = ...  # 7
+        HIVE: Transform.SQLDialect.ValueType = ...  # 8
+    class SQLDialect(_SQLDialect, metaclass=_SQLDialectEnumTypeWrapper):
+        pass
+
+    NONE: Transform.SQLDialect.ValueType = ...  # 0
+    POSTGRES: Transform.SQLDialect.ValueType = ...  # 1
+    SQL_SERVER: Transform.SQLDialect.ValueType = ...  # 2
+    MY_SQL: Transform.SQLDialect.ValueType = ...  # 3
+    SQLLITE: Transform.SQLDialect.ValueType = ...  # 4
+    ORACLE: Transform.SQLDialect.ValueType = ...  # 5
+    BIG_QUERY: Transform.SQLDialect.ValueType = ...  # 6
+    REDSHIFT: Transform.SQLDialect.ValueType = ...  # 7
+    HIVE: Transform.SQLDialect.ValueType = ...  # 8
+
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         value: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
     class Spec(google.protobuf.message.Message):
         """Definitions"""
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         IDENTITY_FIELD_NUMBER: builtins.int
         VARIABLE_FIELD_NUMBER: builtins.int
         COMPOSED_FIELD_NUMBER: builtins.int
@@ -60,14 +87,15 @@
         GROUP_BY_PE_FIELD_NUMBER: builtins.int
         SAMPLING_RATIOS_FIELD_NUMBER: builtins.int
         SELECT_SQL_FIELD_NUMBER: builtins.int
         EXTRACT_FIELD_NUMBER: builtins.int
         RELATIONSHIP_SPEC_FIELD_NUMBER: builtins.int
         DIFFERENTIATED_SAMPLE_FIELD_NUMBER: builtins.int
         VALIDATED_USER_TYPE_FIELD_NUMBER: builtins.int
+        DP_SELECT_SQL_FIELD_NUMBER: builtins.int
         @property
         def identity(self) -> global___Transform.Identity: ...
         @property
         def variable(self) -> global___Transform.Variable: ...
         @property
         def composed(self) -> global___Transform.Composed: ...
         @property
@@ -124,14 +152,16 @@
         def extract(self) -> global___Transform.Extract: ...
         @property
         def relationship_spec(self) -> global___Transform.RelationshipSpec: ...
         @property
         def differentiated_sample(self) -> global___Transform.DifferentiatedSample: ...
         @property
         def validated_user_type(self) -> global___Transform.ValidatedUserType: ...
+        @property
+        def dp_select_sql(self) -> global___Transform.DPSelectSql: ...
         def __init__(self,
             *,
             identity : typing.Optional[global___Transform.Identity] = ...,
             variable : typing.Optional[global___Transform.Variable] = ...,
             composed : typing.Optional[global___Transform.Composed] = ...,
             project : typing.Optional[global___Transform.Project] = ...,
             filter : typing.Optional[global___Transform.Filter] = ...,
@@ -157,18 +187,19 @@
             group_by_pe : typing.Optional[global___Transform.GroupByPE] = ...,
             sampling_ratios : typing.Optional[global___Transform.SamplingRatios] = ...,
             select_sql : typing.Optional[global___Transform.SelectSql] = ...,
             extract : typing.Optional[global___Transform.Extract] = ...,
             relationship_spec : typing.Optional[global___Transform.RelationshipSpec] = ...,
             differentiated_sample : typing.Optional[global___Transform.DifferentiatedSample] = ...,
             validated_user_type : typing.Optional[global___Transform.ValidatedUserType] = ...,
+            dp_select_sql : typing.Optional[global___Transform.DPSelectSql] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"validated_user_type",b"validated_user_type",u"variable",b"variable"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"validated_user_type",b"validated_user_type",u"variable",b"variable"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","protect_dataset","external","synthetic","transcode","inverse_transcode","get_item","protected_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","external",b"external","extract",b"extract","filter",b"filter","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","project",b"project","protect_dataset",b"protect_dataset","protected_paths",b"protected_paths","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","external",b"external","extract",b"extract","filter",b"filter","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","project",b"project","protect_dataset",b"protect_dataset","protected_paths",b"protected_paths","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","protect_dataset","external","synthetic","transcode","inverse_transcode","get_item","protected_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql"]]: ...
 
     class External(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class OpIdentifier(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             STD_FIELD_NUMBER: builtins.int
             PANDAS_FIELD_NUMBER: builtins.int
@@ -205,123 +236,123 @@
                 tensorflow : typing.Optional[global___Transform.External.Tensorflow] = ...,
                 sklearn : typing.Optional[global___Transform.External.Sklearn] = ...,
                 pandas_profiling : typing.Optional[global___Transform.External.PandasProfiling] = ...,
                 xgboost : typing.Optional[global___Transform.External.XGBoost] = ...,
                 skopt : typing.Optional[global___Transform.External.Skopt] = ...,
                 imblearn : typing.Optional[global___Transform.External.Imblearn] = ...,
                 ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal[u"imblearn",b"imblearn",u"numpy",b"numpy",u"op",b"op",u"pandas",b"pandas",u"pandas_profiling",b"pandas_profiling",u"sklearn",b"sklearn",u"skopt",b"skopt",u"std",b"std",u"tensorflow",b"tensorflow",u"xgboost",b"xgboost"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"imblearn",b"imblearn",u"numpy",b"numpy",u"op",b"op",u"pandas",b"pandas",u"pandas_profiling",b"pandas_profiling",u"sklearn",b"sklearn",u"skopt",b"skopt",u"std",b"std",u"tensorflow",b"tensorflow",u"xgboost",b"xgboost"]) -> None: ...
-            def WhichOneof(self, oneof_group: typing_extensions.Literal[u"op",b"op"]) -> typing.Optional[typing_extensions.Literal["std","pandas","numpy","tensorflow","sklearn","pandas_profiling","xgboost","skopt","imblearn"]]: ...
+            def HasField(self, field_name: typing_extensions.Literal["imblearn",b"imblearn","numpy",b"numpy","op",b"op","pandas",b"pandas","pandas_profiling",b"pandas_profiling","sklearn",b"sklearn","skopt",b"skopt","std",b"std","tensorflow",b"tensorflow","xgboost",b"xgboost"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing_extensions.Literal["imblearn",b"imblearn","numpy",b"numpy","op",b"op","pandas",b"pandas","pandas_profiling",b"pandas_profiling","sklearn",b"sklearn","skopt",b"skopt","std",b"std","tensorflow",b"tensorflow","xgboost",b"xgboost"]) -> None: ...
+            def WhichOneof(self, oneof_group: typing_extensions.Literal["op",b"op"]) -> typing.Optional[typing_extensions.Literal["std","pandas","numpy","tensorflow","sklearn","pandas_profiling","xgboost","skopt","imblearn"]]: ...
 
         class Std(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Pandas(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Numpy(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Tensorflow(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Sklearn(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class PandasProfiling(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class XGBoost(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Skopt(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         class Imblearn(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             NAME_FIELD_NUMBER: builtins.int
             name: typing.Text = ...
             def __init__(self,
                 *,
                 name : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["name",b"name"]) -> None: ...
 
         ARGUMENTS_FIELD_NUMBER: builtins.int
         NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
         OP_IDENTIFIER_FIELD_NUMBER: builtins.int
         arguments: builtins.bytes = ...
         named_arguments: builtins.bytes = ...
         @property
         def op_identifier(self) -> global___Transform.External.OpIdentifier: ...
         def __init__(self,
             *,
             arguments : builtins.bytes = ...,
             named_arguments : builtins.bytes = ...,
             op_identifier : typing.Optional[global___Transform.External.OpIdentifier] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"op_identifier",b"op_identifier"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"named_arguments",b"named_arguments",u"op_identifier",b"op_identifier"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["op_identifier",b"op_identifier"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","named_arguments",b"named_arguments","op_identifier",b"op_identifier"]) -> None: ...
 
     class Identity(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class Variable(google.protobuf.message.Message):
@@ -331,30 +362,30 @@
         position: builtins.int = ...
         name: typing.Text = ...
         def __init__(self,
             *,
             position : builtins.int = ...,
             name : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"position",b"position"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["name",b"name","position",b"position"]) -> None: ...
 
     class Composed(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class NamedArgumentsEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: typing.Text = ...
             value: typing.Text = ...
             def __init__(self,
                 *,
                 key : typing.Text = ...,
                 value : typing.Text = ...,
                 ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
 
         TRANSFORM_FIELD_NUMBER: builtins.int
         ARGUMENTS_FIELD_NUMBER: builtins.int
         NAMED_ARGUMENTS_FIELD_NUMBER: builtins.int
         transform: typing.Text = ...
         """Transform"""
 
@@ -366,43 +397,43 @@
         def named_arguments(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
         def __init__(self,
             *,
             transform : typing.Text = ...,
             arguments : typing.Optional[typing.Iterable[typing.Text]] = ...,
             named_arguments : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"arguments",b"arguments",u"named_arguments",b"named_arguments",u"transform",b"transform"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["arguments",b"arguments","named_arguments",b"named_arguments","transform",b"transform"]) -> None: ...
 
     class Project(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         PROJECTION_FIELD_NUMBER: builtins.int
         @property
         def projection(self) -> sarus_data_spec.protobuf.type_pb2.Type:
             """This should be a 'supertype' the type the data can project into."""
             pass
         def __init__(self,
             *,
             projection : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"projection",b"projection"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"projection",b"projection"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["projection",b"projection"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["projection",b"projection"]) -> None: ...
 
     class Filter(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         FILTER_FIELD_NUMBER: builtins.int
         @property
         def filter(self) -> sarus_data_spec.protobuf.type_pb2.Type:
             """This should be a 'subtype' the type the data can be retricted to."""
             pass
         def __init__(self,
             *,
             filter : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"filter",b"filter"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"filter",b"filter"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["filter",b"filter"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["filter",b"filter"]) -> None: ...
 
     class Shuffle(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class Join(google.protobuf.message.Message):
@@ -412,30 +443,30 @@
         def on(self) -> sarus_data_spec.protobuf.type_pb2.Type:
             """This should be a common 'supertype' between tables."""
             pass
         def __init__(self,
             *,
             on : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"on",b"on"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"on",b"on"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["on",b"on"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["on",b"on"]) -> None: ...
 
     class Cast(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         TYPE_FIELD_NUMBER: builtins.int
         @property
         def type(self) -> sarus_data_spec.protobuf.type_pb2.Type:
             """Type to cast into."""
             pass
         def __init__(self,
             *,
             type : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"type",b"type"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"type",b"type"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["type",b"type"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["type",b"type"]) -> None: ...
 
     class Sample(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         FRACTION_FIELD_NUMBER: builtins.int
         SIZE_FIELD_NUMBER: builtins.int
         SEED_FIELD_NUMBER: builtins.int
         fraction: builtins.float = ...
@@ -444,49 +475,50 @@
         def seed(self) -> sarus_data_spec.protobuf.scalar_pb2.Scalar: ...
         def __init__(self,
             *,
             fraction : builtins.float = ...,
             size : builtins.int = ...,
             seed : typing.Optional[sarus_data_spec.protobuf.scalar_pb2.Scalar] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"fraction",b"fraction",u"proportion",b"proportion",u"seed",b"seed",u"size",b"size"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"fraction",b"fraction",u"proportion",b"proportion",u"seed",b"seed",u"size",b"size"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"proportion",b"proportion"]) -> typing.Optional[typing_extensions.Literal["fraction","size"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["proportion",b"proportion"]) -> typing.Optional[typing_extensions.Literal["fraction","size"]]: ...
 
     class SchemaInference(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        class CastPolicy(_CastPolicy, metaclass=_CastPolicyEnumTypeWrapper):
-            pass
         class _CastPolicy:
-            V = typing.NewType('V', builtins.int)
-        class _CastPolicyEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CastPolicy.V], builtins.type):
+            ValueType = typing.NewType('ValueType', builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+        class _CastPolicyEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CastPolicy.ValueType], builtins.type):
             DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-            NONE = Transform.SchemaInference.CastPolicy.V(0)
-            MOST_LIKELY = Transform.SchemaInference.CastPolicy.V(1)
+            NONE: Transform.SchemaInference.CastPolicy.ValueType = ...  # 0
+            MOST_LIKELY: Transform.SchemaInference.CastPolicy.ValueType = ...  # 1
+        class CastPolicy(_CastPolicy, metaclass=_CastPolicyEnumTypeWrapper):
+            pass
 
-        NONE = Transform.SchemaInference.CastPolicy.V(0)
-        MOST_LIKELY = Transform.SchemaInference.CastPolicy.V(1)
+        NONE: Transform.SchemaInference.CastPolicy.ValueType = ...  # 0
+        MOST_LIKELY: Transform.SchemaInference.CastPolicy.ValueType = ...  # 1
 
         CAST_POLICY_FIELD_NUMBER: builtins.int
-        cast_policy: global___Transform.SchemaInference.CastPolicy.V = ...
+        cast_policy: global___Transform.SchemaInference.CastPolicy.ValueType = ...
         def __init__(self,
             *,
-            cast_policy : global___Transform.SchemaInference.CastPolicy.V = ...,
+            cast_policy : global___Transform.SchemaInference.CastPolicy.ValueType = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"cast_policy",b"cast_policy"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["cast_policy",b"cast_policy"]) -> None: ...
 
     class GroupBy(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         def __init__(self,
             *,
             key : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key",b"key"]) -> None: ...
 
     class Synthetic(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class UserSettings(google.protobuf.message.Message):
@@ -498,15 +530,15 @@
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         MAX_CATEGORIES_FIELD_NUMBER: builtins.int
         max_categories: builtins.int = ...
         def __init__(self,
             *,
             max_categories : builtins.int = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"max_categories",b"max_categories"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["max_categories",b"max_categories"]) -> None: ...
 
     class Protect(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class Transcode(google.protobuf.message.Message):
@@ -530,17 +562,17 @@
         def seed(self) -> sarus_data_spec.protobuf.scalar_pb2.Scalar: ...
         def __init__(self,
             *,
             fraction : builtins.float = ...,
             size : builtins.int = ...,
             seed : typing.Optional[sarus_data_spec.protobuf.scalar_pb2.Scalar] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"fraction",b"fraction",u"proportion",b"proportion",u"seed",b"seed",u"size",b"size"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"fraction",b"fraction",u"proportion",b"proportion",u"seed",b"seed",u"size",b"size"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"proportion",b"proportion"]) -> typing.Optional[typing_extensions.Literal["fraction","size"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["proportion",b"proportion"]) -> typing.Optional[typing_extensions.Literal["fraction","size"]]: ...
 
     class ProtectedPaths(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class PublicPaths(google.protobuf.message.Message):
@@ -553,16 +585,16 @@
         PATH_FIELD_NUMBER: builtins.int
         @property
         def path(self) -> sarus_data_spec.protobuf.path_pb2.Path: ...
         def __init__(self,
             *,
             path : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"path",b"path"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"path",b"path"]) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["path",b"path"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["path",b"path"]) -> None: ...
 
     class AssignBudget(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class AutomaticBudget(google.protobuf.message.Message):
@@ -584,15 +616,15 @@
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         RANDOM_INTEGER_FIELD_NUMBER: builtins.int
         random_integer: builtins.int = ...
         def __init__(self,
             *,
             random_integer : builtins.int = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"random_integer",b"random_integer"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["random_integer",b"random_integer"]) -> None: ...
 
     class GroupByPE(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class SamplingRatios(google.protobuf.message.Message):
@@ -603,92 +635,85 @@
     class RelationshipSpec(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class SelectSql(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        class SQLDialect(_SQLDialect, metaclass=_SQLDialectEnumTypeWrapper):
-            pass
-        class _SQLDialect:
-            V = typing.NewType('V', builtins.int)
-        class _SQLDialectEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SQLDialect.V], builtins.type):
-            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-            NONE = Transform.SelectSql.SQLDialect.V(0)
-            POSTGRES = Transform.SelectSql.SQLDialect.V(1)
-            SQL_SERVER = Transform.SelectSql.SQLDialect.V(2)
-            MY_SQL = Transform.SelectSql.SQLDialect.V(3)
-            SQLLITE = Transform.SelectSql.SQLDialect.V(4)
-            ORACLE = Transform.SelectSql.SQLDialect.V(5)
-            BIG_QUERY = Transform.SelectSql.SQLDialect.V(6)
-            REDSHIFT = Transform.SelectSql.SQLDialect.V(7)
-            HIVE = Transform.SelectSql.SQLDialect.V(8)
-
-        NONE = Transform.SelectSql.SQLDialect.V(0)
-        POSTGRES = Transform.SelectSql.SQLDialect.V(1)
-        SQL_SERVER = Transform.SelectSql.SQLDialect.V(2)
-        MY_SQL = Transform.SelectSql.SQLDialect.V(3)
-        SQLLITE = Transform.SelectSql.SQLDialect.V(4)
-        ORACLE = Transform.SelectSql.SQLDialect.V(5)
-        BIG_QUERY = Transform.SelectSql.SQLDialect.V(6)
-        REDSHIFT = Transform.SelectSql.SQLDialect.V(7)
-        HIVE = Transform.SelectSql.SQLDialect.V(8)
-
-        class AliasedQueries(google.protobuf.message.Message):
-            DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-            ALIASED_QUERY_FIELD_NUMBER: builtins.int
-            @property
-            def aliased_query(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Transform.SelectSql.AliasedQuery]: ...
-            def __init__(self,
-                *,
-                aliased_query : typing.Optional[typing.Iterable[global___Transform.SelectSql.AliasedQuery]] = ...,
-                ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"aliased_query",b"aliased_query"]) -> None: ...
-
-        class AliasedQuery(google.protobuf.message.Message):
-            DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-            PATH_FIELD_NUMBER: builtins.int
-            QUERY_FIELD_NUMBER: builtins.int
-            @property
-            def path(self) -> sarus_data_spec.protobuf.path_pb2.Path: ...
-            query: typing.Text = ...
-            def __init__(self,
-                *,
-                path : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
-                query : typing.Text = ...,
-                ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal[u"path",b"path"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal[u"path",b"path",u"query",b"query"]) -> None: ...
+        QUERY_FIELD_NUMBER: builtins.int
+        ALIASED_QUERIES_FIELD_NUMBER: builtins.int
+        SQL_DIALECT_FIELD_NUMBER: builtins.int
+        query: typing.Text = ...
+        @property
+        def aliased_queries(self) -> global___Transform.AliasedQueries: ...
+        sql_dialect: global___Transform.SQLDialect.ValueType = ...
+        def __init__(self,
+            *,
+            query : typing.Text = ...,
+            aliased_queries : typing.Optional[global___Transform.AliasedQueries] = ...,
+            sql_dialect : global___Transform.SQLDialect.ValueType = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["aliased_queries",b"aliased_queries","query",b"query","select",b"select"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["aliased_queries",b"aliased_queries","query",b"query","select",b"select","sql_dialect",b"sql_dialect"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["select",b"select"]) -> typing.Optional[typing_extensions.Literal["query","aliased_queries"]]: ...
 
+    class DPSelectSql(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         QUERY_FIELD_NUMBER: builtins.int
         ALIASED_QUERIES_FIELD_NUMBER: builtins.int
         SQL_DIALECT_FIELD_NUMBER: builtins.int
         query: typing.Text = ...
         @property
-        def aliased_queries(self) -> global___Transform.SelectSql.AliasedQueries: ...
-        sql_dialect: global___Transform.SelectSql.SQLDialect.V = ...
+        def aliased_queries(self) -> global___Transform.AliasedQueries: ...
+        sql_dialect: global___Transform.SQLDialect.ValueType = ...
         def __init__(self,
             *,
             query : typing.Text = ...,
-            aliased_queries : typing.Optional[global___Transform.SelectSql.AliasedQueries] = ...,
-            sql_dialect : global___Transform.SelectSql.SQLDialect.V = ...,
+            aliased_queries : typing.Optional[global___Transform.AliasedQueries] = ...,
+            sql_dialect : global___Transform.SQLDialect.ValueType = ...,
+            ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["aliased_queries",b"aliased_queries","query",b"query","select",b"select"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["aliased_queries",b"aliased_queries","query",b"query","select",b"select","sql_dialect",b"sql_dialect"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["select",b"select"]) -> typing.Optional[typing_extensions.Literal["query","aliased_queries"]]: ...
+
+    class AliasedQueries(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        ALIASED_QUERY_FIELD_NUMBER: builtins.int
+        @property
+        def aliased_query(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Transform.AliasedQuery]: ...
+        def __init__(self,
+            *,
+            aliased_query : typing.Optional[typing.Iterable[global___Transform.AliasedQuery]] = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["aliased_query",b"aliased_query"]) -> None: ...
+
+    class AliasedQuery(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        PATH_FIELD_NUMBER: builtins.int
+        QUERY_FIELD_NUMBER: builtins.int
+        @property
+        def path(self) -> sarus_data_spec.protobuf.path_pb2.Path: ...
+        query: typing.Text = ...
+        def __init__(self,
+            *,
+            path : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
+            query : typing.Text = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"aliased_queries",b"aliased_queries",u"query",b"query",u"select",b"select"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"aliased_queries",b"aliased_queries",u"query",b"query",u"select",b"select",u"sql_dialect",b"sql_dialect"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"select",b"select"]) -> typing.Optional[typing_extensions.Literal["query","aliased_queries"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["path",b"path"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["path",b"path","query",b"query"]) -> None: ...
 
     class Extract(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         SIZE_FIELD_NUMBER: builtins.int
         size: builtins.int = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"size",b"size"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["size",b"size"]) -> None: ...
 
     class ValidatedUserType(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
@@ -719,10 +744,10 @@
         name : typing.Text = ...,
         doc : typing.Text = ...,
         spec : typing.Optional[global___Transform.Spec] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         inversible : builtins.bool = ...,
         schema_preserving : builtins.bool = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"spec",b"spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"doc",b"doc",u"inversible",b"inversible",u"name",b"name",u"properties",b"properties",u"schema_preserving",b"schema_preserving",u"spec",b"spec",u"uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["spec",b"spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["doc",b"doc","inversible",b"inversible","name",b"name","properties",b"properties","schema_preserving",b"schema_preserving","spec",b"spec","uuid",b"uuid"]) -> None: ...
 global___Transform = Transform
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/size.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/status.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/storage/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 from itertools import chain, combinations
 from typing import (
     Callable,
     Collection,
     DefaultDict,
+    Dict,
     Final,
     FrozenSet,
     List,
     MutableMapping,
     Optional,
     Set,
     Tuple,
@@ -171,14 +172,59 @@
             referred_uuid = {referred.uuid()}
         else:
             referred_uuid = {value.uuid() for value in referred}
         return self.referring_uuid(
             referred_uuid=referred_uuid, type_name=type_name
         )
 
+    def batch_referring(
+        self,
+        collection_referred: Collection[
+            Union[
+                Referrable[ProtobufWithUUID],
+                Collection[Referrable[ProtobufWithUUID]],
+            ]
+        ],
+        type_names: Optional[Collection[str]] = None,
+    ) -> Optional[Dict[str, Set[Referring[ProtobufWithUUID]]]]:
+        referred_strings = []
+        for referred in collection_referred:
+            if isinstance(referred, Referrable):
+                referred_strings.append(
+                    referrable_collection_string([referred])
+                )
+            else:
+                referred_strings.append(referrable_collection_string(referred))
+
+        referring_uuids: List[str] = []
+        for referred_string in referred_strings:
+            referring_uuids.extend(self._referring[referred_string])
+
+        referrings: List[Referring[ProtobufWithUUID]] = []
+        for uuid in referring_uuids:
+            ref = self.referrable(uuid)
+            assert ref is not None
+            referring = cast(Referring[ProtobufWithUUID], ref)
+            referrings.append(referring)
+
+        # init result dict with types
+        result_dict: Dict[str, Set[Referring[ProtobufWithUUID]]] = {}
+        if type_names is not None:
+            for type_name in type_names:
+                result_dict[type_name] = set()
+
+        for referring in referrings:
+            typename = referring.type_name()
+            if typename in result_dict:
+                result_dict[typename].add(referring)
+            else:
+                result_dict[typename] = {referring}
+
+        return result_dict
+
     def sources(
         self,
         value: Referrable[ProtobufWithUUID],
         type_name: Optional[str] = None,
     ) -> Set[DataSpec]:
         """Returns a set of all sources of a referrable."""
         if not isinstance(value, Referring):
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/storage/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     Callable,
     Collection,
+    Dict,
     Optional,
     Protocol,
     Set,
     Tuple,
     Union,
     runtime_checkable,
 )
@@ -49,14 +50,28 @@
             Collection[Referrable[ProtobufWithUUID]],
         ],
         type_name: Optional[str] = None,
     ) -> Collection[Referring[ProtobufWithUUID]]:
         """List all values referring to one referred."""
         ...
 
+    def batch_referring(
+        self,
+        collection_referred: Collection[
+            Union[
+                Referrable[ProtobufWithUUID],
+                Collection[Referrable[ProtobufWithUUID]],
+            ]
+        ],
+        type_names: Optional[Collection[str]] = None,
+    ) -> Optional[Dict[str, Set[Referring[ProtobufWithUUID]]]]:
+        """Returns the list of all the referring
+        (for multiples type_name) of several Referrables."""
+        ...
+
     def sources(
         self,
         referring: Referrable[ProtobufWithUUID],
         type_name: Optional[str] = None,
     ) -> Set[DataSpec]:
         """List all sources."""
         ...
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return self._protobuf.spec.HasField('composed')
 
     def is_variable(self) -> bool:
         """Is the transform a variable."""
         return self._protobuf.spec.HasField('variable')
 
     def spec(self) -> str:
-        return t.cast(str, self.protobuf().spec.WhichOneof('spec'))
+        return t.cast(str, self._protobuf.spec.WhichOneof('spec'))
 
     def is_external(self) -> bool:
         """Is the transform an external operation."""
         return self._protobuf.spec.HasField("external")
 
     def infer_output_type(
         self,
@@ -865,17 +865,17 @@
     dialect: t.Optional[st.SQLDialect] = None,
 ) -> st.Transform:
     """Transform that applies a query or a batch of aliased queries to
     a dataset.Calling .schema() or .to_arrow() on a select_sql transformed
     dataset the .sql method will be invoked and the query will be executed.
     """
     sql_dialect = (
-        sp.Transform.SelectSql.SQLDialect.POSTGRES
+        sp.Transform.SQLDialect.POSTGRES
         if not dialect
-        else sp.Transform.SelectSql.SQLDialect.Value(dialect.name)
+        else sp.Transform.SQLDialect.Value(dialect.name)
     )
     if isinstance(query, str):
         select_sql = sp.Transform.SelectSql(
             query=query,
             sql_dialect=sql_dialect,
         )
     elif len(query) == 0:
@@ -891,17 +891,17 @@
                     if isinstance(name, t.Tuple)  # type: ignore
                     else (name,)
                 )
             ): qry
             for (name, qry) in query.items()
         }
         select_sql = sp.Transform.SelectSql(
-            aliased_queries=sp.Transform.SelectSql.AliasedQueries(
+            aliased_queries=sp.Transform.AliasedQueries(
                 aliased_query=(
-                    sp.Transform.SelectSql.AliasedQuery(
+                    sp.Transform.AliasedQuery(
                         path=_path.protobuf(),
                         query=qry,
                     )
                     for (_path, qry) in queries.items()
                 ),
             ),
             sql_dialect=sql_dialect,
@@ -913,14 +913,70 @@
             spec=sp.Transform.Spec(select_sql=select_sql),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
+def dp_select_sql(
+    query: t.Union[str, t.Dict[t.Union[str, t.Tuple[str]], str]],
+    dialect: t.Optional[st.SQLDialect] = None,
+) -> st.Transform:
+    """DP variant of select_sql transform. It should be called with a budget
+    and a seed as every dp transform.
+    """
+    sql_dialect = (
+        sp.Transform.SQLDialect.POSTGRES
+        if not dialect
+        else sp.Transform.SQLDialect.Value(dialect.name)
+    )
+    if isinstance(query, str):
+        proto = sp.Transform.DPSelectSql(
+            query=query,
+            sql_dialect=sql_dialect,
+        )
+    elif len(query) == 0:
+        raise ValueError(
+            """Transform `SelecltSQL` must be used with
+            at least one query"""
+        )
+    else:
+        queries = {
+            straight_path(
+                list(
+                    name
+                    if isinstance(name, t.Tuple)  # type: ignore
+                    else (name,)
+                )
+            ): qry
+            for (name, qry) in query.items()
+        }
+        proto = sp.Transform.DPSelectSql(
+            aliased_queries=sp.Transform.AliasedQueries(
+                aliased_query=(
+                    sp.Transform.AliasedQuery(
+                        path=_path.protobuf(),
+                        query=qry,
+                    )
+                    for (_path, qry) in queries.items()
+                ),
+            ),
+            sql_dialect=sql_dialect,
+        )
+
+    return Transform(
+        sp.Transform(
+            name='dp_select_sql',
+            spec=sp.Transform.Spec(dp_select_sql=proto),
+            inversible=False,
+            schema_preserving=False,
+        )
+    )
+
+
 def extract(
     size: int,
 ) -> st.Transform:
     """Transform that should be called on a dataset from which we want to
     extract some rows from according to the size parameter and a kwargs
     random_seed, a scalar that is a seed. For now, seed and size are
     ignored and iterating on the extract transfomed dataset will be as
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/type.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.5.5/sarus_data_spec/variant_constraint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from __future__ import annotations
 
 from typing import List, Optional, Type, cast
 import json
 
 from sarus_data_spec.base import Referring
-from sarus_data_spec.constants import IS_PUBLIC, PEP_TOKEN, PRIVACY_LIMIT
+from sarus_data_spec.constants import (
+    IS_PUBLIC,
+    IS_SYNTHETIC,
+    PEP_TOKEN,
+    PRIVACY_LIMIT,
+)
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
 class VariantConstraint(Referring[sp.VariantConstraint]):
     def __init__(
@@ -98,23 +103,27 @@
         )
     )
 
 
 def syn_constraint(
     dataspec: st.DataSpec,
     required_context: Optional[List[str]] = None,
+    is_synthetic: bool = True,
 ) -> VariantConstraint:
     """Create a variant constraint specifying a dataspec is synthetic."""
     if required_context is None:
         required_context = []
     return VariantConstraint(
         sp.VariantConstraint(
             dataspec=dataspec.uuid(),
             constraint_kind=sp.ConstraintKind.SYNTHETIC,
             required_context=required_context,
+            properties={
+                IS_SYNTHETIC: str(is_synthetic),
+            },
         )
     )
 
 
 def mock_constraint(
     dataspec: st.DataSpec,
     required_context: Optional[List[str]] = None,
```

### Comparing `sarus_data_spec_public-3.5.1/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.5.5/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/setup.cfg` & `sarus_data_spec_public-3.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.5.1/setup.py` & `sarus_data_spec_public-3.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.5.1')
+    setup(version='3.5.5')
```

