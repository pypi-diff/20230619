# Comparing `tmp/pydebiaseddta-0.0.5.tar.gz` & `tmp/pydebiaseddta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydebiaseddta-0.0.5.tar", last modified: Fri Dec 16 20:45:26 2022, max compression
+gzip compressed data, was "pydebiaseddta-0.1.0.tar", last modified: Mon Jun 19 08:22:12 2023, max compression
```

## Comparing `pydebiaseddta-0.0.5.tar` & `pydebiaseddta-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,60 @@
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/
--rw-rw-r--   0 riza      (1003) riza      (1003)     1073 2022-07-11 15:26:37.000000 pydebiaseddta-0.0.5/LICENSE
--rw-rw-r--   0 riza      (1003) riza      (1003)      275 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/MANIFEST.in
--rw-rw-r--   0 riza      (1003) riza      (1003)     1927 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/PKG-INFO
--rw-rw-r--   0 riza      (1003) riza      (1003)      872 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/README.md
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.088058 pydebiaseddta-0.0.5/pydebiaseddta/
--rw-rw-r--   0 riza      (1003) riza      (1003)      238 2022-11-01 16:43:25.000000 pydebiaseddta-0.0.5/pydebiaseddta/__init__.py
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.088058 pydebiaseddta-0.0.5/pydebiaseddta/data/
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.092058 pydebiaseddta-0.0.5/pydebiaseddta/data/dta/
--rw-rw-r--   0 riza      (1003) riza      (1003)  4137612 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/dta/dta_sample_data.json
--rw-rw-r--   0 riza      (1003) riza      (1003)    83719 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/dta/dta_sample_data.mini.json
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.096058 pydebiaseddta-0.0.5/pydebiaseddta/data/sequence/
--rw-rw-r--   0 riza      (1003) riza      (1003)    76202 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/sequence/chembl27.mini.smiles
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.096058 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.096058 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/
--rw-rw-r--   0 riza      (1003) riza      (1003)    18181 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_enc_94.json
--rw-rw-r--   0 riza      (1003) riza      (1003)   392442 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_enc_bpe_8000.json
--rw-rw-r--   0 riza      (1003) riza      (1003)     1325 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_encoding.json
--rw-rw-r--   0 riza      (1003) riza      (1003)    48818 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical_mini_test.json
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.096058 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/protein/
--rw-rw-r--   0 riza      (1003) riza      (1003)     5325 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/protein/uniprot_26.json
--rw-rw-r--   0 riza      (1003) riza      (1003)  1147352 2022-07-12 10:00:53.000000 pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/protein/uniprot_bpe_32000.json
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/pydebiaseddta/debiasing/
--rw-rw-r--   0 riza      (1003) riza      (1003)     3214 2022-11-01 16:43:03.000000 pydebiaseddta-0.0.5/pydebiaseddta/debiasing/__init__.py
--rw-rw-r--   0 riza      (1003) riza      (1003)    10760 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/pydebiaseddta/debiasing/debiaseddta.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     3324 2022-10-21 12:54:15.000000 pydebiaseddta-0.0.5/pydebiaseddta/evaluation.py
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/pydebiaseddta/guides/
--rw-rw-r--   0 riza      (1003) riza      (1003)      370 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/pydebiaseddta/guides/__init__.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     1504 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/pydebiaseddta/guides/abstract_guide.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     5716 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/pydebiaseddta/guides/bowdta.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     3340 2022-12-16 20:39:10.000000 pydebiaseddta-0.0.5/pydebiaseddta/guides/iddta.py
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/pydebiaseddta/predictors/
--rw-rw-r--   0 riza      (1003) riza      (1003)      382 2022-10-21 14:02:22.000000 pydebiaseddta-0.0.5/pydebiaseddta/predictors/__init__.py
--rw-rw-r--   0 riza      (1003) riza      (1003)    11138 2022-12-16 20:36:20.000000 pydebiaseddta-0.0.5/pydebiaseddta/predictors/abstract_predictors.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     8214 2022-11-01 13:58:27.000000 pydebiaseddta-0.0.5/pydebiaseddta/predictors/bpedta.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     8150 2022-11-01 13:58:21.000000 pydebiaseddta-0.0.5/pydebiaseddta/predictors/deepdta.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     5876 2022-11-01 14:24:42.000000 pydebiaseddta-0.0.5/pydebiaseddta/predictors/lmdta.py
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/pydebiaseddta/sequence/
--rw-rw-r--   0 riza      (1003) riza      (1003)      271 2022-10-21 14:00:04.000000 pydebiaseddta-0.0.5/pydebiaseddta/sequence/__init__.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     4982 2022-10-25 06:20:49.000000 pydebiaseddta-0.0.5/pydebiaseddta/sequence/smiles_processing.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     7682 2022-10-25 06:20:49.000000 pydebiaseddta-0.0.5/pydebiaseddta/sequence/word_identification.py
--rw-rw-r--   0 riza      (1003) riza      (1003)     2200 2022-10-21 13:54:20.000000 pydebiaseddta-0.0.5/pydebiaseddta/utils.py
-drwxrwxr-x   0 riza      (1003) riza      (1003)        0 2022-12-16 20:45:26.088058 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/
--rw-rw-r--   0 riza      (1003) riza      (1003)     1927 2022-12-16 20:45:26.000000 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/PKG-INFO
--rw-rw-r--   0 riza      (1003) riza      (1003)     1381 2022-12-16 20:45:26.000000 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/SOURCES.txt
--rw-rw-r--   0 riza      (1003) riza      (1003)        1 2022-12-16 20:45:26.000000 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/dependency_links.txt
--rw-rw-r--   0 riza      (1003) riza      (1003)       92 2022-12-16 20:45:26.000000 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/requires.txt
--rw-rw-r--   0 riza      (1003) riza      (1003)       14 2022-12-16 20:45:26.000000 pydebiaseddta-0.0.5/pydebiaseddta.egg-info/top_level.txt
--rw-rw-r--   0 riza      (1003) riza      (1003)     1016 2022-12-16 20:37:19.000000 pydebiaseddta-0.0.5/pyproject.toml
--rw-rw-r--   0 riza      (1003) riza      (1003)       38 2022-12-16 20:45:26.100057 pydebiaseddta-0.0.5/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.121590 pydebiaseddta-0.1.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      374 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1912 2023-06-19 08:22:12.121383 pydebiaseddta-0.1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4108 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.083355 pydebiaseddta-0.1.0/pydebiaseddta/
+-rwxrwxrwx   0 root         (0) root         (0)      415 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.074059 pydebiaseddta-0.1.0/pydebiaseddta/data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.085506 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.100737 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data/
+-rwxrwxrwx   0 root         (0) root         (0)   861391 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data/test.csv
+-rwxrwxrwx   0 root         (0) root         (0)  2360482 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data/train.csv
+-rwxrwxrwx   0 root         (0) root         (0)   737458 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data/val.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.104982 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data_mini/
+-rwxrwxrwx   0 root         (0) root         (0)     8505 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data_mini/test.csv
+-rwxrwxrwx   0 root         (0) root         (0)    70827 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data_mini/train.csv
+-rwxrwxrwx   0 root         (0) root         (0)     8175 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_data_mini/val.csv
+-rwxrwxrwx   0 root         (0) root         (0)   425807 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/dta/dta_sample_sw_sim_matrix.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.105328 pydebiaseddta-0.1.0/pydebiaseddta/data/sequence/
+-rwxrwxrwx   0 root         (0) root         (0)    76202 2023-06-14 19:19:39.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/sequence/chembl27.mini.smiles
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.106135 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.109600 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/
+-rwxrwxrwx   0 root         (0) root         (0)    18181 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_enc_94.json
+-rwxrwxrwx   0 root         (0) root         (0)   392442 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_enc_bpe_8000.json
+-rwxrwxrwx   0 root         (0) root         (0)     1325 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_encoding.json
+-rwxrwxrwx   0 root         (0) root         (0)    48818 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand_mini_test.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.110240 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/protein/
+-rwxrwxrwx   0 root         (0) root         (0)     5325 2023-06-14 19:19:39.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/protein/uniprot_26.json
+-rwxrwxrwx   0 root         (0) root         (0)  1147352 2023-06-14 19:19:39.000000 pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/protein/uniprot_bpe_32000.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.116696 pydebiaseddta-0.1.0/pydebiaseddta/debiasing/
+-rwxrwxrwx   0 root         (0) root         (0)     3212 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/debiasing/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17394 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/debiasing/debiaseddta.py
+-rwxrwxrwx   0 root         (0) root         (0)     3809 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/evaluation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.118557 pydebiaseddta-0.1.0/pydebiaseddta/guides/
+-rwxrwxrwx   0 root         (0) root         (0)      423 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1504 2023-06-14 19:19:39.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/abstract_guide.py
+-rwxrwxrwx   0 root         (0) root         (0)     8306 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/bowdta.py
+-rwxrwxrwx   0 root         (0) root         (0)     4232 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/iddta.py
+-rwxrwxrwx   0 root         (0) root         (0)     4376 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/outdta.py
+-rwxrwxrwx   0 root         (0) root         (0)     8619 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/guides/rfdta.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.120106 pydebiaseddta-0.1.0/pydebiaseddta/predictors/
+-rwxrwxrwx   0 root         (0) root         (0)      425 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/predictors/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15528 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/predictors/abstract_predictors.py
+-rwxrwxrwx   0 root         (0) root         (0)    10342 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/predictors/bpedta.py
+-rwxrwxrwx   0 root         (0) root         (0)    10246 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/predictors/deepdta.py
+-rwxrwxrwx   0 root         (0) root         (0)     8114 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/predictors/lmdta.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.120990 pydebiaseddta-0.1.0/pydebiaseddta/sequence/
+-rwxrwxrwx   0 root         (0) root         (0)      271 2023-06-14 19:19:39.000000 pydebiaseddta-0.1.0/pydebiaseddta/sequence/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4980 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/sequence/smiles_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)     7671 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/sequence/word_identification.py
+-rwxrwxrwx   0 root         (0) root         (0)    12442 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     9733 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pydebiaseddta/visualization.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-19 08:22:12.085156 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1912 2023-06-19 08:22:12.000000 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1727 2023-06-19 08:22:12.000000 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-19 08:22:12.000000 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      191 2023-06-19 08:22:12.000000 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-06-19 08:22:12.000000 pydebiaseddta-0.1.0/pydebiaseddta.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1156 2023-06-19 08:16:47.000000 pydebiaseddta-0.1.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-19 08:22:12.121681 pydebiaseddta-0.1.0/setup.cfg
```

### Comparing `pydebiaseddta-0.0.5/LICENSE` & `pydebiaseddta-0.1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018 The Python Packaging Authority
+Copyright (c) 2023 Rıza Özçelik
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydebiaseddta-0.0.5/PKG-INFO` & `pydebiaseddta-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydebiaseddta
-Version: 0.0.5
+Version: 0.1.0
 Summary: Python library to improve generalizability of the drug-target prediction models via DebiasedDTA
 Author-email: Rıza Özçelik <riza.ozcelik@boun.edu.tr>
