# Comparing `tmp/mlpf-0.0.3.tar.gz` & `tmp/mlpf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.3.tar", last modified: Mon Jun 19 07:56:28 2023, max compression
+gzip compressed data, was "mlpf-0.0.4.tar", last modified: Mon Jun 19 08:31:54 2023, max compression
```

## Comparing `mlpf-0.0.3.tar` & `mlpf-0.0.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.726969 mlpf-0.0.3/
--rw-rw-rw-   0        0        0       50 2023-06-17 23:02:26.000000 mlpf-0.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1461 2023-06-19 07:56:28.726969 mlpf-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      846 2023-06-11 14:41:11.000000 mlpf-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.669007 mlpf-0.0.3/examples/
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.669007 mlpf-0.0.3/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.691951 mlpf-0.0.3/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2711 2023-06-11 14:41:11.000000 mlpf-0.0.3/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.669007 mlpf-0.0.3/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.693103 mlpf-0.0.3/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     4940 2023-06-17 16:14:26.000000 mlpf-0.0.3/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4180 2023-06-17 16:14:26.000000 mlpf-0.0.3/examples/torch/supervised_power_flow/mlp.py
--rw-rw-rw-   0        0        0     2327 2023-06-11 14:41:11.000000 mlpf-0.0.3/experiment.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.693103 mlpf-0.0.3/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.700636 mlpf-0.0.3/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.700636 mlpf-0.0.3/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.700636 mlpf-0.0.3/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.708504 mlpf-0.0.3/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.708504 mlpf-0.0.3/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.708504 mlpf-0.0.3/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     3961 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.708504 mlpf-0.0.3/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4022 2023-06-11 16:38:41.000000 mlpf-0.0.3/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.711432 mlpf-0.0.3/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.711432 mlpf-0.0.3/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.711432 mlpf-0.0.3/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/utils/conversion.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.716435 mlpf-0.0.3/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.720270 mlpf-0.0.3/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.720270 mlpf-0.0.3/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.724299 mlpf-0.0.3/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.725816 mlpf-0.0.3/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.3/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.3/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.3/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.726969 mlpf-0.0.3/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.3/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.700636 mlpf-0.0.3/mlpf.egg-info/
--rw-rw-rw-   0        0        0     1461 2023-06-19 07:56:28.000000 mlpf-0.0.3/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2021 2023-06-19 07:56:28.000000 mlpf-0.0.3/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:56:28.000000 mlpf-0.0.3/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-19 07:56:28.000000 mlpf-0.0.3/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-19 07:56:28.000000 mlpf-0.0.3/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 07:56:28.728759 mlpf-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-06-19 07:56:19.000000 mlpf-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:56:28.726969 mlpf-0.0.3/test/
--rw-rw-rw-   0        0        0     2994 2023-06-11 16:38:41.000000 mlpf-0.0.3/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/
+-rw-rw-rw-   0        0        0       50 2023-06-17 23:02:26.000000 mlpf-0.0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1549 2023-06-19 08:31:54.885695 mlpf-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-06-19 08:31:30.000000 mlpf-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.838093 mlpf-0.0.4/examples/
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.838093 mlpf-0.0.4/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.852446 mlpf-0.0.4/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2711 2023-06-11 14:41:11.000000 mlpf-0.0.4/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.838093 mlpf-0.0.4/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.852446 mlpf-0.0.4/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     4940 2023-06-17 16:14:26.000000 mlpf-0.0.4/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4180 2023-06-17 16:14:26.000000 mlpf-0.0.4/examples/torch/supervised_power_flow/mlp.py
+-rw-rw-rw-   0        0        0     2327 2023-06-11 14:41:11.000000 mlpf-0.0.4/experiment.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.852446 mlpf-0.0.4/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     3961 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     4022 2023-06-11 16:38:41.000000 mlpf-0.0.4/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.878953 mlpf-0.0.4/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.882507 mlpf-0.0.4/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/utils/conversion.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.4/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.4/mlpf/loss/torch/metrics/power_flow.py
+-rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.4/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.4/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.863863 mlpf-0.0.4/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     1549 2023-06-19 08:31:54.000000 mlpf-0.0.4/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2021 2023-06-19 08:31:54.000000 mlpf-0.0.4/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:31:54.000000 mlpf-0.0.4/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-19 08:31:54.000000 mlpf-0.0.4/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-19 08:31:54.000000 mlpf-0.0.4/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:31:54.885695 mlpf-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-06-19 08:31:43.000000 mlpf-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:31:54.885695 mlpf-0.0.4/test/
+-rw-rw-rw-   0        0        0     2994 2023-06-11 16:38:41.000000 mlpf-0.0.4/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.3/LICENCE.txt` & `mlpf-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/PKG-INFO` & `mlpf-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -13,17 +13,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 <p align="center">
-<img src="images/logo.png" width="650">
+<img src="https://github.com/viktor-ktorvi/mlpf/assets/69254199/333dfd18-7c60-4874-a89b-92eecf32ac96?raw=True" width="650">
 </p>
 
