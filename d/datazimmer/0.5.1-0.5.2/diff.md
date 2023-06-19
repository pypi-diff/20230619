# Comparing `tmp/datazimmer-0.5.1.tar.gz` & `tmp/datazimmer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazimmer-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "datazimmer-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datazimmer-0.5.1.tar` & `datazimmer-0.5.2.tar`

### file list

```diff
@@ -1,148 +1,149 @@
--rw-r--r--   0        0        0     1003 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/compatibility_test.yml
--rw-r--r--   0        0        0     1299 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1795 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.gitignore
--rw-r--r--   0        0        0      288 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      491 2023-06-18 14:15:24.928776 datazimmer-0.5.1/CITATION.cff
--rw-r--r--   0        0        0     1077 2023-06-18 14:15:24.928776 datazimmer-0.5.1/LICENSE
--rw-r--r--   0        0        0     3122 2023-06-18 14:15:24.928776 datazimmer-0.5.1/README.md
--rw-r--r--   0        0        0     4074 2023-06-18 14:15:24.928776 datazimmer-0.5.1/conftest.py
--rw-r--r--   0        0        0      634 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/aswan_integration.py
--rw-r--r--   0        0        0     7923 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/config_loading.py
--rw-r--r--   0        0        0     2112 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/dvc_util.py
--rw-r--r--   0        0        0      144 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/exceptions.py
--rw-r--r--   0        0        0      624 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/get_runtime.py
--rw-r--r--   0        0        0     2434 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/gh_actions.py
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/__init__.py
--rw-r--r--   0        0        0     6235 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/atoms.py
--rw-r--r--   0        0        0     1422 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/complete_id.py
--rw-r--r--   0        0        0     1744 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/datascript.py
--rw-r--r--   0        0        0     4537 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/high_level.py
--rw-r--r--   0        0        0     4798 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/scrutable.py
--rw-r--r--   0        0        0     3456 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/naming.py
--rw-r--r--   0        0        0      526 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/persistent_state.py
--rw-r--r--   0        0        0     8463 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/pipeline_element.py
--rw-r--r--   0        0        0     7648 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/project_runtime.py
--rw-r--r--   0        0        0      935 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/raw_data.py
--rw-r--r--   0        0        0     6177 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/registry.py
--rw-r--r--   0        0        0      863 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/reporting.py
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/__init__.py
--rw-r--r--   0        0        0       87 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/draw.py
--rw-r--r--   0        0        0     9259 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/loader.py
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/__init__.py
--rw-r--r--   0        0        0     4692 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/create_dogshow.py
--rw-r--r--   0        0        0      845 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_commands.py
--rw-r--r--   0        0        0      346 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_config.py
--rw-r--r--   0        0        0     4366 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_full_integration.py
--rw-r--r--   0        0        0      465 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_registry.py
--rw-r--r--   0        0        0      294 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_runtime.py
--rw-r--r--   0        0        0     1799 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_scrutable.py
--rw-r--r--   0        0        0      152 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_sql.py
--rw-r--r--   0        0        0      235 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_util.py
--rw-r--r--   0        0        0      943 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_validation.py
--rw-r--r--   0        0        0      939 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/util.py
--rw-r--r--   0        0        0    10109 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/typer_commands.py
--rw-r--r--   0        0        0     3260 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/utils.py
--rw-r--r--   0        0        0     2957 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/validation_functions.py
--rw-r--r--   0        0        0    10327 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/zenodo.py
--rw-r--r--   0        0        0      114 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.AbstractEntity.rst
--rw-r--r--   0        0        0      123 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.CompositeTypeBase.rst
--rw-r--r--   0        0        0      746 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.DzAswan.rst
--rw-r--r--   0        0        0      739 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.EntityClass.rst
--rw-r--r--   0        0        0       87 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.Index.rst
--rw-r--r--   0        0        0       96 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.Nullable.rst
--rw-r--r--   0        0        0      444 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.PersistentState.rst
--rw-r--r--   0        0        0      592 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.ReportFile.rst
--rw-r--r--   0        0        0      565 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.ScruTable.rst
--rw-r--r--   0        0        0       99 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.SourceUrl.rst
--rw-r--r--   0        0        0      107 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.dump_dfs_to_tables.rst
--rw-r--r--   0        0        0      104 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.get_raw_data_path.rst
--rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.parse_df.rst
--rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register.rst
--rw-r--r--   0        0        0      113 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register_data_loader.rst
--rw-r--r--   0        0        0      113 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register_env_creator.rst
--rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/autosumm.rst
--rw-r--r--   0        0        0     2402 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/conf.py
--rw-r--r--   0        0        0      263 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/index.rst
--rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-001-intro.rst
--rw-r--r--   0        0        0     4171 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-002-glossary.rst
--rw-r--r--   0        0        0      616 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-003-mock-projects.rst
--rw-r--r--   0        0        0     1269 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-004-rules-conventions.rst
--rw-r--r--   0        0        0      284 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-005-cli.rst
--rw-r--r--   0        0        0      102 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/main.rst
--rw-r--r--   0        0        0       45 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       46 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       27 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.2.rst
--rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.3.rst
--rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.4.rst
--rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.5.rst
--rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.1.rst
--rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.2.rst
--rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.3.rst
--rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.4.rst
--rw-r--r--   0        0        0       29 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.5.rst
--rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.6.rst
--rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.7.rst
--rw-r--r--   0        0        0       45 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.0.rst
--rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.1.rst
--rw-r--r--   0        0        0       48 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.10.rst
--rw-r--r--   0        0        0       47 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.2.rst
--rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.3.rst
--rw-r--r--   0        0        0       33 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.4.rst
--rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.5.rst
--rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.6.rst
--rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.7.rst
--rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.8.rst
--rw-r--r--   0        0        0       35 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.9.rst
--rw-r--r--   0        0        0       37 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.0.rst
--rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.1.rst
--rw-r--r--   0        0        0       70 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.10.rst
--rw-r--r--   0        0        0       55 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.11.rst
--rw-r--r--   0        0        0       45 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.12.rst
--rw-r--r--   0        0        0       68 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.13.rst
--rw-r--r--   0        0        0       68 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.14.rst
--rw-r--r--   0        0        0       42 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.15.rst
--rw-r--r--   0        0        0       52 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.2.rst
--rw-r--r--   0        0        0       66 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.3.rst
--rw-r--r--   0        0        0       53 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.4.rst
--rw-r--r--   0        0        0       45 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.5.rst
--rw-r--r--   0        0        0       41 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.6.rst
--rw-r--r--   0        0        0       71 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.7.rst
--rw-r--r--   0        0        0       47 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.8.rst
--rw-r--r--   0        0        0       53 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.9.rst
--rw-r--r--   0        0        0       64 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.5.0.rst
--rw-r--r--   0        0        0       50 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.5.1.rst
--rw-r--r--   0        0        0      159 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/confs.yaml
--rw-r--r--   0        0        0     1773 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/data/photo.csv
--rw-r--r--   0        0        0      655 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/minimal.py
--rw-r--r--   0        0        0     9861 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
--rw-r--r--   0        0        0       57 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
--rw-r--r--   0        0        0     2304 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
--rw-r--r--   0        0        0     1566 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
--rw-r--r--   0        0        0     3192 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
--rw-r--r--   0        0        0      307 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0      674 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
--rw-r--r--   0        0        0      261 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
--rw-r--r--   0        0        0      120 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0       65 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
--rw-r--r--   0        0        0      421 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
--rw-r--r--   0        0        0      945 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
--rw-r--r--   0        0        0     1093 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
--rw-r--r--   0        0        0     2415 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
--rw-r--r--   0        0        0      810 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
--rw-r--r--   0        0        0      575 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0     2940 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/todo/complex_success.py
--rw-r--r--   0        0        0      612 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-001-intro.ipynb
--rw-r--r--   0        0        0     5328 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-002-glossary.ipynb
--rw-r--r--   0        0        0     1877 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-003-mock-projects.ipynb
--rw-r--r--   0        0        0     1928 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-004-rules-conventions.ipynb
--rw-r--r--   0        0        0     1235 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-005-cli.ipynb
--rw-r--r--   0        0        0     1102 2023-06-18 14:15:24.932776 datazimmer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 datazimmer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/compatibility_test.yml
+-rw-r--r--   0        0        0     1299 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1795 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.gitignore
+-rw-r--r--   0        0        0      288 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0      491 2023-06-19 14:24:46.688842 datazimmer-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     1077 2023-06-19 14:24:46.688842 datazimmer-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3122 2023-06-19 14:24:46.692842 datazimmer-0.5.2/README.md
+-rw-r--r--   0        0        0     4074 2023-06-19 14:24:46.692842 datazimmer-0.5.2/conftest.py
+-rw-r--r--   0        0        0      634 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/aswan_integration.py
+-rw-r--r--   0        0        0     7923 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/config_loading.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/dvc_util.py
+-rw-r--r--   0        0        0      144 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/exceptions.py
+-rw-r--r--   0        0        0      624 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/get_runtime.py
+-rw-r--r--   0        0        0     2434 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/gh_actions.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/__init__.py
+-rw-r--r--   0        0        0     6235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/atoms.py
+-rw-r--r--   0        0        0     1422 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/complete_id.py
+-rw-r--r--   0        0        0     1744 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/datascript.py
+-rw-r--r--   0        0        0     4537 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/high_level.py
+-rw-r--r--   0        0        0     4798 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/scrutable.py
+-rw-r--r--   0        0        0     3456 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/naming.py
+-rw-r--r--   0        0        0      526 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/persistent_state.py
+-rw-r--r--   0        0        0     8463 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/pipeline_element.py
+-rw-r--r--   0        0        0     7648 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/project_runtime.py
+-rw-r--r--   0        0        0      935 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/raw_data.py
+-rw-r--r--   0        0        0     6235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/registry.py
+-rw-r--r--   0        0        0      863 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/reporting.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/draw.py
+-rw-r--r--   0        0        0     7107 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/loader.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/__init__.py
+-rw-r--r--   0        0        0     4692 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/create_dogshow.py
+-rw-r--r--   0        0        0      845 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_commands.py
+-rw-r--r--   0        0        0      346 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_config.py
+-rw-r--r--   0        0        0     4366 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_full_integration.py
+-rw-r--r--   0        0        0      465 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_registry.py
+-rw-r--r--   0        0        0      294 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_runtime.py
+-rw-r--r--   0        0        0     1799 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_scrutable.py
+-rw-r--r--   0        0        0      152 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_sql.py
+-rw-r--r--   0        0        0      235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_util.py
+-rw-r--r--   0        0        0      943 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_validation.py
+-rw-r--r--   0        0        0      939 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/util.py
+-rw-r--r--   0        0        0    10109 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/typer_commands.py
+-rw-r--r--   0        0        0     3260 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/utils.py
+-rw-r--r--   0        0        0     2957 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/validation_functions.py
+-rw-r--r--   0        0        0    10327 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/zenodo.py
+-rw-r--r--   0        0        0      114 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.AbstractEntity.rst
+-rw-r--r--   0        0        0      123 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.CompositeTypeBase.rst
+-rw-r--r--   0        0        0      746 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.DzAswan.rst
+-rw-r--r--   0        0        0      739 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.EntityClass.rst
+-rw-r--r--   0        0        0       87 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.Index.rst
+-rw-r--r--   0        0        0       96 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.Nullable.rst
+-rw-r--r--   0        0        0      444 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.PersistentState.rst
+-rw-r--r--   0        0        0      592 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.ReportFile.rst
+-rw-r--r--   0        0        0      565 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.ScruTable.rst
+-rw-r--r--   0        0        0       99 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.SourceUrl.rst
+-rw-r--r--   0        0        0      107 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.dump_dfs_to_tables.rst
+-rw-r--r--   0        0        0      104 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.get_raw_data_path.rst
+-rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.parse_df.rst
+-rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register.rst
+-rw-r--r--   0        0        0      113 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register_data_loader.rst
+-rw-r--r--   0        0        0      113 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register_env_creator.rst
+-rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/autosumm.rst
+-rw-r--r--   0        0        0     2402 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/index.rst
+-rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-001-intro.rst
+-rw-r--r--   0        0        0     4171 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-002-glossary.rst
+-rw-r--r--   0        0        0      616 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-003-mock-projects.rst
+-rw-r--r--   0        0        0     1269 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-004-rules-conventions.rst
+-rw-r--r--   0        0        0      284 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-005-cli.rst
+-rw-r--r--   0        0        0      102 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       46 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       27 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.2.rst
+-rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.3.rst
+-rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.4.rst
+-rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.5.rst
+-rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.1.rst
+-rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.2.rst
+-rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.3.rst
+-rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.4.rst
+-rw-r--r--   0        0        0       29 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.5.rst
+-rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.6.rst
+-rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.7.rst
+-rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.0.rst
+-rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.1.rst
+-rw-r--r--   0        0        0       48 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.10.rst
+-rw-r--r--   0        0        0       47 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.2.rst
+-rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.3.rst
+-rw-r--r--   0        0        0       33 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.4.rst
+-rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.5.rst
+-rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.6.rst
+-rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.7.rst
+-rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.8.rst
+-rw-r--r--   0        0        0       35 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.9.rst
+-rw-r--r--   0        0        0       37 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.0.rst
+-rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.1.rst
+-rw-r--r--   0        0        0       70 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.10.rst
+-rw-r--r--   0        0        0       55 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.11.rst
+-rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.12.rst
+-rw-r--r--   0        0        0       68 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.13.rst
+-rw-r--r--   0        0        0       68 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.14.rst
+-rw-r--r--   0        0        0       42 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.15.rst
+-rw-r--r--   0        0        0       52 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.2.rst
+-rw-r--r--   0        0        0       66 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.3.rst
+-rw-r--r--   0        0        0       53 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.4.rst
+-rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.5.rst
+-rw-r--r--   0        0        0       41 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.6.rst
+-rw-r--r--   0        0        0       71 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.7.rst
+-rw-r--r--   0        0        0       47 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.8.rst
+-rw-r--r--   0        0        0       53 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.9.rst
+-rw-r--r--   0        0        0       64 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.0.rst
+-rw-r--r--   0        0        0       50 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.1.rst
+-rw-r--r--   0        0        0       51 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.2.rst
+-rw-r--r--   0        0        0      159 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/confs.yaml
+-rw-r--r--   0        0        0     1773 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/data/photo.csv
+-rw-r--r--   0        0        0      655 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/minimal.py
+-rw-r--r--   0        0        0     9861 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
+-rw-r--r--   0        0        0       57 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
+-rw-r--r--   0        0        0     1566 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
+-rw-r--r--   0        0        0     3192 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
+-rw-r--r--   0        0        0      307 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
+-rw-r--r--   0        0        0      261 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
+-rw-r--r--   0        0        0      120 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
+-rw-r--r--   0        0        0      945 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
+-rw-r--r--   0        0        0     1093 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
+-rw-r--r--   0        0        0     2415 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
+-rw-r--r--   0        0        0      810 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
+-rw-r--r--   0        0        0      575 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0     2940 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/todo/complex_success.py
+-rw-r--r--   0        0        0      612 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-001-intro.ipynb
+-rw-r--r--   0        0        0     5328 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-002-glossary.ipynb
+-rw-r--r--   0        0        0     1877 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-003-mock-projects.ipynb
+-rw-r--r--   0        0        0     1928 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-004-rules-conventions.ipynb
+-rw-r--r--   0        0        0     1235 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-005-cli.ipynb
+-rw-r--r--   0        0        0     1109 2023-06-19 14:24:46.696843 datazimmer-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 datazimmer-0.5.2/PKG-INFO
```