-License: Copyright (c) 2018 The Python Packaging Authority
+License: Copyright (c) 2023 Rıza Özçelik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/sequence/chembl27.mini.smiles` & `pydebiaseddta-0.1.0/pydebiaseddta/data/sequence/chembl27.mini.smiles`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_enc_94.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_enc_94.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_enc_bpe_8000.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_enc_bpe_8000.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical/chembl27_encoding.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand/chembl27_encoding.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/chemical_mini_test.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/ligand_mini_test.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/protein/uniprot_26.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/protein/uniprot_26.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/data/word_identification/protein/uniprot_bpe_32000.json` & `pydebiaseddta-0.1.0/pydebiaseddta/data/word_identification/protein/uniprot_bpe_32000.json`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/debiasing/__init__.py` & `pydebiaseddta-0.1.0/pydebiaseddta/debiasing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 One run of cross-validation yields one squared-error measurement per protein-ligand pair as each pair is placed in the mini-validation set
 exactly once. In order to better estimate the performance on each sample, DebiasedDTA runs the cross-validation `n_bootstrapping`  times and
 obtains `n_bootstrapping` error measurements per sample. DebiasedDTA computes the median of the `n_bootstrapping` squared errors
 and calls it the "importance coefficient" of a protein-ligand pair. The importance coefficients guide the training of the predictor after being converted
 into training weights.
 
 In the DebiasedDTA training framework, the predictor is the model that will be trained with the training samples weighted
-by the guide to ultimately predict target protein-chemical affinities. The predictor can adopt any biomolecule representation,
+by the guide to ultimately predict target protein-ligand affinities. The predictor can adopt any biomolecule representation,
 but has to be able to weight the training samples during training to comply with the weight adaptation strategy proposed in DebiasedDTA.
 
 The proposed strategy initializes the training sample weights to 1 and updates them at each epoch such that the
 weight of each training sample converges to its importance coefficient at the last epoch. When trained with this strategy,
 the predictor attributes higher importance to samples with more information on binding rules (*i.e.* samples with higher
 importance coefficient) as the learning continues. Our weight adaptation strategy is formulated as
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/debiasing/debiaseddta.py` & `pydebiaseddta-0.1.0/pydebiaseddta/predictors/deepdta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,248 +1,252 @@
-import random
-from typing import Any, Dict, List, Tuple, Type
-
+from typing import List
 import numpy as np
-
-from pydebiaseddta import guides, predictors
+from tensorflow.keras.layers import Conv1D, GlobalMaxPooling1D
+from tensorflow.keras.layers import Dense, Dropout, Concatenate
+from tensorflow.keras.layers import Input, Embedding
+from tensorflow.keras.models import Model
+from tensorflow.keras.optimizers import Adam, SGD
+
+from .abstract_predictors import TFPredictor
+from ..sequence.word_identification import (
+    load_ligand_word_identifier,
+    load_protein_word_identifier,
+)
+from ..sequence.smiles_processing import (
+    smiles_to_unichar_batch,
+    load_smiles_to_unichar_encoding,
+)
 
 
-class DebiasedDTA:
+class DeepDTA(TFPredictor):
     def __init__(
         self,
-        guide_cls: Type[guides.Guide],
-        predictor_cls: Type[predictors.BasePredictor],
-        mini_val_frac: float = 0.2,
-        n_bootstrapping: int = 10,
-        guide_params: Dict = None,
-        predictor_params: Dict = None,
+        max_smi_len: int = 100,
+        max_prot_len: int = 1000,
+        embedding_dim: int = 128,
+        learning_rate: float = 0.001,
+        batch_size: int = 256,
+        n_epochs: int = 200,
+        num_filters: int = 32,
+        smi_filter_len: int = 4,
+        prot_filter_len: int = 6,
+        early_stopping_metric: str = "mse",
+        early_stopping_metric_threshold: float = -1e6,
+        early_stopping_num_epochs: int = 0,
+        early_stopping_split: str = "train",
+        optimizer: str = "adam",
+        min_epochs: int = 0,
+        seed: int = 0,
+        **kwargs
     ):
-        """Constructor to initiate a DebiasedDTA training framework. 
-        
-        Parameters
-        ----------
-        guide_cls : Type[guides.AbstractGuide]
-            The `Guide` class for debiasing. Note that the input is not an instance, but a class, *e.g.*, `BoWDTA`, not `BoWDTA()`.
-            The instance is created during the model training by the DebiasedDTA module.
-        predictor_cls : Type[predictors.BasePredictor]
-            Class of the `Predictor` to debias. Note that the input is not an instance, but a class, *e.g.*, `BPEDTA`, not `BPEDTA()`.
-            The instance is created during the model training by the DebiasedDTA module.
-        mini_val_frac : float, optional
-            Fraction of the validation data to separate for guide evaluation, by default 0.2
-        n_bootstrapping : int, optional
-            Number of times to train guides on the training set, by default 10
-        guide_params : Dict, optional
-            Parameter dictionary necessary to create the `Guide`. 
-            The dictionary should map the name of the constructor parameters to their values. 
-            An empty dictionary is used during the creation by default.
-        predictor_params : Dict, optional
-            Parameter dictionary necessary to create the `Predictor`. 
-            The dictionary should map the name of the constructor parameters to their values, and
-            `n_epochs` **must** be among the parameters for debiasing to work.
-            An empty dictionary is used during the creation by default.
-
-        Raises
-        ------
-        ValueError
-            A `ValueError` is raised if `n_epochs` is not among the predictor parameters.
-        """
-        self.guide_cls = guide_cls
-        self.predictor_cls = predictor_cls
-        self.mini_val_frac = mini_val_frac
-        self.n_bootstrapping = n_bootstrapping
-
-        self.guide_params = dict() if guide_params is None else guide_params
-        self.predictor_params = {} if predictor_params is None else predictor_params
-        self.predictor_instance = self.predictor_cls(**self.predictor_params)
-        if "n_epochs" not in self.predictor_instance.__dict__:
-            raise ValueError(
-                'The predictor must have a field named "n_epochs" to be debiased'
-            )
-
-    @staticmethod
-    def save_importance_coefficients(
-        interactions: List[Tuple[int, Any, Any, float]], importance_coefficients: List[float], savedir: str
-    ):
-        """Saves the importance coefficients learned by the `guide`.
+        """Constructor to create a DeepDTA instance.
+        DeepDTA segments SMILES strings of ligands and amino-acid sequences of proteins into characters,
+        and applies three layers of convolutions to learn latent representations. 
+        A fully-connected neural network with three layers is used afterwards to predict affinities.
 
         Parameters
         ----------
