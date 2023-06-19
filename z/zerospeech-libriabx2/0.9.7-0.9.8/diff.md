# Comparing `tmp/zerospeech-libriabx2-0.9.7.tar.gz` & `tmp/zerospeech-libriabx2-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerospeech-libriabx2-0.9.7.tar", last modified: Mon Jan  2 16:58:00 2023, max compression
+gzip compressed data, was "zerospeech-libriabx2-0.9.8.tar", last modified: Mon Jun 19 12:59:52 2023, max compression
```

## Comparing `zerospeech-libriabx2-0.9.7.tar` & `zerospeech-libriabx2-0.9.8.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.797074 zerospeech-libriabx2-0.9.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.797074 zerospeech-libriabx2-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/.github/workflows/pipy-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.797074 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-02 16:58:00.000000 zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.797074 zerospeech-libriabx2-0.9.7/zrc_abx2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_feature_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_feature_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_item_file_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterators_anycontext.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/abx_group_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)   921981 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/dtw.c
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/dtw.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/cpc_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/seq_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/feature_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 16:58:00.801074 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/unit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-01-02 16:57:40.000000 zerospeech-libriabx2-0.9.7/zrc_abx2/eval_ABX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.700447 zerospeech-libriabx2-0.9.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.704447 zerospeech-libriabx2-0.9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/.github/workflows/conda-build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/.github/workflows/pipy-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.704447 zerospeech-libriabx2-0.9.8/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.704447 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 12:59:52.000000 zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.704447 zerospeech-libriabx2-0.9.8/zrc_abx2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.704447 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_feature_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_feature_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_item_file_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterators_anycontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/abx_group_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   921981 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/dtw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/dtw.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/cpc_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/seq_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/feature_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:59:52.708447 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/unit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-19 12:59:28.000000 zerospeech-libriabx2-0.9.8/zrc_abx2/eval_ABX.py
```

### Comparing `zerospeech-libriabx2-0.9.7/.github/workflows/pipy-publish.yaml` & `zerospeech-libriabx2-0.9.8/.github/workflows/pipy-publish.yaml`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/.gitignore` & `zerospeech-libriabx2-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/LICENCE.txt` & `zerospeech-libriabx2-0.9.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/PKG-INFO` & `zerospeech-libriabx2-0.9.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: zerospeech-libriabx2
-Version: 0.9.7
+Version: 0.9.8
 Summary: Package implementing a revamped method to the librilight-abx.
 Author-email: Mark Hallap <mark.hallap@mail.utoronto.ca>, CoML Team <dev@zerospeech.com>, Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>
 Project-URL: documentation, https://zerospeech.com/toolbox/
 Project-URL: homepage, https://zerospeech.com/
 Project-URL: repository, https://github.com/zerospeech/libri-light-abx2
 Keywords: speech,machine-learning,challenges,research-tool,benchmark-speech,zerospeech
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # libri-light-abx2
@@ -24,14 +28,18 @@
 
 `pip install zerospeech-libriabx2`
 
 Or you can install from source by cloning this repository and running: 
 
 `pip install .`
 
+As the final alternative, you can install into a conda environment by running:
+
+`conda install -c conda-forge -c pytorch -c coml zerospeech-libriabx2 pytorch::pytorch`
+
 ### Usage
 ### From command line
 
 ```
 usage: zrc-abx2 [-h] [--path_checkpoint PATH_CHECKPOINT]
                 [--file_extension {.pt,.npy,.wav,.flac,.mp3,.npz,.txt}]
                 [--feature_size FEATURE_SIZE] [--cuda]
```

### Comparing `zerospeech-libriabx2-0.9.7/README.md` & `zerospeech-libriabx2-0.9.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 `pip install zerospeech-libriabx2`
 
 Or you can install from source by cloning this repository and running: 
 
 `pip install .`
 
+As the final alternative, you can install into a conda environment by running:
+
+`conda install -c conda-forge -c pytorch -c coml zerospeech-libriabx2 pytorch::pytorch`
+
 ### Usage
 ### From command line
 
 ```
 usage: zrc-abx2 [-h] [--path_checkpoint PATH_CHECKPOINT]
                 [--file_extension {.pt,.npy,.wav,.flac,.mp3,.npz,.txt}]
                 [--feature_size FEATURE_SIZE] [--cuda]
```