### Comparing `datazimmer-0.5.1/.github/workflows/compatibility_test.yml` & `datazimmer-0.5.2/.github/workflows/compatibility_test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/.github/workflows/test.yml` & `datazimmer-0.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/.github/workflows/twine_release.yml` & `datazimmer-0.5.2/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/.gitignore` & `datazimmer-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/LICENSE` & `datazimmer-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/README.md` & `datazimmer-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/conftest.py` & `datazimmer-0.5.2/conftest.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/__init__.py` & `datazimmer-0.5.2/datazimmer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .persistent_state import PersistentState
 from .pipeline_element import register, register_data_loader, register_env_creator
 from .project_runtime import dump_dfs_to_tables
 from .raw_data import get_raw_data_path
 from .reporting import ReportFile
 from .typer_commands import app
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
```

### Comparing `datazimmer-0.5.1/datazimmer/aswan_integration.py` & `datazimmer-0.5.2/datazimmer/aswan_integration.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/config_loading.py` & `datazimmer-0.5.2/datazimmer/config_loading.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/dvc_util.py` & `datazimmer-0.5.2/datazimmer/dvc_util.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/get_runtime.py` & `datazimmer-0.5.2/datazimmer/get_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/gh_actions.py` & `datazimmer-0.5.2/datazimmer/gh_actions.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/metadata/atoms.py` & `datazimmer-0.5.2/datazimmer/metadata/atoms.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/metadata/complete_id.py` & `datazimmer-0.5.2/datazimmer/metadata/complete_id.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/metadata/datascript.py` & `datazimmer-0.5.2/datazimmer/metadata/datascript.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/metadata/high_level.py` & `datazimmer-0.5.2/datazimmer/metadata/high_level.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/metadata/scrutable.py` & `datazimmer-0.5.2/datazimmer/metadata/scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/naming.py` & `datazimmer-0.5.2/datazimmer/naming.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/persistent_state.py` & `datazimmer-0.5.2/datazimmer/persistent_state.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/pipeline_element.py` & `datazimmer-0.5.2/datazimmer/pipeline_element.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/project_runtime.py` & `datazimmer-0.5.2/datazimmer/project_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/raw_data.py` & `datazimmer-0.5.2/datazimmer/raw_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/registry.py` & `datazimmer-0.5.2/datazimmer/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import toml
 import yaml
 from flit.build import main
 from structlog import get_logger
 
 from .config_loading import get_full_auth