-        interactions : List[Tuple[int, Any, Any, float]]
-            The List of training interactions as a Tuple of interaction id (assigned by the guide),
-            ligand, chemical, and affinity score.
-        importance_coefficients : List[float]
-            The importance coefficient for each interaction.
-        savedir : str
-            Path to save the coefficients.
+        max_smi_len : int, optional
+            Maximum number of characters in a SMILES string, by default 100. 
+            Longer SMILES strings are truncated.
+        max_prot_len : int, optional
+            Maximum number of amino-acids a protein sequence, by default 1000. 
+            Longer sequences are truncated.
+        embedding_dim : int, optional
+            The dimension of the biomolecule characters, by default 128.
+        learning_rate : float, optional
+            Learning rate during optimization, by default 0.001.
+        batch_size : int, optional
+            Batch size during training, by default 256.
+        n_epochs : int, optional
+            Number of epochs to train the model, by default 200.
+        num_filters : int, optional
+            Number of filters in the first convolution block. The next blocks use two and three times of this number, respectively. y default 32.
+        smi_filter_len : int, optional
+            Length of filters in the convolution blocks for ligands, by default 4.
+        prot_filter_len : int, optional
+            Length of filters in the convolution blocks for proteins, by default 6.
+        early_stopping_metric : str, optional
+            Metric for early stopping of the training. Available options are "mse", "rmse", "mae", "r2", "ci".
+        early_stopping_metric_threshold : float, optional
+            If the performance in the specified metric in the specified split 
+            fall below this value the training is stopped early. Available options are
+            "mse" and "mae". Set to a negative value by default with no effects.
+        early_stopping_num_epochs : int, optional
+            If this value is set > 0, then if the training has not been better than the
+            best recorded performance for this many epochs on the specified split, the
+            training is stopped early. Set to 0 by default with no effect.
+        early_stopping_split:
+            The split for conducting early stopping checks. Available options are "train"
+            and the keys in the val_split dictionary.
+        optimizer : str, optional
+            The optimizer used in training. Available options are "adam" and "sgd".
+        min_epochs : int, optional
+            Initial number of epochs for which the early stopping computations will be overrided.
+        seed : int, optional
+            Seed for the initialized model.
         """    
-        dump_content = []
-        for interaction_id, ligand, protein, label in interactions:
-            importance_coefficient = importance_coefficients[interaction_id]
-            dump_content.append(f"{ligand},{protein},{label},{importance_coefficient}")
-        dump = "\n".join(dump_content)
-        with open(savedir) as f:
-            f.write(dump)
+        self.max_smi_len = max_smi_len
+        self.max_prot_len = max_prot_len
+        self.embedding_dim = embedding_dim
+        self.num_filters = num_filters
+        self.smi_filter_len = smi_filter_len
+        self.prot_filter_len = prot_filter_len
+
+        self.optimizer = optimizer
+        self.early_stopping_metric = early_stopping_metric
+        self.early_stopping_metric_threshold = early_stopping_metric_threshold
+        self.early_stopping_num_epochs = early_stopping_num_epochs
+        self.early_stopping_split = early_stopping_split
+        self.min_epochs = min_epochs
+
+        self.chem_vocab_size = 94
+        self.prot_vocab_size = 26
+        TFPredictor.__init__(self, n_epochs, learning_rate, batch_size, seed=seed)
 
-    def learn_importance_coefficients(
-        self,
-        train_ligands: List[Any],
-        train_proteins: List[Any],
-        train_labels: List[float],
-        savedir: str = None,
-    ) -> List[float]:
-        """Learns importance coefficients using the `Guide` model specified during the construction.
+    def build(self):
+        """Builds a `DeepDTA` predictor in `keras` with the parameters specified during construction.
+
+        Returns
+        -------
+        tensorflow.keras.models.Model
+            The built model.
+        """    
+        # Inputs
+        ligands = Input(shape=(self.max_smi_len,), dtype="int32")
+
+        # ligand representation
+        ligand_representation = Embedding(
+            input_dim=self.chem_vocab_size + 1,
+            output_dim=self.embedding_dim,
+            input_length=self.max_smi_len,
+            mask_zero=True,
+        )(ligands)
+        ligand_representation = Conv1D(
+            filters=self.num_filters,
+            kernel_size=self.smi_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(ligand_representation)
+        ligand_representation = Conv1D(
+            filters=self.num_filters * 2,
+            kernel_size=self.smi_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(ligand_representation)
+        ligand_representation = Conv1D(
+            filters=self.num_filters * 3,
+            kernel_size=self.smi_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(ligand_representation)
+        ligand_representation = GlobalMaxPooling1D()(ligand_representation)
+
+        # Protein representation
+        proteins = Input(shape=(self.max_prot_len,), dtype="int32")
+        protein_representation = Embedding(
+            input_dim=self.prot_vocab_size + 1,
+            output_dim=self.embedding_dim,
+            input_length=self.max_prot_len,
+            mask_zero=True,
+        )(proteins)
+        protein_representation = Conv1D(
+            filters=self.num_filters,
+            kernel_size=self.prot_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(protein_representation)
+        protein_representation = Conv1D(
+            filters=self.num_filters * 2,
+            kernel_size=self.prot_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(protein_representation)
+        protein_representation = Conv1D(
+            filters=self.num_filters * 3,
+            kernel_size=self.prot_filter_len,
+            activation="relu",
+            padding="valid",
+            strides=1,
+        )(protein_representation)
+        protein_representation = GlobalMaxPooling1D()(protein_representation)
+
+        interaction_representation = Concatenate(axis=-1)(
+            [ligand_representation, protein_representation]
+        )
+
+        # Fully connected layers
+        FC1 = Dense(1024, activation="relu")(interaction_representation)
+        FC1 = Dropout(0.1)(FC1)
+        FC2 = Dense(1024, activation="relu")(FC1)
+        FC2 = Dropout(0.1)(FC2)
+        FC3 = Dense(512, activation="relu")(FC2)
+        predictions = Dense(1, kernel_initializer="normal")(FC3)
+
+        if self.optimizer == "adam":
+            opt = Adam(self.learning_rate)
+        elif self.optimizer == "sgd":
+            opt = SGD(self.learning_rate)
+        else:
+            raise ValueError(f"The optimizer {self.optimizer} is not found.")
+        deepdta = Model(inputs=[ligands, proteins], outputs=[predictions])
+        deepdta.compile(
+            optimizer=opt,
+            loss="mean_squared_error",
+            metrics=["mean_squared_error"],
+        )
+        return deepdta
+
+    def vectorize_ligands(self, ligands: List[str]) -> np.array:
+        """Segments SMILES strings of ligands into characters and applies label encoding.
+        Truncation and padding are also applied to prepare ligands for training and/or prediction.
 
         Parameters
         ----------
-        train_ligands : List[Any]
-            List of the training ligands used by the `Guide` model. 
-            DebiasedDTA training framework imposes no restriction on the representation type of the ligands.
-        train_proteins : List[Any]
-            List of the training proteins used by the `Guide` model. 
-            DebiasedDTA training framework imposes no restriction on the representation type of the proteins.
-        train_labels : List[float]
-            Affinity scores of the training protein-ligand pairs.
-        savedir : str, optional
-            Path to save the learned importance coefficients. By default `None` and the coefficients are not saved.
+        ligands : List[str]
+            The SMILES strings of ligands.
 
         Returns
         -------
-        List[float]
-            The importance coefficients learned by the guide.
-        """
-        train_size = len(train_ligands)
-        train_interactions = list(
-            zip(range(train_size), train_ligands, train_proteins, train_labels,)
-        )
-        mini_val_data_size = int(train_size * self.mini_val_frac) + 1
-        interaction_id_to_sq_diff = [[] for _ in range(train_size)]
+        np.array
+            An $N \\times max\\_smi\\_len$ ($N$ is the number of the input ligands) matrix that contains label encoded sequences of SMILES tokens.
+        """     
+        smi_to_unichar_encoding = load_smiles_to_unichar_encoding()
+        unichars = smiles_to_unichar_batch(ligands, smi_to_unichar_encoding)
+        word_identifier = load_ligand_word_identifier(vocab_size=94)
 
-        for _ in range(self.n_bootstrapping):
-            random.shuffle(train_interactions)
-            n_mini_val = int(1 / self.mini_val_frac)
-            for mini_val_ix in range(n_mini_val):
-                val_start_ix = mini_val_ix * mini_val_data_size
-                val_end_ix = val_start_ix + mini_val_data_size
-                mini_val_interactions = train_interactions[val_start_ix:val_end_ix]
-                mini_train_interactions = (
-                    train_interactions[:val_start_ix] + train_interactions[val_end_ix:]
-                )
-
-                mini_train_ligands = [
-                    interaction[1] for interaction in mini_train_interactions
-                ]
-                mini_train_proteins = [
-                    interaction[2] for interaction in mini_train_interactions
-                ]
-                mini_train_labels = [
-                    interaction[3] for interaction in mini_train_interactions
-                ]
-                guide_instance = self.guide_cls(**self.guide_params)
-                guide_instance.train(
-                    mini_train_ligands, mini_train_proteins, mini_train_labels,
-                )
-
-                mini_val_ligands = [
-                    interaction[1] for interaction in mini_val_interactions
-                ]
-                mini_val_proteins = [
-                    interaction[2] for interaction in mini_val_interactions
-                ]
-                preds = guide_instance.predict(mini_val_ligands, mini_val_proteins)
-                mini_val_labels = [
-                    interaction[3] for interaction in mini_val_interactions
-                ]
-                mini_val_sq_diffs = (np.array(mini_val_labels) - np.array(preds)) ** 2
-                mini_val_interaction_ids = [
-                    interaction[0] for interaction in mini_val_interactions
-                ]
-                for interaction_id, sq_diff in zip(
-                    mini_val_interaction_ids, mini_val_sq_diffs
-                ):
-                    interaction_id_to_sq_diff[interaction_id].append(sq_diff)
-
-        interaction_id_to_med_diff = [
-            np.median(diffs) for diffs in interaction_id_to_sq_diff
-        ]
-        importance_coefficients = [
-            med / sum(interaction_id_to_med_diff) for med in interaction_id_to_med_diff
-        ]
-
-        if savedir is not None:
-            DebiasedDTA.save_importance_coefficients(
-                train_interactions, importance_coefficients, savedir
-            )
+        return np.array(
+            word_identifier.encode_sequences(unichars, self.max_smi_len)
+        )
 
-        return importance_coefficients
+    def vectorize_proteins(self, aa_sequences: List[str]) -> np.array:
+        """Segments amino-acid sequences of proteins into characters and applies label encoding.
+        Truncation and padding are also applied to prepare proteins for training and/or prediction.
 
-    def train(
-        self,
-        train_ligands: List[Any],
-        train_proteins: List[Any],
-        train_labels: List[float],
-        val_ligands: List[Any] = None,
-        val_proteins: List[Any] = None,
-        val_labels: List[float] = None,
-        coeffs_save_path: str = None,
-    ) -> Any:
-        """Starts the DebiasedDTA training framework.
-        The importance coefficients are learned with the guide and used to weight the samples during the predictor's training.
-        Performance on the validation set is also measured, if provided.
         Parameters
         ----------
-        train_ligands : List[Any]
-            List of the training ligands used by the `Predictor`. 
-            DebiasedDTA training framework imposes no restriction on the representation type of the ligands.
-        train_proteins : List[Any]
-            List of the training ligands used by the `Predictor`. 
-            DebiasedDTA training framework imposes no restriction on the representation type of the proteins.
-        train_labels : List[float]
-            Affinity scores of the training protein-ligand pairs.
-        val_ligands : List[Any], optional
-            Validation ligands to measure predictor performance, by default `None` and no validation is applied.
-        val_proteins : List[Any], optional
-            Validation proteins to measure predictor performance, by default `None` and no validation is applied.
-        val_labels : List[float], optional
-            Affinity scores of the Validatio pairs, by default `None` and no validation is applied.
-        coeffs_save_path : str, optional
-            Path to save importance coefficients learned by the `guide`. Defaults to `None` and no saving is performed.
+        aa_sequences : List[str]
+            The amino-acid sequences of proteins.
 
         Returns
         -------
-        Any
-            Output of the train function of the predictor.
-
+        np.array
+            An $N \\times max\\_prot\\_len$ ($N$ is the number of the input proteins) matrix that contains label encoded sequences of amino-acids.
         """
-        train_ligands = train_ligands.copy()
-        train_proteins = train_proteins.copy()
-
-        importance_coefficients = self.learn_importance_coefficients(
-            train_ligands, train_proteins, train_labels, savedir=coeffs_save_path,
+        word_identifier = load_protein_word_identifier(vocab_size=26)
+        return np.array(
+            word_identifier.encode_sequences(aa_sequences, self.max_prot_len)
         )
 
-        n_epochs = self.predictor_instance.n_epochs
-        ic = np.array(importance_coefficients)
-        weights_by_epoch = [
-            1 - (e / n_epochs) + ic * (e / n_epochs) for e in range(n_epochs)
-        ]
-
-        if (
-            val_ligands is not None
-            and val_proteins is not None
-            and val_labels is not None
-        ):
-            return self.predictor_instance.train(
-                train_ligands,
-                train_proteins,
-                train_labels,
-                val_ligands=val_ligands,
-                val_proteins=val_proteins,
-                val_labels=val_labels,
-                sample_weights_by_epoch=weights_by_epoch,
-            )
-
-        return self.predictor_instance.train(
-            train_ligands,
-            train_proteins,
-            train_labels,
-            sample_weights_by_epoch=weights_by_epoch,
-        )
+
+if __name__ == "__main__":
+
+    from pydebiaseddta.utils import load_sample_dta_data
+
+    train_ligands, train_proteins, train_labels = load_sample_dta_data(mini=True, split="train")
+    deepdta = DeepDTA(n_epochs=5)
+    deepdta.train(train_ligands, train_proteins, train_labels)
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/evaluation.py` & `pydebiaseddta-0.1.0/pydebiaseddta/evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict
 from itertools import combinations
 
-from sklearn.metrics import mean_squared_error, r2_score
+from sklearn.metrics import mean_squared_error, r2_score, mean_absolute_error
 
 
 def ci(gold_truths: List[float], predictions: List[float]) -> float:
     """Computes concordance index (CI) between the expected values and predictions. 
     See [Gönen and Heller (2005)](https://www.jstor.org/stable/20441249) for the details of the metric.
 
     Parameters
@@ -80,14 +80,32 @@
     -------
     float
         $R^2$ (coefficient of determinant) score.
     """
     return float(r2_score(gold_truths, predictions))
 
 
+def mae(gold_truths: List[float], predictions: List[float]) -> float:
+    """Computes mean absolute error between expected and predicted values.
+
+    Parameters
+    ----------
+    gold_truths : List[float]
+        The gold labels in the dataset.
+    predictions : List[float]
+        Predictions of a model.
+
+    Returns
+    -------
+    float
+        Mean squared error.
+    """
+    return float(mean_absolute_error(gold_truths, predictions))
+
+
 def evaluate_predictions(
     gold_truths: List[float], predictions: List[float], metrics: List[str] = None
 ) -> Dict[str, float]:
     """Computes multiple metrics with a single call for convenience. 
 
     Parameters
     ----------
@@ -101,12 +119,12 @@
 
     Returns
     -------
     Dict[str,float]
         A dictionary that maps each metric name to the computed value.
     """
     if metrics is None:
-        metrics = ["ci", "r2", "rmse", "mse"]
+        metrics = ["ci", "r2", "rmse", "mse", "mae"]
 
     metrics = [metric.lower() for metric in metrics]
-    name_to_fn = {"ci": ci, "r2": r2, "rmse": rmse, "mse": mse}
+    name_to_fn = {"ci": ci, "r2": r2, "rmse": rmse, "mse": mse, "mae": mae}
     return {metric: name_to_fn[metric](gold_truths, predictions) for metric in metrics}
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/guides/abstract_guide.py` & `pydebiaseddta-0.1.0/pydebiaseddta/guides/abstract_guide.py`

 * *Files identical despite different names*

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/guides/bowdta.py` & `pydebiaseddta-0.1.0/pydebiaseddta/guides/bowdta.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,64 +8,107 @@
     load_ligand_word_identifier,
     load_protein_word_identifier,
 )
 from ..sequence.smiles_processing import (
     smiles_to_unichar_batch,
     load_smiles_to_unichar_encoding,
 )
-
+VOCAB_SIZES_LIGAND = {"high": 8000, "low":94}
+VOCAB_SIZES_PROTEIN = {"high": 32000, "low":26}
 
 class BoWDTA(Guide):
-    def __init__(self):
+    def __init__(
+            self,
+            max_depth: int = None,
+            min_samples_split: int = 2,
+            min_samples_leaf: int = 1,
+            criterion: str = "squared_error",
+            vocab_size: str = "high",
+            ligand_vector_mode: str = "freq",
+            prot_vector_mode: str = "freq",
+            input_rank=0,
+            **kwargs):
         """Constructor to create a BoWDTA model.
         BoWDTA represents the proteins and ligands as "bag-of-words`
         and uses a decision tree for prediction. BoWDTA uses the same biomolecule vocabulary
         as BPEDTA.
+
+        Parameters
+        ----------
+        max_depth : int, optional
+            Determines the maximum depth of the decision tree regressor.
+        min_samples_split : int, optional
+            Determines the minimum samples to split a leaf for the decision
+            tree regressor.
+        min_samples_leaf : int, optional
+            Determines the minimum samples a leaf can have for the decision
+            tree regressor.
+        criterion : str, optional
+            Criterion according to which the decision tree regressor will be trained.
+        vocab_size : str, optional
+            Vocabulary size that will be used for tokenizing ligands and proteins.
+        ligand_vector_mode : str, optional
+            Method to use when creating the matrix representation for ligand tokens.
+        prot_vector_mode : str, optional
+            Method to use when creating the matrix representation for protein tokens.
+        input_rank : int, optional
+            If set > 0, uses a low-rank approximation of the input representation with
+            the given rank.
         """        
         self.ligand_bow_vectorizer = Tokenizer(
             filters=None, lower=False, oov_token="C"
         )
         self.protein_bow_vectorizer = Tokenizer(
             filters=None, lower=False, oov_token="$"
         )
-        self.prediction_model = DecisionTreeRegressor()
-
-    def tokenize_ligands(self, smiles: List[str]) -> List[List[int]]:
+        self.prediction_model = DecisionTreeRegressor(
+            max_depth=max_depth, min_samples_split=min_samples_split, min_samples_leaf=min_samples_leaf, criterion=criterion
+            )
+        self.input_rank = input_rank
+        self.vocab_size = vocab_size
+        self.ligand_vector_mode = ligand_vector_mode
+        self.prot_vector_mode = prot_vector_mode
+    
+    def tokenize_ligands(self, smiles: List[str], vocab_size: str = "high") -> List[List[int]]:
         """Segments SMILES strings of the ligands into their ligand words and applies label encoding.
 
         Parameters
         ----------
         smiles : List[str]
             The SMILES strings of the ligands
+        vocab_size : str, optional
+            Vocabulary size that will be used for tokenizing ligands.
 
         Returns
         -------
         List[List[int]]
             Label encoded sequences of ligand words.
         """
         smi_to_unichar_encoding = load_smiles_to_unichar_encoding()
         unichars = smiles_to_unichar_batch(smiles, smi_to_unichar_encoding)
-        word_identifier = load_ligand_word_identifier(vocab_size=8000)
+        word_identifier = load_ligand_word_identifier(vocab_size=VOCAB_SIZES_LIGAND[vocab_size])
 
         return word_identifier.encode_sequences(unichars, 100)
 
-    def tokenize_proteins(self, aa_sequences: List[str]) -> List[List[int]]:
+    def tokenize_proteins(self, aa_sequences: List[str], vocab_size: str = "high"):
         """Segments amino-acid sequences of the proteins into their protein words and applies label encoding.
 
         Parameters
         ----------
         aa_sequences : List[str]
             The amino-acid sequences of the proteins.
+        vocab_size : str, optional
+            Vocabulary size that will be used for tokenizing proteins.
 
         Returns
         -------
         List[List[int]]
             Label encoded sequences of protein words.
         """
-        word_identifier = load_protein_word_identifier(vocab_size=32000)
+        word_identifier = load_protein_word_identifier(vocab_size=VOCAB_SIZES_PROTEIN[vocab_size])
         return word_identifier.encode_sequences(aa_sequences, 1000)
 
     def vectorize_ligands(self, smiles_words: List[List[int]]) -> np.array:
         """Computes bag-of-words vectors of the ligands based on their frequency.
 
         Parameters
         ----------
@@ -74,15 +117,15 @@
 
         Returns
         -------
         np.array
             Bag-of-words vectors stacked in a matrix.
         """        
         return self.ligand_bow_vectorizer.texts_to_matrix(
-            smiles_words, mode="freq"
+            smiles_words, mode=self.ligand_vector_mode
         )
 
     def vectorize_proteins(self, protein_words: List[List[int]]) -> np.array:
         """Computes bag-of-words vectors of the proteins based on their frequency.
 
         Parameters
         ----------
@@ -91,43 +134,52 @@
 
         Returns
         -------
         np.array
             Bag-of-words vectors stacked in a matrix.
         """  
         return self.protein_bow_vectorizer.texts_to_matrix(
-            protein_words, mode="freq"
+            protein_words, mode=self.prot_vector_mode
         )
 
     def train(
         self,
         train_ligands: List[str],
         train_proteins: List[str],
         train_labels: List[float],
+        **kwargs
     ):
         """Trains a BoWDTA model on the provided protein-ligand interactions.
         The biomolecules are represented as bag of their biomolecule words and a
         decision tree is used for affinity prediction.
 
         Parameters
         ----------
         train_ligands : List[str]
             SMILES strings of the training ligands.
         train_proteins : List[str]
             Amino-acid sequences of the training ligands.
         train_labels : List[float]
             Affinity scores of the training interactions.
         """    
-        tokenized_ligands = self.tokenize_ligands(train_ligands)
-        tokenized_proteins = self.tokenize_proteins(train_proteins)
+        tokenized_ligands = self.tokenize_ligands(train_ligands, self.vocab_size)
+        tokenized_proteins = self.tokenize_proteins(train_proteins, self.vocab_size)
         self.ligand_bow_vectorizer.fit_on_texts(tokenized_ligands)
         self.protein_bow_vectorizer.fit_on_texts(tokenized_proteins)
 
         ligand_vectors = self.vectorize_ligands(tokenized_ligands)
         protein_vectors = self.vectorize_proteins(tokenized_proteins)
+
+        if self.input_rank > 0:
+            R = self.input_rank
+            U, s, Vh = np.linalg.svd(ligand_vectors, full_matrices=False)
+            ligand_vectors = U[:, :R] @ np.diag(s[:R]) @ Vh[:R]
+            U, s, Vh = np.linalg.svd(protein_vectors, full_matrices=False)
+            protein_vectors  = U[:, :R] @ np.diag(s[:R]) @ Vh[:R]
+
         X_train = np.hstack([ligand_vectors, protein_vectors])
         self.prediction_model.fit(X_train, train_labels)
 
     def predict(
         self, ligands: List[str], proteins: List[str]
     ) -> List[float]:
         """Predicts the affinities of a list of protein-ligand pairs.
@@ -140,27 +192,25 @@
             Amino-acid sequences of the proteins.
 
         Returns
         -------
         List[float]
             Predicted affinities.
         """    
-        tokenized_ligands = self.tokenize_ligands(ligands)
-        tokenized_proteins = self.tokenize_proteins(proteins)
+        tokenized_ligands = self.tokenize_ligands(ligands, self.vocab_size)
+        tokenized_proteins = self.tokenize_proteins(proteins, self.vocab_size)
 
         ligand_vectors = self.vectorize_ligands(tokenized_ligands)
         protein_vectors = self.vectorize_proteins(tokenized_proteins)
 
         interaction = np.hstack([ligand_vectors, protein_vectors])
         return self.prediction_model.predict(interaction).tolist()
 
 
 if __name__ == "__main__":
 
     from pydebiaseddta.utils import load_sample_dta_data
 
-    train_ligands, train_proteins, train_labels = load_sample_dta_data(
-        mini=True
-    )["train"]
+    train_ligands, train_proteins, train_labels = load_sample_dta_data(mini=True, split="train")
     bowdta = BoWDTA()
     bowdta.train(train_ligands, train_proteins, train_labels)
     preds = bowdta.predict(train_ligands, train_proteins)
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/guides/iddta.py` & `pydebiaseddta-0.1.0/pydebiaseddta/guides/iddta.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,20 +7,40 @@
 
 
 def _list_to_numpy(lst):
     return np.array(lst).reshape(-1, 1)
 
 
 class IDDTA(Guide):
-    def __init__(self):
+    def __init__(self,
+                 max_depth=None,
+                 min_samples_split=2,
+                 min_samples_leaf=1,
+                 criterion="squared_error",
+                 **kwargs):
         """Constructor to create an IDDTA model.
         IDDTA represents the proteins and ligands with one-hot vectors of their identities
         and uses a decision tree for prediction. 
+
+        Parameters
+        ----------
+        max_depth : int, optional
+            Determines the maximum depth of the decision tree regressor.
+        min_samples_split : int, optional
+            Determines the minimum samples to split a leaf for the decision
+            tree regressor.
+        min_samples_leaf : int, optional
+            Determines the minimum samples a leaf can have for the decision
+            tree regressor.
+        criterion : str, optional
+            Criterion according to which the decision tree regressor will be trained.
         """
-        self.prediction_model = DecisionTreeRegressor()
+        self.prediction_model =  DecisionTreeRegressor(
+            max_depth=max_depth, min_samples_split=min_samples_split, min_samples_leaf=min_samples_leaf, criterion=criterion
+            )
         self.ligand_encoder = OneHotEncoder(handle_unknown="ignore")
         self.protein_encoder = OneHotEncoder(handle_unknown="ignore")
 
     def vectorize_ligands(self, ligands: List[str]) -> np.array:
         """Creates one-hot vectors of the ligands.
 
         Parameters
@@ -53,14 +73,15 @@
         return self.protein_encoder.transform(proteins).todense()
 
     def train(
         self,
         train_ligands: List[str],
         train_proteins: List[str],
         train_labels: List[float],
+        **kwargs
     ):
         """Trains the IDDTA model. IDDTA represents the biomolecules with 
         one-hot-encoding of their identities and applies decision tree for affinity prediction.
 
         Parameters
         ----------
         train_ligands : List[str]
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/predictors/bpedta.py` & `pydebiaseddta-0.1.0/pydebiaseddta/predictors/bpedta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import List
 import numpy as np
 from tensorflow.keras.layers import Conv1D, GlobalMaxPooling1D
 from tensorflow.keras.layers import Dense, Dropout, Concatenate
 from tensorflow.keras.layers import Input, Embedding
 from tensorflow.keras.models import Model
 from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.optimizers import SGD
 
 from .abstract_predictors import TFPredictor
 from ..sequence.word_identification import (
-    load_chemical_word_identifier,
+    load_ligand_word_identifier,
     load_protein_word_identifier,
 )
 from ..sequence.smiles_processing import (
     smiles_to_unichar_batch,
     load_smiles_to_unichar_encoding,
 )
 
@@ -25,25 +26,33 @@
         embedding_dim: int = 128,
         learning_rate: float = 0.001,
         batch_size: int = 256,
         n_epochs: int = 200,
         num_filters: int = 32,
         smi_filter_len: int = 4,
         prot_filter_len: int = 6,
+        early_stopping_metric: str = "mse",
+        early_stopping_metric_threshold: float = -1e6,
+        early_stopping_num_epochs: int = 0,
+        early_stopping_split: str = "train",
+        optimizer: str = "adam",
+        min_epochs: int = 0,
+        seed: int = 0,
+        **kwargs
     ):
         """Constructor to create a BPE-DTA instance.
         BPE-DTA segments SMILES strings of ligands and amino-acid sequences of proteins into biomolecule words,
         and applies three layers of convolutions to learn latent representations. 
         A fully-connected neural network with three layers is used afterwards to predict affinities.
 
         Parameters
         ----------
         max_smi_len : int, optional
-            Maximum number of chemical words in a SMILES string, by default 100. 
-            SMILES strings that contain more chemical words are truncated.
+            Maximum number of ligand words in a SMILES string, by default 100. 
+            SMILES strings that contain more ligand words are truncated.
         max_prot_len : int, optional
             Maximum number of protein words in an amino-acid sequence, by default 1000. 
             Amino-acid sequences that contain more proteins words are truncated.
         embedding_dim : int, optional
             The dimension of the biomolecule words, by default 128.
         learning_rate : float, optional
             Learning rate during optimization, by default 0.001.
@@ -53,37 +62,64 @@
             Number of epochs to train the model, by default 200.
         num_filters : int, optional
             Number of filters in the first convolution block. The next blocks use two and three times of this number, respectively. y default 32.
         smi_filter_len : int, optional
             Length of filters in the convolution blocks for ligands, by default 4.
         prot_filter_len : int, optional
             Length of filters in the convolution blocks for proteins, by default 6.
+        early_stopping_metric : str, optional
+            Metric for early stopping of the training. Available options are "mse", "rmse", "mae", "r2", "ci".
+        early_stopping_metric_threshold : float, optional
+            If the performance in the specified metric in the specified split 
+            fall below this value the training is stopped early. Available options are
+            "mse" and "mae". Set to a negative value by default with no effects.
+        early_stopping_num_epochs : int, optional
+            If this value is set > 0, then if the training has not been better than the
+            best recorded performance for this many epochs on the specified split, the
+            training is stopped early. Set to 0 by default with no effect.
+        early_stopping_split:
+            The split for conducting early stopping checks. Available options are "train"
+            and the keys in the val_split dictionary.
+        optimizer : str, optional
+            The optimizer used in training. Available options are "adam" and "sgd".
+        min_epochs : int, optional
+            Initial number of epochs for which the early stopping computations will be overrided.
+        seed : int, optional
+            Seed for the initialized model.
         """    
         self.max_smi_len = max_smi_len
         self.max_prot_len = max_prot_len
         self.embedding_dim = embedding_dim
         self.num_filters = num_filters
         self.smi_filter_len = smi_filter_len
         self.prot_filter_len = prot_filter_len
 
+        self.optimizer = optimizer
+        self.early_stopping_metric = early_stopping_metric
+        self.early_stopping_metric_threshold = early_stopping_metric_threshold
+        self.early_stopping_num_epochs = early_stopping_num_epochs
+        self.early_stopping_split = early_stopping_split
+        self.min_epochs = min_epochs
+
         self.chem_vocab_size = 8000
         self.prot_vocab_size = 32000
-        TFPredictor.__init__(self, n_epochs, learning_rate, batch_size)
+        TFPredictor.__init__(self, n_epochs, learning_rate, batch_size, seed=seed)
+
 
     def build(self) -> Model:
         """Builds a `BPEDTA` predictor in `keras` with the parameters specified during construction.
 
         Returns
         -------
         tensorflow.keras.models.Model
             The built model.
         """        
         # Inputs
         ligands = Input(shape=(self.max_smi_len,), dtype="int32")
-        # chemical representation
+        # ligand representation
         ligand_representation = Embedding(
             input_dim=self.chem_vocab_size + 1,
             output_dim=self.embedding_dim,
             input_length=self.max_smi_len,
             mask_zero=True,
         )(ligands)
         ligand_representation = Conv1D(
@@ -148,38 +184,43 @@
         FC1 = Dense(1024, activation="relu")(interaction_representation)
         FC1 = Dropout(0.1)(FC1)
         FC2 = Dense(1024, activation="relu")(FC1)
         FC2 = Dropout(0.1)(FC2)
         FC3 = Dense(512, activation="relu")(FC2)
         predictions = Dense(1, kernel_initializer="normal")(FC3)
 
-        opt = Adam(self.learning_rate)
+        if self.optimizer == "adam":
+            opt = Adam(self.learning_rate)
+        elif self.optimizer == "sgd":
+            opt = SGD(self.learning_rate)
+        else:
+            raise ValueError(f"The optimizer {self.optimizer} is not found.")
         bpedta = Model(inputs=[ligands, proteins], outputs=[predictions])
         bpedta.compile(
             optimizer=opt, loss="mean_squared_error", metrics=["mean_squared_error"],
         )
         return bpedta
 
     def vectorize_ligands(self, ligands: List[str]) -> np.array:
-        """Segments SMILES strings of ligands into chemical words and applies label encoding.
+        """Segments SMILES strings of ligands into ligand words and applies label encoding.
         Truncation and padding are also applied to prepare ligands for training and/or prediction.
 
         Parameters
         ----------
         ligands : List[str]
             The SMILES strings of ligands.
 
         Returns
         -------
         np.array
-            An $N \\times max\\_smi\\_len$ ($N$ is the number of the input ligands) matrix that contains label encoded sequences of chemical words.
+            An $N \\times max\\_smi\\_len$ ($N$ is the number of the input ligands) matrix that contains label encoded sequences of ligand words.
         """        
         smi_to_unichar_encoding = load_smiles_to_unichar_encoding()
         unichars = smiles_to_unichar_batch(ligands, smi_to_unichar_encoding)
-        word_identifier = load_chemical_word_identifier(vocab_size=8000)
+        word_identifier = load_ligand_word_identifier(vocab_size=8000)
 
         return np.array(word_identifier.encode_sequences(unichars, self.max_smi_len))
 
     def vectorize_proteins(self, aa_sequences: List[str]) -> np.array:
         """Segments amino-acid sequences of proteins into protein words and applies label encoding.
         Truncation and padding are also applied to prepare proteins for training and/or prediction.
 
@@ -198,12 +239,10 @@
             word_identifier.encode_sequences(aa_sequences, self.max_prot_len)
         )
 
 
 if __name__ == "__main__":
     from pydebiaseddta.utils import load_sample_dta_data
 
-    train_chemicals, train_proteins, train_labels = load_sample_dta_data(mini=True)[
-        "train"
-    ]
+    train_ligands, train_proteins, train_labels = load_sample_dta_data(mini=True, split="train")
     bpedta = BPEDTA(n_epochs=5)
-    bpedta.train(train_chemicals, train_proteins, train_labels)
+    bpedta.train(train_ligands, train_proteins, train_labels)
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/predictors/lmdta.py` & `pydebiaseddta-0.1.0/pydebiaseddta/predictors/lmdta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,115 @@
 import re
 from functools import lru_cache
 from typing import List
+import os
+os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 import numpy as np
 import transformers
 from tensorflow.keras.layers import Input, Concatenate, Dense, Dropout
 from tensorflow.keras.models import Model
-from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.optimizers import Adam, SGD
 from transformers import AutoTokenizer, AutoModel
 
 from .abstract_predictors import TFPredictor
 
 
 class LMDTA(TFPredictor):
     def __init__(
-        self, n_epochs: int = 200, learning_rate: float = 0.001, batch_size: int = 256
-    ):
+            self,
+            n_epochs: int = 200,
+            learning_rate: float = 0.001,
+            batch_size: int = 256,
+            early_stopping_metric: str = "mse",
+            early_stopping_metric_threshold: float = -1e6,
+            early_stopping_num_epochs: int = 0,
+            early_stopping_split: str = "train",
+            optimizer: str = "adam",
+            min_epochs: int = 0,
+            seed: int = 0,
+            **kwargs
+            ):
         """Constructor to create a LMDTA instance.
         LMDTA represents ligands and proteins with pre-trained language model embeddings
         obtained via [`ChemBERTa`](https://arxiv.org/abs/2010.09885) and  [`ProtBert`](https://www.biorxiv.org/content/biorxiv/early/2020/07/21/2020.07.12.199554.full.pdf) models, respectively. 
         A fully-connected neural network with two layers is used afterwards to predict affinities.
 
         Parameters
         ----------
         n_epochs : int, optional
             Number of epochs to train the model, by default 200.
         learning_rate : float, optional
             Learning rate during optimization, by default 0.001.
         batch_size : int, optional
              Batch size during training, by default 256.
+        early_stopping_metric : str, optional
+            Metric for early stopping of the training. Available options are "mse", "rmse", "mae", "r2", "ci".
+        early_stopping_metric_threshold : float, optional
+            If the performance in the specified metric in the specified split 
+            fall below this value the training is stopped early. Available options are
+            "mse" and "mae". Set to a negative value by default with no effects.
+        early_stopping_num_epochs : int, optional
+            If this value is set > 0, then if the training has not been better than the
+            best recorded performance for this many epochs on the specified split, the
+            training is stopped early. Set to 0 by default with no effect.
+        early_stopping_split:
+            The split for conducting early stopping checks. Available options are "train"
+            and the keys in the val_split dictionary.
+        optimizer : str, optional
+            The optimizer used in training. Available options are "adam" and "sgd".
+        min_epochs : int, optional
+            Initial number of epochs for which the early stopping computations will be overrided.
+        seed : int, optional
+            Seed for the initialized model.
         """
+        self.optimizer = optimizer
+        self.early_stopping_metric = early_stopping_metric
+        self.early_stopping_metric_threshold = early_stopping_metric_threshold
+        self.early_stopping_num_epochs = early_stopping_num_epochs
+        self.early_stopping_split = early_stopping_split
+        self.min_epochs = min_epochs
+
         transformers.logging.set_verbosity(transformers.logging.CRITICAL)
-        self.chemical_tokenizer = AutoTokenizer.from_pretrained(
+        self.ligand_tokenizer = AutoTokenizer.from_pretrained(
             "seyonec/PubChem10M_SMILES_BPE_450k"
         )
         self.chemberta = AutoModel.from_pretrained("seyonec/PubChem10M_SMILES_BPE_450k")
 
         self.protein_tokenizer = AutoTokenizer.from_pretrained(
             "Rostlab/prot_bert", do_lower_case=False
         )
         self.protbert = AutoModel.from_pretrained("Rostlab/prot_bert")
-        TFPredictor.__init__(self, n_epochs, learning_rate, batch_size)
+        TFPredictor.__init__(self, n_epochs, learning_rate, batch_size, seed=seed)
 
     def build(self):
         """Builds a `LMDTA` predictor in `keras` with the parameters specified during construction.
 
         Returns
         -------
         tensorflow.keras.models.Model
             The built model.
         """
-        chemicals = Input(shape=(768,), dtype="float32")
+        ligands = Input(shape=(768,), dtype="float32")
         proteins = Input(shape=(1024,), dtype="float32")
 
-        interaction_representation = Concatenate(axis=-1)([chemicals, proteins])
+        interaction_representation = Concatenate(axis=-1)([ligands, proteins])
 
         FC1 = Dense(1024, activation="relu")(interaction_representation)
         FC1 = Dropout(0.1)(FC1)
         FC2 = Dense(512, activation="relu")(FC1)
         predictions = Dense(1, kernel_initializer="normal")(FC2)
 
-        opt = Adam(self.learning_rate)
-        lmdta = Model(inputs=[chemicals, proteins], outputs=[predictions])
+        if self.optimizer == "adam":
+            opt = Adam(self.learning_rate)
+        elif self.optimizer == "sgd":
+            opt = SGD(self.learning_rate)
+        else:
+            raise ValueError(f"The optimizer {self.optimizer} is not found.")
+        lmdta = Model(inputs=[ligands, proteins], outputs=[predictions])
         lmdta.compile(
             optimizer=opt, loss="mean_squared_error", metrics=["mean_squared_error"]
         )
         return lmdta
 
     @lru_cache(maxsize=2048)
     def get_chemberta_embedding(self, smiles: str) -> np.array:
@@ -78,15 +122,15 @@
             SMILES string of the ligand.
 
         Returns
         -------
         np.array
             [`ChemBERTa`](https://arxiv.org/abs/2010.09885) vector (768-dimensional) of the ligand.
         """        
-        tokens = self.chemical_tokenizer(smiles, return_tensors="pt")
+        tokens = self.ligand_tokenizer(smiles, return_tensors="pt")
         output = self.chemberta(**tokens)
         return output.last_hidden_state.detach().numpy().mean(axis=1)
 
     def vectorize_ligands(self, ligands: List[str]) -> np.array:
         """Vectorizes the ligands with [`ChemBERTa`](https://arxiv.org/abs/2010.09885) embeddings.
 
         Parameters
@@ -96,15 +140,15 @@
 
         Returns
         -------
         np.array
             An $N \\times 768$ ($N$ is the number of the input ligands) matrix that contains [`ChemBERTa`](https://arxiv.org/abs/2010.09885) vectors of the ligands.
         """        
         return np.vstack(
-            [self.get_chemberta_embedding(chemical) for chemical in ligands]
+            [self.get_chemberta_embedding(ligand) for ligand in ligands]
         )
 
     @lru_cache(maxsize=1024)
     def get_protbert_embedding(self, aa_sequence: str) -> np.array:
         """Computes the [`ProtBert`](https://www.biorxiv.org/content/biorxiv/early/2020/07/21/2020.07.12.199554.full.pdf) vector for a protein. 
         Since the creating the vector is computation-heavy, an `lru_cache` of size 2048 is used to store produced vectors.
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/sequence/smiles_processing.py` & `pydebiaseddta-0.1.0/pydebiaseddta/sequence/smiles_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if token not in source_to_target_mapping:
             source_to_target_mapping[token] = remainings.pop()
     return source_to_target_mapping
 
 
 def load_smiles_to_unichar_encoding() -> Dict[str, str]:
     return load_json(
-        f"{package_path}/data/word_identification/chemical/chembl27_encoding.json"
+        f"{package_path}/data/word_identification/ligand/chembl27_encoding.json"
     )
 
 
 def load_unichar_to_smiles_encoding() -> Dict[str, str]:
     smi_to_unichar_encoding = load_smiles_to_unichar_encoding()
     return {v: k for k, v in smi_to_unichar_encoding.items()}
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta/sequence/word_identification.py` & `pydebiaseddta-0.1.0/pydebiaseddta/sequence/word_identification.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             The path to dump the instance. File extension is added automatically.
         """        
         if not savepath.endswith(FILE_EXTENSION):
             savepath = savepath + FILE_EXTENSION
         save_json(json.loads(self.tokenizer.to_str()), savepath)
 
 
-def load_chemical_word_identifier(vocab_size: int) -> WordIdentifier:
+def load_ligand_word_identifier(vocab_size: int) -> WordIdentifier:
     """A convenience function to load word vocabularies learned for SMILES strings in the study.
     The possible vocabularies to load are for DeepDTA and BPE-DTA. 
 
     Parameters
     ----------
     vocab_size : int
         Size of the learned SMILES word vocabulary. The allowed values are 94 and 8000, for DeepDTA and BPE-DTA, respectively.
@@ -142,18 +142,18 @@
     ------
     ValueError
         If vocabulary size besides 94 and 8000 is passed, a `ValueError` is raised.
     """    
     if vocab_size not in [94, 8000]:
         raise ValueError("Supported vocab sizes are 94 and 8000")
 
-    protein_vocab_path = f"{package_path}/data/word_identification/chemical"
-    vocab_path = f"{protein_vocab_path}/chembl27_enc_94.json"
+    ligand_vocab_path = f"{package_path}/data/word_identification/ligand"
+    vocab_path = f"{ligand_vocab_path}/chembl27_enc_94.json"
     if vocab_size == 8000:
-        vocab_path = f"{protein_vocab_path}/chembl27_enc_bpe_8000.json"
+        vocab_path = f"{ligand_vocab_path}/chembl27_enc_bpe_8000.json"
 
     return WordIdentifier.from_file(vocab_path)
 
 
 def load_protein_word_identifier(vocab_size: int)-> WordIdentifier:
     """A convenience function to load word vocabularies learned for amino-acid sequences in the study.
     The possible vocabularies to load are for DeepDTA and BPE-DTA. 
@@ -195,18 +195,18 @@
 
     merged = ["".join(seq) for seq in tok_seqs]
     stripped = [seq.strip() for seq in sequences]
     if merged != stripped:
         raise ValueError("Tokenization broke the sequences")
 
     word_identifier.save(
-        f"{package_path}/data/word_identification/chemical_mini_test.json"
+        f"{package_path}/data/word_identification/ligand_mini_test.json"
     )
     loaded_identifier = WordIdentifier.from_file(
-        f"{package_path}/data/word_identification/chemical_mini_test.json"
+        f"{package_path}/data/word_identification/ligand_mini_test.json"
     )
 
     is_save_load_ok = (
         word_identifier.tokenizer.to_str()
         == loaded_identifier.tokenizer.to_str()
         and word_identifier.vocab_size == loaded_identifier.vocab_size
     )
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta.egg-info/PKG-INFO` & `pydebiaseddta-0.1.0/pydebiaseddta.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydebiaseddta
-Version: 0.0.5
+Version: 0.1.0
 Summary: Python library to improve generalizability of the drug-target prediction models via DebiasedDTA
 Author-email: Rıza Özçelik <riza.ozcelik@boun.edu.tr>
-License: Copyright (c) 2018 The Python Packaging Authority
+License: Copyright (c) 2023 Rıza Özçelik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `pydebiaseddta-0.0.5/pydebiaseddta.egg-info/SOURCES.txt` & `pydebiaseddta-0.1.0/pydebiaseddta.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 pydebiaseddta/__init__.py
 pydebiaseddta/evaluation.py
 pydebiaseddta/utils.py
+pydebiaseddta/visualization.py
 pydebiaseddta.egg-info/PKG-INFO
 pydebiaseddta.egg-info/SOURCES.txt
 pydebiaseddta.egg-info/dependency_links.txt
 pydebiaseddta.egg-info/requires.txt
 pydebiaseddta.egg-info/top_level.txt
-pydebiaseddta/data/dta/dta_sample_data.json
-pydebiaseddta/data/dta/dta_sample_data.mini.json
+pydebiaseddta/data/dta/dta_sample_sw_sim_matrix.csv
+pydebiaseddta/data/dta/dta_sample_data/test.csv
+pydebiaseddta/data/dta/dta_sample_data/train.csv
+pydebiaseddta/data/dta/dta_sample_data/val.csv
+pydebiaseddta/data/dta/dta_sample_data_mini/test.csv
+pydebiaseddta/data/dta/dta_sample_data_mini/train.csv
+pydebiaseddta/data/dta/dta_sample_data_mini/val.csv
 pydebiaseddta/data/sequence/chembl27.mini.smiles
-pydebiaseddta/data/word_identification/chemical_mini_test.json
-pydebiaseddta/data/word_identification/chemical/chembl27_enc_94.json
-pydebiaseddta/data/word_identification/chemical/chembl27_enc_bpe_8000.json
-pydebiaseddta/data/word_identification/chemical/chembl27_encoding.json
+pydebiaseddta/data/word_identification/ligand_mini_test.json
+pydebiaseddta/data/word_identification/ligand/chembl27_enc_94.json
+pydebiaseddta/data/word_identification/ligand/chembl27_enc_bpe_8000.json
+pydebiaseddta/data/word_identification/ligand/chembl27_encoding.json
 pydebiaseddta/data/word_identification/protein/uniprot_26.json
 pydebiaseddta/data/word_identification/protein/uniprot_bpe_32000.json
 pydebiaseddta/debiasing/__init__.py
 pydebiaseddta/debiasing/debiaseddta.py
 pydebiaseddta/guides/__init__.py
 pydebiaseddta/guides/abstract_guide.py
 pydebiaseddta/guides/bowdta.py
 pydebiaseddta/guides/iddta.py
+pydebiaseddta/guides/outdta.py
+pydebiaseddta/guides/rfdta.py
 pydebiaseddta/predictors/__init__.py
 pydebiaseddta/predictors/abstract_predictors.py
 pydebiaseddta/predictors/bpedta.py
 pydebiaseddta/predictors/deepdta.py
 pydebiaseddta/predictors/lmdta.py
 pydebiaseddta/sequence/__init__.py
 pydebiaseddta/sequence/smiles_processing.py
```

### Comparing `pydebiaseddta-0.0.5/pyproject.toml` & `pydebiaseddta-0.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 [project]
 name = "pydebiaseddta"
-version="0.0.5"
+version="0.1.0"
 authors = [
     {name = "Rıza Özçelik", email = "riza.ozcelik@boun.edu.tr"}
 ]
 description = "Python library to improve generalizability of the drug-target prediction models via DebiasedDTA"
 readme = "README.rst"
 license= { file="LICENSE"}
 requires-python = ">=3.9.7"
 dependencies = [
     "numpy==1.21.2",
     "scikit_learn==1.1.1",
     "tensorflow==2.7.0",
     "tokenizers==0.10.3",
-    "transformers==4.14.1",
+    "transformers==4.4.0",
+    "pandas==1.4.4",
+    "ipykernel==6.15.2",
+    "protobuf==3.20.0",
+    "packaging==21.3",
+    "rdkit==2022.09.5",
+    "matplotlib==3.5.2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
```