+
+
 __MLPF__ is a python library for (optimal) power flow calculations with machine learning.
 It offers:
 
 * efficient loss functions compatible with both _PyTorch_ and _scikit-learn_!
 * utilities such as data structures and loading pipelines that make it easy to go from
   _pandapower_ nets or _PYPOWER_ case files to arrays and tensors in just one line of code!
 * visualization and description tools to take a quick look at your data
```

### Comparing `mlpf-0.0.3/README.md` & `mlpf-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <p align="center">
-<img src="images/logo.png" width="650">
+<img src="https://github.com/viktor-ktorvi/mlpf/assets/69254199/333dfd18-7c60-4874-a89b-92eecf32ac96?raw=True" width="650">
 </p>
 
+
+
 __MLPF__ is a python library for (optimal) power flow calculations with machine learning.
 It offers:
 
 * efficient loss functions compatible with both _PyTorch_ and _scikit-learn_!
 * utilities such as data structures and loading pipelines that make it easy to go from
   _pandapower_ nets or _PYPOWER_ case files to arrays and tensors in just one line of code!
 * visualization and description tools to take a quick look at your data
```

### Comparing `mlpf-0.0.3/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.4/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.4/examples/torch/supervised_power_flow/gcn.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.4/examples/torch/supervised_power_flow/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/experiment.py` & `mlpf-0.0.4/experiment.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.4/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.4/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.4/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/utils.py` & `mlpf-0.0.4/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.4/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.4/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.4/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.4/mlpf/data/data/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/data/torch/power_flow.py` & `mlpf-0.0.4/mlpf/data/data/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.4/mlpf/data/generate/generate_uniform_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/loading/load_data.py` & `mlpf-0.0.4/mlpf/data/loading/load_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/utils/conversion.py` & `mlpf-0.0.4/mlpf/data/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/utils/masks.py` & `mlpf-0.0.4/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.4/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/data/utils/saving.py` & `mlpf-0.0.4/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/enumerations/generator_table.py` & `mlpf-0.0.4/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.4/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.4/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.4/mlpf/loss/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/numpy/utils.py` & `mlpf-0.0.4/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/relative_values.py` & `mlpf-0.0.4/mlpf/loss/relative_values.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.4/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/torch/metrics/power_flow.py` & `mlpf-0.0.4/mlpf/loss/torch/metrics/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.4/mlpf/loss/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/loss/torch/utils.py` & `mlpf-0.0.4/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf/utils/standard_scaler.py` & `mlpf-0.0.4/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.4/mlpf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -13,17 +13,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 <p align="center">
-<img src="images/logo.png" width="650">
+<img src="https://github.com/viktor-ktorvi/mlpf/assets/69254199/333dfd18-7c60-4874-a89b-92eecf32ac96?raw=True" width="650">
 </p>
 
+
+
 __MLPF__ is a python library for (optimal) power flow calculations with machine learning.
 It offers:
 
 * efficient loss functions compatible with both _PyTorch_ and _scikit-learn_!
 * utilities such as data structures and loading pipelines that make it easy to go from
   _pandapower_ nets or _PYPOWER_ case files to arrays and tensors in just one line of code!
 * visualization and description tools to take a quick look at your data
```

### Comparing `mlpf-0.0.3/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.4/mlpf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.3/setup.py` & `mlpf-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.3',
+    version='0.0.4',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
```

### Comparing `mlpf-0.0.3/test/test_power_flow_loss.py` & `mlpf-0.0.4/test/test_power_flow_loss.py`

 * *Files identical despite different names*