### Comparing `zerospeech-libriabx2-0.9.7/pyproject.toml` & `zerospeech-libriabx2-0.9.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.8"
 keywords = [
     "speech", "machine-learning", "challenges",
     "research-tool", "benchmark-speech", "zerospeech"
 ]
 classifiers = [
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Intended Audience :: Science/Research"
 ]
 dependencies = [
     'tqdm',
     'torch',
     'soundfile',
```

### Comparing `zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/PKG-INFO` & `zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: zerospeech-libriabx2
-Version: 0.9.7
+Version: 0.9.8
 Summary: Package implementing a revamped method to the librilight-abx.
 Author-email: Mark Hallap <mark.hallap@mail.utoronto.ca>, CoML Team <dev@zerospeech.com>, Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>
 Project-URL: documentation, https://zerospeech.com/toolbox/
 Project-URL: homepage, https://zerospeech.com/
 Project-URL: repository, https://github.com/zerospeech/libri-light-abx2
 Keywords: speech,machine-learning,challenges,research-tool,benchmark-speech,zerospeech
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # libri-light-abx2
@@ -24,14 +28,18 @@
 
 `pip install zerospeech-libriabx2`
 
 Or you can install from source by cloning this repository and running: 
 
 `pip install .`
 
+As the final alternative, you can install into a conda environment by running:
+
+`conda install -c conda-forge -c pytorch -c coml zerospeech-libriabx2 pytorch::pytorch`
+
 ### Usage
 ### From command line
 
 ```
 usage: zrc-abx2 [-h] [--path_checkpoint PATH_CHECKPOINT]
                 [--file_extension {.pt,.npy,.wav,.flac,.mp3,.npz,.txt}]
                 [--feature_size FEATURE_SIZE] [--cuda]
```

### Comparing `zerospeech-libriabx2-0.9.7/zerospeech_libriabx2.egg-info/SOURCES.txt` & `zerospeech-libriabx2-0.9.8/zerospeech_libriabx2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 .gitignore
 LICENCE.txt
 README.md
+environment.yml
 pyproject.toml
 setup.py
+.github/workflows/conda-build.yaml
 .github/workflows/pipy-publish.yaml
+conda-recipe/meta.yaml
 zerospeech_libriabx2.egg-info/PKG-INFO
 zerospeech_libriabx2.egg-info/SOURCES.txt
 zerospeech_libriabx2.egg-info/dependency_links.txt
 zerospeech_libriabx2.egg-info/entry_points.txt
 zerospeech_libriabx2.egg-info/not-zip-safe
 zerospeech_libriabx2.egg-info/requires.txt
 zerospeech_libriabx2.egg-info/top_level.txt
```

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_feature_dataset.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_feature_loader.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_feature_loader.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXDataset/abx_item_file_loader.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXDataset/abx_item_file_loader.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterator_factory.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterator_factory.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterators.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterators.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/ABXIterators/abx_iterators_anycontext.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/ABXIterators/abx_iterators_anycontext.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/abx_group_computation.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/abx_group_computation.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/dtw.c` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/dtw.c`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/dtw.pyx` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/dtw.pyx`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/ABX_src/models.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/ABX_src/models.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/LICENSE` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/LICENSE`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/README.md` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/README.md`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/cpc_default_config.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/cpc_default_config.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/criterion.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/criterion.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/custom_layers.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/criterion/seq_alignment.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/criterion/seq_alignment.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/dataset.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/dataset.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/feature_loader.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/feature_loader.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/model.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/model.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/train.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/train.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/transformers.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/transformers.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/misc.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/misc.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/cpc/utils/unit_tests.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/cpc/utils/unit_tests.py`

 * *Files identical despite different names*

### Comparing `zerospeech-libriabx2-0.9.7/zrc_abx2/eval_ABX.py` & `zerospeech-libriabx2-0.9.8/zrc_abx2/eval_ABX.py`

 * *Files identical despite different names*

