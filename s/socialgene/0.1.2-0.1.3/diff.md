# Comparing `tmp/socialgene-0.1.2.tar.gz` & `tmp/socialgene-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialgene-0.1.2.tar", last modified: Fri Jun 16 15:50:25 2023, max compression
+gzip compressed data, was "socialgene-0.1.3.tar", last modified: Mon Jun 19 13:42:59 2023, max compression
```

## Comparing `socialgene-0.1.2.tar` & `socialgene-0.1.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.778579 socialgene-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-16 15:50:15.000000 socialgene-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-16 15:50:25.778579 socialgene-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-16 15:50:15.000000 socialgene-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-16 15:50:15.000000 socialgene-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-16 15:50:25.778579 socialgene-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-16 15:50:15.000000 socialgene-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.762578 socialgene-0.1.2/socialgene/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.762578 socialgene-0.1.2/socialgene/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/base/compare_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/base/molbio.py
--rw-r--r--   0 runner    (1001) docker     (123)    26075 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/base/socialgene.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/clean_hmms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/create_neo4j_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/export_neo4j_header_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/export_protein_loci_assembly_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/parameter_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/parse_ncbi_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/parse_ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/process_domtblout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/cli/socialgene_hmm_tsv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/clustermap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/clustermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/clustermap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/common_parameters.env
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/data/biosample_attributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/findmybgc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/findmybgc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/findmybgc/findmybgc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/hashing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/hashing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/hashing/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.766579 socialgene-0.1.2/socialgene/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/hmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/hmm/hmmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/hmm/hmminfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.770578 socialgene-0.1.2/socialgene/mmseqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/mmseqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/mmseqs/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/mmseqs/index_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/mmseqs/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.770578 socialgene-0.1.2/socialgene/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/admin_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/ingest_from_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/queries.cypher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.770578 socialgene-0.1.2/socialgene/neo4j/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/define_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/define_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/define_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/node_relationship_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/schema/socialgene_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.770578 socialgene-0.1.2/socialgene/neo4j/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/search/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/neo4j/single_protein_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.774579 socialgene-0.1.2/socialgene/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/datasets_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/hmmer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/hmmmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/ncbi_feature_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/parsers/sequence_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.774579 socialgene-0.1.2/socialgene/scoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/scoring/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.774579 socialgene-0.1.2/socialgene/taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/taxonomy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.778579 socialgene-0.1.2/socialgene/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/chunker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/get_ncbi_biosample_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/goterms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/ncbi_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/nextflow_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/np_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/prep_ncbi_biosample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/run_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/simple_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/untargz.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 15:50:15.000000 socialgene-0.1.2/socialgene/utils/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:50:25.762578 socialgene-0.1.2/socialgene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 15:50:25.000000 socialgene-0.1.2/socialgene.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.186603 socialgene-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 13:42:49.000000 socialgene-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-19 13:42:59.186603 socialgene-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-19 13:42:49.000000 socialgene-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-19 13:42:49.000000 socialgene-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-19 13:42:59.186603 socialgene-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-19 13:42:49.000000 socialgene-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/base/compare_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/base/molbio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26075 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/base/socialgene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/clean_hmms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/create_neo4j_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/export_neo4j_header_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/export_protein_loci_assembly_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/parameter_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/parse_ncbi_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/parse_ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/process_domtblout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/cli/socialgene_hmm_tsv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene/clustermap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/clustermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/clustermap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/common_parameters.env
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/data/biosample_attributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/findmybgc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/findmybgc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/findmybgc/findmybgc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/hashing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/hashing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/hashing/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/hmm/hmmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/hmm/hmminfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/mmseqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/mmseqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/mmseqs/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/mmseqs/index_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/mmseqs/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/admin_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/ingest_from_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/queries.cypher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.178603 socialgene-0.1.3/socialgene/neo4j/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/define_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/define_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/define_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/node_relationship_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/schema/socialgene_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.182603 socialgene-0.1.3/socialgene/neo4j/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/search/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/neo4j/single_protein_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.182603 socialgene-0.1.3/socialgene/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/datasets_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/hmmer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/hmmmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/ncbi_feature_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/parsers/sequence_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.182603 socialgene-0.1.3/socialgene/scoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/scoring/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.182603 socialgene-0.1.3/socialgene/taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/taxonomy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.186603 socialgene-0.1.3/socialgene/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/chunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/get_ncbi_biosample_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/goterms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/ncbi_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/nextflow_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/np_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/prep_ncbi_biosample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/run_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/simple_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/untargz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 13:42:49.000000 socialgene-0.1.3/socialgene/utils/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:42:59.174603 socialgene-0.1.3/socialgene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 13:42:59.000000 socialgene-0.1.3/socialgene.egg-info/top_level.txt
```

### Comparing `socialgene-0.1.2/LICENSE.md` & `socialgene-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/PKG-INFO` & `socialgene-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.2
+Version: 0.1.3
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,34 +21,39 @@
 Provides-Extra: full
 Provides-Extra: ci
 Provides-Extra: cd
 License-File: LICENSE.md
 
 Note: All releases may intorduce breaking changes until the release of v1.0.0
 