+from .dvc_util import DVC_ENV_EXC
 from .metadata.high_level import PROJ_KEYS
 from .naming import (
     GIT_TOKEN_ENV_VAR,
     MAIN_MODULE_NAME,
     META_MODULE_NAME,
     PYV,
     REQUIREMENTS_FILE,
@@ -78,15 +79,15 @@
         ypath = self.paths.info_yaml_of(project_name, version)
         if ypath.exists():
             return yaml.safe_load(ypath.read_text())
         logger.warning(f"info for {project_name} {version} requested but not found")
 
     def full_build(self, global_conf=False):
         self.dump_info()
-        get_full_auth().dump_dvc(local=not global_conf)
+        get_full_auth().dump_dvc(local=not global_conf, executable=DVC_ENV_EXC)
         if not self._is_released():
             self._package()
         if self.requires:
             self._install_no_server(self.requires)
 
     def update(self):
         self._git_run(pull=True)
```

### Comparing `datazimmer-0.5.1/datazimmer/reporting.py` & `datazimmer-0.5.2/datazimmer/reporting.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/sql/loader.py` & `datazimmer-0.5.2/datazimmer/sql/loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -212,72 +212,9 @@
         loader.setup_schema()
         yield constr
     finally:
         loader.purge()
         sqlpath.unlink()
 
 
-@dataclass
-class SqlFilter:
-    project: str
-    namespace: str
-    tables: list
-    col_renamer: dict
-
-    @contextmanager
-    def filter(self, constr):
-        engine = sa.create_engine(constr)
-        meta = sa.MetaData(bind=engine)
-        sa.MetaData.reflect(meta)
-        new_meta = self._convert(meta)
-        db_file = Path("_filtered.db")
-        new_constr = f"sqlite:///{db_file}"
-        engine = sa.create_engine(new_constr)
-        new_meta.create_all(engine)
-        yield new_constr
-        db_file.unlink()
-
-    def _convert(self, meta: sa.MetaData):
-        new_meta = sa.MetaData()
-        for table in meta.tables.values():
-            new_table_name = self._get_new_table_name(table.name)
-            if not new_table_name:
-                continue
-            new_cols = []
-            for col in table.columns:
-                new_col_name = self._get_new_col_name(col.name, new_table_name)
-                fks = filter(None, map(self._get_fk, col.foreign_keys))
-                new_cols.append(
-                    sa.Column(
-                        new_col_name,
-                        col.type,
-                        *fks,
-                        primary_key=col.primary_key,
-                        nullable=col.nullable,
-                    ),
-                )
-            sa.Table(new_table_name, new_meta, *new_cols)
-        return new_meta
-
-    def _get_fk(self, old_fk: sa.ForeignKey):
-        old_fk_table_name, fk_colname = old_fk.target_fullname.split(".")
-        new_fk_table_name = self._get_new_table_name(old_fk_table_name)
-        if not new_fk_table_name:
-            return
-        fk_col = self._get_new_col_name(fk_colname, new_fk_table_name)
-        return sa.ForeignKey(f"{new_fk_table_name}.{fk_col}")
-
-    def _get_new_table_name(self, name):
-        pid, nsid, tname = name.split(PREFIX_SEP)
-        if (
-            (pid == self.project)
-            and (nsid == self.namespace)
-            and (tname in self.tables)
-        ):
-            return tname
-
-    def _get_new_col_name(self, colname, tablename):
-        return self.col_renamer.get(tablename, self.col_renamer).get(colname, colname)
-
-
 def _parse_d(d):
     return {k: None if pd.isna(v) else v for k, v in d.items()}
```

### Comparing `datazimmer-0.5.1/datazimmer/tests/create_dogshow.py` & `datazimmer-0.5.2/datazimmer/tests/create_dogshow.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/tests/test_commands.py` & `datazimmer-0.5.2/datazimmer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/tests/test_full_integration.py` & `datazimmer-0.5.2/datazimmer/tests/test_full_integration.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/tests/test_scrutable.py` & `datazimmer-0.5.2/datazimmer/tests/test_scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/tests/test_validation.py` & `datazimmer-0.5.2/datazimmer/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/tests/util.py` & `datazimmer-0.5.2/datazimmer/tests/util.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/typer_commands.py` & `datazimmer-0.5.2/datazimmer/typer_commands.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/utils.py` & `datazimmer-0.5.2/datazimmer/utils.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/validation_functions.py` & `datazimmer-0.5.2/datazimmer/validation_functions.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/datazimmer/zenodo.py` & `datazimmer-0.5.2/datazimmer/zenodo.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/api/datazimmer.DzAswan.rst` & `datazimmer-0.5.2/docs/api/datazimmer.DzAswan.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/api/datazimmer.EntityClass.rst` & `datazimmer-0.5.2/docs/api/datazimmer.EntityClass.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/api/datazimmer.ReportFile.rst` & `datazimmer-0.5.2/docs/api/datazimmer.ReportFile.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/api/datazimmer.ScruTable.rst` & `datazimmer-0.5.2/docs/api/datazimmer.ScruTable.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/conf.py` & `datazimmer-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/notebooks/doc-002-glossary.rst` & `datazimmer-0.5.2/docs/notebooks/doc-002-glossary.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/notebooks/doc-003-mock-projects.rst` & `datazimmer-0.5.2/docs/notebooks/doc-003-mock-projects.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/docs/notebooks/doc-004-rules-conventions.rst` & `datazimmer-0.5.2/docs/notebooks/doc-004-rules-conventions.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/data/photo.csv` & `datazimmer-0.5.2/dogshow/data/photo.csv`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/minimal.py` & `datazimmer-0.5.2/dogshow/minimal.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb` & `datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py` & `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py` & `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py` & `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py` & `datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py` & `datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py` & `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py` & `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py` & `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py` & `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml` & `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/dogshow/todo/complex_success.py` & `datazimmer-0.5.2/dogshow/todo/complex_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/notebooks/doc-001-intro.ipynb` & `datazimmer-0.5.2/notebooks/doc-001-intro.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/notebooks/doc-002-glossary.ipynb` & `datazimmer-0.5.2/notebooks/doc-002-glossary.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/notebooks/doc-003-mock-projects.ipynb` & `datazimmer-0.5.2/notebooks/doc-003-mock-projects.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/notebooks/doc-004-rules-conventions.ipynb` & `datazimmer-0.5.2/notebooks/doc-004-rules-conventions.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/notebooks/doc-005-cli.ipynb` & `datazimmer-0.5.2/notebooks/doc-005-cli.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.1/pyproject.toml` & `datazimmer-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "pyyaml",
     "structlog",
     "toml",
     "typer",
     "cookiecutter",
     "sqlmermaid",
     "metazimmer",
-    "zimmauth"
+    "zimmauth>=0.1.0"
 ]
 
 [project.optional-dependencies]
 collect = ["aswan[remote]>=0.4.2"]
 postgres = ["psycopg2"]
 profile = ["pyinstrument"]
 zenodo = ["requests", "markdown2"]
```

### Comparing `datazimmer-0.5.1/PKG-INFO` & `datazimmer-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datazimmer
-Version: 0.5.1
+Version: 0.5.2
 Summary: sscu-budapest utilities for scientific data engineering
 Author-email: Social Science Computing Unit Budapest <borza.endre@krtk.hu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: flit
 Requires-Dist: wheel>=0.37.0
 Requires-Dist: pip>=22.0.0
@@ -16,15 +16,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: structlog
 Requires-Dist: toml
 Requires-Dist: typer
 Requires-Dist: cookiecutter
 Requires-Dist: sqlmermaid
 Requires-Dist: metazimmer
-Requires-Dist: zimmauth
+Requires-Dist: zimmauth>=0.1.0
 Requires-Dist: aswan[remote]>=0.4.2 ; extra == "collect"
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
 Requires-Dist: psycopg2 ; extra == "postgres"
 Requires-Dist: pyinstrument ; extra == "profile"
 Requires-Dist: branthebuilder ; extra == "test"
 Requires-Dist: zimmauth[test] ; extra == "test"
 Requires-Dist: atqo ; extra == "test"
```

