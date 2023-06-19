# Comparing `tmp/deepchem-2.7.2.dev20230619133526.tar.gz` & `tmp/deepchem-2.7.2.dev20230619133609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230619133526.tar", last modified: Mon Jun 19 13:35:26 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230619133609.tar", last modified: Mon Jun 19 13:36:09 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230619133526.tar` & `deepchem-2.7.2.dev20230619133609.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.619757 deepchem-2.7.2.dev20230619133526/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-06-19 13:35:12.000000 deepchem-2.7.2.dev20230619133526/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-19 13:35:26.619757 deepchem-2.7.2.dev20230619133526/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-19 13:35:12.000000 deepchem-2.7.2.dev20230619133526/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.587756 deepchem-2.7.2.dev20230619133526/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.587756 deepchem-2.7.2.dev20230619133526/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.587756 deepchem-2.7.2.dev20230619133526/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.591756 deepchem-2.7.2.dev20230619133526/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.591756 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.591756 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.595757 deepchem-2.7.2.dev20230619133526/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.599757 deepchem-2.7.2.dev20230619133526/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.603757 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   115619 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.607757 deepchem-2.7.2.dev20230619133526/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.611757 deepchem-2.7.2.dev20230619133526/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.615757 deepchem-2.7.2.dev20230619133526/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.619757 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:26.587756 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-19 13:35:26.000000 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-19 13:35:26.000000 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:35:26.000000 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 13:35:26.000000 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:35:26.000000 deepchem-2.7.2.dev20230619133526/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 13:35:26.619757 deepchem-2.7.2.dev20230619133526/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-19 13:35:13.000000 deepchem-2.7.2.dev20230619133526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.531857 deepchem-2.7.2.dev20230619133609/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-06-19 13:35:53.000000 deepchem-2.7.2.dev20230619133609/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-19 13:36:09.531857 deepchem-2.7.2.dev20230619133609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-19 13:35:53.000000 deepchem-2.7.2.dev20230619133609/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.503855 deepchem-2.7.2.dev20230619133609/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.511856 deepchem-2.7.2.dev20230619133609/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.515856 deepchem-2.7.2.dev20230619133609/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.515856 deepchem-2.7.2.dev20230619133609/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.515856 deepchem-2.7.2.dev20230619133609/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.515856 deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.519856 deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.519856 deepchem-2.7.2.dev20230619133609/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.519856 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.523856 deepchem-2.7.2.dev20230619133609/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.527857 deepchem-2.7.2.dev20230619133609/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.531857 deepchem-2.7.2.dev20230619133609/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.531857 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:36:09.507856 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-19 13:36:09.000000 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-19 13:36:09.000000 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:36:09.000000 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 13:36:09.000000 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:36:09.000000 deepchem-2.7.2.dev20230619133609/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 13:36:09.535857 deepchem-2.7.2.dev20230619133609/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-19 13:35:54.000000 deepchem-2.7.2.dev20230619133609/setup.py
```

### Comparing `deepchem-2.7.2.dev20230619133526/LICENSE` & `deepchem-2.7.2.dev20230619133609/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/PKG-INFO` & `deepchem-2.7.2.dev20230619133609/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230619133526
+Version: 2.7.2.dev20230619133609
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230619133526/README.md` & `deepchem-2.7.2.dev20230619133609/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230619133609/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230619133609/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230619133609/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230619133609/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230619133609/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230619133609/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230619133609/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230619133609/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230619133609/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230619133609/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230619133609/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230619133609/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230619133609/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230619133609/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230619133609/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/models.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7220,8 +7220,193 @@
 0001c330: 7220 7573 696e 6720 7468 6520 6d61 736b  r using the mask
 0001c340: 730a 2020 2020 2020 2020 7061 7274 6974  s.        partit
 0001c350: 696f 6e73 203d 205b 696e 7075 745f 7465  ions = [input_te
 0001c360: 6e73 6f72 5b6d 6173 6b5d 2066 6f72 206d  nsor[mask] for m
 0001c370: 6173 6b20 696e 2070 6172 7469 7469 6f6e  ask in partition
 0001c380: 5f6d 6173 6b73 5d0a 0a20 2020 2020 2020  _masks]..       
 0001c390: 2072 6574 7572 6e20 7061 7274 6974 696f   return partitio