-![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy)
-[![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy)
-[![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml)
-[![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml)
-[![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+# Status
 
-Both user and developer documentation can be found at: <https://socialgene.github.io>
+## Github
 
-![classes](classes_sgpy.png)
-![packages](packages_sgpy.png)
+![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+## PyPI
+
+![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
+
+# Contributing
+
+Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
+
+# Documentation
+
+Both user and developer documentation can be found at: <https://socialgene.github.io>
 
 <!---
 To create the UML diagram of the library:
 ```bash
 pyreverse -o png -p sgpy socialgene
 ```
 --->
 
 ## Installation with pip
-![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 ```bash
 pip install socialgene
 ```
 
 ## Create conda environment and install python package inside
 
@@ -62,38 +67,21 @@
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make install_python
 ```
 
-# Run all tests
+## Run all tests
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make run_ci
 ```
 
-## User-facing classes
-
-### `SocialGene()`
 
-This is the main class that most other user-facing classes should/do inherit from
-
-### `FindMyBGC()`
-
-### `SingleProteinSearch()`
-
-#### Common example use cases
-
-Starting with a single input protein and
-
-- [want to compare it against all other proteins in the Neo4j database](jupyter/single_protein_search.ipynb)
-
-Starting with a set of proteins (BGC) and
-
-- [want to compare against all other proteins in the Neo4j database](jupyter/findmybgc.ipynb)
-
-## Other
+## Classes:
+![classes](classes_sgpy.png)
 
-Most of the the classes that describe the structure of `SocialGene()` (e.g. proteins, domains, loci) live in `socialgene/src/socialgene/classes/molbio.py`
+## Modules
+![modules](packages_sgpy.png)
```

### Comparing `socialgene-0.1.2/README.md` & `socialgene-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Note: All releases may intorduce breaking changes until the release of v1.0.0
 
-![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy)
-[![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy)
-[![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml)
-[![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml)
-[![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+# Status
 
-Both user and developer documentation can be found at: <https://socialgene.github.io>
+## Github
 
-![classes](classes_sgpy.png)
-![packages](packages_sgpy.png)
+![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+## PyPI
+
+![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
+
+# Contributing
+
+Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
+
+# Documentation
+
+Both user and developer documentation can be found at: <https://socialgene.github.io>
 
 <!---
 To create the UML diagram of the library:
 ```bash
 pyreverse -o png -p sgpy socialgene
 ```
 --->
 
 ## Installation with pip
-![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 ```bash
 pip install socialgene
 ```
 
 ## Create conda environment and install python package inside
 
@@ -37,38 +42,21 @@
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make install_python
 ```
 
-# Run all tests
+## Run all tests
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make run_ci
 ```
 
-## User-facing classes
-
-### `SocialGene()`
 
-This is the main class that most other user-facing classes should/do inherit from
-
-### `FindMyBGC()`
-
-### `SingleProteinSearch()`
-
-#### Common example use cases
-
-Starting with a single input protein and
-
-- [want to compare it against all other proteins in the Neo4j database](jupyter/single_protein_search.ipynb)
-
-Starting with a set of proteins (BGC) and
-
-- [want to compare against all other proteins in the Neo4j database](jupyter/findmybgc.ipynb)
-
-## Other
+## Classes:
+![classes](classes_sgpy.png)
 
-Most of the the classes that describe the structure of `SocialGene()` (e.g. proteins, domains, loci) live in `socialgene/src/socialgene/classes/molbio.py`
+## Modules
+![modules](packages_sgpy.png)
```

### Comparing `socialgene-0.1.2/pyproject.toml` & `socialgene-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socialgene"
-version = "0.1.2"
+version = "0.1.3"
 description = "Creating and interacting with graph databases of protein domains and their genome coordinates"
 readme = "README.md"
 authors =  [
     {name = "Chase M. Clark", email = "chasingmicrobes@gmail.com"},
 ]
 keywords = []  #! TODO
 # Pypi classifiers: https://pypi.org/classifiers/
@@ -37,15 +37,15 @@
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/socialgene/sgpy"
 homepage = "https://socialgene.github.io"
 
 [project.optional-dependencies]
-full = ["rich>=10.12.0", "networkx", "obonet"]
+full = ["rich>=10.12.0"]
 ci = ["pytest-cov"]
 cd = ["twine"]
 
 [project.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "socialgene"="socialgene.cli.__main__:main"
 "sg_process_domtblout"="socialgene.cli.process_domtblout:main"
```

### Comparing `socialgene-0.1.2/setup.cfg` & `socialgene-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/setup.py` & `socialgene-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/base/compare_protein.py` & `socialgene-0.1.3/socialgene/base/compare_protein.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/base/molbio.py` & `socialgene-0.1.3/socialgene/base/molbio.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/base/socialgene.py` & `socialgene-0.1.3/socialgene/base/socialgene.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/__main__.py` & `socialgene-0.1.3/socialgene/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/clean_hmms.py` & `socialgene-0.1.3/socialgene/cli/clean_hmms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/create_neo4j_db.py` & `socialgene-0.1.3/socialgene/cli/create_neo4j_db.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/export_neo4j_header_files.py` & `socialgene-0.1.3/socialgene/cli/export_neo4j_header_files.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/export_protein_loci_assembly_tables.py` & `socialgene-0.1.3/socialgene/cli/export_protein_loci_assembly_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/parameter_export.py` & `socialgene-0.1.3/socialgene/cli/parameter_export.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/parse_ncbi_feature_tables.py` & `socialgene-0.1.3/socialgene/cli/parse_ncbi_feature_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/parse_ncbi_taxonomy.py` & `socialgene-0.1.3/socialgene/cli/parse_ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/process_domtblout.py` & `socialgene-0.1.3/socialgene/cli/process_domtblout.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/protein_sqlite.py` & `socialgene-0.1.3/socialgene/cli/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/cli/socialgene_hmm_tsv_parser.py` & `socialgene-0.1.3/socialgene/cli/socialgene_hmm_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/clustermap/clustermap.py` & `socialgene-0.1.3/socialgene/clustermap/clustermap.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/common_parameters.env` & `socialgene-0.1.3/socialgene/common_parameters.env`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/config.py` & `socialgene-0.1.3/socialgene/config.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/data/biosample_attributes` & `socialgene-0.1.3/socialgene/data/biosample_attributes`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/findmybgc/findmybgc.py` & `socialgene-0.1.3/socialgene/findmybgc/findmybgc.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/hashing/hashing.py` & `socialgene-0.1.3/socialgene/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/hmm/hmmer.py` & `socialgene-0.1.3/socialgene/hmm/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/hmm/hmminfo.py` & `socialgene-0.1.3/socialgene/hmm/hmminfo.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/mmseqs/create_database.py` & `socialgene-0.1.3/socialgene/mmseqs/create_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/mmseqs/index_database.py` & `socialgene-0.1.3/socialgene/mmseqs/index_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/mmseqs/search.py` & `socialgene-0.1.3/socialgene/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/admin_import.py` & `socialgene-0.1.3/socialgene/neo4j/admin_import.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/ingest_from_neo4j.py` & `socialgene-0.1.3/socialgene/neo4j/ingest_from_neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/neo4j.py` & `socialgene-0.1.3/socialgene/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/queries.cypher` & `socialgene-0.1.3/socialgene/neo4j/queries.cypher`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/schema/define_modules.py` & `socialgene-0.1.3/socialgene/neo4j/schema/define_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/schema/define_nodes.py` & `socialgene-0.1.3/socialgene/neo4j/schema/define_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             ],
         )
         self.add_node(
             neo4j_label="goterm",
             header_filename="goterms.header",
             target_subdirectory="goterms",
             target_extension="goterms",
-            header=["uid:ID(goterm)", "namespace", "name", "def"],
+            header=["uid:ID(goterm)", "name", "namespace", "def"],
         )
 
         self.add_node(
             neo4j_label="tigrfam_role",
             header_filename="tigrfam_role.header",
             target_subdirectory="tigrfam_info",
             target_extension="tigrfam_role",
```

### Comparing `socialgene-0.1.2/socialgene/neo4j/schema/define_relationships.py` & `socialgene-0.1.3/socialgene/neo4j/schema/define_relationships.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/schema/node_relationship_class.py` & `socialgene-0.1.3/socialgene/neo4j/schema/node_relationship_class.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/schema/socialgene_modules.py` & `socialgene-0.1.3/socialgene/neo4j/schema/socialgene_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/search/basic.py` & `socialgene-0.1.3/socialgene/neo4j/search/basic.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/neo4j/single_protein_search.py` & `socialgene-0.1.3/socialgene/neo4j/single_protein_search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/datasets_parse.py` & `socialgene-0.1.3/socialgene/parsers/datasets_parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/hmmer_parser.py` & `socialgene-0.1.3/socialgene/parsers/hmmer_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/hmmmodel.py` & `socialgene-0.1.3/socialgene/parsers/hmmmodel.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/ncbi_feature_table.py` & `socialgene-0.1.3/socialgene/parsers/ncbi_feature_table.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/ncbi_taxonomy.py` & `socialgene-0.1.3/socialgene/parsers/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/parsers/sequence_parser.py` & `socialgene-0.1.3/socialgene/parsers/sequence_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/scoring/scoring.py` & `socialgene-0.1.3/socialgene/scoring/scoring.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/chunker.py` & `socialgene-0.1.3/socialgene/utils/chunker.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/file_handling.py` & `socialgene-0.1.3/socialgene/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/get_ncbi_biosample_attributes.py` & `socialgene-0.1.3/socialgene/utils/get_ncbi_biosample_attributes.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/logging.py` & `socialgene-0.1.3/socialgene/utils/logging.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/ncbi_ftp.py` & `socialgene-0.1.3/socialgene/utils/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/nextflow_test_utils.py` & `socialgene-0.1.3/socialgene/utils/nextflow_test_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/pandas_utils.py` & `socialgene-0.1.3/socialgene/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/prep_ncbi_biosample_data.py` & `socialgene-0.1.3/socialgene/utils/prep_ncbi_biosample_data.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/protein_sqlite.py` & `socialgene-0.1.3/socialgene/utils/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/run_subprocess.py` & `socialgene-0.1.3/socialgene/utils/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene/utils/untargz.py` & `socialgene-0.1.3/socialgene/utils/untargz.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene.egg-info/PKG-INFO` & `socialgene-0.1.3/socialgene.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.2
+Version: 0.1.3
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,34 +21,39 @@
 Provides-Extra: full
 Provides-Extra: ci
 Provides-Extra: cd
 License-File: LICENSE.md
 
 Note: All releases may intorduce breaking changes until the release of v1.0.0
 
-![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy)
-[![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy)
-[![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml)
-[![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml)
-[![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+# Status
 
-Both user and developer documentation can be found at: <https://socialgene.github.io>
+## Github
 
-![classes](classes_sgpy.png)
-![packages](packages_sgpy.png)
+![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/socialgene/sgpy) [![codecov](https://codecov.io/gh/socialgene/sgpy/branch/main/graph/badge.svg?token=8f8GCc4J3G)](https://codecov.io/gh/socialgene/sgpy) [![Linting](https://github.com/socialgene/sgpy/actions/workflows/linters.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/linters.yml) [![Continuous Integration](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pr_ci.yml) [![Continuous Deployment](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml/badge.svg)](https://github.com/socialgene/sgpy/actions/workflows/pypi_autodeploy_python.yml)
+## PyPI
+
+![PyPI](https://img.shields.io/pypi/v/socialgene) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socialgene) ![PyPI - Status](https://img.shields.io/pypi/status/socialgene) ![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
+
+# Contributing
+
+Please see https://github.com/socialgene/sgpy/blob/main/CONTRIBUTING.md
+
+# Documentation
+
+Both user and developer documentation can be found at: <https://socialgene.github.io>
 
 <!---
 To create the UML diagram of the library:
 ```bash
 pyreverse -o png -p sgpy socialgene
 ```
 --->
 
 ## Installation with pip
-![https://pypi.org/project/socialgene](https://img.shields.io/pypi/dm/socialgene)
 
 ```bash
 pip install socialgene
 ```
 
 ## Create conda environment and install python package inside
 
@@ -62,38 +67,21 @@
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make install_python
 ```
 
-# Run all tests
+## Run all tests
 
 ```bash
 git clone https://github.com/socialgene/sgpy.git
 cd sgpy
 make run_ci
 ```
 
-## User-facing classes
-
-### `SocialGene()`
 
-This is the main class that most other user-facing classes should/do inherit from
-
-### `FindMyBGC()`
-
-### `SingleProteinSearch()`
-
-#### Common example use cases
-
-Starting with a single input protein and
-
-- [want to compare it against all other proteins in the Neo4j database](jupyter/single_protein_search.ipynb)
-
-Starting with a set of proteins (BGC) and
-
-- [want to compare against all other proteins in the Neo4j database](jupyter/findmybgc.ipynb)
-
-## Other
+## Classes:
+![classes](classes_sgpy.png)
 
-Most of the the classes that describe the structure of `SocialGene()` (e.g. proteins, domains, loci) live in `socialgene/src/socialgene/classes/molbio.py`
+## Modules
+![modules](packages_sgpy.png)
```

### Comparing `socialgene-0.1.2/socialgene.egg-info/SOURCES.txt` & `socialgene-0.1.3/socialgene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.2/socialgene.egg-info/entry_points.txt` & `socialgene-0.1.3/socialgene.egg-info/entry_points.txt`

 * *Files identical despite different names*