-0001c3a0: 6e73 0a                                  ns.
+0001c3a0: 6e73 0a0a 0a63 6c61 7373 2044 544e 4e45  ns...class DTNNE
+0001c3b0: 6d62 6564 6469 6e67 286e 6e2e 4d6f 6475  mbedding(nn.Modu
+0001c3c0: 6c65 293a 0a20 2020 2022 2222 4454 4e4e  le):.    """DTNN
+0001c3d0: 456d 6265 6464 696e 6720 6c61 7965 7220  Embedding layer 
+0001c3e0: 666f 7220 4454 4e4e 206d 6f64 656c 2e0a  for DTNN model..
+0001c3f0: 0a20 2020 2041 7373 6967 6e20 696e 6974  .    Assign init
+0001c400: 6961 6c20 6174 6f6d 6963 2064 6573 6372  ial atomic descr
+0001c410: 6970 746f 7273 2e20 5b31 5d5f 0a0a 2020  iptors. [1]_..  
+0001c420: 2020 5468 6973 206c 6179 6572 2063 7265    This layer cre
+0001c430: 6174 6573 2027 6e27 206e 756d 6265 7220  ates 'n' number 
+0001c440: 6f66 2065 6d62 6564 6469 6e67 7320 6173  of embeddings as
+0001c450: 2069 6e69 7469 616c 2061 746f 6d69 6320   initial atomic 
+0001c460: 6465 7363 7269 7074 6f72 732e 2041 6363  descriptors. Acc
+0001c470: 6f72 6469 6e67 2074 6f20 7468 6520 7265  ording to the re
+0001c480: 7175 6972 6564 2077 6569 6768 7420 696e  quired weight in
+0001c490: 6974 6961 6c69 7a65 7220 616e 6420 7065  itializer and pe
+0001c4a0: 7269 6f64 6963 5f74 6162 6c65 5f6c 656e  riodic_table_len
+0001c4b0: 6774 6820 2854 6f74 616c 206e 756d 6265  gth (Total numbe
+0001c4c0: 7220 6f66 2075 6e69 7175 6520 6174 6f6d  r of unique atom
+0001c4d0: 7329 2e0a 0a20 2020 2052 6566 6572 656e  s)...    Referen
+0001c4e0: 6365 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ces.    --------
+0001c4f0: 2d2d 0a20 2020 205b 315d 2053 6368 c3bc  --.    [1] Sch..
+0001c500: 7474 2c20 4b72 6973 746f 6620 542e 2c20  tt, Kristof T., 
+0001c510: 6574 2061 6c2e 2022 5175 616e 7475 6d2d  et al. "Quantum-
+0001c520: 6368 656d 6963 616c 2069 6e73 6967 6874  chemical insight
+0001c530: 7320 6672 6f6d 2064 6565 700a 2020 2020  s from deep.    
+0001c540: 2020 2020 7465 6e73 6f72 206e 6575 7261      tensor neura
+0001c550: 6c20 6e65 7477 6f72 6b73 2e22 204e 6174  l networks." Nat
+0001c560: 7572 6520 636f 6d6d 756e 6963 6174 696f  ure communicatio
+0001c570: 6e73 2038 2e31 2028 3230 3137 293a 2031  ns 8.1 (2017): 1
+0001c580: 2d38 2e0a 0a20 2020 2050 6172 616d 6574  -8...    Paramet
+0001c590: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+0001c5a0: 2d2d 0a20 2020 206e 5f65 6d62 6564 6469  --.    n_embeddi
+0001c5b0: 6e67 3a20 696e 742c 206f 7074 696f 6e61  ng: int, optiona
+0001c5c0: 6c0a 2020 2020 2020 2020 4e75 6d62 6572  l.        Number
+0001c5d0: 206f 6620 6665 6174 7572 6573 2066 6f72   of features for
+0001c5e0: 2065 6163 6820 6174 6f6d 0a20 2020 2070   each atom.    p
+0001c5f0: 6572 696f 6469 635f 7461 626c 655f 6c65  eriodic_table_le
+0001c600: 6e67 7468 3a20 696e 742c 206f 7074 696f  ngth: int, optio
+0001c610: 6e61 6c0a 2020 2020 2020 2020 4c65 6e67  nal.        Leng
+0001c620: 7468 206f 6620 656d 6265 6464 696e 672c  th of embedding,
+0001c630: 2038 333d 4269 0a20 2020 2069 6e69 7461   83=Bi.    inita
+0001c640: 6c69 7a65 723a 2073 7472 2c20 6f70 7469  lizer: str, opti
+0001c650: 6f6e 616c 0a20 2020 2020 2020 2057 6569  onal.        Wei
+0001c660: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
+0001c670: 6f6e 2066 6f72 2066 696c 7465 7273 2e0a  on for filters..
+0001c680: 2020 2020 2020 2020 4f70 7469 6f6e 733a          Options:
+0001c690: 207b 7861 7669 6572 5f75 6e69 666f 726d   {xavier_uniform
+0001c6a0: 5f2c 2078 6176 6965 725f 6e6f 726d 616c  _, xavier_normal
+0001c6b0: 5f2c 206b 6169 6d69 6e67 5f75 6e69 666f  _, kaiming_unifo
+0001c6c0: 726d 5f2c 206b 6169 6d69 6e67 5f6e 6f72  rm_, kaiming_nor
+0001c6d0: 6d61 6c5f 2c20 7472 756e 635f 6e6f 726d  mal_, trunc_norm
+0001c6e0: 616c 5f7d 0a0a 2020 2020 4578 616d 706c  al_}..    Exampl
+0001c6f0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001c700: 2020 2020 3e3e 3e20 6672 6f6d 2064 6565      >>> from dee
+0001c710: 7063 6865 6d2e 6d6f 6465 6c73 2e74 6f72  pchem.models.tor
+0001c720: 6368 5f6d 6f64 656c 7320 696d 706f 7274  ch_models import
+0001c730: 206c 6179 6572 730a 2020 2020 3e3e 3e20   layers.    >>> 
+0001c740: 696d 706f 7274 2074 6f72 6368 0a20 2020  import torch.   
+0001c750: 203e 3e3e 206c 6179 6572 203d 206c 6179   >>> layer = lay
+0001c760: 6572 732e 4454 4e4e 456d 6265 6464 696e  ers.DTNNEmbeddin
+0001c770: 6728 3330 2c20 3330 2c20 2778 6176 6965  g(30, 30, 'xavie
+0001c780: 725f 756e 6966 6f72 6d5f 2729 0a20 2020  r_uniform_').   
+0001c790: 203e 3e3e 206f 7574 7075 7420 3d20 6c61   >>> output = la
+0001c7a0: 7965 7228 746f 7263 682e 7465 6e73 6f72  yer(torch.tensor
+0001c7b0: 285b 302c 2031 2c20 322c 2033 2c20 342c  ([0, 1, 2, 3, 4,
+0001c7c0: 2035 2c20 362c 2037 2c20 382c 2039 5d29   5, 6, 7, 8, 9])
+0001c7d0: 290a 2020 2020 3e3e 3e20 6f75 7470 7574  ).    >>> output
+0001c7e0: 2e73 6861 7065 0a20 2020 2074 6f72 6368  .shape.    torch
+0001c7f0: 2e53 697a 6528 5b31 302c 2033 305d 290a  .Size([10, 30]).
+0001c800: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+0001c810: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0001c820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c830: 2020 6e5f 656d 6265 6464 696e 673a 2069    n_embedding: i
+0001c840: 6e74 203d 2033 302c 0a20 2020 2020 2020  nt = 30,.       
+0001c850: 2020 2020 2020 2020 2020 7065 7269 6f64            period
+0001c860: 6963 5f74 6162 6c65 5f6c 656e 6774 683a  ic_table_length:
+0001c870: 2069 6e74 203d 2033 302c 0a20 2020 2020   int = 30,.     
+0001c880: 2020 2020 2020 2020 2020 2020 696e 6974              init
+0001c890: 616c 697a 6572 3a20 7374 7220 3d20 2778  alizer: str = 'x
+0001c8a0: 6176 6965 725f 756e 6966 6f72 6d5f 272c  avier_uniform_',
+0001c8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c8c0: 2020 2a2a 6b77 6172 6773 293a 0a0a 2020    **kwargs):..  
+0001c8d0: 2020 2020 2020 7375 7065 7228 4454 4e4e        super(DTNN
+0001c8e0: 456d 6265 6464 696e 672c 2073 656c 6629  Embedding, self)
+0001c8f0: 2e5f 5f69 6e69 745f 5f28 2a2a 6b77 6172  .__init__(**kwar
+0001c900: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
+0001c910: 2e6e 5f65 6d62 6564 6469 6e67 203d 206e  .n_embedding = n
+0001c920: 5f65 6d62 6564 6469 6e67 0a20 2020 2020  _embedding.     
+0001c930: 2020 2073 656c 662e 7065 7269 6f64 6963     self.periodic
+0001c940: 5f74 6162 6c65 5f6c 656e 6774 6820 3d20  _table_length = 
+0001c950: 7065 7269 6f64 6963 5f74 6162 6c65 5f6c  periodic_table_l
+0001c960: 656e 6774 680a 2020 2020 2020 2020 7365  ength.        se
+0001c970: 6c66 2e69 6e69 7461 6c69 7a65 7220 3d20  lf.initalizer = 
+0001c980: 696e 6974 616c 697a 6572 2020 2320 5365  initalizer  # Se
+0001c990: 7420 7765 6967 6874 2069 6e69 7469 616c  t weight initial
+0001c9a0: 697a 6174 696f 6e0a 0a20 2020 2020 2020  ization..       
+0001c9b0: 2069 6e69 745f 6675 6e63 3a20 4361 6c6c   init_func: Call
+0001c9c0: 6162 6c65 203d 2067 6574 6174 7472 2869  able = getattr(i
+0001c9d0: 6e69 7469 616c 697a 6572 732c 2073 656c  nitializers, sel
+0001c9e0: 662e 696e 6974 616c 697a 6572 290a 2020  f.initalizer).  
+0001c9f0: 2020 2020 2020 7365 6c66 2e65 6d62 6564        self.embed
+0001ca00: 6469 6e67 5f6c 6973 743a 2074 6f72 6368  ding_list: torch
+0001ca10: 2e54 656e 736f 7220 3d20 696e 6974 5f66  .Tensor = init_f
+0001ca20: 756e 6328 0a20 2020 2020 2020 2020 2020  unc(.           
+0001ca30: 2074 6f72 6368 2e65 6d70 7479 285b 7365   torch.empty([se
+0001ca40: 6c66 2e70 6572 696f 6469 635f 7461 626c  lf.periodic_tabl
+0001ca50: 655f 6c65 6e67 7468 2c20 7365 6c66 2e6e  e_length, self.n
+0001ca60: 5f65 6d62 6564 6469 6e67 5d29 290a 0a20  _embedding])).. 
+0001ca70: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+0001ca80: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0001ca90: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
+0001caa0: 2061 2073 7472 696e 6720 7265 7072 6573   a string repres
+0001cab0: 656e 7469 6e67 2074 6865 2063 6f6e 6669  enting the confi
+0001cac0: 6775 7261 7469 6f6e 206f 6620 7468 6520  guration of the 
+0001cad0: 6c61 7965 722e 0a0a 2020 2020 2020 2020  layer...        
+0001cae0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0001caf0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001cb00: 6e5f 656d 6265 6464 696e 673a 2069 6e74  n_embedding: int
+0001cb10: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001cb20: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+0001cb30: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
+0001cb40: 6368 2061 746f 6d0a 2020 2020 2020 2020  ch atom.        
+0001cb50: 7065 7269 6f64 6963 5f74 6162 6c65 5f6c  periodic_table_l
+0001cb60: 656e 6774 683a 2069 6e74 2c20 6f70 7469  ength: int, opti
+0001cb70: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0001cb80: 204c 656e 6774 6820 6f66 2065 6d62 6564   Length of embed
+0001cb90: 6469 6e67 2c20 3833 3d42 690a 2020 2020  ding, 83=Bi.    
+0001cba0: 2020 2020 696e 6974 616c 697a 6572 3a20      initalizer: 
+0001cbb0: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+0001cbc0: 2020 2020 2020 2020 2020 5765 6967 6874            Weight
+0001cbd0: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
+0001cbe0: 666f 7220 6669 6c74 6572 732e 0a20 2020  for filters..   
+0001cbf0: 2020 2020 2020 2020 204f 7074 696f 6e73           Options
+0001cc00: 3a20 7b78 6176 6965 725f 756e 6966 6f72  : {xavier_unifor
+0001cc10: 6d5f 2c20 7861 7669 6572 5f6e 6f72 6d61  m_, xavier_norma
+0001cc20: 6c5f 2c20 6b61 696d 696e 675f 756e 6966  l_, kaiming_unif
+0001cc30: 6f72 6d5f 2c20 6b61 696d 696e 675f 6e6f  orm_, kaiming_no
+0001cc40: 726d 616c 5f2c 2074 7275 6e63 5f6e 6f72  rmal_, trunc_nor
+0001cc50: 6d61 6c5f 7d0a 0a20 2020 2020 2020 2022  mal_}..        "
+0001cc60: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0001cc70: 6e20 6627 7b73 656c 662e 5f5f 636c 6173  n f'{self.__clas
+0001cc80: 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f  s__.__name__}(n_
+0001cc90: 656d 6265 6464 696e 673d 7b73 656c 662e  embedding={self.
+0001cca0: 6e5f 656d 6265 6464 696e 677d 2c20 7065  n_embedding}, pe
+0001ccb0: 7269 6f64 6963 5f74 6162 6c65 5f6c 656e  riodic_table_len
+0001ccc0: 6774 683d 7b73 656c 662e 7065 7269 6f64  gth={self.period
+0001ccd0: 6963 5f74 6162 6c65 5f6c 656e 6774 687d  ic_table_length}
+0001cce0: 2c20 696e 6974 616c 697a 6572 3d7b 7365  , initalizer={se
+0001ccf0: 6c66 2e69 6e69 7461 6c69 7a65 727d 2927  lf.initalizer})'
+0001cd00: 0a0a 2020 2020 6465 6620 666f 7277 6172  ..    def forwar
+0001cd10: 6428 7365 6c66 2c20 696e 7075 7473 3a20  d(self, inputs: 
+0001cd20: 746f 7263 682e 5465 6e73 6f72 293a 0a20  torch.Tensor):. 
+0001cd30: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0001cd40: 7320 456d 6265 6464 696e 6773 2061 6363  s Embeddings acc
+0001cd50: 6f72 6469 6e67 2074 6f20 696e 6469 6365  ording to indice
+0001cd60: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
+0001cd70: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0001cd80: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0001cd90: 2020 696e 7075 7473 3a20 746f 7263 682e    inputs: torch.
+0001cda0: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
+0001cdb0: 2020 2049 6e64 6963 6573 206f 6620 4174     Indices of At
+0001cdc0: 6f6d 7320 7768 6f73 6520 656d 6265 6464  oms whose embedd
+0001cdd0: 696e 6773 2061 7265 2072 6571 7565 7374  ings are request
+0001cde0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+0001cdf0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0001ce00: 2d2d 2d2d 0a20 2020 2020 2020 2061 746f  ----.        ato
+0001ce10: 6d5f 656d 6265 6464 696e 6773 3a20 746f  m_embeddings: to
+0001ce20: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+0001ce30: 2020 2020 2020 2045 6d62 6564 6469 6e67         Embedding
+0001ce40: 7320 6f66 2061 746f 6d73 2061 6363 6f72  s of atoms accor
+0001ce50: 6469 6e67 7320 746f 2069 6e64 6963 6573  dings to indices
+0001ce60: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+0001ce70: 2020 2020 2020 2061 746f 6d5f 6e75 6d62         atom_numb
+0001ce80: 6572 203d 2069 6e70 7574 730a 2020 2020  er = inputs.    
+0001ce90: 2020 2020 6174 6f6d 5f65 6e62 6564 6469      atom_enbeddi
+0001cea0: 6e67 7320 3d20 746f 7263 682e 6e6e 2e66  ngs = torch.nn.f
+0001ceb0: 756e 6374 696f 6e61 6c2e 656d 6265 6464  unctional.embedd
+0001cec0: 696e 6728 6174 6f6d 5f6e 756d 6265 722c  ing(atom_number,
+0001ced0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf00: 2020 2020 2020 2020 2073 656c 662e 656d           self.em
+0001cf10: 6265 6464 696e 675f 6c69 7374 290a 2020  bedding_list).  
+0001cf20: 2020 2020 2020 7265 7475 726e 2061 746f        return ato
+0001cf30: 6d5f 656e 6265 6464 696e 6773 0a         m_enbeddings.
```

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230619133609/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230619133609/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230619133609/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230619133609/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230619133609/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230619133609/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230619133609/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230619133609/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230619133609/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230619133609/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230619133526
+Version: 2.7.2.dev20230619133609
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230619133526/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230619133609/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/setup.cfg` & `deepchem-2.7.2.dev20230619133609/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230619133526/setup.py` & `deepchem-2.7.2.dev20230619133609/setup.py`

 * *Files identical despite different names*

