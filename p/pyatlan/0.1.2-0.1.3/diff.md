# Comparing `tmp/pyatlan-0.1.2.tar.gz` & `tmp/pyatlan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.1.2.tar", last modified: Wed Jun 14 12:25:50 2023, max compression
+gzip compressed data, was "pyatlan-0.1.3.tar", last modified: Mon Jun 19 11:26:22 2023, max compression
```

## Comparing `pyatlan-0.1.2.tar` & `pyatlan-0.1.3.tar`

### file list

```diff
@@ -1,84 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.303921 pyatlan-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-14 12:25:38.000000 pyatlan-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 12:25:38.000000 pyatlan-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 12:25:38.000000 pyatlan-0.1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 12:25:50.303921 pyatlan-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 12:25:38.000000 pyatlan-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.291921 pyatlan-0.1.2/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/classification_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42383 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   900272 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    54059 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:25:38.000000 pyatlan-0.1.2/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.295921 pyatlan-0.1.2/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 12:25:50.000000 pyatlan-0.1.2/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:25:50.303921 pyatlan-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-14 12:25:38.000000 pyatlan-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.299921 pyatlan-0.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/classification_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:25:50.303921 pyatlan-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_classification_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    64432 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-14 12:25:38.000000 pyatlan-0.1.2/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-06-19 11:26:11.000000 pyatlan-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 11:26:11.000000 pyatlan-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 11:26:11.000000 pyatlan-0.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-19 11:26:22.771959 pyatlan-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-19 11:26:11.000000 pyatlan-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.759959 pyatlan-0.1.3/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/classification_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43669 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   986605 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56226 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59796 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 11:26:11.000000 pyatlan-0.1.3/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.763959 pyatlan-0.1.3/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 11:26:22.000000 pyatlan-0.1.3/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:26:22.771959 pyatlan-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-19 11:26:11.000000 pyatlan-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.767959 pyatlan-0.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:22.771959 pyatlan-0.1.3/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_classification_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31770 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 11:26:11.000000 pyatlan-0.1.3/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.1.2/LICENSE` & `pyatlan-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/PKG-INFO` & `pyatlan-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.2/README.md` & `pyatlan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/classification_cache.py` & `pyatlan-0.1.3/pyatlan/cache/classification_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.1.3/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/enum_cache.py` & `pyatlan-0.1.3/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/group_cache.py` & `pyatlan-0.1.3/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/role_cache.py` & `pyatlan-0.1.3/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/cache/user_cache.py` & `pyatlan-0.1.3/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/client/atlan.py` & `pyatlan-0.1.3/pyatlan/client/atlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     Asset,
     AtlasGlossary,
     AtlasGlossaryCategory,
     AtlasGlossaryTerm,
     Connection,
     Database,
     MaterialisedView,
+    Persona,
+    Purpose,
     Referenceable,
     Schema,
     Table,
     View,
 )
 from pyatlan.model.atlan_image import AtlanImage
 from pyatlan.model.core import (
@@ -1232,7 +1234,49 @@
             raise InvalidRequestException(
                 message="Unable to request both directions of lineage at the same time through the lineage list API.",
             )
         raw_json = self._call_api(
             GET_LINEAGE_LIST, None, lineage_request, exclude_unset=True
         )
         return LineageListResponse(**raw_json)
+
+    @validate_arguments()
+    def find_personas_by_name(
+        self,
+        name: str,
+        attributes: Optional[list[str]] = None,
+    ) -> list[Persona]:
+        if attributes is None:
+            attributes = []
+        query = (
+            Term.with_state("ACTIVE")
+            + Term.with_type_name("PERSONA")
+            + Term.with_name(name)
+        )
+        dsl = DSL(query=query)
+        search_request = IndexSearchRequest(
+            dsl=dsl,
+            attributes=attributes,
+        )
+        results = self.search(search_request)
+        return [asset for asset in results if isinstance(asset, Persona)]
+
+    @validate_arguments()
+    def find_purposes_by_name(
+        self,
+        name: str,
+        attributes: Optional[list[str]] = None,
+    ) -> list[Purpose]:
+        if attributes is None:
+            attributes = []
+        query = (
+            Term.with_state("ACTIVE")
+            + Term.with_type_name("PURPOSE")
+            + Term.with_name(name)
+        )
+        dsl = DSL(query=query)
+        search_request = IndexSearchRequest(
+            dsl=dsl,
+            attributes=attributes,
+        )
+        results = self.search(search_request)
+        return [asset for asset in results if isinstance(asset, Purpose)]
```

### Comparing `pyatlan-0.1.2/pyatlan/client/constants.py` & `pyatlan-0.1.3/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/error.py` & `pyatlan-0.1.3/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/exceptions.py` & `pyatlan-0.1.3/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.1.3/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/assets.py` & `pyatlan-0.1.3/pyatlan/model/assets.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Based on original code from https://github.com/apache/atlas (under Apache-2.0 license)
 from __future__ import annotations
 
 import hashlib
 import sys
 from datetime import datetime
 from io import StringIO
-from typing import Any, ClassVar, Dict, List, Optional, TypeVar
+from typing import Any, ClassVar, Dict, List, Optional, Set, Type, TypeVar
 from urllib.parse import quote, unquote
 
 from pydantic import Field, PrivateAttr, StrictStr, root_validator, validator
 
 from pyatlan.model.core import Announcement, AtlanObject, Classification, Meaning
 from pyatlan.model.custom_metadata import CustomMetadataDict, CustomMetadataProxy
 from pyatlan.model.enums import (
@@ -24,22 +24,28 @@
     ADLSObjectType,
     ADLSPerformance,
     ADLSProvisionState,
     ADLSReplicationType,
     ADLSStorageKind,
     AnnouncementType,
     AtlanConnectorType,
+    AuthPolicyCategory,
+    AuthPolicyResourceCategory,
     AuthPolicyType,
     CertificateStatus,
+    DataAction,
     EntityStatus,
     FileType,
     GoogleDatastudioAssetType,
     IconType,
     KafkaTopicCompressionType,
+    PersonaGlossaryAction,
+    PersonaMetadataAction,
     PowerbiEndorsement,
+    PurposeMetadataAction,
     QueryUsernameStrategy,
     QuickSightAnalysisStatus,
     QuickSightDatasetFieldType,
     QuickSightDatasetImportMode,
     QuickSightFolderType,
     SourceCostUnitType,
 )
@@ -104,45 +110,45 @@
         "replicated_from",
         "replicated_to",
         "assigned_terms",
     ]
 
     @property
     def qualified_name(self) -> str:
-        return self.attributes.qualified_name
+        return None if self.attributes is None else self.attributes.qualified_name
 
     @qualified_name.setter
     def qualified_name(self, qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qualified_name = qualified_name
 
     @property
     def replicated_from(self) -> Optional[list[AtlasServer]]:
-        return self.attributes.replicated_from
+        return None if self.attributes is None else self.attributes.replicated_from
 
     @replicated_from.setter
     def replicated_from(self, replicated_from: Optional[list[AtlasServer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replicated_from = replicated_from
 
     @property
     def replicated_to(self) -> Optional[list[AtlasServer]]:
-        return self.attributes.replicated_to
+        return None if self.attributes is None else self.attributes.replicated_to
 
     @replicated_to.setter
     def replicated_to(self, replicated_to: Optional[list[AtlasServer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replicated_to = replicated_to
 
     @property
     def assigned_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.meanings
+        return None if self.attributes is None else self.attributes.meanings
 
     @assigned_terms.setter
     def assigned_terms(self, assigned_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.meanings = assigned_terms
 
@@ -399,521 +405,559 @@
         "metrics",
         "readme",
         "assigned_terms",
     ]
 
     @property
     def name(self) -> str:
-        return self.attributes.name
+        return None if self.attributes is None else self.attributes.name
 
     @name.setter
     def name(self, name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.name = name
 
     @property
     def display_name(self) -> Optional[str]:
-        return self.attributes.display_name
+        return None if self.attributes is None else self.attributes.display_name
 
     @display_name.setter
     def display_name(self, display_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.display_name = display_name
 
     @property
     def description(self) -> Optional[str]:
-        return self.attributes.description
+        return None if self.attributes is None else self.attributes.description
 
     @description.setter
     def description(self, description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.description = description
 
     @property
     def user_description(self) -> Optional[str]:
-        return self.attributes.user_description
+        return None if self.attributes is None else self.attributes.user_description
 
     @user_description.setter
     def user_description(self, user_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.user_description = user_description
 
     @property
     def tenant_id(self) -> Optional[str]:
-        return self.attributes.tenant_id
+        return None if self.attributes is None else self.attributes.tenant_id
 
     @tenant_id.setter
     def tenant_id(self, tenant_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tenant_id = tenant_id
 
     @property
     def certificate_status(self) -> Optional[CertificateStatus]:
-        return self.attributes.certificate_status
+        return None if self.attributes is None else self.attributes.certificate_status
 
     @certificate_status.setter
     def certificate_status(self, certificate_status: Optional[CertificateStatus]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certificate_status = certificate_status
 
     @property
     def certificate_status_message(self) -> Optional[str]:
-        return self.attributes.certificate_status_message
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.certificate_status_message
+        )
 
     @certificate_status_message.setter
     def certificate_status_message(self, certificate_status_message: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certificate_status_message = certificate_status_message
 
     @property
     def certificate_updated_by(self) -> Optional[str]:
-        return self.attributes.certificate_updated_by
+        return (
+            None if self.attributes is None else self.attributes.certificate_updated_by
+        )
 
     @certificate_updated_by.setter
     def certificate_updated_by(self, certificate_updated_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certificate_updated_by = certificate_updated_by
 
     @property
     def certificate_updated_at(self) -> Optional[datetime]:
-        return self.attributes.certificate_updated_at
+        return (
+            None if self.attributes is None else self.attributes.certificate_updated_at
+        )
 
     @certificate_updated_at.setter
     def certificate_updated_at(self, certificate_updated_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certificate_updated_at = certificate_updated_at
 
     @property
     def announcement_title(self) -> Optional[str]:
-        return self.attributes.announcement_title
+        return None if self.attributes is None else self.attributes.announcement_title
 
     @announcement_title.setter
     def announcement_title(self, announcement_title: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.announcement_title = announcement_title
 
     @property
     def announcement_message(self) -> Optional[str]:
-        return self.attributes.announcement_message
+        return None if self.attributes is None else self.attributes.announcement_message
 
     @announcement_message.setter
     def announcement_message(self, announcement_message: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.announcement_message = announcement_message
 
     @property
     def announcement_type(self) -> Optional[str]:
-        return self.attributes.announcement_type
+        return None if self.attributes is None else self.attributes.announcement_type
 
     @announcement_type.setter
     def announcement_type(self, announcement_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.announcement_type = announcement_type
 
     @property
     def announcement_updated_at(self) -> Optional[datetime]:
-        return self.attributes.announcement_updated_at
+        return (
+            None if self.attributes is None else self.attributes.announcement_updated_at
+        )
 
     @announcement_updated_at.setter
     def announcement_updated_at(self, announcement_updated_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.announcement_updated_at = announcement_updated_at
 
     @property
     def announcement_updated_by(self) -> Optional[str]:
-        return self.attributes.announcement_updated_by
+        return (
+            None if self.attributes is None else self.attributes.announcement_updated_by
+        )
 
     @announcement_updated_by.setter
     def announcement_updated_by(self, announcement_updated_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.announcement_updated_by = announcement_updated_by
 
     @property
     def owner_users(self) -> Optional[set[str]]:
-        return self.attributes.owner_users
+        return None if self.attributes is None else self.attributes.owner_users
 
     @owner_users.setter
     def owner_users(self, owner_users: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.owner_users = owner_users
 
     @property
     def owner_groups(self) -> Optional[set[str]]:
-        return self.attributes.owner_groups
+        return None if self.attributes is None else self.attributes.owner_groups
 
     @owner_groups.setter
     def owner_groups(self, owner_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.owner_groups = owner_groups
 
     @property
     def admin_users(self) -> Optional[set[str]]:
-        return self.attributes.admin_users
+        return None if self.attributes is None else self.attributes.admin_users
 
     @admin_users.setter
     def admin_users(self, admin_users: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.admin_users = admin_users
 
     @property
     def admin_groups(self) -> Optional[set[str]]:
-        return self.attributes.admin_groups
+        return None if self.attributes is None else self.attributes.admin_groups
 
     @admin_groups.setter
     def admin_groups(self, admin_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.admin_groups = admin_groups
 
     @property
     def viewer_users(self) -> Optional[set[str]]:
-        return self.attributes.viewer_users
+        return None if self.attributes is None else self.attributes.viewer_users
 
     @viewer_users.setter
     def viewer_users(self, viewer_users: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.viewer_users = viewer_users
 
     @property
     def viewer_groups(self) -> Optional[set[str]]:
-        return self.attributes.viewer_groups
+        return None if self.attributes is None else self.attributes.viewer_groups
 
     @viewer_groups.setter
     def viewer_groups(self, viewer_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.viewer_groups = viewer_groups
 
     @property
     def connector_name(self) -> Optional[str]:
-        return self.attributes.connector_name
+        return None if self.attributes is None else self.attributes.connector_name
 
     @connector_name.setter
     def connector_name(self, connector_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connector_name = connector_name
 
     @property
     def connection_name(self) -> Optional[str]:
-        return self.attributes.connection_name
+        return None if self.attributes is None else self.attributes.connection_name
 
     @connection_name.setter
     def connection_name(self, connection_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_name = connection_name
 
     @property
     def connection_qualified_name(self) -> Optional[str]:
-        return self.attributes.connection_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.connection_qualified_name
+        )
 
     @connection_qualified_name.setter
     def connection_qualified_name(self, connection_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_qualified_name = connection_qualified_name
 
     @property
     def has_lineage(self) -> Optional[bool]:
-        return self.attributes.has_lineage
+        return None if self.attributes is None else self.attributes.has_lineage
 
     @has_lineage.setter
     def has_lineage(self, has_lineage: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.has_lineage = has_lineage
 
     @property
     def is_discoverable(self) -> Optional[bool]:
-        return self.attributes.is_discoverable
+        return None if self.attributes is None else self.attributes.is_discoverable
 
     @is_discoverable.setter
     def is_discoverable(self, is_discoverable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_discoverable = is_discoverable
 
     @property
     def is_editable(self) -> Optional[bool]:
-        return self.attributes.is_editable
+        return None if self.attributes is None else self.attributes.is_editable
 
     @is_editable.setter
     def is_editable(self, is_editable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_editable = is_editable
 
     @property
     def sub_type(self) -> Optional[str]:
-        return self.attributes.sub_type
+        return None if self.attributes is None else self.attributes.sub_type
 
     @sub_type.setter
     def sub_type(self, sub_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sub_type = sub_type
 
     @property
     def view_score(self) -> Optional[float]:
-        return self.attributes.view_score
+        return None if self.attributes is None else self.attributes.view_score
 
     @view_score.setter
     def view_score(self, view_score: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_score = view_score
 
     @property
     def popularity_score(self) -> Optional[float]:
-        return self.attributes.popularity_score
+        return None if self.attributes is None else self.attributes.popularity_score
 
     @popularity_score.setter
     def popularity_score(self, popularity_score: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.popularity_score = popularity_score
 
     @property
     def source_owners(self) -> Optional[str]:
-        return self.attributes.source_owners
+        return None if self.attributes is None else self.attributes.source_owners
 
     @source_owners.setter
     def source_owners(self, source_owners: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_owners = source_owners
 
     @property
     def source_created_by(self) -> Optional[str]:
-        return self.attributes.source_created_by
+        return None if self.attributes is None else self.attributes.source_created_by
 
     @source_created_by.setter
     def source_created_by(self, source_created_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_created_by = source_created_by
 
     @property
     def source_created_at(self) -> Optional[datetime]:
-        return self.attributes.source_created_at
+        return None if self.attributes is None else self.attributes.source_created_at
 
     @source_created_at.setter
     def source_created_at(self, source_created_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_created_at = source_created_at
 
     @property
     def source_updated_at(self) -> Optional[datetime]:
-        return self.attributes.source_updated_at
+        return None if self.attributes is None else self.attributes.source_updated_at
 
     @source_updated_at.setter
     def source_updated_at(self, source_updated_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_updated_at = source_updated_at
 
     @property
     def source_updated_by(self) -> Optional[str]:
-        return self.attributes.source_updated_by
+        return None if self.attributes is None else self.attributes.source_updated_by
 
     @source_updated_by.setter
     def source_updated_by(self, source_updated_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_updated_by = source_updated_by
 
     @property
     def source_url(self) -> Optional[str]:
-        return self.attributes.source_url
+        return None if self.attributes is None else self.attributes.source_url
 
     @source_url.setter
     def source_url(self, source_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_url = source_url
 
     @property
     def source_embed_url(self) -> Optional[str]:
-        return self.attributes.source_embed_url
+        return None if self.attributes is None else self.attributes.source_embed_url
 
     @source_embed_url.setter
     def source_embed_url(self, source_embed_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_embed_url = source_embed_url
 
     @property
     def last_sync_workflow_name(self) -> Optional[str]:
-        return self.attributes.last_sync_workflow_name
+        return (
+            None if self.attributes is None else self.attributes.last_sync_workflow_name
+        )
 
     @last_sync_workflow_name.setter
     def last_sync_workflow_name(self, last_sync_workflow_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_sync_workflow_name = last_sync_workflow_name
 
     @property
     def last_sync_run_at(self) -> Optional[datetime]:
-        return self.attributes.last_sync_run_at
+        return None if self.attributes is None else self.attributes.last_sync_run_at
 
     @last_sync_run_at.setter
     def last_sync_run_at(self, last_sync_run_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_sync_run_at = last_sync_run_at
 
     @property
     def last_sync_run(self) -> Optional[str]:
-        return self.attributes.last_sync_run
+        return None if self.attributes is None else self.attributes.last_sync_run
 
     @last_sync_run.setter
     def last_sync_run(self, last_sync_run: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_sync_run = last_sync_run
 
     @property
     def admin_roles(self) -> Optional[set[str]]:
-        return self.attributes.admin_roles
+        return None if self.attributes is None else self.attributes.admin_roles
 
     @admin_roles.setter
     def admin_roles(self, admin_roles: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.admin_roles = admin_roles
 
     @property
     def source_read_count(self) -> Optional[int]:
-        return self.attributes.source_read_count
+        return None if self.attributes is None else self.attributes.source_read_count
 
     @source_read_count.setter
     def source_read_count(self, source_read_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_count = source_read_count
 
     @property
     def source_read_user_count(self) -> Optional[int]:
-        return self.attributes.source_read_user_count
+        return (
+            None if self.attributes is None else self.attributes.source_read_user_count
+        )
 
     @source_read_user_count.setter
     def source_read_user_count(self, source_read_user_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_user_count = source_read_user_count
 
     @property
     def source_last_read_at(self) -> Optional[datetime]:
-        return self.attributes.source_last_read_at
+        return None if self.attributes is None else self.attributes.source_last_read_at
 
     @source_last_read_at.setter
     def source_last_read_at(self, source_last_read_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_read_at = source_last_read_at
 
     @property
     def last_row_changed_at(self) -> Optional[datetime]:
-        return self.attributes.last_row_changed_at
+        return None if self.attributes is None else self.attributes.last_row_changed_at
 
     @last_row_changed_at.setter
     def last_row_changed_at(self, last_row_changed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_row_changed_at = last_row_changed_at
 
     @property
     def source_total_cost(self) -> Optional[float]:
-        return self.attributes.source_total_cost
+        return None if self.attributes is None else self.attributes.source_total_cost
 
     @source_total_cost.setter
     def source_total_cost(self, source_total_cost: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_total_cost = source_total_cost
 
     @property
     def source_cost_unit(self) -> Optional[SourceCostUnitType]:
-        return self.attributes.source_cost_unit
+        return None if self.attributes is None else self.attributes.source_cost_unit
 
     @source_cost_unit.setter
     def source_cost_unit(self, source_cost_unit: Optional[SourceCostUnitType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_cost_unit = source_cost_unit
 
     @property
     def source_read_query_cost(self) -> Optional[float]:
-        return self.attributes.source_read_query_cost
+        return (
+            None if self.attributes is None else self.attributes.source_read_query_cost
+        )
 
     @source_read_query_cost.setter
     def source_read_query_cost(self, source_read_query_cost: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_query_cost = source_read_query_cost
 
     @property
     def source_read_recent_user_list(self) -> Optional[set[str]]:
-        return self.attributes.source_read_recent_user_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_recent_user_list
+        )
 
     @source_read_recent_user_list.setter
     def source_read_recent_user_list(
         self, source_read_recent_user_list: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_recent_user_list = source_read_recent_user_list
 
     @property
     def source_read_recent_user_record_list(self) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_read_recent_user_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_recent_user_record_list
+        )
 
     @source_read_recent_user_record_list.setter
     def source_read_recent_user_record_list(
         self, source_read_recent_user_record_list: Optional[list[PopularityInsights]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_recent_user_record_list = (
             source_read_recent_user_record_list
         )
 
     @property
     def source_read_top_user_list(self) -> Optional[set[str]]:
-        return self.attributes.source_read_top_user_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_top_user_list
+        )
 
     @source_read_top_user_list.setter
     def source_read_top_user_list(self, source_read_top_user_list: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_top_user_list = source_read_top_user_list
 
     @property
     def source_read_top_user_record_list(self) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_read_top_user_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_top_user_record_list
+        )
 
     @source_read_top_user_record_list.setter
     def source_read_top_user_record_list(
         self, source_read_top_user_record_list: Optional[list[PopularityInsights]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -921,15 +965,19 @@
             source_read_top_user_record_list
         )
 
     @property
     def source_read_popular_query_record_list(
         self,
     ) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_read_popular_query_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_popular_query_record_list
+        )
 
     @source_read_popular_query_record_list.setter
     def source_read_popular_query_record_list(
         self, source_read_popular_query_record_list: Optional[list[PopularityInsights]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -937,808 +985,996 @@
             source_read_popular_query_record_list
         )
 
     @property
     def source_read_expensive_query_record_list(
         self,
     ) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_read_expensive_query_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_expensive_query_record_list
+        )
 
     @source_read_expensive_query_record_list.setter
     def source_read_expensive_query_record_list(
         self,
         source_read_expensive_query_record_list: Optional[list[PopularityInsights]],
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_expensive_query_record_list = (
             source_read_expensive_query_record_list
         )
 
     @property
     def source_read_slow_query_record_list(self) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_read_slow_query_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_read_slow_query_record_list
+        )
 
     @source_read_slow_query_record_list.setter
     def source_read_slow_query_record_list(
         self, source_read_slow_query_record_list: Optional[list[PopularityInsights]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_read_slow_query_record_list = (
             source_read_slow_query_record_list
         )
 
     @property
     def source_query_compute_cost_list(self) -> Optional[set[str]]:
-        return self.attributes.source_query_compute_cost_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_query_compute_cost_list
+        )
 
     @source_query_compute_cost_list.setter
     def source_query_compute_cost_list(
         self, source_query_compute_cost_list: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_query_compute_cost_list = source_query_compute_cost_list
 
     @property
     def source_query_compute_cost_record_list(
         self,
     ) -> Optional[list[PopularityInsights]]:
-        return self.attributes.source_query_compute_cost_record_list
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_query_compute_cost_record_list
+        )
 
     @source_query_compute_cost_record_list.setter
     def source_query_compute_cost_record_list(
         self, source_query_compute_cost_record_list: Optional[list[PopularityInsights]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_query_compute_cost_record_list = (
             source_query_compute_cost_record_list
         )
 
     @property
     def dbt_qualified_name(self) -> Optional[str]:
-        return self.attributes.dbt_qualified_name
+        return None if self.attributes is None else self.attributes.dbt_qualified_name
 
     @dbt_qualified_name.setter
     def dbt_qualified_name(self, dbt_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_qualified_name = dbt_qualified_name
 
     @property
     def asset_dbt_alias(self) -> Optional[str]:
-        return self.attributes.asset_dbt_alias
+        return None if self.attributes is None else self.attributes.asset_dbt_alias
 
     @asset_dbt_alias.setter
     def asset_dbt_alias(self, asset_dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_alias = asset_dbt_alias
 
     @property
     def asset_dbt_meta(self) -> Optional[str]:
-        return self.attributes.asset_dbt_meta
+        return None if self.attributes is None else self.attributes.asset_dbt_meta
 
     @asset_dbt_meta.setter
     def asset_dbt_meta(self, asset_dbt_meta: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_meta = asset_dbt_meta
 
     @property
     def asset_dbt_unique_id(self) -> Optional[str]:
-        return self.attributes.asset_dbt_unique_id
+        return None if self.attributes is None else self.attributes.asset_dbt_unique_id
 
     @asset_dbt_unique_id.setter
     def asset_dbt_unique_id(self, asset_dbt_unique_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_unique_id = asset_dbt_unique_id
 
     @property
     def asset_dbt_account_name(self) -> Optional[str]:
-        return self.attributes.asset_dbt_account_name
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_account_name
+        )
 
     @asset_dbt_account_name.setter
     def asset_dbt_account_name(self, asset_dbt_account_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_account_name = asset_dbt_account_name
 
     @property
     def asset_dbt_project_name(self) -> Optional[str]:
-        return self.attributes.asset_dbt_project_name
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_project_name
+        )
 
     @asset_dbt_project_name.setter
     def asset_dbt_project_name(self, asset_dbt_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_project_name = asset_dbt_project_name
 
     @property
     def asset_dbt_package_name(self) -> Optional[str]:
-        return self.attributes.asset_dbt_package_name
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_package_name
+        )
 
     @asset_dbt_package_name.setter
     def asset_dbt_package_name(self, asset_dbt_package_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_package_name = asset_dbt_package_name
 
     @property
     def asset_dbt_job_name(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_name
+        return None if self.attributes is None else self.attributes.asset_dbt_job_name
 
     @asset_dbt_job_name.setter
     def asset_dbt_job_name(self, asset_dbt_job_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_name = asset_dbt_job_name
 
     @property
     def asset_dbt_job_schedule(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_schedule
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_job_schedule
+        )
 
     @asset_dbt_job_schedule.setter
     def asset_dbt_job_schedule(self, asset_dbt_job_schedule: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_schedule = asset_dbt_job_schedule
 
     @property
     def asset_dbt_job_status(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_status
+        return None if self.attributes is None else self.attributes.asset_dbt_job_status
 
     @asset_dbt_job_status.setter
     def asset_dbt_job_status(self, asset_dbt_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_status = asset_dbt_job_status
 
     @property
     def asset_dbt_job_schedule_cron_humanized(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_schedule_cron_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_schedule_cron_humanized
+        )
 
     @asset_dbt_job_schedule_cron_humanized.setter
     def asset_dbt_job_schedule_cron_humanized(
         self, asset_dbt_job_schedule_cron_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_schedule_cron_humanized = (
             asset_dbt_job_schedule_cron_humanized
         )
 
     @property
     def asset_dbt_job_last_run(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_last_run
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_job_last_run
+        )
 
     @asset_dbt_job_last_run.setter
     def asset_dbt_job_last_run(self, asset_dbt_job_last_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run = asset_dbt_job_last_run
 
     @property
     def asset_dbt_job_last_run_url(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_url
+        )
 
     @asset_dbt_job_last_run_url.setter
     def asset_dbt_job_last_run_url(self, asset_dbt_job_last_run_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_url = asset_dbt_job_last_run_url
 
     @property
     def asset_dbt_job_last_run_created_at(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_last_run_created_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_created_at
+        )
 
     @asset_dbt_job_last_run_created_at.setter
     def asset_dbt_job_last_run_created_at(
         self, asset_dbt_job_last_run_created_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_created_at = (
             asset_dbt_job_last_run_created_at
         )
 
     @property
     def asset_dbt_job_last_run_updated_at(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_last_run_updated_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_updated_at
+        )
 
     @asset_dbt_job_last_run_updated_at.setter
     def asset_dbt_job_last_run_updated_at(
         self, asset_dbt_job_last_run_updated_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_updated_at = (
             asset_dbt_job_last_run_updated_at
         )
 
     @property
     def asset_dbt_job_last_run_dequed_at(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_last_run_dequed_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_dequed_at
+        )
 
     @asset_dbt_job_last_run_dequed_at.setter
     def asset_dbt_job_last_run_dequed_at(
         self, asset_dbt_job_last_run_dequed_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_dequed_at = (
             asset_dbt_job_last_run_dequed_at
         )
 
     @property
     def asset_dbt_job_last_run_started_at(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_last_run_started_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_started_at
+        )
 
     @asset_dbt_job_last_run_started_at.setter
     def asset_dbt_job_last_run_started_at(
         self, asset_dbt_job_last_run_started_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_started_at = (
             asset_dbt_job_last_run_started_at
         )
 
     @property
     def asset_dbt_job_last_run_total_duration(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_total_duration
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_total_duration
+        )
 
     @asset_dbt_job_last_run_total_duration.setter
     def asset_dbt_job_last_run_total_duration(
         self, asset_dbt_job_last_run_total_duration: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_total_duration = (
             asset_dbt_job_last_run_total_duration
         )
 
     @property
     def asset_dbt_job_last_run_total_duration_humanized(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_total_duration_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_total_duration_humanized
+        )
 
     @asset_dbt_job_last_run_total_duration_humanized.setter
     def asset_dbt_job_last_run_total_duration_humanized(
         self, asset_dbt_job_last_run_total_duration_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_total_duration_humanized = (
             asset_dbt_job_last_run_total_duration_humanized
         )
 
     @property
     def asset_dbt_job_last_run_queued_duration(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_queued_duration
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_queued_duration
+        )
 
     @asset_dbt_job_last_run_queued_duration.setter
     def asset_dbt_job_last_run_queued_duration(
         self, asset_dbt_job_last_run_queued_duration: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_queued_duration = (
             asset_dbt_job_last_run_queued_duration
         )
 
     @property
     def asset_dbt_job_last_run_queued_duration_humanized(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_queued_duration_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_queued_duration_humanized
+        )
 
     @asset_dbt_job_last_run_queued_duration_humanized.setter
     def asset_dbt_job_last_run_queued_duration_humanized(
         self, asset_dbt_job_last_run_queued_duration_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_queued_duration_humanized = (
             asset_dbt_job_last_run_queued_duration_humanized
         )
 
     @property
     def asset_dbt_job_last_run_run_duration(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_run_duration
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_run_duration
+        )
 
     @asset_dbt_job_last_run_run_duration.setter
     def asset_dbt_job_last_run_run_duration(
         self, asset_dbt_job_last_run_run_duration: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_run_duration = (
             asset_dbt_job_last_run_run_duration
         )
 
     @property
     def asset_dbt_job_last_run_run_duration_humanized(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_run_duration_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_run_duration_humanized
+        )
 
     @asset_dbt_job_last_run_run_duration_humanized.setter
     def asset_dbt_job_last_run_run_duration_humanized(
         self, asset_dbt_job_last_run_run_duration_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_run_duration_humanized = (
             asset_dbt_job_last_run_run_duration_humanized
         )
 
     @property
     def asset_dbt_job_last_run_git_branch(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_git_branch
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_git_branch
+        )
 
     @asset_dbt_job_last_run_git_branch.setter
     def asset_dbt_job_last_run_git_branch(
         self, asset_dbt_job_last_run_git_branch: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_git_branch = (
             asset_dbt_job_last_run_git_branch
         )
 
     @property
     def asset_dbt_job_last_run_git_sha(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_git_sha
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_git_sha
+        )
 
     @asset_dbt_job_last_run_git_sha.setter
     def asset_dbt_job_last_run_git_sha(
         self, asset_dbt_job_last_run_git_sha: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_git_sha = asset_dbt_job_last_run_git_sha
 
     @property
     def asset_dbt_job_last_run_status_message(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_status_message
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_status_message
+        )
 
     @asset_dbt_job_last_run_status_message.setter
     def asset_dbt_job_last_run_status_message(
         self, asset_dbt_job_last_run_status_message: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_status_message = (
             asset_dbt_job_last_run_status_message
         )
 
     @property
     def asset_dbt_job_last_run_owner_thread_id(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_owner_thread_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_owner_thread_id
+        )
 
     @asset_dbt_job_last_run_owner_thread_id.setter
     def asset_dbt_job_last_run_owner_thread_id(
         self, asset_dbt_job_last_run_owner_thread_id: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_owner_thread_id = (
             asset_dbt_job_last_run_owner_thread_id
         )
 
     @property
     def asset_dbt_job_last_run_executed_by_thread_id(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_executed_by_thread_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_executed_by_thread_id
+        )
 
     @asset_dbt_job_last_run_executed_by_thread_id.setter
     def asset_dbt_job_last_run_executed_by_thread_id(
         self, asset_dbt_job_last_run_executed_by_thread_id: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_executed_by_thread_id = (
             asset_dbt_job_last_run_executed_by_thread_id
         )
 
     @property
     def asset_dbt_job_last_run_artifacts_saved(self) -> Optional[bool]:
-        return self.attributes.asset_dbt_job_last_run_artifacts_saved
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_artifacts_saved
+        )
 
     @asset_dbt_job_last_run_artifacts_saved.setter
     def asset_dbt_job_last_run_artifacts_saved(
         self, asset_dbt_job_last_run_artifacts_saved: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_artifacts_saved = (
             asset_dbt_job_last_run_artifacts_saved
         )
 
     @property
     def asset_dbt_job_last_run_artifact_s3_path(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_last_run_artifact_s3_path
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_artifact_s3_path
+        )
 
     @asset_dbt_job_last_run_artifact_s3_path.setter
     def asset_dbt_job_last_run_artifact_s3_path(
         self, asset_dbt_job_last_run_artifact_s3_path: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_artifact_s3_path = (
             asset_dbt_job_last_run_artifact_s3_path
         )
 
     @property
     def asset_dbt_job_last_run_has_docs_generated(self) -> Optional[bool]:
-        return self.attributes.asset_dbt_job_last_run_has_docs_generated
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_has_docs_generated
+        )
 
     @asset_dbt_job_last_run_has_docs_generated.setter
     def asset_dbt_job_last_run_has_docs_generated(
         self, asset_dbt_job_last_run_has_docs_generated: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_has_docs_generated = (
             asset_dbt_job_last_run_has_docs_generated
         )
 
     @property
     def asset_dbt_job_last_run_has_sources_generated(self) -> Optional[bool]:
-        return self.attributes.asset_dbt_job_last_run_has_sources_generated
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_has_sources_generated
+        )
 
     @asset_dbt_job_last_run_has_sources_generated.setter
     def asset_dbt_job_last_run_has_sources_generated(
         self, asset_dbt_job_last_run_has_sources_generated: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_has_sources_generated = (
             asset_dbt_job_last_run_has_sources_generated
         )
 
     @property
     def asset_dbt_job_last_run_notifications_sent(self) -> Optional[bool]:
-        return self.attributes.asset_dbt_job_last_run_notifications_sent
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_last_run_notifications_sent
+        )
 
     @asset_dbt_job_last_run_notifications_sent.setter
     def asset_dbt_job_last_run_notifications_sent(
         self, asset_dbt_job_last_run_notifications_sent: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_last_run_notifications_sent = (
             asset_dbt_job_last_run_notifications_sent
         )
 
     @property
     def asset_dbt_job_next_run(self) -> Optional[datetime]:
-        return self.attributes.asset_dbt_job_next_run
+        return (
+            None if self.attributes is None else self.attributes.asset_dbt_job_next_run
+        )
 
     @asset_dbt_job_next_run.setter
     def asset_dbt_job_next_run(self, asset_dbt_job_next_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_next_run = asset_dbt_job_next_run
 
     @property
     def asset_dbt_job_next_run_humanized(self) -> Optional[str]:
-        return self.attributes.asset_dbt_job_next_run_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_job_next_run_humanized
+        )
 
     @asset_dbt_job_next_run_humanized.setter
     def asset_dbt_job_next_run_humanized(
         self, asset_dbt_job_next_run_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_job_next_run_humanized = (
             asset_dbt_job_next_run_humanized
         )
 
     @property
     def asset_dbt_environment_name(self) -> Optional[str]:
-        return self.attributes.asset_dbt_environment_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_environment_name
+        )
 
     @asset_dbt_environment_name.setter
     def asset_dbt_environment_name(self, asset_dbt_environment_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_environment_name = asset_dbt_environment_name
 
     @property
     def asset_dbt_environment_dbt_version(self) -> Optional[str]:
-        return self.attributes.asset_dbt_environment_dbt_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_environment_dbt_version
+        )
 
     @asset_dbt_environment_dbt_version.setter
     def asset_dbt_environment_dbt_version(
         self, asset_dbt_environment_dbt_version: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_environment_dbt_version = (
             asset_dbt_environment_dbt_version
         )
 
     @property
     def asset_dbt_tags(self) -> Optional[set[str]]:
-        return self.attributes.asset_dbt_tags
+        return None if self.attributes is None else self.attributes.asset_dbt_tags
 
     @asset_dbt_tags.setter
     def asset_dbt_tags(self, asset_dbt_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_tags = asset_dbt_tags
 
     @property
     def asset_dbt_semantic_layer_proxy_url(self) -> Optional[str]:
-        return self.attributes.asset_dbt_semantic_layer_proxy_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_semantic_layer_proxy_url
+        )
 
     @asset_dbt_semantic_layer_proxy_url.setter
     def asset_dbt_semantic_layer_proxy_url(
         self, asset_dbt_semantic_layer_proxy_url: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_semantic_layer_proxy_url = (
             asset_dbt_semantic_layer_proxy_url
         )
 
     @property
     def asset_dbt_source_freshness_criteria(self) -> Optional[str]:
-        return self.attributes.asset_dbt_source_freshness_criteria
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_source_freshness_criteria
+        )
 
     @asset_dbt_source_freshness_criteria.setter
     def asset_dbt_source_freshness_criteria(
         self, asset_dbt_source_freshness_criteria: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_dbt_source_freshness_criteria = (
             asset_dbt_source_freshness_criteria
         )
 
     @property
     def sample_data_url(self) -> Optional[str]:
-        return self.attributes.sample_data_url
+        return None if self.attributes is None else self.attributes.sample_data_url
 
     @sample_data_url.setter
     def sample_data_url(self, sample_data_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sample_data_url = sample_data_url
 
     @property
     def asset_tags(self) -> Optional[set[str]]:
-        return self.attributes.asset_tags
+        return None if self.attributes is None else self.attributes.asset_tags
 
     @asset_tags.setter
     def asset_tags(self, asset_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_tags = asset_tags
 
     @property
     def asset_mc_incident_names(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_names
+        return (
+            None if self.attributes is None else self.attributes.asset_mc_incident_names
+        )
 
     @asset_mc_incident_names.setter
     def asset_mc_incident_names(self, asset_mc_incident_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_names = asset_mc_incident_names
 
     @property
     def asset_mc_incident_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_incident_qualified_names
+        )
 
     @asset_mc_incident_qualified_names.setter
     def asset_mc_incident_qualified_names(
         self, asset_mc_incident_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_qualified_names = (
             asset_mc_incident_qualified_names
         )
 
     @property
     def asset_mc_monitor_names(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_monitor_names
+        return (
+            None if self.attributes is None else self.attributes.asset_mc_monitor_names
+        )
 
     @asset_mc_monitor_names.setter
     def asset_mc_monitor_names(self, asset_mc_monitor_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_monitor_names = asset_mc_monitor_names
 
     @property
     def asset_mc_monitor_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_monitor_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_monitor_qualified_names
+        )
 
     @asset_mc_monitor_qualified_names.setter
     def asset_mc_monitor_qualified_names(
         self, asset_mc_monitor_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_monitor_qualified_names = (
             asset_mc_monitor_qualified_names
         )
 
     @property
     def asset_mc_monitor_statuses(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_monitor_statuses
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_monitor_statuses
+        )
 
     @asset_mc_monitor_statuses.setter
     def asset_mc_monitor_statuses(self, asset_mc_monitor_statuses: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_monitor_statuses = asset_mc_monitor_statuses
 
     @property
     def asset_mc_monitor_types(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_monitor_types
+        return (
+            None if self.attributes is None else self.attributes.asset_mc_monitor_types
+        )
 
     @asset_mc_monitor_types.setter
     def asset_mc_monitor_types(self, asset_mc_monitor_types: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_monitor_types = asset_mc_monitor_types
 
     @property
     def asset_mc_monitor_schedule_types(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_monitor_schedule_types
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_monitor_schedule_types
+        )
 
     @asset_mc_monitor_schedule_types.setter
     def asset_mc_monitor_schedule_types(
         self, asset_mc_monitor_schedule_types: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_monitor_schedule_types = (
             asset_mc_monitor_schedule_types
         )
 
     @property
     def asset_mc_incident_types(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_types
+        return (
+            None if self.attributes is None else self.attributes.asset_mc_incident_types
+        )
 
     @asset_mc_incident_types.setter
     def asset_mc_incident_types(self, asset_mc_incident_types: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_types = asset_mc_incident_types
 
     @property
     def asset_mc_incident_sub_types(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_sub_types
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_incident_sub_types
+        )
 
     @asset_mc_incident_sub_types.setter
     def asset_mc_incident_sub_types(
         self, asset_mc_incident_sub_types: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_sub_types = asset_mc_incident_sub_types
 
     @property
     def asset_mc_incident_severities(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_severities
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_incident_severities
+        )
 
     @asset_mc_incident_severities.setter
     def asset_mc_incident_severities(
         self, asset_mc_incident_severities: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_severities = asset_mc_incident_severities
 
     @property
     def asset_mc_incident_states(self) -> Optional[set[str]]:
-        return self.attributes.asset_mc_incident_states
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_incident_states
+        )
 
     @asset_mc_incident_states.setter
     def asset_mc_incident_states(self, asset_mc_incident_states: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_incident_states = asset_mc_incident_states
 
     @property
     def asset_mc_last_sync_run_at(self) -> Optional[datetime]:
-        return self.attributes.asset_mc_last_sync_run_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_mc_last_sync_run_at
+        )
 
     @asset_mc_last_sync_run_at.setter
     def asset_mc_last_sync_run_at(self, asset_mc_last_sync_run_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset_mc_last_sync_run_at = asset_mc_last_sync_run_at
 
     @property
     def starred_by(self) -> Optional[set[str]]:
-        return self.attributes.starred_by
+        return None if self.attributes is None else self.attributes.starred_by
 
     @starred_by.setter
     def starred_by(self, starred_by: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.starred_by = starred_by
 
     @property
     def mc_monitors(self) -> Optional[list[MCMonitor]]:
-        return self.attributes.mc_monitors
+        return None if self.attributes is None else self.attributes.mc_monitors
 
     @mc_monitors.setter
     def mc_monitors(self, mc_monitors: Optional[list[MCMonitor]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitors = mc_monitors
 
     @property
     def files(self) -> Optional[list[File]]:
-        return self.attributes.files
+        return None if self.attributes is None else self.attributes.files
 
     @files.setter
     def files(self, files: Optional[list[File]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.files = files
 
     @property
     def mc_incidents(self) -> Optional[list[MCIncident]]:
-        return self.attributes.mc_incidents
+        return None if self.attributes is None else self.attributes.mc_incidents
 
     @mc_incidents.setter
     def mc_incidents(self, mc_incidents: Optional[list[MCIncident]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incidents = mc_incidents
 
     @property
     def links(self) -> Optional[list[Link]]:
-        return self.attributes.links
+        return None if self.attributes is None else self.attributes.links
 
     @links.setter
     def links(self, links: Optional[list[Link]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.links = links
 
     @property
     def metrics(self) -> Optional[list[Metric]]:
-        return self.attributes.metrics
+        return None if self.attributes is None else self.attributes.metrics
 
     @metrics.setter
     def metrics(self, metrics: Optional[list[Metric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metrics = metrics
 
     @property
     def readme(self) -> Optional[Readme]:
-        return self.attributes.readme
+        return None if self.attributes is None else self.attributes.readme
 
     @readme.setter
     def readme(self, readme: Optional[Readme]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.readme = readme
 
     @property
     def assigned_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.meanings
+        return None if self.attributes is None else self.attributes.meanings
 
     @assigned_terms.setter
     def assigned_terms(self, assigned_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.meanings = assigned_terms
 
     _subtypes_: dict[str, type] = dict()
 
     def __init_subclass__(cls, type_name=None):
         cls._subtypes_[type_name or cls.__name__.lower()] = cls
 
+    def trim_to_required(self: SelfAsset) -> SelfAsset:
+        return self.create_for_modification(
+            qualified_name=self.qualified_name, name=self.name
+        )
+
+    @classmethod
+    def create(cls: Type[SelfAsset], *args, **kwargs) -> SelfAsset:
+        raise NotImplementedError(
+            "Create has not been implemented for this class. Please submit an enhancement"
+            "request if you need it implemented."
+        )
+
     @classmethod
     def create_for_modification(
         cls: type[SelfAsset], qualified_name: str = "", name: str = ""
     ) -> SelfAsset:
         validate_required_fields(
             ["name", "qualified_name"],
             [name, qualified_name],
@@ -2227,246 +2463,283 @@
         "query_preview_config",
         "query_config",
         "credential_strategy",
         "preview_credential_strategy",
         "policy_strategy",
         "query_username_strategy",
         "row_limit",
+        "query_timeout",
         "default_credential_guid",
         "connector_icon",
         "connector_image",
         "source_logo",
         "is_sample_data_preview_enabled",
         "popularity_insights_timeframe",
         "has_popularity_insights",
         "connection_dbt_environments",
         "connection_s_s_o_credential_guid",
     ]
 
     @property
     def category(self) -> Optional[str]:
-        return self.attributes.category
+        return None if self.attributes is None else self.attributes.category
 
     @category.setter
     def category(self, category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.category = category
 
     @property
     def sub_category(self) -> Optional[str]:
-        return self.attributes.sub_category
+        return None if self.attributes is None else self.attributes.sub_category
 
     @sub_category.setter
     def sub_category(self, sub_category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sub_category = sub_category
 
     @property
     def host(self) -> Optional[str]:
-        return self.attributes.host
+        return None if self.attributes is None else self.attributes.host
 
     @host.setter
     def host(self, host: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.host = host
 
     @property
     def port(self) -> Optional[int]:
-        return self.attributes.port
+        return None if self.attributes is None else self.attributes.port
 
     @port.setter
     def port(self, port: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.port = port
 
     @property
     def allow_query(self) -> Optional[bool]:
-        return self.attributes.allow_query
+        return None if self.attributes is None else self.attributes.allow_query
 
     @allow_query.setter
     def allow_query(self, allow_query: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.allow_query = allow_query
 
     @property
     def allow_query_preview(self) -> Optional[bool]:
-        return self.attributes.allow_query_preview
+        return None if self.attributes is None else self.attributes.allow_query_preview
 
     @allow_query_preview.setter
     def allow_query_preview(self, allow_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.allow_query_preview = allow_query_preview
 
     @property
     def query_preview_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.query_preview_config
+        return None if self.attributes is None else self.attributes.query_preview_config
 
     @query_preview_config.setter
     def query_preview_config(self, query_preview_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_preview_config = query_preview_config
 
     @property
     def query_config(self) -> Optional[str]:
-        return self.attributes.query_config
+        return None if self.attributes is None else self.attributes.query_config
 
     @query_config.setter
     def query_config(self, query_config: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_config = query_config
 
     @property
     def credential_strategy(self) -> Optional[str]:
-        return self.attributes.credential_strategy
+        return None if self.attributes is None else self.attributes.credential_strategy
 
     @credential_strategy.setter
     def credential_strategy(self, credential_strategy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.credential_strategy = credential_strategy
 
     @property
     def preview_credential_strategy(self) -> Optional[str]:
-        return self.attributes.preview_credential_strategy
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preview_credential_strategy
+        )
 
     @preview_credential_strategy.setter
     def preview_credential_strategy(self, preview_credential_strategy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preview_credential_strategy = preview_credential_strategy
 
     @property
     def policy_strategy(self) -> Optional[str]:
-        return self.attributes.policy_strategy
+        return None if self.attributes is None else self.attributes.policy_strategy
 
     @policy_strategy.setter
     def policy_strategy(self, policy_strategy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_strategy = policy_strategy
 
     @property
     def query_username_strategy(self) -> Optional[QueryUsernameStrategy]:
-        return self.attributes.query_username_strategy
+        return (
+            None if self.attributes is None else self.attributes.query_username_strategy
+        )
 
     @query_username_strategy.setter
     def query_username_strategy(
         self, query_username_strategy: Optional[QueryUsernameStrategy]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_username_strategy = query_username_strategy
 
     @property
     def row_limit(self) -> Optional[int]:
-        return self.attributes.row_limit
+        return None if self.attributes is None else self.attributes.row_limit
 
     @row_limit.setter
     def row_limit(self, row_limit: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_limit = row_limit
 
     @property
+    def query_timeout(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.query_timeout
+
+    @query_timeout.setter
+    def query_timeout(self, query_timeout: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.query_timeout = query_timeout
+
+    @property
     def default_credential_guid(self) -> Optional[str]:
-        return self.attributes.default_credential_guid
+        return (
+            None if self.attributes is None else self.attributes.default_credential_guid
+        )
 
     @default_credential_guid.setter
     def default_credential_guid(self, default_credential_guid: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_credential_guid = default_credential_guid
 
     @property
     def connector_icon(self) -> Optional[str]:
-        return self.attributes.connector_icon
+        return None if self.attributes is None else self.attributes.connector_icon
 
     @connector_icon.setter
     def connector_icon(self, connector_icon: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connector_icon = connector_icon
 
     @property
     def connector_image(self) -> Optional[str]:
-        return self.attributes.connector_image
+        return None if self.attributes is None else self.attributes.connector_image
 
     @connector_image.setter
     def connector_image(self, connector_image: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connector_image = connector_image
 
     @property
     def source_logo(self) -> Optional[str]:
-        return self.attributes.source_logo
+        return None if self.attributes is None else self.attributes.source_logo
 
     @source_logo.setter
     def source_logo(self, source_logo: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_logo = source_logo
 
     @property
     def is_sample_data_preview_enabled(self) -> Optional[bool]:
-        return self.attributes.is_sample_data_preview_enabled
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.is_sample_data_preview_enabled
+        )
 
     @is_sample_data_preview_enabled.setter
     def is_sample_data_preview_enabled(
         self, is_sample_data_preview_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_sample_data_preview_enabled = is_sample_data_preview_enabled
 
     @property
     def popularity_insights_timeframe(self) -> Optional[int]:
-        return self.attributes.popularity_insights_timeframe
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.popularity_insights_timeframe
+        )
 
     @popularity_insights_timeframe.setter
     def popularity_insights_timeframe(
         self, popularity_insights_timeframe: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.popularity_insights_timeframe = popularity_insights_timeframe
 
     @property
     def has_popularity_insights(self) -> Optional[bool]:
-        return self.attributes.has_popularity_insights
+        return (
+            None if self.attributes is None else self.attributes.has_popularity_insights
+        )
 
     @has_popularity_insights.setter
     def has_popularity_insights(self, has_popularity_insights: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.has_popularity_insights = has_popularity_insights
 
     @property
     def connection_dbt_environments(self) -> Optional[set[str]]:
-        return self.attributes.connection_dbt_environments
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.connection_dbt_environments
+        )
 
     @connection_dbt_environments.setter
     def connection_dbt_environments(
         self, connection_dbt_environments: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_dbt_environments = connection_dbt_environments
 
     @property
     def connection_s_s_o_credential_guid(self) -> Optional[str]:
-        return self.attributes.connection_s_s_o_credential_guid
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.connection_s_s_o_credential_guid
+        )
 
     @connection_s_s_o_credential_guid.setter
     def connection_s_s_o_credential_guid(
         self, connection_s_s_o_credential_guid: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -2504,14 +2777,15 @@
         policy_strategy: Optional[str] = Field(
             None, description="", alias="policyStrategy"
         )
         query_username_strategy: Optional[QueryUsernameStrategy] = Field(
             None, description="", alias="queryUsernameStrategy"
         )
         row_limit: Optional[int] = Field(None, description="", alias="rowLimit")
+        query_timeout: Optional[int] = Field(None, description="", alias="queryTimeout")
         default_credential_guid: Optional[str] = Field(
             None, description="", alias="defaultCredentialGuid"
         )
         connector_icon: Optional[str] = Field(
             None, description="", alias="connectorIcon"
         )
         connector_image: Optional[str] = Field(
@@ -2583,17 +2857,17 @@
                         f"Provided username {username} was not found in Atlan."
                     )
         attr = cls.Attributes(
             name=name,
             qualified_name=connector_type.to_qualified_name(),
             connector_name=connector_type.value,
             category=connector_type.category.value,
-            admin_users=admin_users if admin_users else [],
-            admin_groups=admin_groups if admin_groups else [],
-            admin_roles=admin_roles if admin_roles else [],
+            admin_users=admin_users or [],
+            admin_groups=admin_groups or [],
+            admin_roles=admin_roles or [],
         )
         return cls(attributes=attr)
 
 
 class Process(Asset, type_name="Process"):
     """Description"""
 
@@ -2609,65 +2883,65 @@
         "sql",
         "ast",
         "column_processes",
     ]
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.inputs
+        return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
     @property
     def outputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.outputs
+        return None if self.attributes is None else self.attributes.outputs
 
     @outputs.setter
     def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.outputs = outputs
 
     @property
     def code(self) -> Optional[str]:
-        return self.attributes.code
+        return None if self.attributes is None else self.attributes.code
 
     @code.setter
     def code(self, code: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.code = code
 
     @property
     def sql(self) -> Optional[str]:
-        return self.attributes.sql
+        return None if self.attributes is None else self.attributes.sql
 
     @sql.setter
     def sql(self, sql: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql = sql
 
     @property
     def ast(self) -> Optional[str]:
-        return self.attributes.ast
+        return None if self.attributes is None else self.attributes.ast
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
     def column_processes(self) -> Optional[list[ColumnProcess]]:
-        return self.attributes.column_processes
+        return None if self.attributes is None else self.attributes.column_processes
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
@@ -2797,75 +3071,77 @@
         "anchor",
         "parent_category",
         "children_categories",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
-        return self.attributes.short_description
+        return None if self.attributes is None else self.attributes.short_description
 
     @short_description.setter
     def short_description(self, short_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.short_description = short_description
 
     @property
     def long_description(self) -> Optional[str]:
-        return self.attributes.long_description
+        return None if self.attributes is None else self.attributes.long_description
 
     @long_description.setter
     def long_description(self, long_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.long_description = long_description
 
     @property
     def additional_attributes(self) -> Optional[dict[str, str]]:
-        return self.attributes.additional_attributes
+        return (
+            None if self.attributes is None else self.attributes.additional_attributes
+        )
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
     def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.terms
+        return None if self.attributes is None else self.attributes.terms
 
     @terms.setter
     def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.terms = terms
 
     @property
     def anchor(self) -> AtlasGlossary:
-        return self.attributes.anchor
+        return None if self.attributes is None else self.attributes.anchor
 
     @anchor.setter
     def anchor(self, anchor: AtlasGlossary):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.anchor = anchor
 
     @property
     def parent_category(self) -> Optional[AtlasGlossaryCategory]:
-        return self.attributes.parent_category
+        return None if self.attributes is None else self.attributes.parent_category
 
     @parent_category.setter
     def parent_category(self, parent_category: Optional[AtlasGlossaryCategory]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_category = parent_category
 
     @property
     def children_categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.children_categories
+        return None if self.attributes is None else self.attributes.children_categories
 
     @children_categories.setter
     def children_categories(
         self, children_categories: Optional[list[AtlasGlossaryCategory]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -2947,14 +3223,42 @@
         validate_required_fields(["name", "anchor"], [name, anchor])
         return cls(
             attributes=AtlasGlossaryCategory.Attributes.create(
                 name=name, anchor=anchor, parent_category=parent_category
             )
         )
 
+    def trim_to_required(self) -> AtlasGlossaryCategory:
+        if self.anchor is None or not self.anchor.guid:
+            raise ValueError("anchor.guid must be available")
+        return self.create_for_modification(
+            qualified_name=self.qualified_name,
+            name=self.name,
+            glossary_guid=self.anchor.guid,
+        )
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        glossary_guid: str = "",
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "glossary_guid"],
+            [name, qualified_name, glossary_guid],
+        )
+        glossary = AtlasGlossary()
+        glossary.guid = glossary_guid
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name, name=name, anchor=glossary
+            )
+        )
+
 
 class Badge(Asset, type_name="Badge"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Badge._convience_properties:
             return object.__setattr__(self, name, value)
@@ -2963,25 +3267,29 @@
     _convience_properties: ClassVar[list[str]] = [
         "badge_conditions",
         "badge_metadata_attribute",
     ]
 
     @property
     def badge_conditions(self) -> Optional[list[BadgeCondition]]:
-        return self.attributes.badge_conditions
+        return None if self.attributes is None else self.attributes.badge_conditions
 
     @badge_conditions.setter
     def badge_conditions(self, badge_conditions: Optional[list[BadgeCondition]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.badge_conditions = badge_conditions
 
     @property
     def badge_metadata_attribute(self) -> Optional[str]:
-        return self.attributes.badge_metadata_attribute
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.badge_metadata_attribute
+        )
 
     @badge_metadata_attribute.setter
     def badge_metadata_attribute(self, badge_metadata_attribute: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.badge_metadata_attribute = badge_metadata_attribute
 
@@ -3069,57 +3377,65 @@
         "deny_asset_tabs",
         "channel_link",
         "policies",
     ]
 
     @property
     def is_access_control_enabled(self) -> Optional[bool]:
-        return self.attributes.is_access_control_enabled
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.is_access_control_enabled
+        )
 
     @is_access_control_enabled.setter
     def is_access_control_enabled(self, is_access_control_enabled: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_access_control_enabled = is_access_control_enabled
 
     @property
     def deny_custom_metadata_guids(self) -> Optional[set[str]]:
-        return self.attributes.deny_custom_metadata_guids
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.deny_custom_metadata_guids
+        )
 
     @deny_custom_metadata_guids.setter
     def deny_custom_metadata_guids(
         self, deny_custom_metadata_guids: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.deny_custom_metadata_guids = deny_custom_metadata_guids
 
     @property
     def deny_asset_tabs(self) -> Optional[set[str]]:
-        return self.attributes.deny_asset_tabs
+        return None if self.attributes is None else self.attributes.deny_asset_tabs
 
     @deny_asset_tabs.setter
     def deny_asset_tabs(self, deny_asset_tabs: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.deny_asset_tabs = deny_asset_tabs
 
     @property
     def channel_link(self) -> Optional[str]:
-        return self.attributes.channel_link
+        return None if self.attributes is None else self.attributes.channel_link
 
     @channel_link.setter
     def channel_link(self, channel_link: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.channel_link = channel_link
 
     @property
     def policies(self) -> Optional[list[AuthPolicy]]:
-        return self.attributes.policies
+        return None if self.attributes is None else self.attributes.policies
 
     @policies.setter
     def policies(self, policies: Optional[list[AuthPolicy]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policies = policies
 
@@ -3164,25 +3480,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "children_queries",
         "children_folders",
     ]
 
     @property
     def children_queries(self) -> Optional[list[Query]]:
-        return self.attributes.children_queries
+        return None if self.attributes is None else self.attributes.children_queries
 
     @children_queries.setter
     def children_queries(self, children_queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.children_queries = children_queries
 
     @property
     def children_folders(self) -> Optional[list[Folder]]:
-        return self.attributes.children_folders
+        return None if self.attributes is None else self.attributes.children_folders
 
     @children_folders.setter
     def children_folders(self, children_folders: Optional[list[Folder]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.children_folders = children_folders
 
@@ -3220,25 +3536,27 @@
     _convience_properties: ClassVar[list[str]] = [
         "input_to_processes",
         "output_from_processes",
     ]
 
     @property
     def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
+        return None if self.attributes is None else self.attributes.input_to_processes
 
     @input_to_processes.setter
     def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.input_to_processes = input_to_processes
 
     @property
     def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
+        return (
+            None if self.attributes is None else self.attributes.output_from_processes
+        )
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
@@ -3281,75 +3599,77 @@
         "additional_attributes",
         "terms",
         "categories",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
-        return self.attributes.short_description
+        return None if self.attributes is None else self.attributes.short_description
 
     @short_description.setter
     def short_description(self, short_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.short_description = short_description
 
     @property
     def long_description(self) -> Optional[str]:
-        return self.attributes.long_description
+        return None if self.attributes is None else self.attributes.long_description
 
     @long_description.setter
     def long_description(self, long_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.long_description = long_description
 
     @property
     def language(self) -> Optional[str]:
-        return self.attributes.language
+        return None if self.attributes is None else self.attributes.language
 
     @language.setter
     def language(self, language: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.language = language
 
     @property
     def usage(self) -> Optional[str]:
-        return self.attributes.usage
+        return None if self.attributes is None else self.attributes.usage
 
     @usage.setter
     def usage(self, usage: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.usage = usage
 
     @property
     def additional_attributes(self) -> Optional[dict[str, str]]:
-        return self.attributes.additional_attributes
+        return (
+            None if self.attributes is None else self.attributes.additional_attributes
+        )
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
     def terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.terms
+        return None if self.attributes is None else self.attributes.terms
 
     @terms.setter
     def terms(self, terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.terms = terms
 
     @property
     def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.categories
+        return None if self.attributes is None else self.attributes.categories
 
     @categories.setter
     def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.categories = categories
 
@@ -3436,187 +3756,201 @@
         "policy_delegate_admin",
         "policy_conditions",
         "access_control",
     ]
 
     @property
     def policy_type(self) -> Optional[AuthPolicyType]:
-        return self.attributes.policy_type
+        return None if self.attributes is None else self.attributes.policy_type
 
     @policy_type.setter
     def policy_type(self, policy_type: Optional[AuthPolicyType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_type = policy_type
 
     @property
     def policy_service_name(self) -> Optional[str]:
-        return self.attributes.policy_service_name
+        return None if self.attributes is None else self.attributes.policy_service_name
 
     @policy_service_name.setter
     def policy_service_name(self, policy_service_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_service_name = policy_service_name
 
     @property
     def policy_category(self) -> Optional[str]:
-        return self.attributes.policy_category
+        return None if self.attributes is None else self.attributes.policy_category
 
     @policy_category.setter
     def policy_category(self, policy_category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_category = policy_category
 
     @property
     def policy_sub_category(self) -> Optional[str]:
-        return self.attributes.policy_sub_category
+        return None if self.attributes is None else self.attributes.policy_sub_category
 
     @policy_sub_category.setter
     def policy_sub_category(self, policy_sub_category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_sub_category = policy_sub_category
 
     @property
     def policy_users(self) -> Optional[set[str]]:
-        return self.attributes.policy_users
+        return None if self.attributes is None else self.attributes.policy_users
 
     @policy_users.setter
     def policy_users(self, policy_users: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_users = policy_users
 
     @property
     def policy_groups(self) -> Optional[set[str]]:
-        return self.attributes.policy_groups
+        return None if self.attributes is None else self.attributes.policy_groups
 
     @policy_groups.setter
     def policy_groups(self, policy_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_groups = policy_groups
 
     @property
     def policy_roles(self) -> Optional[set[str]]:
-        return self.attributes.policy_roles
+        return None if self.attributes is None else self.attributes.policy_roles
 
     @policy_roles.setter
     def policy_roles(self, policy_roles: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_roles = policy_roles
 
     @property
     def policy_actions(self) -> Optional[set[str]]:
-        return self.attributes.policy_actions
+        return None if self.attributes is None else self.attributes.policy_actions
 
     @policy_actions.setter
     def policy_actions(self, policy_actions: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_actions = policy_actions
 
     @property
     def policy_resources(self) -> Optional[set[str]]:
-        return self.attributes.policy_resources
+        return None if self.attributes is None else self.attributes.policy_resources
 
     @policy_resources.setter
     def policy_resources(self, policy_resources: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_resources = policy_resources
 
     @property
     def policy_resource_category(self) -> Optional[str]:
-        return self.attributes.policy_resource_category
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.policy_resource_category
+        )
 
     @policy_resource_category.setter
     def policy_resource_category(self, policy_resource_category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_resource_category = policy_resource_category
 
     @property
     def policy_priority(self) -> Optional[int]:
-        return self.attributes.policy_priority
+        return None if self.attributes is None else self.attributes.policy_priority
 
     @policy_priority.setter
     def policy_priority(self, policy_priority: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_priority = policy_priority
 
     @property
     def is_policy_enabled(self) -> Optional[bool]:
-        return self.attributes.is_policy_enabled
+        return None if self.attributes is None else self.attributes.is_policy_enabled
 
     @is_policy_enabled.setter
     def is_policy_enabled(self, is_policy_enabled: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_policy_enabled = is_policy_enabled
 
     @property
     def policy_mask_type(self) -> Optional[str]:
-        return self.attributes.policy_mask_type
+        return None if self.attributes is None else self.attributes.policy_mask_type
 
     @policy_mask_type.setter
     def policy_mask_type(self, policy_mask_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_mask_type = policy_mask_type
 
     @property
     def policy_validity_schedule(self) -> Optional[list[AuthPolicyValiditySchedule]]:
-        return self.attributes.policy_validity_schedule
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.policy_validity_schedule
+        )
 
     @policy_validity_schedule.setter
     def policy_validity_schedule(
         self, policy_validity_schedule: Optional[list[AuthPolicyValiditySchedule]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_validity_schedule = policy_validity_schedule
 
     @property
     def policy_resource_signature(self) -> Optional[str]:
-        return self.attributes.policy_resource_signature
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.policy_resource_signature
+        )
 
     @policy_resource_signature.setter
     def policy_resource_signature(self, policy_resource_signature: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_resource_signature = policy_resource_signature
 
     @property
     def policy_delegate_admin(self) -> Optional[bool]:
-        return self.attributes.policy_delegate_admin
+        return (
+            None if self.attributes is None else self.attributes.policy_delegate_admin
+        )
 
     @policy_delegate_admin.setter
     def policy_delegate_admin(self, policy_delegate_admin: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_delegate_admin = policy_delegate_admin
 
     @property
     def policy_conditions(self) -> Optional[list[AuthPolicyCondition]]:
-        return self.attributes.policy_conditions
+        return None if self.attributes is None else self.attributes.policy_conditions
 
     @policy_conditions.setter
     def policy_conditions(self, policy_conditions: Optional[list[AuthPolicyCondition]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.policy_conditions = policy_conditions
 
     @property
     def access_control(self) -> Optional[AccessControl]:
-        return self.attributes.access_control
+        return None if self.attributes is None else self.attributes.access_control
 
     @access_control.setter
     def access_control(self, access_control: Optional[AccessControl]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.access_control = access_control
 
@@ -3680,20 +4014,37 @@
         policy_conditions: Optional[list[AuthPolicyCondition]] = Field(
             None, description="", alias="policyConditions"
         )
         access_control: Optional[AccessControl] = Field(
             None, description="", alias="accessControl"
         )  # relationship
 
+        @classmethod
+        # @validate_arguments()
+        def create(cls, name: str) -> AuthPolicy.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["name"], [name])
+            return AuthPolicy.Attributes(
+                qualified_name=name, name=name, display_name=""
+            )
+
     attributes: "AuthPolicy.Attributes" = Field(
         default_factory=lambda: AuthPolicy.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str) -> AuthPolicy:
+        validate_required_fields(["name"], [name])
+        attributes = AuthPolicy.Attributes.create(name=name)
+        return cls(attributes=attributes)
+
 
 class ProcessExecution(Asset, type_name="ProcessExecution"):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in ProcessExecution._convience_properties:
             return object.__setattr__(self, name, value)
@@ -3741,225 +4092,227 @@
         "categories",
         "preferred_to_terms",
         "preferred_terms",
     ]
 
     @property
     def short_description(self) -> Optional[str]:
-        return self.attributes.short_description
+        return None if self.attributes is None else self.attributes.short_description
 
     @short_description.setter
     def short_description(self, short_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.short_description = short_description
 
     @property
     def long_description(self) -> Optional[str]:
-        return self.attributes.long_description
+        return None if self.attributes is None else self.attributes.long_description
 
     @long_description.setter
     def long_description(self, long_description: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.long_description = long_description
 
     @property
     def examples(self) -> Optional[set[str]]:
-        return self.attributes.examples
+        return None if self.attributes is None else self.attributes.examples
 
     @examples.setter
     def examples(self, examples: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.examples = examples
 
     @property
     def abbreviation(self) -> Optional[str]:
-        return self.attributes.abbreviation
+        return None if self.attributes is None else self.attributes.abbreviation
 
     @abbreviation.setter
     def abbreviation(self, abbreviation: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.abbreviation = abbreviation
 
     @property
     def usage(self) -> Optional[str]:
-        return self.attributes.usage
+        return None if self.attributes is None else self.attributes.usage
 
     @usage.setter
     def usage(self, usage: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.usage = usage
 
     @property
     def additional_attributes(self) -> Optional[dict[str, str]]:
-        return self.attributes.additional_attributes
+        return (
+            None if self.attributes is None else self.attributes.additional_attributes
+        )
 
     @additional_attributes.setter
     def additional_attributes(self, additional_attributes: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.additional_attributes = additional_attributes
 
     @property
     def translation_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.translation_terms
+        return None if self.attributes is None else self.attributes.translation_terms
 
     @translation_terms.setter
     def translation_terms(self, translation_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.translation_terms = translation_terms
 
     @property
     def valid_values_for(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.valid_values_for
+        return None if self.attributes is None else self.attributes.valid_values_for
 
     @valid_values_for.setter
     def valid_values_for(self, valid_values_for: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.valid_values_for = valid_values_for
 
     @property
     def synonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.synonyms
+        return None if self.attributes is None else self.attributes.synonyms
 
     @synonyms.setter
     def synonyms(self, synonyms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.synonyms = synonyms
 
     @property
     def replaced_by(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.replaced_by
+        return None if self.attributes is None else self.attributes.replaced_by
 
     @replaced_by.setter
     def replaced_by(self, replaced_by: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replaced_by = replaced_by
 
     @property
     def valid_values(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.valid_values
+        return None if self.attributes is None else self.attributes.valid_values
 
     @valid_values.setter
     def valid_values(self, valid_values: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.valid_values = valid_values
 
     @property
     def replacement_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.replacement_terms
+        return None if self.attributes is None else self.attributes.replacement_terms
 
     @replacement_terms.setter
     def replacement_terms(self, replacement_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.replacement_terms = replacement_terms
 
     @property
     def see_also(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.see_also
+        return None if self.attributes is None else self.attributes.see_also
 
     @see_also.setter
     def see_also(self, see_also: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.see_also = see_also
 
     @property
     def translated_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.translated_terms
+        return None if self.attributes is None else self.attributes.translated_terms
 
     @translated_terms.setter
     def translated_terms(self, translated_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.translated_terms = translated_terms
 
     @property
     def is_a(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.is_a
+        return None if self.attributes is None else self.attributes.is_a
 
     @is_a.setter
     def is_a(self, is_a: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_a = is_a
 
     @property
     def anchor(self) -> AtlasGlossary:
-        return self.attributes.anchor
+        return None if self.attributes is None else self.attributes.anchor
 
     @anchor.setter
     def anchor(self, anchor: AtlasGlossary):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.anchor = anchor
 
     @property
     def antonyms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.antonyms
+        return None if self.attributes is None else self.attributes.antonyms
 
     @antonyms.setter
     def antonyms(self, antonyms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.antonyms = antonyms
 
     @property
     def assigned_entities(self) -> Optional[list[Referenceable]]:
-        return self.attributes.assigned_entities
+        return None if self.attributes is None else self.attributes.assigned_entities
 
     @assigned_entities.setter
     def assigned_entities(self, assigned_entities: Optional[list[Referenceable]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.assigned_entities = assigned_entities
 
     @property
     def classifies(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.classifies
+        return None if self.attributes is None else self.attributes.classifies
 
     @classifies.setter
     def classifies(self, classifies: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.classifies = classifies
 
     @property
     def categories(self) -> Optional[list[AtlasGlossaryCategory]]:
-        return self.attributes.categories
+        return None if self.attributes is None else self.attributes.categories
 
     @categories.setter
     def categories(self, categories: Optional[list[AtlasGlossaryCategory]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.categories = categories
 
     @property
     def preferred_to_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.preferred_to_terms
+        return None if self.attributes is None else self.attributes.preferred_to_terms
 
     @preferred_to_terms.setter
     def preferred_to_terms(self, preferred_to_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preferred_to_terms = preferred_to_terms
 
     @property
     def preferred_terms(self) -> Optional[list[AtlasGlossaryTerm]]:
-        return self.attributes.preferred_terms
+        return None if self.attributes is None else self.attributes.preferred_terms
 
     @preferred_terms.setter
     def preferred_terms(self, preferred_terms: Optional[list[AtlasGlossaryTerm]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preferred_terms = preferred_terms
 
@@ -4096,14 +4449,23 @@
                 anchor=anchor,
                 glossary_qualified_name=glossary_qualified_name,
                 glossary_guid=glossary_guid,
                 categories=categories,
             )
         )
 
+    def trim_to_required(self) -> AtlasGlossaryTerm:
+        if self.anchor is None or not self.anchor.guid:
+            raise ValueError("anchor.guid must be available")
+        return self.create_for_modification(
+            qualified_name=self.qualified_name,
+            name=self.name,
+            glossary_guid=self.anchor.guid,
+        )
+
     @classmethod
     def create_for_modification(
         cls: type[SelfAsset],
         qualified_name: str = "",
         name: str = "",
         glossary_guid: str = "",
     ) -> SelfAsset:
@@ -4134,55 +4496,61 @@
         "auth_service_is_enabled",
         "auth_service_config",
         "auth_service_policy_last_sync",
     ]
 
     @property
     def auth_service_type(self) -> Optional[str]:
-        return self.attributes.auth_service_type
+        return None if self.attributes is None else self.attributes.auth_service_type
 
     @auth_service_type.setter
     def auth_service_type(self, auth_service_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.auth_service_type = auth_service_type
 
     @property
     def tag_service(self) -> Optional[str]:
-        return self.attributes.tag_service
+        return None if self.attributes is None else self.attributes.tag_service
 
     @tag_service.setter
     def tag_service(self, tag_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_service = tag_service
 
     @property
     def auth_service_is_enabled(self) -> Optional[bool]:
-        return self.attributes.auth_service_is_enabled
+        return (
+            None if self.attributes is None else self.attributes.auth_service_is_enabled
+        )
 
     @auth_service_is_enabled.setter
     def auth_service_is_enabled(self, auth_service_is_enabled: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.auth_service_is_enabled = auth_service_is_enabled
 
     @property
     def auth_service_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.auth_service_config
+        return None if self.attributes is None else self.attributes.auth_service_config
 
     @auth_service_config.setter
     def auth_service_config(self, auth_service_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.auth_service_config = auth_service_config
 
     @property
     def auth_service_policy_last_sync(self) -> Optional[int]:
-        return self.attributes.auth_service_policy_last_sync
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.auth_service_policy_last_sync
+        )
 
     @auth_service_policy_last_sync.setter
     def auth_service_policy_last_sync(
         self, auth_service_policy_last_sync: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -4267,25 +4635,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "outputs",
         "inputs",
     ]
 
     @property
     def outputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.outputs
+        return None if self.attributes is None else self.attributes.outputs
 
     @outputs.setter
     def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.outputs = outputs
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.inputs
+        return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
@@ -4324,35 +4692,35 @@
         "outputs",
         "process",
         "inputs",
     ]
 
     @property
     def outputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.outputs
+        return None if self.attributes is None else self.attributes.outputs
 
     @outputs.setter
     def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.outputs = outputs
 
     @property
     def process(self) -> Optional[Process]:
-        return self.attributes.process
+        return None if self.attributes is None else self.attributes.process
 
     @process.setter
     def process(self, process: Optional[Process]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.process = process
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.inputs
+        return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
@@ -4394,35 +4762,35 @@
         "persona_groups",
         "persona_users",
         "role_id",
     ]
 
     @property
     def persona_groups(self) -> Optional[set[str]]:
-        return self.attributes.persona_groups
+        return None if self.attributes is None else self.attributes.persona_groups
 
     @persona_groups.setter
     def persona_groups(self, persona_groups: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.persona_groups = persona_groups
 
     @property
     def persona_users(self) -> Optional[set[str]]:
-        return self.attributes.persona_users
+        return None if self.attributes is None else self.attributes.persona_users
 
     @persona_users.setter
     def persona_users(self, persona_users: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.persona_users = persona_users
 
     @property
     def role_id(self) -> Optional[str]:
-        return self.attributes.role_id
+        return None if self.attributes is None else self.attributes.role_id
 
     @role_id.setter
     def role_id(self, role_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.role_id = role_id
 
@@ -4439,20 +4807,148 @@
             None, description="", alias="personaGroups"
         )
         persona_users: Optional[set[str]] = Field(
             None, description="", alias="personaUsers"
         )
         role_id: Optional[str] = Field(None, description="", alias="roleId")
 
+        @classmethod
+        # @validate_arguments()
+        def create(cls, name: str) -> Persona.Attributes:
+            if not name:
+                raise ValueError("name cannot be blank")
+            validate_required_fields(["name"], [name])
+            return Persona.Attributes(
+                qualified_name=name,
+                name=name,
+                display_name=name,
+                is_access_control_enabled=True,
+                description="",
+            )
+
     attributes: "Persona.Attributes" = Field(
         default_factory=lambda: Persona.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str) -> Persona:
+        validate_required_fields(["name"], [name])
+        attributes = Persona.Attributes.create(name=name)
+        return cls(attributes=attributes)
+
+    @classmethod
+    # @validate_arguments()
+    def create_metadata_policy(
+        cls,
+        *,
+        name: str,
+        persona_id: str,
+        policy_type: AuthPolicyType,
+        actions: Set[PersonaMetadataAction],
+        connection_qualified_name: str,
+        resources: Set[str],
+    ) -> AuthPolicy:
+        validate_required_fields(
+            ["name", "persona_id", "policy_type", "actions", "resources"],
+            [name, persona_id, policy_type, actions, resources],
+        )
+        policy = AuthPolicy.create(name=name)
+        policy.policy_actions = {x.value for x in actions}
+        policy.policy_category = AuthPolicyCategory.PERSONA.value
+        policy.policy_type = policy_type
+        policy.connection_qualified_name = connection_qualified_name
+        policy.policy_resources = resources
+        policy.policy_resource_category = AuthPolicyResourceCategory.CUSTOM.value
+        policy.policy_service_name = "atlas"
+        policy.policy_sub_category = "metadata"
+        persona = Persona()
+        persona.guid = persona_id
+        policy.access_control = persona
+        return policy
+
+    @classmethod
+    # @validate_arguments()
+    def create_data_policy(
+        cls,
+        *,
+        name: str,
+        persona_id: str,
+        policy_type: AuthPolicyType,
+        connection_qualified_name: str,
+        resources: Set[str],
+    ) -> AuthPolicy:
+        validate_required_fields(
+            ["name", "persona_id", "policy_type", "resources"],
+            [name, persona_id, policy_type, resources],
+        )
+        policy = AuthPolicy.create(name=name)
+        policy.policy_actions = {DataAction.SELECT.value}
+        policy.policy_category = AuthPolicyCategory.PERSONA.value
+        policy.policy_type = policy_type
+        policy.connection_qualified_name = connection_qualified_name
+        policy.policy_resources = resources
+        policy.policy_resources.add("entity-type:*")
+        policy.policy_resource_category = AuthPolicyResourceCategory.ENTITY.value
+        policy.policy_service_name = "heka"
+        policy.policy_sub_category = "data"
+        persona = Persona()
+        persona.guid = persona_id
+        policy.access_control = persona
+        return policy
+
+    @classmethod
+    # @validate_arguments()
+    def create_glossary_policy(
+        cls,
+        *,
+        name: str,
+        persona_id: str,
+        policy_type: AuthPolicyType,
+        actions: Set[PersonaGlossaryAction],
+        resources: Set[str],
+    ) -> AuthPolicy:
+        validate_required_fields(
+            ["name", "persona_id", "policy_type", "actions", "resources"],
+            [name, persona_id, policy_type, actions, resources],
+        )
+        policy = AuthPolicy.create(name=name)
+        policy.policy_actions = {x.value for x in actions}
+        policy.policy_category = AuthPolicyCategory.PERSONA.value
+        policy.policy_type = policy_type
+        policy.policy_resources = resources
+        policy.policy_resource_category = AuthPolicyResourceCategory.CUSTOM.value
+        policy.policy_service_name = "atlas"
+        policy.policy_sub_category = "glossary"
+        persona = Persona()
+        persona.guid = persona_id
+        policy.access_control = persona
+        return policy
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        is_enabled: bool = True,
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "is_enabled"],
+            [name, qualified_name, is_enabled],
+        )
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name,
+                name=name,
+                is_access_control_enabled=is_enabled,
+            )
+        )
+
 
 class Purpose(AccessControl):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Purpose._convience_properties:
             return object.__setattr__(self, name, value)
@@ -4460,15 +4956,17 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "purpose_classifications",
     ]
 
     @property
     def purpose_classifications(self) -> Optional[set[str]]:
-        return self.attributes.purpose_classifications
+        return (
+            None if self.attributes is None else self.attributes.purpose_classifications
+        )
 
     @purpose_classifications.setter
     def purpose_classifications(self, purpose_classifications: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.purpose_classifications = purpose_classifications
 
@@ -4481,20 +4979,182 @@
         return v
 
     class Attributes(AccessControl.Attributes):
         purpose_classifications: Optional[set[str]] = Field(
             None, description="", alias="purposeClassifications"
         )
 
+        @classmethod
+        # @validate_arguments()
+        def create(cls, name: str, classifications: list[str]) -> Purpose.Attributes:
+            validate_required_fields(
+                ["name", "classifications"], [name, classifications]
+            )
+            return Purpose.Attributes(
+                qualified_name=name,
+                name=name,
+                display_name=name,
+                is_access_control_enabled=True,
+                description="",
+                purpose_classifications=classifications,
+            )
+
     attributes: "Purpose.Attributes" = Field(
         default_factory=lambda: Purpose.Attributes(),
         description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
         "type, so are described in the sub-types of this schema.\n",
     )
 
+    @classmethod
+    # @validate_arguments()
+    def create(cls, *, name: str, classifications: list[str]) -> Purpose:
+        validate_required_fields(["name", "classifications"], [name, classifications])
+        attributes = Purpose.Attributes.create(
+            name=name, classifications=classifications
+        )
+        return cls(attributes=attributes)
+
+    @classmethod
+    # @validate_arguments()
+    def create_metadata_policy(
+        cls,
+        *,
+        name: str,
+        purpose_id: str,
+        policy_type: AuthPolicyType,
+        actions: Set[PurposeMetadataAction],
+        policy_groups: Optional[Set[str]] = None,
+        policy_users: Optional[Set[str]] = None,
+        all_users: bool = False,
+    ) -> AuthPolicy:
+        validate_required_fields(
+            ["name", "purpose_id", "policy_type", "actions"],
+            [name, purpose_id, policy_type, actions],
+        )
+        target_found = False
+        policy = AuthPolicy.create(name=name)
+        policy.policy_actions = {x.value for x in actions}
+        policy.policy_category = AuthPolicyCategory.PURPOSE.value
+        policy.policy_type = policy_type
+        policy.policy_resource_category = AuthPolicyResourceCategory.TAG.value
+        policy.policy_service_name = "atlas_tag"
+        policy.policy_sub_category = "metadata"
+        purpose = Purpose()
+        purpose.guid = purpose_id
+        policy.access_control = purpose
+        if all_users:
+            target_found = True
+            policy.policy_groups = {"public"}
+        else:
+            if policy_groups:
+                from pyatlan.cache.group_cache import GroupCache
+
+                for group_alias in policy_groups:
+                    if not GroupCache.get_id_for_alias(group_alias):
+                        raise ValueError(
+                            f"Provided group name {group_alias} was not found in Atlan."
+                        )
+                target_found = True
+                policy.policy_groups = policy_groups
+            else:
+                policy.policy_groups = None
+            if policy_users:
+                from pyatlan.cache.user_cache import UserCache
+
+                for username in policy_users:
+                    if not UserCache.get_id_for_name(username):
+                        raise ValueError(
+                            f"Provided username {username} was not found in Atlan."
+                        )
+                target_found = True
+                policy.policy_users = policy_users
+            else:
+                policy.policy_users = None
+        if target_found:
+            return policy
+        else:
+            raise ValueError("No user or group specified for the policy.")
+
+    @classmethod
+    # @validate_arguments()
+    def create_data_policy(
+        cls,
+        *,
+        name: str,
+        purpose_id: str,
+        policy_type: AuthPolicyType,
+        policy_groups: Optional[Set[str]] = None,
+        policy_users: Optional[Set[str]] = None,
+        all_users: bool = False,
+    ) -> AuthPolicy:
+        validate_required_fields(
+            ["name", "purpose_id", "policy_type"], [name, purpose_id, policy_type]
+        )
+        policy = AuthPolicy.create(name=name)
+        policy.policy_actions = {DataAction.SELECT.value}
+        policy.policy_category = AuthPolicyCategory.PURPOSE.value
+        policy.policy_type = policy_type
+        policy.policy_resource_category = AuthPolicyResourceCategory.TAG.value
+        policy.policy_service_name = "atlas_tag"
+        policy.policy_sub_category = "data"
+        purpose = Purpose()
+        purpose.guid = purpose_id
+        policy.access_control = purpose
+        if all_users:
+            target_found = True
+            policy.policy_groups = {"public"}
+        else:
+            if policy_groups:
+                from pyatlan.cache.group_cache import GroupCache
+
+                for group_alias in policy_groups:
+                    if not GroupCache.get_id_for_alias(group_alias):
+                        raise ValueError(
+                            f"Provided group name {group_alias} was not found in Atlan."
+                        )
+                target_found = True
+                policy.policy_groups = policy_groups
+            else:
+                policy.policy_groups = None
+            if policy_users:
+                from pyatlan.cache.user_cache import UserCache
+
+                for username in policy_users:
+                    if not UserCache.get_id_for_name(username):
+                        raise ValueError(
+                            f"Provided username {username} was not found in Atlan."
+                        )
+                target_found = True
+                policy.policy_users = policy_users
+            else:
+                policy.policy_users = None
+        if target_found:
+            return policy
+        else:
+            raise ValueError("No user or group specified for the policy.")
+
+    @classmethod
+    def create_for_modification(
+        cls: type[SelfAsset],
+        qualified_name: str = "",
+        name: str = "",
+        is_enabled: bool = True,
+    ) -> SelfAsset:
+        validate_required_fields(
+            ["name", "qualified_name", "is_enabled"],
+            [name, qualified_name, is_enabled],
+        )
+        return cls(
+            attributes=cls.Attributes(
+                qualified_name=qualified_name,
+                name=name,
+                is_access_control_enabled=is_enabled,
+            )
+        )
+
 
 class Collection(Namespace):
     """Description"""
 
     def __setattr__(self, name, value):
         if name in Collection._convience_properties:
             return object.__setattr__(self, name, value)
@@ -4503,25 +5163,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
     ]
 
     @property
     def icon(self) -> Optional[str]:
-        return self.attributes.icon
+        return None if self.attributes is None else self.attributes.icon
 
     @icon.setter
     def icon(self, icon: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon = icon
 
     @property
     def icon_type(self) -> Optional[IconType]:
-        return self.attributes.icon_type
+        return None if self.attributes is None else self.attributes.icon_type
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
@@ -4556,35 +5216,41 @@
         "parent_qualified_name",
         "collection_qualified_name",
         "parent",
     ]
 
     @property
     def parent_qualified_name(self) -> str:
-        return self.attributes.parent_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.parent_qualified_name
+        )
 
     @parent_qualified_name.setter
     def parent_qualified_name(self, parent_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_qualified_name = parent_qualified_name
 
     @property
     def collection_qualified_name(self) -> str:
-        return self.attributes.collection_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.collection_qualified_name
+        )
 
     @collection_qualified_name.setter
     def collection_qualified_name(self, collection_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.collection_qualified_name = collection_qualified_name
 
     @property
     def parent(self) -> Namespace:
-        return self.attributes.parent
+        return None if self.attributes is None else self.attributes.parent
 
     @parent.setter
     def parent(self, parent: Namespace):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent = parent
 
@@ -4734,189 +5400,207 @@
         "dbt_tags",
         "dbt_connection_context",
         "dbt_semantic_layer_proxy_url",
     ]
 
     @property
     def dbt_alias(self) -> Optional[str]:
-        return self.attributes.dbt_alias
+        return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_alias = dbt_alias
 
     @property
     def dbt_meta(self) -> Optional[str]:
-        return self.attributes.dbt_meta
+        return None if self.attributes is None else self.attributes.dbt_meta
 
     @dbt_meta.setter
     def dbt_meta(self, dbt_meta: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_meta = dbt_meta
 
     @property
     def dbt_unique_id(self) -> Optional[str]:
-        return self.attributes.dbt_unique_id
+        return None if self.attributes is None else self.attributes.dbt_unique_id
 
     @dbt_unique_id.setter
     def dbt_unique_id(self, dbt_unique_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_unique_id = dbt_unique_id
 
     @property
     def dbt_account_name(self) -> Optional[str]:
-        return self.attributes.dbt_account_name
+        return None if self.attributes is None else self.attributes.dbt_account_name
 
     @dbt_account_name.setter
     def dbt_account_name(self, dbt_account_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_account_name = dbt_account_name
 
     @property
     def dbt_project_name(self) -> Optional[str]:
-        return self.attributes.dbt_project_name
+        return None if self.attributes is None else self.attributes.dbt_project_name
 
     @dbt_project_name.setter
     def dbt_project_name(self, dbt_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_project_name = dbt_project_name
 
     @property
     def dbt_package_name(self) -> Optional[str]:
-        return self.attributes.dbt_package_name
+        return None if self.attributes is None else self.attributes.dbt_package_name
 
     @dbt_package_name.setter
     def dbt_package_name(self, dbt_package_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_package_name = dbt_package_name
 
     @property
     def dbt_job_name(self) -> Optional[str]:
-        return self.attributes.dbt_job_name
+        return None if self.attributes is None else self.attributes.dbt_job_name
 
     @dbt_job_name.setter
     def dbt_job_name(self, dbt_job_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_name = dbt_job_name
 
     @property
     def dbt_job_schedule(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule
+        return None if self.attributes is None else self.attributes.dbt_job_schedule
 
     @dbt_job_schedule.setter
     def dbt_job_schedule(self, dbt_job_schedule: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule = dbt_job_schedule
 
     @property
     def dbt_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_job_status
+        return None if self.attributes is None else self.attributes.dbt_job_status
 
     @dbt_job_status.setter
     def dbt_job_status(self, dbt_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_status = dbt_job_status
 
     @property
     def dbt_job_schedule_cron_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule_cron_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_schedule_cron_humanized
+        )
 
     @dbt_job_schedule_cron_humanized.setter
     def dbt_job_schedule_cron_humanized(
         self, dbt_job_schedule_cron_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule_cron_humanized = (
             dbt_job_schedule_cron_humanized
         )
 
     @property
     def dbt_job_last_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_last_run
+        return None if self.attributes is None else self.attributes.dbt_job_last_run
 
     @dbt_job_last_run.setter
     def dbt_job_last_run(self, dbt_job_last_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_last_run = dbt_job_last_run
 
     @property
     def dbt_job_next_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_next_run
+        return None if self.attributes is None else self.attributes.dbt_job_next_run
 
     @dbt_job_next_run.setter
     def dbt_job_next_run(self, dbt_job_next_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run = dbt_job_next_run
 
     @property
     def dbt_job_next_run_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_next_run_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_next_run_humanized
+        )
 
     @dbt_job_next_run_humanized.setter
     def dbt_job_next_run_humanized(self, dbt_job_next_run_humanized: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run_humanized = dbt_job_next_run_humanized
 
     @property
     def dbt_environment_name(self) -> Optional[str]:
-        return self.attributes.dbt_environment_name
+        return None if self.attributes is None else self.attributes.dbt_environment_name
 
     @dbt_environment_name.setter
     def dbt_environment_name(self, dbt_environment_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_name = dbt_environment_name
 
     @property
     def dbt_environment_dbt_version(self) -> Optional[str]:
-        return self.attributes.dbt_environment_dbt_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_environment_dbt_version
+        )
 
     @dbt_environment_dbt_version.setter
     def dbt_environment_dbt_version(self, dbt_environment_dbt_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_dbt_version = dbt_environment_dbt_version
 
     @property
     def dbt_tags(self) -> Optional[set[str]]:
-        return self.attributes.dbt_tags
+        return None if self.attributes is None else self.attributes.dbt_tags
 
     @dbt_tags.setter
     def dbt_tags(self, dbt_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_tags = dbt_tags
 
     @property
     def dbt_connection_context(self) -> Optional[str]:
-        return self.attributes.dbt_connection_context
+        return (
+            None if self.attributes is None else self.attributes.dbt_connection_context
+        )
 
     @dbt_connection_context.setter
     def dbt_connection_context(self, dbt_connection_context: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_connection_context = dbt_connection_context
 
     @property
     def dbt_semantic_layer_proxy_url(self) -> Optional[str]:
-        return self.attributes.dbt_semantic_layer_proxy_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_semantic_layer_proxy_url
+        )
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
@@ -4994,45 +5678,45 @@
         "is_global",
         "reference",
         "resource_metadata",
     ]
 
     @property
     def link(self) -> Optional[str]:
-        return self.attributes.link
+        return None if self.attributes is None else self.attributes.link
 
     @link.setter
     def link(self, link: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.link = link
 
     @property
     def is_global(self) -> Optional[bool]:
-        return self.attributes.is_global
+        return None if self.attributes is None else self.attributes.is_global
 
     @is_global.setter
     def is_global(self, is_global: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_global = is_global
 
     @property
     def reference(self) -> Optional[str]:
-        return self.attributes.reference
+        return None if self.attributes is None else self.attributes.reference
 
     @reference.setter
     def reference(self, reference: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.reference = reference
 
     @property
     def resource_metadata(self) -> Optional[dict[str, str]]:
-        return self.attributes.resource_metadata
+        return None if self.attributes is None else self.attributes.resource_metadata
 
     @resource_metadata.setter
     def resource_metadata(self, resource_metadata: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.resource_metadata = resource_metadata
 
@@ -5093,65 +5777,67 @@
         "api_spec_qualified_name",
         "api_external_docs",
         "api_is_auth_optional",
     ]
 
     @property
     def api_spec_type(self) -> Optional[str]:
-        return self.attributes.api_spec_type
+        return None if self.attributes is None else self.attributes.api_spec_type
 
     @api_spec_type.setter
     def api_spec_type(self, api_spec_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_type = api_spec_type
 
     @property
     def api_spec_version(self) -> Optional[str]:
-        return self.attributes.api_spec_version
+        return None if self.attributes is None else self.attributes.api_spec_version
 
     @api_spec_version.setter
     def api_spec_version(self, api_spec_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_version = api_spec_version
 
     @property
     def api_spec_name(self) -> Optional[str]:
-        return self.attributes.api_spec_name
+        return None if self.attributes is None else self.attributes.api_spec_name
 
     @api_spec_name.setter
     def api_spec_name(self, api_spec_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_name = api_spec_name
 
     @property
     def api_spec_qualified_name(self) -> Optional[str]:
-        return self.attributes.api_spec_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.api_spec_qualified_name
+        )
 
     @api_spec_qualified_name.setter
     def api_spec_qualified_name(self, api_spec_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_qualified_name = api_spec_qualified_name
 
     @property
     def api_external_docs(self) -> Optional[dict[str, str]]:
-        return self.attributes.api_external_docs
+        return None if self.attributes is None else self.attributes.api_external_docs
 
     @api_external_docs.setter
     def api_external_docs(self, api_external_docs: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_external_docs = api_external_docs
 
     @property
     def api_is_auth_optional(self) -> Optional[bool]:
-        return self.attributes.api_is_auth_optional
+        return None if self.attributes is None else self.attributes.api_is_auth_optional
 
     @api_is_auth_optional.setter
     def api_is_auth_optional(self, api_is_auth_optional: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_is_auth_optional = api_is_auth_optional
 
@@ -5199,45 +5885,49 @@
         "tag_attributes",
         "tag_allowed_values",
         "mapped_classification_name",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
-        return self.attributes.tag_id
+        return None if self.attributes is None else self.attributes.tag_id
 
     @tag_id.setter
     def tag_id(self, tag_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_id = tag_id
 
     @property
     def tag_attributes(self) -> Optional[list[SourceTagAttribute]]:
-        return self.attributes.tag_attributes
+        return None if self.attributes is None else self.attributes.tag_attributes
 
     @tag_attributes.setter
     def tag_attributes(self, tag_attributes: Optional[list[SourceTagAttribute]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_attributes = tag_attributes
 
     @property
     def tag_allowed_values(self) -> Optional[set[str]]:
-        return self.attributes.tag_allowed_values
+        return None if self.attributes is None else self.attributes.tag_allowed_values
 
     @tag_allowed_values.setter
     def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_allowed_values = tag_allowed_values
 
     @property
     def mapped_classification_name(self) -> Optional[str]:
-        return self.attributes.mapped_classification_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mapped_classification_name
+        )
 
     @mapped_classification_name.setter
     def mapped_classification_name(self, mapped_classification_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mapped_classification_name = mapped_classification_name
 
@@ -5295,185 +5985,191 @@
         "sql_dbt_models",
         "sql_dbt_sources",
         "dbt_models",
     ]
 
     @property
     def query_count(self) -> Optional[int]:
-        return self.attributes.query_count
+        return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_count = query_count
 
     @property
     def query_user_count(self) -> Optional[int]:
-        return self.attributes.query_user_count
+        return None if self.attributes is None else self.attributes.query_user_count
 
     @query_user_count.setter
     def query_user_count(self, query_user_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_user_count = query_user_count
 
     @property
     def query_user_map(self) -> Optional[dict[str, int]]:
-        return self.attributes.query_user_map
+        return None if self.attributes is None else self.attributes.query_user_map
 
     @query_user_map.setter
     def query_user_map(self, query_user_map: Optional[dict[str, int]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_user_map = query_user_map
 
     @property
     def query_count_updated_at(self) -> Optional[datetime]:
-        return self.attributes.query_count_updated_at
+        return (
+            None if self.attributes is None else self.attributes.query_count_updated_at
+        )
 
     @query_count_updated_at.setter
     def query_count_updated_at(self, query_count_updated_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_count_updated_at = query_count_updated_at
 
     @property
     def database_name(self) -> Optional[str]:
-        return self.attributes.database_name
+        return None if self.attributes is None else self.attributes.database_name
 
     @database_name.setter
     def database_name(self, database_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.database_name = database_name
 
     @property
     def database_qualified_name(self) -> Optional[str]:
-        return self.attributes.database_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.database_qualified_name
+        )
 
     @database_qualified_name.setter
     def database_qualified_name(self, database_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.database_qualified_name = database_qualified_name
 
     @property
     def schema_name(self) -> Optional[str]:
-        return self.attributes.schema_name
+        return None if self.attributes is None else self.attributes.schema_name
 
     @schema_name.setter
     def schema_name(self, schema_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_name = schema_name
 
     @property
     def schema_qualified_name(self) -> Optional[str]:
-        return self.attributes.schema_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.schema_qualified_name
+        )
 
     @schema_qualified_name.setter
     def schema_qualified_name(self, schema_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_qualified_name = schema_qualified_name
 
     @property
     def table_name(self) -> Optional[str]:
-        return self.attributes.table_name
+        return None if self.attributes is None else self.attributes.table_name
 
     @table_name.setter
     def table_name(self, table_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_name = table_name
 
     @property
     def table_qualified_name(self) -> Optional[str]:
-        return self.attributes.table_qualified_name
+        return None if self.attributes is None else self.attributes.table_qualified_name
 
     @table_qualified_name.setter
     def table_qualified_name(self, table_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_qualified_name = table_qualified_name
 
     @property
     def view_name(self) -> Optional[str]:
-        return self.attributes.view_name
+        return None if self.attributes is None else self.attributes.view_name
 
     @view_name.setter
     def view_name(self, view_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_name = view_name
 
     @property
     def view_qualified_name(self) -> Optional[str]:
-        return self.attributes.view_qualified_name
+        return None if self.attributes is None else self.attributes.view_qualified_name
 
     @view_qualified_name.setter
     def view_qualified_name(self, view_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_qualified_name = view_qualified_name
 
     @property
     def is_profiled(self) -> Optional[bool]:
-        return self.attributes.is_profiled
+        return None if self.attributes is None else self.attributes.is_profiled
 
     @is_profiled.setter
     def is_profiled(self, is_profiled: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_profiled = is_profiled
 
     @property
     def last_profiled_at(self) -> Optional[datetime]:
-        return self.attributes.last_profiled_at
+        return None if self.attributes is None else self.attributes.last_profiled_at
 
     @last_profiled_at.setter
     def last_profiled_at(self, last_profiled_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_profiled_at = last_profiled_at
 
     @property
     def dbt_sources(self) -> Optional[list[DbtSource]]:
-        return self.attributes.dbt_sources
+        return None if self.attributes is None else self.attributes.dbt_sources
 
     @dbt_sources.setter
     def dbt_sources(self, dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_sources = dbt_sources
 
     @property
     def sql_dbt_models(self) -> Optional[list[DbtModel]]:
-        return self.attributes.sql_dbt_models
+        return None if self.attributes is None else self.attributes.sql_dbt_models
 
     @sql_dbt_models.setter
     def sql_dbt_models(self, sql_dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_dbt_models = sql_dbt_models
 
     @property
     def sql_dbt_sources(self) -> Optional[list[DbtSource]]:
-        return self.attributes.sql_dbt_sources
+        return None if self.attributes is None else self.attributes.sql_dbt_sources
 
     @sql_dbt_sources.setter
     def sql_dbt_sources(self, sql_dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_dbt_sources = sql_dbt_sources
 
     @property
     def dbt_models(self) -> Optional[list[DbtModel]]:
-        return self.attributes.dbt_models
+        return None if self.attributes is None else self.attributes.dbt_models
 
     @dbt_models.setter
     def dbt_models(self, dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_models = dbt_models
 
@@ -5553,85 +6249,87 @@
         "google_location_type",
         "google_labels",
         "google_tags",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
+        return None if self.attributes is None else self.attributes.google_service
 
     @google_service.setter
     def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_service = google_service
 
     @property
     def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
+        return None if self.attributes is None else self.attributes.google_project_name
 
     @google_project_name.setter
     def google_project_name(self, google_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_name = google_project_name
 
     @property
     def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
+        return None if self.attributes is None else self.attributes.google_project_id
 
     @google_project_id.setter
     def google_project_id(self, google_project_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_id = google_project_id
 
     @property
     def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
+        return (
+            None if self.attributes is None else self.attributes.google_project_number
+        )
 
     @google_project_number.setter
     def google_project_number(self, google_project_number: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_number = google_project_number
 
     @property
     def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
+        return None if self.attributes is None else self.attributes.google_location
 
     @google_location.setter
     def google_location(self, google_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location = google_location
 
     @property
     def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
+        return None if self.attributes is None else self.attributes.google_location_type
 
     @google_location_type.setter
     def google_location_type(self, google_location_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location_type = google_location_type
 
     @property
     def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
+        return None if self.attributes is None else self.attributes.google_labels
 
     @google_labels.setter
     def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_labels = google_labels
 
     @property
     def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
+        return None if self.attributes is None else self.attributes.google_tags
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
@@ -5689,49 +6387,53 @@
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
     ]
 
     @property
     def azure_resource_id(self) -> Optional[str]:
-        return self.attributes.azure_resource_id
+        return None if self.attributes is None else self.attributes.azure_resource_id
 
     @azure_resource_id.setter
     def azure_resource_id(self, azure_resource_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_resource_id = azure_resource_id
 
     @property
     def azure_location(self) -> Optional[str]:
-        return self.attributes.azure_location
+        return None if self.attributes is None else self.attributes.azure_location
 
     @azure_location.setter
     def azure_location(self, azure_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_location = azure_location
 
     @property
     def adls_account_secondary_location(self) -> Optional[str]:
-        return self.attributes.adls_account_secondary_location
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_secondary_location
+        )
 
     @adls_account_secondary_location.setter
     def adls_account_secondary_location(
         self, adls_account_secondary_location: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_secondary_location = (
             adls_account_secondary_location
         )
 
     @property
     def azure_tags(self) -> Optional[list[AzureTag]]:
-        return self.attributes.azure_tags
+        return None if self.attributes is None else self.attributes.azure_tags
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
@@ -5782,95 +6484,95 @@
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
     ]
 
     @property
     def aws_arn(self) -> Optional[str]:
-        return self.attributes.aws_arn
+        return None if self.attributes is None else self.attributes.aws_arn
 
     @aws_arn.setter
     def aws_arn(self, aws_arn: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_arn = aws_arn
 
     @property
     def aws_partition(self) -> Optional[str]:
-        return self.attributes.aws_partition
+        return None if self.attributes is None else self.attributes.aws_partition
 
     @aws_partition.setter
     def aws_partition(self, aws_partition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_partition = aws_partition
 
     @property
     def aws_service(self) -> Optional[str]:
-        return self.attributes.aws_service
+        return None if self.attributes is None else self.attributes.aws_service
 
     @aws_service.setter
     def aws_service(self, aws_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_service = aws_service
 
     @property
     def aws_region(self) -> Optional[str]:
-        return self.attributes.aws_region
+        return None if self.attributes is None else self.attributes.aws_region
 
     @aws_region.setter
     def aws_region(self, aws_region: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_region = aws_region
 
     @property
     def aws_account_id(self) -> Optional[str]:
-        return self.attributes.aws_account_id
+        return None if self.attributes is None else self.attributes.aws_account_id
 
     @aws_account_id.setter
     def aws_account_id(self, aws_account_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_account_id = aws_account_id
 
     @property
     def aws_resource_id(self) -> Optional[str]:
-        return self.attributes.aws_resource_id
+        return None if self.attributes is None else self.attributes.aws_resource_id
 
     @aws_resource_id.setter
     def aws_resource_id(self, aws_resource_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_resource_id = aws_resource_id
 
     @property
     def aws_owner_name(self) -> Optional[str]:
-        return self.attributes.aws_owner_name
+        return None if self.attributes is None else self.attributes.aws_owner_name
 
     @aws_owner_name.setter
     def aws_owner_name(self, aws_owner_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_owner_name = aws_owner_name
 
     @property
     def aws_owner_id(self) -> Optional[str]:
-        return self.attributes.aws_owner_id
+        return None if self.attributes is None else self.attributes.aws_owner_id
 
     @aws_owner_id.setter
     def aws_owner_id(self, aws_owner_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_owner_id = aws_owner_id
 
     @property
     def aws_tags(self) -> Optional[list[AwsTag]]:
-        return self.attributes.aws_tags
+        return None if self.attributes is None else self.attributes.aws_tags
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
@@ -5941,271 +6643,293 @@
         "ast",
         "process",
         "column_processes",
     ]
 
     @property
     def dbt_column_process_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_column_process_job_status
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_column_process_job_status
+        )
 
     @dbt_column_process_job_status.setter
     def dbt_column_process_job_status(
         self, dbt_column_process_job_status: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_column_process_job_status = dbt_column_process_job_status
 
     @property
     def dbt_alias(self) -> Optional[str]:
-        return self.attributes.dbt_alias
+        return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_alias = dbt_alias
 
     @property
     def dbt_meta(self) -> Optional[str]:
-        return self.attributes.dbt_meta
+        return None if self.attributes is None else self.attributes.dbt_meta
 
     @dbt_meta.setter
     def dbt_meta(self, dbt_meta: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_meta = dbt_meta
 
     @property
     def dbt_unique_id(self) -> Optional[str]:
-        return self.attributes.dbt_unique_id
+        return None if self.attributes is None else self.attributes.dbt_unique_id
 
     @dbt_unique_id.setter
     def dbt_unique_id(self, dbt_unique_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_unique_id = dbt_unique_id
 
     @property
     def dbt_account_name(self) -> Optional[str]:
-        return self.attributes.dbt_account_name
+        return None if self.attributes is None else self.attributes.dbt_account_name
 
     @dbt_account_name.setter
     def dbt_account_name(self, dbt_account_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_account_name = dbt_account_name
 
     @property
     def dbt_project_name(self) -> Optional[str]:
-        return self.attributes.dbt_project_name
+        return None if self.attributes is None else self.attributes.dbt_project_name
 
     @dbt_project_name.setter
     def dbt_project_name(self, dbt_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_project_name = dbt_project_name
 
     @property
     def dbt_package_name(self) -> Optional[str]:
-        return self.attributes.dbt_package_name
+        return None if self.attributes is None else self.attributes.dbt_package_name
 
     @dbt_package_name.setter
     def dbt_package_name(self, dbt_package_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_package_name = dbt_package_name
 
     @property
     def dbt_job_name(self) -> Optional[str]:
-        return self.attributes.dbt_job_name
+        return None if self.attributes is None else self.attributes.dbt_job_name
 
     @dbt_job_name.setter
     def dbt_job_name(self, dbt_job_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_name = dbt_job_name
 
     @property
     def dbt_job_schedule(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule
+        return None if self.attributes is None else self.attributes.dbt_job_schedule
 
     @dbt_job_schedule.setter
     def dbt_job_schedule(self, dbt_job_schedule: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule = dbt_job_schedule
 
     @property
     def dbt_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_job_status
+        return None if self.attributes is None else self.attributes.dbt_job_status
 
     @dbt_job_status.setter
     def dbt_job_status(self, dbt_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_status = dbt_job_status
 
     @property
     def dbt_job_schedule_cron_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule_cron_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_schedule_cron_humanized
+        )
 
     @dbt_job_schedule_cron_humanized.setter
     def dbt_job_schedule_cron_humanized(
         self, dbt_job_schedule_cron_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule_cron_humanized = (
             dbt_job_schedule_cron_humanized
         )
 
     @property
     def dbt_job_last_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_last_run
+        return None if self.attributes is None else self.attributes.dbt_job_last_run
 
     @dbt_job_last_run.setter
     def dbt_job_last_run(self, dbt_job_last_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_last_run = dbt_job_last_run
 
     @property
     def dbt_job_next_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_next_run
+        return None if self.attributes is None else self.attributes.dbt_job_next_run
 
     @dbt_job_next_run.setter
     def dbt_job_next_run(self, dbt_job_next_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run = dbt_job_next_run
 
     @property
     def dbt_job_next_run_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_next_run_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_next_run_humanized
+        )
 
     @dbt_job_next_run_humanized.setter
     def dbt_job_next_run_humanized(self, dbt_job_next_run_humanized: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run_humanized = dbt_job_next_run_humanized
 
     @property
     def dbt_environment_name(self) -> Optional[str]:
-        return self.attributes.dbt_environment_name
+        return None if self.attributes is None else self.attributes.dbt_environment_name
 
     @dbt_environment_name.setter
     def dbt_environment_name(self, dbt_environment_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_name = dbt_environment_name
 
     @property
     def dbt_environment_dbt_version(self) -> Optional[str]:
-        return self.attributes.dbt_environment_dbt_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_environment_dbt_version
+        )
 
     @dbt_environment_dbt_version.setter
     def dbt_environment_dbt_version(self, dbt_environment_dbt_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_dbt_version = dbt_environment_dbt_version
 
     @property
     def dbt_tags(self) -> Optional[set[str]]:
-        return self.attributes.dbt_tags
+        return None if self.attributes is None else self.attributes.dbt_tags
 
     @dbt_tags.setter
     def dbt_tags(self, dbt_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_tags = dbt_tags
 
     @property
     def dbt_connection_context(self) -> Optional[str]:
-        return self.attributes.dbt_connection_context
+        return (
+            None if self.attributes is None else self.attributes.dbt_connection_context
+        )
 
     @dbt_connection_context.setter
     def dbt_connection_context(self, dbt_connection_context: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_connection_context = dbt_connection_context
 
     @property
     def dbt_semantic_layer_proxy_url(self) -> Optional[str]:
-        return self.attributes.dbt_semantic_layer_proxy_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_semantic_layer_proxy_url
+        )
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.inputs
+        return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
     @property
     def outputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.outputs
+        return None if self.attributes is None else self.attributes.outputs
 
     @outputs.setter
     def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.outputs = outputs
 
     @property
     def code(self) -> Optional[str]:
-        return self.attributes.code
+        return None if self.attributes is None else self.attributes.code
 
     @code.setter
     def code(self, code: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.code = code
 
     @property
     def sql(self) -> Optional[str]:
-        return self.attributes.sql
+        return None if self.attributes is None else self.attributes.sql
 
     @sql.setter
     def sql(self, sql: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql = sql
 
     @property
     def ast(self) -> Optional[str]:
-        return self.attributes.ast
+        return None if self.attributes is None else self.attributes.ast
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
     def process(self) -> Optional[Process]:
-        return self.attributes.process
+        return None if self.attributes is None else self.attributes.process
 
     @process.setter
     def process(self, process: Optional[Process]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.process = process
 
     @property
     def column_processes(self) -> Optional[list[ColumnProcess]]:
-        return self.attributes.column_processes
+        return None if self.attributes is None else self.attributes.column_processes
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
@@ -6323,115 +7047,115 @@
         "aws_owner_name",
         "aws_owner_id",
         "aws_tags",
     ]
 
     @property
     def s3_e_tag(self) -> Optional[str]:
-        return self.attributes.s3_e_tag
+        return None if self.attributes is None else self.attributes.s3_e_tag
 
     @s3_e_tag.setter
     def s3_e_tag(self, s3_e_tag: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_e_tag = s3_e_tag
 
     @property
     def s3_encryption(self) -> Optional[str]:
-        return self.attributes.s3_encryption
+        return None if self.attributes is None else self.attributes.s3_encryption
 
     @s3_encryption.setter
     def s3_encryption(self, s3_encryption: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_encryption = s3_encryption
 
     @property
     def aws_arn(self) -> Optional[str]:
-        return self.attributes.aws_arn
+        return None if self.attributes is None else self.attributes.aws_arn
 
     @aws_arn.setter
     def aws_arn(self, aws_arn: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_arn = aws_arn
 
     @property
     def aws_partition(self) -> Optional[str]:
-        return self.attributes.aws_partition
+        return None if self.attributes is None else self.attributes.aws_partition
 
     @aws_partition.setter
     def aws_partition(self, aws_partition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_partition = aws_partition
 
     @property
     def aws_service(self) -> Optional[str]:
-        return self.attributes.aws_service
+        return None if self.attributes is None else self.attributes.aws_service
 
     @aws_service.setter
     def aws_service(self, aws_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_service = aws_service
 
     @property
     def aws_region(self) -> Optional[str]:
-        return self.attributes.aws_region
+        return None if self.attributes is None else self.attributes.aws_region
 
     @aws_region.setter
     def aws_region(self, aws_region: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_region = aws_region
 
     @property
     def aws_account_id(self) -> Optional[str]:
-        return self.attributes.aws_account_id
+        return None if self.attributes is None else self.attributes.aws_account_id
 
     @aws_account_id.setter
     def aws_account_id(self, aws_account_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_account_id = aws_account_id
 
     @property
     def aws_resource_id(self) -> Optional[str]:
-        return self.attributes.aws_resource_id
+        return None if self.attributes is None else self.attributes.aws_resource_id
 
     @aws_resource_id.setter
     def aws_resource_id(self, aws_resource_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_resource_id = aws_resource_id
 
     @property
     def aws_owner_name(self) -> Optional[str]:
-        return self.attributes.aws_owner_name
+        return None if self.attributes is None else self.attributes.aws_owner_name
 
     @aws_owner_name.setter
     def aws_owner_name(self, aws_owner_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_owner_name = aws_owner_name
 
     @property
     def aws_owner_id(self) -> Optional[str]:
-        return self.attributes.aws_owner_id
+        return None if self.attributes is None else self.attributes.aws_owner_id
 
     @aws_owner_id.setter
     def aws_owner_id(self, aws_owner_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_owner_id = aws_owner_id
 
     @property
     def aws_tags(self) -> Optional[list[AwsTag]]:
-        return self.attributes.aws_tags
+        return None if self.attributes is None else self.attributes.aws_tags
 
     @aws_tags.setter
     def aws_tags(self, aws_tags: Optional[list[AwsTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.aws_tags = aws_tags
 
@@ -6483,59 +7207,67 @@
         "azure_location",
         "adls_account_secondary_location",
         "azure_tags",
     ]
 
     @property
     def adls_account_qualified_name(self) -> Optional[str]:
-        return self.attributes.adls_account_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_qualified_name
+        )
 
     @adls_account_qualified_name.setter
     def adls_account_qualified_name(self, adls_account_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_qualified_name = adls_account_qualified_name
 
     @property
     def azure_resource_id(self) -> Optional[str]:
-        return self.attributes.azure_resource_id
+        return None if self.attributes is None else self.attributes.azure_resource_id
 
     @azure_resource_id.setter
     def azure_resource_id(self, azure_resource_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_resource_id = azure_resource_id
 
     @property
     def azure_location(self) -> Optional[str]:
-        return self.attributes.azure_location
+        return None if self.attributes is None else self.attributes.azure_location
 
     @azure_location.setter
     def azure_location(self, azure_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_location = azure_location
 
     @property
     def adls_account_secondary_location(self) -> Optional[str]:
-        return self.attributes.adls_account_secondary_location
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_secondary_location
+        )
 
     @adls_account_secondary_location.setter
     def adls_account_secondary_location(
         self, adls_account_secondary_location: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_secondary_location = (
             adls_account_secondary_location
         )
 
     @property
     def azure_tags(self) -> Optional[list[AzureTag]]:
-        return self.attributes.azure_tags
+        return None if self.attributes is None else self.attributes.azure_tags
 
     @azure_tags.setter
     def azure_tags(self, azure_tags: Optional[list[AzureTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_tags = azure_tags
 
@@ -6596,165 +7328,171 @@
         "google_tags",
         "input_to_processes",
         "output_from_processes",
     ]
 
     @property
     def gcs_storage_class(self) -> Optional[str]:
-        return self.attributes.gcs_storage_class
+        return None if self.attributes is None else self.attributes.gcs_storage_class
 
     @gcs_storage_class.setter
     def gcs_storage_class(self, gcs_storage_class: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_storage_class = gcs_storage_class
 
     @property
     def gcs_encryption_type(self) -> Optional[str]:
-        return self.attributes.gcs_encryption_type
+        return None if self.attributes is None else self.attributes.gcs_encryption_type
 
     @gcs_encryption_type.setter
     def gcs_encryption_type(self, gcs_encryption_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_encryption_type = gcs_encryption_type
 
     @property
     def gcs_e_tag(self) -> Optional[str]:
-        return self.attributes.gcs_e_tag
+        return None if self.attributes is None else self.attributes.gcs_e_tag
 
     @gcs_e_tag.setter
     def gcs_e_tag(self, gcs_e_tag: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_e_tag = gcs_e_tag
 
     @property
     def gcs_requester_pays(self) -> Optional[bool]:
-        return self.attributes.gcs_requester_pays
+        return None if self.attributes is None else self.attributes.gcs_requester_pays
 
     @gcs_requester_pays.setter
     def gcs_requester_pays(self, gcs_requester_pays: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_requester_pays = gcs_requester_pays
 
     @property
     def gcs_access_control(self) -> Optional[str]:
-        return self.attributes.gcs_access_control
+        return None if self.attributes is None else self.attributes.gcs_access_control
 
     @gcs_access_control.setter
     def gcs_access_control(self, gcs_access_control: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_access_control = gcs_access_control
 
     @property
     def gcs_meta_generation_id(self) -> Optional[int]:
-        return self.attributes.gcs_meta_generation_id
+        return (
+            None if self.attributes is None else self.attributes.gcs_meta_generation_id
+        )
 
     @gcs_meta_generation_id.setter
     def gcs_meta_generation_id(self, gcs_meta_generation_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_meta_generation_id = gcs_meta_generation_id
 
     @property
     def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
+        return None if self.attributes is None else self.attributes.google_service
 
     @google_service.setter
     def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_service = google_service
 
     @property
     def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
+        return None if self.attributes is None else self.attributes.google_project_name
 
     @google_project_name.setter
     def google_project_name(self, google_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_name = google_project_name
 
     @property
     def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
+        return None if self.attributes is None else self.attributes.google_project_id
 
     @google_project_id.setter
     def google_project_id(self, google_project_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_id = google_project_id
 
     @property
     def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
+        return (
+            None if self.attributes is None else self.attributes.google_project_number
+        )
 
     @google_project_number.setter
     def google_project_number(self, google_project_number: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_number = google_project_number
 
     @property
     def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
+        return None if self.attributes is None else self.attributes.google_location
 
     @google_location.setter
     def google_location(self, google_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location = google_location
 
     @property
     def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
+        return None if self.attributes is None else self.attributes.google_location_type
 
     @google_location_type.setter
     def google_location_type(self, google_location_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location_type = google_location_type
 
     @property
     def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
+        return None if self.attributes is None else self.attributes.google_labels
 
     @google_labels.setter
     def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_labels = google_labels
 
     @property
     def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
+        return None if self.attributes is None else self.attributes.google_tags
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
     @property
     def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
+        return None if self.attributes is None else self.attributes.input_to_processes
 
     @input_to_processes.setter
     def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.input_to_processes = input_to_processes
 
     @property
     def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
+        return (
+            None if self.attributes is None else self.attributes.output_from_processes
+        )
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
@@ -6832,25 +7570,29 @@
     _convience_properties: ClassVar[list[str]] = [
         "mc_labels",
         "mc_asset_qualified_names",
     ]
 
     @property
     def mc_labels(self) -> Optional[set[str]]:
-        return self.attributes.mc_labels
+        return None if self.attributes is None else self.attributes.mc_labels
 
     @mc_labels.setter
     def mc_labels(self, mc_labels: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_labels = mc_labels
 
     @property
     def mc_asset_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.mc_asset_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_asset_qualified_names
+        )
 
     @mc_asset_qualified_names.setter
     def mc_asset_qualified_names(self, mc_asset_qualified_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_asset_qualified_names = mc_asset_qualified_names
 
@@ -6891,77 +7633,83 @@
         "assets",
         "metric_dimension_columns",
         "metric_timestamp_column",
     ]
 
     @property
     def metric_type(self) -> Optional[str]:
-        return self.attributes.metric_type
+        return None if self.attributes is None else self.attributes.metric_type
 
     @metric_type.setter
     def metric_type(self, metric_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_type = metric_type
 
     @property
     def metric_s_q_l(self) -> Optional[str]:
-        return self.attributes.metric_s_q_l
+        return None if self.attributes is None else self.attributes.metric_s_q_l
 
     @metric_s_q_l.setter
     def metric_s_q_l(self, metric_s_q_l: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_s_q_l = metric_s_q_l
 
     @property
     def metric_filters(self) -> Optional[str]:
-        return self.attributes.metric_filters
+        return None if self.attributes is None else self.attributes.metric_filters
 
     @metric_filters.setter
     def metric_filters(self, metric_filters: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_filters = metric_filters
 
     @property
     def metric_time_grains(self) -> Optional[set[str]]:
-        return self.attributes.metric_time_grains
+        return None if self.attributes is None else self.attributes.metric_time_grains
 
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
     @property
     def assets(self) -> Optional[list[Asset]]:
-        return self.attributes.assets
+        return None if self.attributes is None else self.attributes.assets
 
     @assets.setter
     def assets(self, assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.assets = assets
 
     @property
     def metric_dimension_columns(self) -> Optional[list[Column]]:
-        return self.attributes.metric_dimension_columns
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metric_dimension_columns
+        )
 
     @metric_dimension_columns.setter
     def metric_dimension_columns(
         self, metric_dimension_columns: Optional[list[Column]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_dimension_columns = metric_dimension_columns
 
     @property
     def metric_timestamp_column(self) -> Optional[Column]:
-        return self.attributes.metric_timestamp_column
+        return (
+            None if self.attributes is None else self.attributes.metric_timestamp_column
+        )
 
     @metric_timestamp_column.setter
     def metric_timestamp_column(self, metric_timestamp_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_timestamp_column = metric_timestamp_column
 
@@ -7012,49 +7760,57 @@
         "preset_workspace_qualified_name",
         "preset_dashboard_id",
         "preset_dashboard_qualified_name",
     ]
 
     @property
     def preset_workspace_id(self) -> Optional[int]:
-        return self.attributes.preset_workspace_id
+        return None if self.attributes is None else self.attributes.preset_workspace_id
 
     @preset_workspace_id.setter
     def preset_workspace_id(self, preset_workspace_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_id = preset_workspace_id
 
     @property
     def preset_workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.preset_workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_qualified_name
+        )
 
     @preset_workspace_qualified_name.setter
     def preset_workspace_qualified_name(
         self, preset_workspace_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_qualified_name = (
             preset_workspace_qualified_name
         )
 
     @property
     def preset_dashboard_id(self) -> Optional[int]:
-        return self.attributes.preset_dashboard_id
+        return None if self.attributes is None else self.attributes.preset_dashboard_id
 
     @preset_dashboard_id.setter
     def preset_dashboard_id(self, preset_dashboard_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_id = preset_dashboard_id
 
     @property
     def preset_dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.preset_dashboard_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_qualified_name
+        )
 
     @preset_dashboard_qualified_name.setter
     def preset_dashboard_qualified_name(
         self, preset_dashboard_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -7109,97 +7865,111 @@
         "mode_report_qualified_name",
         "mode_query_name",
         "mode_query_qualified_name",
     ]
 
     @property
     def mode_id(self) -> Optional[str]:
-        return self.attributes.mode_id
+        return None if self.attributes is None else self.attributes.mode_id
 
     @mode_id.setter
     def mode_id(self, mode_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_id = mode_id
 
     @property
     def mode_token(self) -> Optional[str]:
-        return self.attributes.mode_token
+        return None if self.attributes is None else self.attributes.mode_token
 
     @mode_token.setter
     def mode_token(self, mode_token: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_token = mode_token
 
     @property
     def mode_workspace_name(self) -> Optional[str]:
-        return self.attributes.mode_workspace_name
+        return None if self.attributes is None else self.attributes.mode_workspace_name
 
     @mode_workspace_name.setter
     def mode_workspace_name(self, mode_workspace_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_workspace_name = mode_workspace_name
 
     @property
     def mode_workspace_username(self) -> Optional[str]:
-        return self.attributes.mode_workspace_username
+        return (
+            None if self.attributes is None else self.attributes.mode_workspace_username
+        )
 
     @mode_workspace_username.setter
     def mode_workspace_username(self, mode_workspace_username: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_workspace_username = mode_workspace_username
 
     @property
     def mode_workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mode_workspace_qualified_name
+        )
 
     @mode_workspace_qualified_name.setter
     def mode_workspace_qualified_name(
         self, mode_workspace_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_workspace_qualified_name = mode_workspace_qualified_name
 
     @property
     def mode_report_name(self) -> Optional[str]:
-        return self.attributes.mode_report_name
+        return None if self.attributes is None else self.attributes.mode_report_name
 
     @mode_report_name.setter
     def mode_report_name(self, mode_report_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_name = mode_report_name
 
     @property
     def mode_report_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_report_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mode_report_qualified_name
+        )
 
     @mode_report_qualified_name.setter
     def mode_report_qualified_name(self, mode_report_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_qualified_name = mode_report_qualified_name
 
     @property
     def mode_query_name(self) -> Optional[str]:
-        return self.attributes.mode_query_name
+        return None if self.attributes is None else self.attributes.mode_query_name
 
     @mode_query_name.setter
     def mode_query_name(self, mode_query_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_name = mode_query_name
 
     @property
     def mode_query_qualified_name(self) -> Optional[str]:
-        return self.attributes.mode_query_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mode_query_qualified_name
+        )
 
     @mode_query_qualified_name.setter
     def mode_query_qualified_name(self, mode_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_qualified_name = mode_query_qualified_name
 
@@ -7258,71 +8028,85 @@
         "sigma_page_name",
         "sigma_data_element_qualified_name",
         "sigma_data_element_name",
     ]
 
     @property
     def sigma_workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_workbook_qualified_name
+        )
 
     @sigma_workbook_qualified_name.setter
     def sigma_workbook_qualified_name(
         self, sigma_workbook_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_workbook_qualified_name = sigma_workbook_qualified_name
 
     @property
     def sigma_workbook_name(self) -> Optional[str]:
-        return self.attributes.sigma_workbook_name
+        return None if self.attributes is None else self.attributes.sigma_workbook_name
 
     @sigma_workbook_name.setter
     def sigma_workbook_name(self, sigma_workbook_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_workbook_name = sigma_workbook_name
 
     @property
     def sigma_page_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_page_qualified_name
+        )
 
     @sigma_page_qualified_name.setter
     def sigma_page_qualified_name(self, sigma_page_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page_qualified_name = sigma_page_qualified_name
 
     @property
     def sigma_page_name(self) -> Optional[str]:
-        return self.attributes.sigma_page_name
+        return None if self.attributes is None else self.attributes.sigma_page_name
 
     @sigma_page_name.setter
     def sigma_page_name(self, sigma_page_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page_name = sigma_page_name
 
     @property
     def sigma_data_element_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_qualified_name
+        )
 
     @sigma_data_element_qualified_name.setter
     def sigma_data_element_qualified_name(
         self, sigma_data_element_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_qualified_name = (
             sigma_data_element_qualified_name
         )
 
     @property
     def sigma_data_element_name(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_name
+        return (
+            None if self.attributes is None else self.attributes.sigma_data_element_name
+        )
 
     @sigma_data_element_name.setter
     def sigma_data_element_name(self, sigma_data_element_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_name = sigma_data_element_name
 
@@ -7409,15 +8193,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_is_published",
     ]
 
     @property
     def redash_is_published(self) -> Optional[bool]:
-        return self.attributes.redash_is_published
+        return None if self.attributes is None else self.attributes.redash_is_published
 
     @redash_is_published.setter
     def redash_is_published(self, redash_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_is_published = redash_is_published
 
@@ -7460,105 +8244,109 @@
         "google_tags",
         "input_to_processes",
         "output_from_processes",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
+        return None if self.attributes is None else self.attributes.google_service
 
     @google_service.setter
     def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_service = google_service
 
     @property
     def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
+        return None if self.attributes is None else self.attributes.google_project_name
 
     @google_project_name.setter
     def google_project_name(self, google_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_name = google_project_name
 
     @property
     def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
+        return None if self.attributes is None else self.attributes.google_project_id
 
     @google_project_id.setter
     def google_project_id(self, google_project_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_id = google_project_id
 
     @property
     def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
+        return (
+            None if self.attributes is None else self.attributes.google_project_number
+        )
 
     @google_project_number.setter
     def google_project_number(self, google_project_number: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_number = google_project_number
 
     @property
     def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
+        return None if self.attributes is None else self.attributes.google_location
 
     @google_location.setter
     def google_location(self, google_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location = google_location
 
     @property
     def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
+        return None if self.attributes is None else self.attributes.google_location_type
 
     @google_location_type.setter
     def google_location_type(self, google_location_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location_type = google_location_type
 
     @property
     def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
+        return None if self.attributes is None else self.attributes.google_labels
 
     @google_labels.setter
     def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_labels = google_labels
 
     @property
     def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
+        return None if self.attributes is None else self.attributes.google_tags
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
     @property
     def input_to_processes(self) -> Optional[list[Process]]:
-        return self.attributes.input_to_processes
+        return None if self.attributes is None else self.attributes.input_to_processes
 
     @input_to_processes.setter
     def input_to_processes(self, input_to_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.input_to_processes = input_to_processes
 
     @property
     def output_from_processes(self) -> Optional[list[Process]]:
-        return self.attributes.output_from_processes
+        return (
+            None if self.attributes is None else self.attributes.output_from_processes
+        )
 
     @output_from_processes.setter
     def output_from_processes(self, output_from_processes: Optional[list[Process]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_processes = output_from_processes
 
@@ -7620,25 +8408,33 @@
     _convience_properties: ClassVar[list[str]] = [
         "metabase_collection_name",
         "metabase_collection_qualified_name",
     ]
 
     @property
     def metabase_collection_name(self) -> Optional[str]:
-        return self.attributes.metabase_collection_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metabase_collection_name
+        )
 
     @metabase_collection_name.setter
     def metabase_collection_name(self, metabase_collection_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection_name = metabase_collection_name
 
     @property
     def metabase_collection_qualified_name(self) -> Optional[str]:
-        return self.attributes.metabase_collection_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metabase_collection_qualified_name
+        )
 
     @metabase_collection_qualified_name.setter
     def metabase_collection_qualified_name(
         self, metabase_collection_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -7681,35 +8477,37 @@
         "quick_sight_id",
         "quick_sight_sheet_id",
         "quick_sight_sheet_name",
     ]
 
     @property
     def quick_sight_id(self) -> Optional[str]:
-        return self.attributes.quick_sight_id
+        return None if self.attributes is None else self.attributes.quick_sight_id
 
     @quick_sight_id.setter
     def quick_sight_id(self, quick_sight_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_id = quick_sight_id
 
     @property
     def quick_sight_sheet_id(self) -> Optional[str]:
-        return self.attributes.quick_sight_sheet_id
+        return None if self.attributes is None else self.attributes.quick_sight_sheet_id
 
     @quick_sight_sheet_id.setter
     def quick_sight_sheet_id(self, quick_sight_sheet_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_sheet_id = quick_sight_sheet_id
 
     @property
     def quick_sight_sheet_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_sheet_name
+        return (
+            None if self.attributes is None else self.attributes.quick_sight_sheet_name
+        )
 
     @quick_sight_sheet_name.setter
     def quick_sight_sheet_name(self, quick_sight_sheet_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_sheet_name = quick_sight_sheet_name
 
@@ -7750,25 +8548,31 @@
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_chart_type",
         "thoughtspot_question_text",
     ]
 
     @property
     def thoughtspot_chart_type(self) -> Optional[str]:
-        return self.attributes.thoughtspot_chart_type
+        return (
+            None if self.attributes is None else self.attributes.thoughtspot_chart_type
+        )
 
     @thoughtspot_chart_type.setter
     def thoughtspot_chart_type(self, thoughtspot_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_chart_type = thoughtspot_chart_type
 
     @property
     def thoughtspot_question_text(self) -> Optional[str]:
-        return self.attributes.thoughtspot_question_text
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.thoughtspot_question_text
+        )
 
     @thoughtspot_question_text.setter
     def thoughtspot_question_text(self, thoughtspot_question_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_question_text = thoughtspot_question_text
 
@@ -7808,47 +8612,55 @@
         "power_b_i_table_qualified_name",
         "power_b_i_format_string",
         "power_b_i_endorsement",
     ]
 
     @property
     def power_b_i_is_hidden(self) -> Optional[bool]:
-        return self.attributes.power_b_i_is_hidden
+        return None if self.attributes is None else self.attributes.power_b_i_is_hidden
 
     @power_b_i_is_hidden.setter
     def power_b_i_is_hidden(self, power_b_i_is_hidden: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_is_hidden = power_b_i_is_hidden
 
     @property
     def power_b_i_table_qualified_name(self) -> Optional[str]:
-        return self.attributes.power_b_i_table_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_table_qualified_name
+        )
 
     @power_b_i_table_qualified_name.setter
     def power_b_i_table_qualified_name(
         self, power_b_i_table_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_qualified_name = power_b_i_table_qualified_name
 
     @property
     def power_b_i_format_string(self) -> Optional[str]:
-        return self.attributes.power_b_i_format_string
+        return (
+            None if self.attributes is None else self.attributes.power_b_i_format_string
+        )
 
     @power_b_i_format_string.setter
     def power_b_i_format_string(self, power_b_i_format_string: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_format_string = power_b_i_format_string
 
     @property
     def power_b_i_endorsement(self) -> Optional[PowerbiEndorsement]:
-        return self.attributes.power_b_i_endorsement
+        return (
+            None if self.attributes is None else self.attributes.power_b_i_endorsement
+        )
 
     @power_b_i_endorsement.setter
     def power_b_i_endorsement(
         self, power_b_i_endorsement: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -7902,121 +8714,159 @@
         "micro_strategy_certified_by",
         "micro_strategy_certified_at",
         "micro_strategy_location",
     ]
 
     @property
     def micro_strategy_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.micro_strategy_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_project_qualified_name
+        )
 
     @micro_strategy_project_qualified_name.setter
     def micro_strategy_project_qualified_name(
         self, micro_strategy_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project_qualified_name = (
             micro_strategy_project_qualified_name
         )
 
     @property
     def micro_strategy_project_name(self) -> Optional[str]:
-        return self.attributes.micro_strategy_project_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_project_name
+        )
 
     @micro_strategy_project_name.setter
     def micro_strategy_project_name(self, micro_strategy_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project_name = micro_strategy_project_name
 
     @property
     def micro_strategy_cube_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_cube_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_cube_qualified_names
+        )
 
     @micro_strategy_cube_qualified_names.setter
     def micro_strategy_cube_qualified_names(
         self, micro_strategy_cube_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cube_qualified_names = (
             micro_strategy_cube_qualified_names
         )
 
     @property
     def micro_strategy_cube_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_cube_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_cube_names
+        )
 
     @micro_strategy_cube_names.setter
     def micro_strategy_cube_names(self, micro_strategy_cube_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cube_names = micro_strategy_cube_names
 
     @property
     def micro_strategy_report_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_report_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_report_qualified_names
+        )
 
     @micro_strategy_report_qualified_names.setter
     def micro_strategy_report_qualified_names(
         self, micro_strategy_report_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_report_qualified_names = (
             micro_strategy_report_qualified_names
         )
 
     @property
     def micro_strategy_report_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_report_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_report_names
+        )
 
     @micro_strategy_report_names.setter
     def micro_strategy_report_names(
         self, micro_strategy_report_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_report_names = micro_strategy_report_names
 
     @property
     def micro_strategy_is_certified(self) -> Optional[bool]:
-        return self.attributes.micro_strategy_is_certified
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_is_certified
+        )
 
     @micro_strategy_is_certified.setter
     def micro_strategy_is_certified(self, micro_strategy_is_certified: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_is_certified = micro_strategy_is_certified
 
     @property
     def micro_strategy_certified_by(self) -> Optional[str]:
-        return self.attributes.micro_strategy_certified_by
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_certified_by
+        )
 
     @micro_strategy_certified_by.setter
     def micro_strategy_certified_by(self, micro_strategy_certified_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_certified_by = micro_strategy_certified_by
 
     @property
     def micro_strategy_certified_at(self) -> Optional[datetime]:
-        return self.attributes.micro_strategy_certified_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_certified_at
+        )
 
     @micro_strategy_certified_at.setter
     def micro_strategy_certified_at(
         self, micro_strategy_certified_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_certified_at = micro_strategy_certified_at
 
     @property
     def micro_strategy_location(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.micro_strategy_location
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_location
+        )
 
     @micro_strategy_location.setter
     def micro_strategy_location(
         self, micro_strategy_location: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -8086,85 +8936,91 @@
         "qlik_app_qualified_name",
         "qlik_owner_id",
         "qlik_is_published",
     ]
 
     @property
     def qlik_id(self) -> Optional[str]:
-        return self.attributes.qlik_id
+        return None if self.attributes is None else self.attributes.qlik_id
 
     @qlik_id.setter
     def qlik_id(self, qlik_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_id = qlik_id
 
     @property
     def qlik_q_r_i(self) -> Optional[str]:
-        return self.attributes.qlik_q_r_i
+        return None if self.attributes is None else self.attributes.qlik_q_r_i
 
     @qlik_q_r_i.setter
     def qlik_q_r_i(self, qlik_q_r_i: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_q_r_i = qlik_q_r_i
 
     @property
     def qlik_space_id(self) -> Optional[str]:
-        return self.attributes.qlik_space_id
+        return None if self.attributes is None else self.attributes.qlik_space_id
 
     @qlik_space_id.setter
     def qlik_space_id(self, qlik_space_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space_id = qlik_space_id
 
     @property
     def qlik_space_qualified_name(self) -> Optional[str]:
-        return self.attributes.qlik_space_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.qlik_space_qualified_name
+        )
 
     @qlik_space_qualified_name.setter
     def qlik_space_qualified_name(self, qlik_space_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space_qualified_name = qlik_space_qualified_name
 
     @property
     def qlik_app_id(self) -> Optional[str]:
-        return self.attributes.qlik_app_id
+        return None if self.attributes is None else self.attributes.qlik_app_id
 
     @qlik_app_id.setter
     def qlik_app_id(self, qlik_app_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app_id = qlik_app_id
 
     @property
     def qlik_app_qualified_name(self) -> Optional[str]:
-        return self.attributes.qlik_app_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.qlik_app_qualified_name
+        )
 
     @qlik_app_qualified_name.setter
     def qlik_app_qualified_name(self, qlik_app_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app_qualified_name = qlik_app_qualified_name
 
     @property
     def qlik_owner_id(self) -> Optional[str]:
-        return self.attributes.qlik_owner_id
+        return None if self.attributes is None else self.attributes.qlik_owner_id
 
     @qlik_owner_id.setter
     def qlik_owner_id(self, qlik_owner_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_owner_id = qlik_owner_id
 
     @property
     def qlik_is_published(self) -> Optional[bool]:
-        return self.attributes.qlik_is_published
+        return None if self.attributes is None else self.attributes.qlik_is_published
 
     @qlik_is_published.setter
     def qlik_is_published(self, qlik_is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_published = qlik_is_published
 
@@ -8210,25 +9066,29 @@
     _convience_properties: ClassVar[list[str]] = [
         "organization_qualified_name",
         "api_name",
     ]
 
     @property
     def organization_qualified_name(self) -> Optional[str]:
-        return self.attributes.organization_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.organization_qualified_name
+        )
 
     @organization_qualified_name.setter
     def organization_qualified_name(self, organization_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.organization_qualified_name = organization_qualified_name
 
     @property
     def api_name(self) -> Optional[str]:
-        return self.attributes.api_name
+        return None if self.attributes is None else self.attributes.api_name
 
     @api_name.setter
     def api_name(self, api_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_name = api_name
 
@@ -8268,67 +9128,81 @@
         "dbt_model_column_sql_columns",
         "sql_column",
         "dbt_model",
     ]
 
     @property
     def dbt_model_qualified_name(self) -> Optional[str]:
-        return self.attributes.dbt_model_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_qualified_name
+        )
 
     @dbt_model_qualified_name.setter
     def dbt_model_qualified_name(self, dbt_model_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_qualified_name = dbt_model_qualified_name
 
     @property
     def dbt_model_column_data_type(self) -> Optional[str]:
-        return self.attributes.dbt_model_column_data_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_column_data_type
+        )
 
     @dbt_model_column_data_type.setter
     def dbt_model_column_data_type(self, dbt_model_column_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_column_data_type = dbt_model_column_data_type
 
     @property
     def dbt_model_column_order(self) -> Optional[int]:
-        return self.attributes.dbt_model_column_order
+        return (
+            None if self.attributes is None else self.attributes.dbt_model_column_order
+        )
 
     @dbt_model_column_order.setter
     def dbt_model_column_order(self, dbt_model_column_order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_column_order = dbt_model_column_order
 
     @property
     def dbt_model_column_sql_columns(self) -> Optional[list[Column]]:
-        return self.attributes.dbt_model_column_sql_columns
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_column_sql_columns
+        )
 
     @dbt_model_column_sql_columns.setter
     def dbt_model_column_sql_columns(
         self, dbt_model_column_sql_columns: Optional[list[Column]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_column_sql_columns = dbt_model_column_sql_columns
 
     @property
     def sql_column(self) -> Optional[Column]:
-        return self.attributes.sql_column
+        return None if self.attributes is None else self.attributes.sql_column
 
     @sql_column.setter
     def sql_column(self, sql_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_column = sql_column
 
     @property
     def dbt_model(self) -> Optional[DbtModel]:
-        return self.attributes.dbt_model
+        return None if self.attributes is None else self.attributes.dbt_model
 
     @dbt_model.setter
     def dbt_model(self, dbt_model: Optional[DbtModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model = dbt_model
 
@@ -8393,185 +9267,217 @@
         "dbt_model_sql_assets",
         "dbt_model_columns",
         "sql_asset",
     ]
 
     @property
     def dbt_status(self) -> Optional[str]:
-        return self.attributes.dbt_status
+        return None if self.attributes is None else self.attributes.dbt_status
 
     @dbt_status.setter
     def dbt_status(self, dbt_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_status = dbt_status
 
     @property
     def dbt_error(self) -> Optional[str]:
-        return self.attributes.dbt_error
+        return None if self.attributes is None else self.attributes.dbt_error
 
     @dbt_error.setter
     def dbt_error(self, dbt_error: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_error = dbt_error
 
     @property
     def dbt_raw_s_q_l(self) -> Optional[str]:
-        return self.attributes.dbt_raw_s_q_l
+        return None if self.attributes is None else self.attributes.dbt_raw_s_q_l
 
     @dbt_raw_s_q_l.setter
     def dbt_raw_s_q_l(self, dbt_raw_s_q_l: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_raw_s_q_l = dbt_raw_s_q_l
 
     @property
     def dbt_compiled_s_q_l(self) -> Optional[str]:
-        return self.attributes.dbt_compiled_s_q_l
+        return None if self.attributes is None else self.attributes.dbt_compiled_s_q_l
 
     @dbt_compiled_s_q_l.setter
     def dbt_compiled_s_q_l(self, dbt_compiled_s_q_l: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_compiled_s_q_l = dbt_compiled_s_q_l
 
     @property
     def dbt_stats(self) -> Optional[str]:
-        return self.attributes.dbt_stats
+        return None if self.attributes is None else self.attributes.dbt_stats
 
     @dbt_stats.setter
     def dbt_stats(self, dbt_stats: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_stats = dbt_stats
 
     @property
     def dbt_materialization_type(self) -> Optional[str]:
-        return self.attributes.dbt_materialization_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_materialization_type
+        )
 
     @dbt_materialization_type.setter
     def dbt_materialization_type(self, dbt_materialization_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_materialization_type = dbt_materialization_type
 
     @property
     def dbt_model_compile_started_at(self) -> Optional[datetime]:
-        return self.attributes.dbt_model_compile_started_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_compile_started_at
+        )
 
     @dbt_model_compile_started_at.setter
     def dbt_model_compile_started_at(
         self, dbt_model_compile_started_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_compile_started_at = dbt_model_compile_started_at
 
     @property
     def dbt_model_compile_completed_at(self) -> Optional[datetime]:
-        return self.attributes.dbt_model_compile_completed_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_compile_completed_at
+        )
 
     @dbt_model_compile_completed_at.setter
     def dbt_model_compile_completed_at(
         self, dbt_model_compile_completed_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_compile_completed_at = dbt_model_compile_completed_at
 
     @property
     def dbt_model_execute_started_at(self) -> Optional[datetime]:
-        return self.attributes.dbt_model_execute_started_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_execute_started_at
+        )
 
     @dbt_model_execute_started_at.setter
     def dbt_model_execute_started_at(
         self, dbt_model_execute_started_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_execute_started_at = dbt_model_execute_started_at
 
     @property
     def dbt_model_execute_completed_at(self) -> Optional[datetime]:
-        return self.attributes.dbt_model_execute_completed_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_execute_completed_at
+        )
 
     @dbt_model_execute_completed_at.setter
     def dbt_model_execute_completed_at(
         self, dbt_model_execute_completed_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_execute_completed_at = dbt_model_execute_completed_at
 
     @property
     def dbt_model_execution_time(self) -> Optional[float]:
-        return self.attributes.dbt_model_execution_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_execution_time
+        )
 
     @dbt_model_execution_time.setter
     def dbt_model_execution_time(self, dbt_model_execution_time: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_execution_time = dbt_model_execution_time
 
     @property
     def dbt_model_run_generated_at(self) -> Optional[datetime]:
-        return self.attributes.dbt_model_run_generated_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_run_generated_at
+        )
 
     @dbt_model_run_generated_at.setter
     def dbt_model_run_generated_at(
         self, dbt_model_run_generated_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_run_generated_at = dbt_model_run_generated_at
 
     @property
     def dbt_model_run_elapsed_time(self) -> Optional[float]:
-        return self.attributes.dbt_model_run_elapsed_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_model_run_elapsed_time
+        )
 
     @dbt_model_run_elapsed_time.setter
     def dbt_model_run_elapsed_time(self, dbt_model_run_elapsed_time: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_run_elapsed_time = dbt_model_run_elapsed_time
 
     @property
     def dbt_metrics(self) -> Optional[list[DbtMetric]]:
-        return self.attributes.dbt_metrics
+        return None if self.attributes is None else self.attributes.dbt_metrics
 
     @dbt_metrics.setter
     def dbt_metrics(self, dbt_metrics: Optional[list[DbtMetric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_metrics = dbt_metrics
 
     @property
     def dbt_model_sql_assets(self) -> Optional[list[SQL]]:
-        return self.attributes.dbt_model_sql_assets
+        return None if self.attributes is None else self.attributes.dbt_model_sql_assets
 
     @dbt_model_sql_assets.setter
     def dbt_model_sql_assets(self, dbt_model_sql_assets: Optional[list[SQL]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_sql_assets = dbt_model_sql_assets
 
     @property
     def dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
-        return self.attributes.dbt_model_columns
+        return None if self.attributes is None else self.attributes.dbt_model_columns
 
     @dbt_model_columns.setter
     def dbt_model_columns(self, dbt_model_columns: Optional[list[DbtModelColumn]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_columns = dbt_model_columns
 
     @property
     def sql_asset(self) -> Optional[SQL]:
-        return self.attributes.sql_asset
+        return None if self.attributes is None else self.attributes.sql_asset
 
     @sql_asset.setter
     def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_asset = sql_asset
 
@@ -8672,291 +9578,319 @@
         "assets",
         "metric_dimension_columns",
         "dbt_metric_filter_columns",
     ]
 
     @property
     def dbt_metric_filters(self) -> Optional[list[DbtMetricFilter]]:
-        return self.attributes.dbt_metric_filters
+        return None if self.attributes is None else self.attributes.dbt_metric_filters
 
     @dbt_metric_filters.setter
     def dbt_metric_filters(self, dbt_metric_filters: Optional[list[DbtMetricFilter]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_metric_filters = dbt_metric_filters
 
     @property
     def dbt_alias(self) -> Optional[str]:
-        return self.attributes.dbt_alias
+        return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_alias = dbt_alias
 
     @property
     def dbt_meta(self) -> Optional[str]:
-        return self.attributes.dbt_meta
+        return None if self.attributes is None else self.attributes.dbt_meta
 
     @dbt_meta.setter
     def dbt_meta(self, dbt_meta: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_meta = dbt_meta
 
     @property
     def dbt_unique_id(self) -> Optional[str]:
-        return self.attributes.dbt_unique_id
+        return None if self.attributes is None else self.attributes.dbt_unique_id
 
     @dbt_unique_id.setter
     def dbt_unique_id(self, dbt_unique_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_unique_id = dbt_unique_id
 
     @property
     def dbt_account_name(self) -> Optional[str]:
-        return self.attributes.dbt_account_name
+        return None if self.attributes is None else self.attributes.dbt_account_name
 
     @dbt_account_name.setter
     def dbt_account_name(self, dbt_account_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_account_name = dbt_account_name
 
     @property
     def dbt_project_name(self) -> Optional[str]:
-        return self.attributes.dbt_project_name
+        return None if self.attributes is None else self.attributes.dbt_project_name
 
     @dbt_project_name.setter
     def dbt_project_name(self, dbt_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_project_name = dbt_project_name
 
     @property
     def dbt_package_name(self) -> Optional[str]:
-        return self.attributes.dbt_package_name
+        return None if self.attributes is None else self.attributes.dbt_package_name
 
     @dbt_package_name.setter
     def dbt_package_name(self, dbt_package_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_package_name = dbt_package_name
 
     @property
     def dbt_job_name(self) -> Optional[str]:
-        return self.attributes.dbt_job_name
+        return None if self.attributes is None else self.attributes.dbt_job_name
 
     @dbt_job_name.setter
     def dbt_job_name(self, dbt_job_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_name = dbt_job_name
 
     @property
     def dbt_job_schedule(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule
+        return None if self.attributes is None else self.attributes.dbt_job_schedule
 
     @dbt_job_schedule.setter
     def dbt_job_schedule(self, dbt_job_schedule: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule = dbt_job_schedule
 
     @property
     def dbt_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_job_status
+        return None if self.attributes is None else self.attributes.dbt_job_status
 
     @dbt_job_status.setter
     def dbt_job_status(self, dbt_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_status = dbt_job_status
 
     @property
     def dbt_job_schedule_cron_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule_cron_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_schedule_cron_humanized
+        )
 
     @dbt_job_schedule_cron_humanized.setter
     def dbt_job_schedule_cron_humanized(
         self, dbt_job_schedule_cron_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule_cron_humanized = (
             dbt_job_schedule_cron_humanized
         )
 
     @property
     def dbt_job_last_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_last_run
+        return None if self.attributes is None else self.attributes.dbt_job_last_run
 
     @dbt_job_last_run.setter
     def dbt_job_last_run(self, dbt_job_last_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_last_run = dbt_job_last_run
 
     @property
     def dbt_job_next_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_next_run
+        return None if self.attributes is None else self.attributes.dbt_job_next_run
 
     @dbt_job_next_run.setter
     def dbt_job_next_run(self, dbt_job_next_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run = dbt_job_next_run
 
     @property
     def dbt_job_next_run_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_next_run_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_next_run_humanized
+        )
 
     @dbt_job_next_run_humanized.setter
     def dbt_job_next_run_humanized(self, dbt_job_next_run_humanized: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run_humanized = dbt_job_next_run_humanized
 
     @property
     def dbt_environment_name(self) -> Optional[str]:
-        return self.attributes.dbt_environment_name
+        return None if self.attributes is None else self.attributes.dbt_environment_name
 
     @dbt_environment_name.setter
     def dbt_environment_name(self, dbt_environment_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_name = dbt_environment_name
 
     @property
     def dbt_environment_dbt_version(self) -> Optional[str]:
-        return self.attributes.dbt_environment_dbt_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_environment_dbt_version
+        )
 
     @dbt_environment_dbt_version.setter
     def dbt_environment_dbt_version(self, dbt_environment_dbt_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_dbt_version = dbt_environment_dbt_version
 
     @property
     def dbt_tags(self) -> Optional[set[str]]:
-        return self.attributes.dbt_tags
+        return None if self.attributes is None else self.attributes.dbt_tags
 
     @dbt_tags.setter
     def dbt_tags(self, dbt_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_tags = dbt_tags
 
     @property
     def dbt_connection_context(self) -> Optional[str]:
-        return self.attributes.dbt_connection_context
+        return (
+            None if self.attributes is None else self.attributes.dbt_connection_context
+        )
 
     @dbt_connection_context.setter
     def dbt_connection_context(self, dbt_connection_context: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_connection_context = dbt_connection_context
 
     @property
     def dbt_semantic_layer_proxy_url(self) -> Optional[str]:
-        return self.attributes.dbt_semantic_layer_proxy_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_semantic_layer_proxy_url
+        )
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
     @property
     def metric_type(self) -> Optional[str]:
-        return self.attributes.metric_type
+        return None if self.attributes is None else self.attributes.metric_type
 
     @metric_type.setter
     def metric_type(self, metric_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_type = metric_type
 
     @property
     def metric_s_q_l(self) -> Optional[str]:
-        return self.attributes.metric_s_q_l
+        return None if self.attributes is None else self.attributes.metric_s_q_l
 
     @metric_s_q_l.setter
     def metric_s_q_l(self, metric_s_q_l: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_s_q_l = metric_s_q_l
 
     @property
     def metric_filters(self) -> Optional[str]:
-        return self.attributes.metric_filters
+        return None if self.attributes is None else self.attributes.metric_filters
 
     @metric_filters.setter
     def metric_filters(self, metric_filters: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_filters = metric_filters
 
     @property
     def metric_time_grains(self) -> Optional[set[str]]:
-        return self.attributes.metric_time_grains
+        return None if self.attributes is None else self.attributes.metric_time_grains
 
     @metric_time_grains.setter
     def metric_time_grains(self, metric_time_grains: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_time_grains = metric_time_grains
 
     @property
     def metric_timestamp_column(self) -> Optional[Column]:
-        return self.attributes.metric_timestamp_column
+        return (
+            None if self.attributes is None else self.attributes.metric_timestamp_column
+        )
 
     @metric_timestamp_column.setter
     def metric_timestamp_column(self, metric_timestamp_column: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_timestamp_column = metric_timestamp_column
 
     @property
     def dbt_model(self) -> Optional[DbtModel]:
-        return self.attributes.dbt_model
+        return None if self.attributes is None else self.attributes.dbt_model
 
     @dbt_model.setter
     def dbt_model(self, dbt_model: Optional[DbtModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model = dbt_model
 
     @property
     def assets(self) -> Optional[list[Asset]]:
-        return self.attributes.assets
+        return None if self.attributes is None else self.attributes.assets
 
     @assets.setter
     def assets(self, assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.assets = assets
 
     @property
     def metric_dimension_columns(self) -> Optional[list[Column]]:
-        return self.attributes.metric_dimension_columns
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metric_dimension_columns
+        )
 
     @metric_dimension_columns.setter
     def metric_dimension_columns(
         self, metric_dimension_columns: Optional[list[Column]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_dimension_columns = metric_dimension_columns
 
     @property
     def dbt_metric_filter_columns(self) -> Optional[list[Column]]:
-        return self.attributes.dbt_metric_filter_columns
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_metric_filter_columns
+        )
 
     @dbt_metric_filter_columns.setter
     def dbt_metric_filter_columns(
         self, dbt_metric_filter_columns: Optional[list[Column]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -9062,45 +9996,47 @@
         "dbt_freshness_criteria",
         "sql_assets",
         "sql_asset",
     ]
 
     @property
     def dbt_state(self) -> Optional[str]:
-        return self.attributes.dbt_state
+        return None if self.attributes is None else self.attributes.dbt_state
 
     @dbt_state.setter
     def dbt_state(self, dbt_state: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_state = dbt_state
 
     @property
     def dbt_freshness_criteria(self) -> Optional[str]:
-        return self.attributes.dbt_freshness_criteria
+        return (
+            None if self.attributes is None else self.attributes.dbt_freshness_criteria
+        )
 
     @dbt_freshness_criteria.setter
     def dbt_freshness_criteria(self, dbt_freshness_criteria: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_freshness_criteria = dbt_freshness_criteria
 
     @property
     def sql_assets(self) -> Optional[list[SQL]]:
-        return self.attributes.sql_assets
+        return None if self.attributes is None else self.attributes.sql_assets
 
     @sql_assets.setter
     def sql_assets(self, sql_assets: Optional[list[SQL]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_assets = sql_assets
 
     @property
     def sql_asset(self) -> Optional[SQL]:
-        return self.attributes.sql_asset
+        return None if self.attributes is None else self.attributes.sql_asset
 
     @sql_asset.setter
     def sql_asset(self, sql_asset: Optional[SQL]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_asset = sql_asset
 
@@ -9165,259 +10101,279 @@
         "sql",
         "ast",
         "column_processes",
     ]
 
     @property
     def dbt_process_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_process_job_status
+        return (
+            None if self.attributes is None else self.attributes.dbt_process_job_status
+        )
 
     @dbt_process_job_status.setter
     def dbt_process_job_status(self, dbt_process_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_process_job_status = dbt_process_job_status
 
     @property
     def dbt_alias(self) -> Optional[str]:
-        return self.attributes.dbt_alias
+        return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_alias = dbt_alias
 
     @property
     def dbt_meta(self) -> Optional[str]:
-        return self.attributes.dbt_meta
+        return None if self.attributes is None else self.attributes.dbt_meta
 
     @dbt_meta.setter
     def dbt_meta(self, dbt_meta: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_meta = dbt_meta
 
     @property
     def dbt_unique_id(self) -> Optional[str]:
-        return self.attributes.dbt_unique_id
+        return None if self.attributes is None else self.attributes.dbt_unique_id
 
     @dbt_unique_id.setter
     def dbt_unique_id(self, dbt_unique_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_unique_id = dbt_unique_id
 
     @property
     def dbt_account_name(self) -> Optional[str]:
-        return self.attributes.dbt_account_name
+        return None if self.attributes is None else self.attributes.dbt_account_name
 
     @dbt_account_name.setter
     def dbt_account_name(self, dbt_account_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_account_name = dbt_account_name
 
     @property
     def dbt_project_name(self) -> Optional[str]:
-        return self.attributes.dbt_project_name
+        return None if self.attributes is None else self.attributes.dbt_project_name
 
     @dbt_project_name.setter
     def dbt_project_name(self, dbt_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_project_name = dbt_project_name
 
     @property
     def dbt_package_name(self) -> Optional[str]:
-        return self.attributes.dbt_package_name
+        return None if self.attributes is None else self.attributes.dbt_package_name
 
     @dbt_package_name.setter
     def dbt_package_name(self, dbt_package_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_package_name = dbt_package_name
 
     @property
     def dbt_job_name(self) -> Optional[str]:
-        return self.attributes.dbt_job_name
+        return None if self.attributes is None else self.attributes.dbt_job_name
 
     @dbt_job_name.setter
     def dbt_job_name(self, dbt_job_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_name = dbt_job_name
 
     @property
     def dbt_job_schedule(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule
+        return None if self.attributes is None else self.attributes.dbt_job_schedule
 
     @dbt_job_schedule.setter
     def dbt_job_schedule(self, dbt_job_schedule: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule = dbt_job_schedule
 
     @property
     def dbt_job_status(self) -> Optional[str]:
-        return self.attributes.dbt_job_status
+        return None if self.attributes is None else self.attributes.dbt_job_status
 
     @dbt_job_status.setter
     def dbt_job_status(self, dbt_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_status = dbt_job_status
 
     @property
     def dbt_job_schedule_cron_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_schedule_cron_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_schedule_cron_humanized
+        )
 
     @dbt_job_schedule_cron_humanized.setter
     def dbt_job_schedule_cron_humanized(
         self, dbt_job_schedule_cron_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_schedule_cron_humanized = (
             dbt_job_schedule_cron_humanized
         )
 
     @property
     def dbt_job_last_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_last_run
+        return None if self.attributes is None else self.attributes.dbt_job_last_run
 
     @dbt_job_last_run.setter
     def dbt_job_last_run(self, dbt_job_last_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_last_run = dbt_job_last_run
 
     @property
     def dbt_job_next_run(self) -> Optional[datetime]:
-        return self.attributes.dbt_job_next_run
+        return None if self.attributes is None else self.attributes.dbt_job_next_run
 
     @dbt_job_next_run.setter
     def dbt_job_next_run(self, dbt_job_next_run: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run = dbt_job_next_run
 
     @property
     def dbt_job_next_run_humanized(self) -> Optional[str]:
-        return self.attributes.dbt_job_next_run_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_job_next_run_humanized
+        )
 
     @dbt_job_next_run_humanized.setter
     def dbt_job_next_run_humanized(self, dbt_job_next_run_humanized: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_job_next_run_humanized = dbt_job_next_run_humanized
 
     @property
     def dbt_environment_name(self) -> Optional[str]:
-        return self.attributes.dbt_environment_name
+        return None if self.attributes is None else self.attributes.dbt_environment_name
 
     @dbt_environment_name.setter
     def dbt_environment_name(self, dbt_environment_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_name = dbt_environment_name
 
     @property
     def dbt_environment_dbt_version(self) -> Optional[str]:
-        return self.attributes.dbt_environment_dbt_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_environment_dbt_version
+        )
 
     @dbt_environment_dbt_version.setter
     def dbt_environment_dbt_version(self, dbt_environment_dbt_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_environment_dbt_version = dbt_environment_dbt_version
 
     @property
     def dbt_tags(self) -> Optional[set[str]]:
-        return self.attributes.dbt_tags
+        return None if self.attributes is None else self.attributes.dbt_tags
 
     @dbt_tags.setter
     def dbt_tags(self, dbt_tags: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_tags = dbt_tags
 
     @property
     def dbt_connection_context(self) -> Optional[str]:
-        return self.attributes.dbt_connection_context
+        return (
+            None if self.attributes is None else self.attributes.dbt_connection_context
+        )
 
     @dbt_connection_context.setter
     def dbt_connection_context(self, dbt_connection_context: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_connection_context = dbt_connection_context
 
     @property
     def dbt_semantic_layer_proxy_url(self) -> Optional[str]:
-        return self.attributes.dbt_semantic_layer_proxy_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dbt_semantic_layer_proxy_url
+        )
 
     @dbt_semantic_layer_proxy_url.setter
     def dbt_semantic_layer_proxy_url(self, dbt_semantic_layer_proxy_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_semantic_layer_proxy_url = dbt_semantic_layer_proxy_url
 
     @property
     def inputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.inputs
+        return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
     def inputs(self, inputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inputs = inputs
 
     @property
     def outputs(self) -> Optional[list[Catalog]]:
-        return self.attributes.outputs
+        return None if self.attributes is None else self.attributes.outputs
 
     @outputs.setter
     def outputs(self, outputs: Optional[list[Catalog]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.outputs = outputs
 
     @property
     def code(self) -> Optional[str]:
-        return self.attributes.code
+        return None if self.attributes is None else self.attributes.code
 
     @code.setter
     def code(self, code: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.code = code
 
     @property
     def sql(self) -> Optional[str]:
-        return self.attributes.sql
+        return None if self.attributes is None else self.attributes.sql
 
     @sql.setter
     def sql(self, sql: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql = sql
 
     @property
     def ast(self) -> Optional[str]:
-        return self.attributes.ast
+        return None if self.attributes is None else self.attributes.ast
 
     @ast.setter
     def ast(self, ast: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.ast = ast
 
     @property
     def column_processes(self) -> Optional[list[ColumnProcess]]:
-        return self.attributes.column_processes
+        return None if self.attributes is None else self.attributes.column_processes
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[list[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
@@ -9504,25 +10460,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "icon",
         "icon_type",
     ]
 
     @property
     def icon(self) -> Optional[str]:
-        return self.attributes.icon
+        return None if self.attributes is None else self.attributes.icon
 
     @icon.setter
     def icon(self, icon: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon = icon
 
     @property
     def icon_type(self) -> Optional[IconType]:
-        return self.attributes.icon_type
+        return None if self.attributes is None else self.attributes.icon_type
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
@@ -9557,35 +10513,35 @@
         "internal",
         "asset",
         "see_also",
     ]
 
     @property
     def internal(self) -> Optional[Internal]:
-        return self.attributes.internal
+        return None if self.attributes is None else self.attributes.internal
 
     @internal.setter
     def internal(self, internal: Optional[Internal]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.internal = internal
 
     @property
     def asset(self) -> Optional[Asset]:
-        return self.attributes.asset
+        return None if self.attributes is None else self.attributes.asset
 
     @asset.setter
     def asset(self, asset: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset = asset
 
     @property
     def see_also(self) -> Optional[list[Readme]]:
-        return self.attributes.see_also
+        return None if self.attributes is None else self.attributes.see_also
 
     @see_also.setter
     def see_also(self, see_also: Optional[list[Readme]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.see_also = see_also
 
@@ -9675,35 +10631,35 @@
         "file_type",
         "file_path",
         "file_assets",
     ]
 
     @property
     def file_type(self) -> Optional[FileType]:
-        return self.attributes.file_type
+        return None if self.attributes is None else self.attributes.file_type
 
     @file_type.setter
     def file_type(self, file_type: Optional[FileType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.file_type = file_type
 
     @property
     def file_path(self) -> Optional[str]:
-        return self.attributes.file_path
+        return None if self.attributes is None else self.attributes.file_path
 
     @file_path.setter
     def file_path(self, file_path: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.file_path = file_path
 
     @property
     def file_assets(self) -> Optional[Asset]:
-        return self.attributes.file_assets
+        return None if self.attributes is None else self.attributes.file_assets
 
     @file_assets.setter
     def file_assets(self, file_assets: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.file_assets = file_assets
 
@@ -9742,45 +10698,45 @@
         "icon_type",
         "internal",
         "asset",
     ]
 
     @property
     def icon(self) -> Optional[str]:
-        return self.attributes.icon
+        return None if self.attributes is None else self.attributes.icon
 
     @icon.setter
     def icon(self, icon: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon = icon
 
     @property
     def icon_type(self) -> Optional[IconType]:
-        return self.attributes.icon_type
+        return None if self.attributes is None else self.attributes.icon_type
 
     @icon_type.setter
     def icon_type(self, icon_type: Optional[IconType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
     @property
     def internal(self) -> Optional[Internal]:
-        return self.attributes.internal
+        return None if self.attributes is None else self.attributes.internal
 
     @internal.setter
     def internal(self, internal: Optional[Internal]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.internal = internal
 
     @property
     def asset(self) -> Optional[Asset]:
-        return self.attributes.asset
+        return None if self.attributes is None else self.attributes.asset
 
     @asset.setter
     def asset(self, asset: Optional[Asset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.asset = asset
 
@@ -9827,97 +10783,113 @@
         "api_spec_contract_version",
         "api_spec_service_alias",
         "api_paths",
     ]
 
     @property
     def api_spec_terms_of_service_url(self) -> Optional[str]:
-        return self.attributes.api_spec_terms_of_service_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.api_spec_terms_of_service_url
+        )
 
     @api_spec_terms_of_service_url.setter
     def api_spec_terms_of_service_url(
         self, api_spec_terms_of_service_url: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_terms_of_service_url = api_spec_terms_of_service_url
 
     @property
     def api_spec_contact_email(self) -> Optional[str]:
-        return self.attributes.api_spec_contact_email
+        return (
+            None if self.attributes is None else self.attributes.api_spec_contact_email
+        )
 
     @api_spec_contact_email.setter
     def api_spec_contact_email(self, api_spec_contact_email: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_contact_email = api_spec_contact_email
 
     @property
     def api_spec_contact_name(self) -> Optional[str]:
-        return self.attributes.api_spec_contact_name
+        return (
+            None if self.attributes is None else self.attributes.api_spec_contact_name
+        )
 
     @api_spec_contact_name.setter
     def api_spec_contact_name(self, api_spec_contact_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_contact_name = api_spec_contact_name
 
     @property
     def api_spec_contact_url(self) -> Optional[str]:
-        return self.attributes.api_spec_contact_url
+        return None if self.attributes is None else self.attributes.api_spec_contact_url
 
     @api_spec_contact_url.setter
     def api_spec_contact_url(self, api_spec_contact_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_contact_url = api_spec_contact_url
 
     @property
     def api_spec_license_name(self) -> Optional[str]:
-        return self.attributes.api_spec_license_name
+        return (
+            None if self.attributes is None else self.attributes.api_spec_license_name
+        )
 
     @api_spec_license_name.setter
     def api_spec_license_name(self, api_spec_license_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_license_name = api_spec_license_name
 
     @property
     def api_spec_license_url(self) -> Optional[str]:
-        return self.attributes.api_spec_license_url
+        return None if self.attributes is None else self.attributes.api_spec_license_url
 
     @api_spec_license_url.setter
     def api_spec_license_url(self, api_spec_license_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_license_url = api_spec_license_url
 
     @property
     def api_spec_contract_version(self) -> Optional[str]:
-        return self.attributes.api_spec_contract_version
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.api_spec_contract_version
+        )
 
     @api_spec_contract_version.setter
     def api_spec_contract_version(self, api_spec_contract_version: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_contract_version = api_spec_contract_version
 
     @property
     def api_spec_service_alias(self) -> Optional[str]:
-        return self.attributes.api_spec_service_alias
+        return (
+            None if self.attributes is None else self.attributes.api_spec_service_alias
+        )
 
     @api_spec_service_alias.setter
     def api_spec_service_alias(self, api_spec_service_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec_service_alias = api_spec_service_alias
 
     @property
     def api_paths(self) -> Optional[list[APIPath]]:
-        return self.attributes.api_paths
+        return None if self.attributes is None else self.attributes.api_paths
 
     @api_paths.setter
     def api_paths(self, api_paths: Optional[list[APIPath]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_paths = api_paths
 
@@ -9981,81 +10953,95 @@
         "api_path_available_response_codes",
         "api_path_is_ingress_exposed",
         "api_spec",
     ]
 
     @property
     def api_path_summary(self) -> Optional[str]:
-        return self.attributes.api_path_summary
+        return None if self.attributes is None else self.attributes.api_path_summary
 
     @api_path_summary.setter
     def api_path_summary(self, api_path_summary: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_summary = api_path_summary
 
     @property
     def api_path_raw_u_r_i(self) -> Optional[str]:
-        return self.attributes.api_path_raw_u_r_i
+        return None if self.attributes is None else self.attributes.api_path_raw_u_r_i
 
     @api_path_raw_u_r_i.setter
     def api_path_raw_u_r_i(self, api_path_raw_u_r_i: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_raw_u_r_i = api_path_raw_u_r_i
 
     @property
     def api_path_is_templated(self) -> Optional[bool]:
-        return self.attributes.api_path_is_templated
+        return (
+            None if self.attributes is None else self.attributes.api_path_is_templated
+        )
 
     @api_path_is_templated.setter
     def api_path_is_templated(self, api_path_is_templated: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_is_templated = api_path_is_templated
 
     @property
     def api_path_available_operations(self) -> Optional[set[str]]:
-        return self.attributes.api_path_available_operations
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.api_path_available_operations
+        )
 
     @api_path_available_operations.setter
     def api_path_available_operations(
         self, api_path_available_operations: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_available_operations = api_path_available_operations
 
     @property
     def api_path_available_response_codes(self) -> Optional[dict[str, str]]:
-        return self.attributes.api_path_available_response_codes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.api_path_available_response_codes
+        )
 
     @api_path_available_response_codes.setter
     def api_path_available_response_codes(
         self, api_path_available_response_codes: Optional[dict[str, str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_available_response_codes = (
             api_path_available_response_codes
         )
 
     @property
     def api_path_is_ingress_exposed(self) -> Optional[bool]:
-        return self.attributes.api_path_is_ingress_exposed
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.api_path_is_ingress_exposed
+        )
 
     @api_path_is_ingress_exposed.setter
     def api_path_is_ingress_exposed(self, api_path_is_ingress_exposed: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_path_is_ingress_exposed = api_path_is_ingress_exposed
 
     @property
     def api_spec(self) -> Optional[APISpec]:
-        return self.attributes.api_spec
+        return None if self.attributes is None else self.attributes.api_spec
 
     @api_spec.setter
     def api_spec(self, api_spec: Optional[APISpec]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.api_spec = api_spec
 
@@ -10129,235 +11115,245 @@
         "sql_dbt_sources",
         "dbt_models",
         "atlan_schema",
     ]
 
     @property
     def tag_id(self) -> Optional[str]:
-        return self.attributes.tag_id
+        return None if self.attributes is None else self.attributes.tag_id
 
     @tag_id.setter
     def tag_id(self, tag_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_id = tag_id
 
     @property
     def tag_attributes(self) -> Optional[list[SourceTagAttribute]]:
-        return self.attributes.tag_attributes
+        return None if self.attributes is None else self.attributes.tag_attributes
 
     @tag_attributes.setter
     def tag_attributes(self, tag_attributes: Optional[list[SourceTagAttribute]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_attributes = tag_attributes
 
     @property
     def tag_allowed_values(self) -> Optional[set[str]]:
-        return self.attributes.tag_allowed_values
+        return None if self.attributes is None else self.attributes.tag_allowed_values
 
     @tag_allowed_values.setter
     def tag_allowed_values(self, tag_allowed_values: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tag_allowed_values = tag_allowed_values
 
     @property
     def mapped_classification_name(self) -> Optional[str]:
-        return self.attributes.mapped_classification_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mapped_classification_name
+        )
 
     @mapped_classification_name.setter
     def mapped_classification_name(self, mapped_classification_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mapped_classification_name = mapped_classification_name
 
     @property
     def query_count(self) -> Optional[int]:
-        return self.attributes.query_count
+        return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_count = query_count
 
     @property
     def query_user_count(self) -> Optional[int]:
-        return self.attributes.query_user_count
+        return None if self.attributes is None else self.attributes.query_user_count
 
     @query_user_count.setter
     def query_user_count(self, query_user_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_user_count = query_user_count
 
     @property
     def query_user_map(self) -> Optional[dict[str, int]]:
-        return self.attributes.query_user_map
+        return None if self.attributes is None else self.attributes.query_user_map
 
     @query_user_map.setter
     def query_user_map(self, query_user_map: Optional[dict[str, int]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_user_map = query_user_map
 
     @property
     def query_count_updated_at(self) -> Optional[datetime]:
-        return self.attributes.query_count_updated_at
+        return (
+            None if self.attributes is None else self.attributes.query_count_updated_at
+        )
 
     @query_count_updated_at.setter
     def query_count_updated_at(self, query_count_updated_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_count_updated_at = query_count_updated_at
 
     @property
     def database_name(self) -> Optional[str]:
-        return self.attributes.database_name
+        return None if self.attributes is None else self.attributes.database_name
 
     @database_name.setter
     def database_name(self, database_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.database_name = database_name
 
     @property
     def database_qualified_name(self) -> Optional[str]:
-        return self.attributes.database_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.database_qualified_name
+        )
 
     @database_qualified_name.setter
     def database_qualified_name(self, database_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.database_qualified_name = database_qualified_name
 
     @property
     def schema_name(self) -> Optional[str]:
-        return self.attributes.schema_name
+        return None if self.attributes is None else self.attributes.schema_name
 
     @schema_name.setter
     def schema_name(self, schema_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_name = schema_name
 
     @property
     def schema_qualified_name(self) -> Optional[str]:
-        return self.attributes.schema_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.schema_qualified_name
+        )
 
     @schema_qualified_name.setter
     def schema_qualified_name(self, schema_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_qualified_name = schema_qualified_name
 
     @property
     def table_name(self) -> Optional[str]:
-        return self.attributes.table_name
+        return None if self.attributes is None else self.attributes.table_name
 
     @table_name.setter
     def table_name(self, table_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_name = table_name
 
     @property
     def table_qualified_name(self) -> Optional[str]:
-        return self.attributes.table_qualified_name
+        return None if self.attributes is None else self.attributes.table_qualified_name
 
     @table_qualified_name.setter
     def table_qualified_name(self, table_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_qualified_name = table_qualified_name
 
     @property
     def view_name(self) -> Optional[str]:
-        return self.attributes.view_name
+        return None if self.attributes is None else self.attributes.view_name
 
     @view_name.setter
     def view_name(self, view_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_name = view_name
 
     @property
     def view_qualified_name(self) -> Optional[str]:
-        return self.attributes.view_qualified_name
+        return None if self.attributes is None else self.attributes.view_qualified_name
 
     @view_qualified_name.setter
     def view_qualified_name(self, view_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_qualified_name = view_qualified_name
 
     @property
     def is_profiled(self) -> Optional[bool]:
-        return self.attributes.is_profiled
+        return None if self.attributes is None else self.attributes.is_profiled
 
     @is_profiled.setter
     def is_profiled(self, is_profiled: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_profiled = is_profiled
 
     @property
     def last_profiled_at(self) -> Optional[datetime]:
-        return self.attributes.last_profiled_at
+        return None if self.attributes is None else self.attributes.last_profiled_at
 
     @last_profiled_at.setter
     def last_profiled_at(self, last_profiled_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.last_profiled_at = last_profiled_at
 
     @property
     def dbt_sources(self) -> Optional[list[DbtSource]]:
-        return self.attributes.dbt_sources
+        return None if self.attributes is None else self.attributes.dbt_sources
 
     @dbt_sources.setter
     def dbt_sources(self, dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_sources = dbt_sources
 
     @property
     def sql_dbt_models(self) -> Optional[list[DbtModel]]:
-        return self.attributes.sql_dbt_models
+        return None if self.attributes is None else self.attributes.sql_dbt_models
 
     @sql_dbt_models.setter
     def sql_dbt_models(self, sql_dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_dbt_models = sql_dbt_models
 
     @property
     def sql_dbt_sources(self) -> Optional[list[DbtSource]]:
-        return self.attributes.sql_dbt_sources
+        return None if self.attributes is None else self.attributes.sql_dbt_sources
 
     @sql_dbt_sources.setter
     def sql_dbt_sources(self, sql_dbt_sources: Optional[list[DbtSource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_dbt_sources = sql_dbt_sources
 
     @property
     def dbt_models(self) -> Optional[list[DbtModel]]:
-        return self.attributes.dbt_models
+        return None if self.attributes is None else self.attributes.dbt_models
 
     @dbt_models.setter
     def dbt_models(self, dbt_models: Optional[list[DbtModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_models = dbt_models
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -10459,175 +11455,183 @@
         "partition_list",
         "columns",
         "parent_table",
     ]
 
     @property
     def constraint(self) -> Optional[str]:
-        return self.attributes.constraint
+        return None if self.attributes is None else self.attributes.constraint
 
     @constraint.setter
     def constraint(self, constraint: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.constraint = constraint
 
     @property
     def column_count(self) -> Optional[int]:
-        return self.attributes.column_count
+        return None if self.attributes is None else self.attributes.column_count
 
     @column_count.setter
     def column_count(self, column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_count = column_count
 
     @property
     def row_count(self) -> Optional[int]:
-        return self.attributes.row_count
+        return None if self.attributes is None else self.attributes.row_count
 
     @row_count.setter
     def row_count(self, row_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_count = row_count
 
     @property
     def size_bytes(self) -> Optional[int]:
-        return self.attributes.size_bytes
+        return None if self.attributes is None else self.attributes.size_bytes
 
     @size_bytes.setter
     def size_bytes(self, size_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.size_bytes = size_bytes
 
     @property
     def alias(self) -> Optional[str]:
-        return self.attributes.alias
+        return None if self.attributes is None else self.attributes.alias
 
     @alias.setter
     def alias(self, alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.alias = alias
 
     @property
     def is_temporary(self) -> Optional[bool]:
-        return self.attributes.is_temporary
+        return None if self.attributes is None else self.attributes.is_temporary
 
     @is_temporary.setter
     def is_temporary(self, is_temporary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_temporary = is_temporary
 
     @property
     def is_query_preview(self) -> Optional[bool]:
-        return self.attributes.is_query_preview
+        return None if self.attributes is None else self.attributes.is_query_preview
 
     @is_query_preview.setter
     def is_query_preview(self, is_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_query_preview = is_query_preview
 
     @property
     def query_preview_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.query_preview_config
+        return None if self.attributes is None else self.attributes.query_preview_config
 
     @query_preview_config.setter
     def query_preview_config(self, query_preview_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_preview_config = query_preview_config
 
     @property
     def external_location(self) -> Optional[str]:
-        return self.attributes.external_location
+        return None if self.attributes is None else self.attributes.external_location
 
     @external_location.setter
     def external_location(self, external_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location = external_location
 
     @property
     def external_location_region(self) -> Optional[str]:
-        return self.attributes.external_location_region
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.external_location_region
+        )
 
     @external_location_region.setter
     def external_location_region(self, external_location_region: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location_region = external_location_region
 
     @property
     def external_location_format(self) -> Optional[str]:
-        return self.attributes.external_location_format
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.external_location_format
+        )
 
     @external_location_format.setter
     def external_location_format(self, external_location_format: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location_format = external_location_format
 
     @property
     def is_partitioned(self) -> Optional[bool]:
-        return self.attributes.is_partitioned
+        return None if self.attributes is None else self.attributes.is_partitioned
 
     @is_partitioned.setter
     def is_partitioned(self, is_partitioned: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_partitioned = is_partitioned
 
     @property
     def partition_strategy(self) -> Optional[str]:
-        return self.attributes.partition_strategy
+        return None if self.attributes is None else self.attributes.partition_strategy
 
     @partition_strategy.setter
     def partition_strategy(self, partition_strategy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_strategy = partition_strategy
 
     @property
     def partition_count(self) -> Optional[int]:
-        return self.attributes.partition_count
+        return None if self.attributes is None else self.attributes.partition_count
 
     @partition_count.setter
     def partition_count(self, partition_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_count = partition_count
 
     @property
     def partition_list(self) -> Optional[str]:
-        return self.attributes.partition_list
+        return None if self.attributes is None else self.attributes.partition_list
 
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
     def columns(self) -> Optional[list[Column]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def parent_table(self) -> Optional[Table]:
-        return self.attributes.parent_table
+        return None if self.attributes is None else self.attributes.parent_table
 
     @parent_table.setter
     def parent_table(self, parent_table: Optional[Table]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_table = parent_table
 
@@ -10716,205 +11720,213 @@
         "facts",
         "atlan_schema",
         "dimensions",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
-        return self.attributes.column_count
+        return None if self.attributes is None else self.attributes.column_count
 
     @column_count.setter
     def column_count(self, column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_count = column_count
 
     @property
     def row_count(self) -> Optional[int]:
-        return self.attributes.row_count
+        return None if self.attributes is None else self.attributes.row_count
 
     @row_count.setter
     def row_count(self, row_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_count = row_count
 
     @property
     def size_bytes(self) -> Optional[int]:
-        return self.attributes.size_bytes
+        return None if self.attributes is None else self.attributes.size_bytes
 
     @size_bytes.setter
     def size_bytes(self, size_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.size_bytes = size_bytes
 
     @property
     def alias(self) -> Optional[str]:
-        return self.attributes.alias
+        return None if self.attributes is None else self.attributes.alias
 
     @alias.setter
     def alias(self, alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.alias = alias
 
     @property
     def is_temporary(self) -> Optional[bool]:
-        return self.attributes.is_temporary
+        return None if self.attributes is None else self.attributes.is_temporary
 
     @is_temporary.setter
     def is_temporary(self, is_temporary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_temporary = is_temporary
 
     @property
     def is_query_preview(self) -> Optional[bool]:
-        return self.attributes.is_query_preview
+        return None if self.attributes is None else self.attributes.is_query_preview
 
     @is_query_preview.setter
     def is_query_preview(self, is_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_query_preview = is_query_preview
 
     @property
     def query_preview_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.query_preview_config
+        return None if self.attributes is None else self.attributes.query_preview_config
 
     @query_preview_config.setter
     def query_preview_config(self, query_preview_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_preview_config = query_preview_config
 
     @property
     def external_location(self) -> Optional[str]:
-        return self.attributes.external_location
+        return None if self.attributes is None else self.attributes.external_location
 
     @external_location.setter
     def external_location(self, external_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location = external_location
 
     @property
     def external_location_region(self) -> Optional[str]:
-        return self.attributes.external_location_region
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.external_location_region
+        )
 
     @external_location_region.setter
     def external_location_region(self, external_location_region: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location_region = external_location_region
 
     @property
     def external_location_format(self) -> Optional[str]:
-        return self.attributes.external_location_format
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.external_location_format
+        )
 
     @external_location_format.setter
     def external_location_format(self, external_location_format: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.external_location_format = external_location_format
 
     @property
     def is_partitioned(self) -> Optional[bool]:
-        return self.attributes.is_partitioned
+        return None if self.attributes is None else self.attributes.is_partitioned
 
     @is_partitioned.setter
     def is_partitioned(self, is_partitioned: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_partitioned = is_partitioned
 
     @property
     def partition_strategy(self) -> Optional[str]:
-        return self.attributes.partition_strategy
+        return None if self.attributes is None else self.attributes.partition_strategy
 
     @partition_strategy.setter
     def partition_strategy(self, partition_strategy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_strategy = partition_strategy
 
     @property
     def partition_count(self) -> Optional[int]:
-        return self.attributes.partition_count
+        return None if self.attributes is None else self.attributes.partition_count
 
     @partition_count.setter
     def partition_count(self, partition_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_count = partition_count
 
     @property
     def partition_list(self) -> Optional[str]:
-        return self.attributes.partition_list
+        return None if self.attributes is None else self.attributes.partition_list
 
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
     def partitions(self) -> Optional[list[TablePartition]]:
-        return self.attributes.partitions
+        return None if self.attributes is None else self.attributes.partitions
 
     @partitions.setter
     def partitions(self, partitions: Optional[list[TablePartition]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partitions = partitions
 
     @property
     def columns(self) -> Optional[list[Column]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def queries(self) -> Optional[list[Query]]:
-        return self.attributes.queries
+        return None if self.attributes is None else self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.queries = queries
 
     @property
     def facts(self) -> Optional[list[Table]]:
-        return self.attributes.facts
+        return None if self.attributes is None else self.attributes.facts
 
     @facts.setter
     def facts(self, facts: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.facts = facts
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
     @property
     def dimensions(self) -> Optional[list[Table]]:
-        return self.attributes.dimensions
+        return None if self.attributes is None else self.attributes.dimensions
 
     @dimensions.setter
     def dimensions(self, dimensions: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dimensions = dimensions
 
@@ -11044,151 +12056,171 @@
         "columns",
         "tables",
         "views",
     ]
 
     @property
     def raw_query(self) -> Optional[str]:
-        return self.attributes.raw_query
+        return None if self.attributes is None else self.attributes.raw_query
 
     @raw_query.setter
     def raw_query(self, raw_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.raw_query = raw_query
 
     @property
     def default_schema_qualified_name(self) -> Optional[str]:
-        return self.attributes.default_schema_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.default_schema_qualified_name
+        )
 
     @default_schema_qualified_name.setter
     def default_schema_qualified_name(
         self, default_schema_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_schema_qualified_name = default_schema_qualified_name
 
     @property
     def default_database_qualified_name(self) -> Optional[str]:
-        return self.attributes.default_database_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.default_database_qualified_name
+        )
 
     @default_database_qualified_name.setter
     def default_database_qualified_name(
         self, default_database_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_database_qualified_name = (
             default_database_qualified_name
         )
 
     @property
     def variables_schema_base64(self) -> Optional[str]:
-        return self.attributes.variables_schema_base64
+        return (
+            None if self.attributes is None else self.attributes.variables_schema_base64
+        )
 
     @variables_schema_base64.setter
     def variables_schema_base64(self, variables_schema_base64: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.variables_schema_base64 = variables_schema_base64
 
     @property
     def is_private(self) -> Optional[bool]:
-        return self.attributes.is_private
+        return None if self.attributes is None else self.attributes.is_private
 
     @is_private.setter
     def is_private(self, is_private: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_private = is_private
 
     @property
     def is_sql_snippet(self) -> Optional[bool]:
-        return self.attributes.is_sql_snippet
+        return None if self.attributes is None else self.attributes.is_sql_snippet
 
     @is_sql_snippet.setter
     def is_sql_snippet(self, is_sql_snippet: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_sql_snippet = is_sql_snippet
 
     @property
     def parent_qualified_name(self) -> str:
-        return self.attributes.parent_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.parent_qualified_name
+        )
 
     @parent_qualified_name.setter
     def parent_qualified_name(self, parent_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_qualified_name = parent_qualified_name
 
     @property
     def collection_qualified_name(self) -> str:
-        return self.attributes.collection_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.collection_qualified_name
+        )
 
     @collection_qualified_name.setter
     def collection_qualified_name(self, collection_qualified_name: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.collection_qualified_name = collection_qualified_name
 
     @property
     def is_visual_query(self) -> Optional[bool]:
-        return self.attributes.is_visual_query
+        return None if self.attributes is None else self.attributes.is_visual_query
 
     @is_visual_query.setter
     def is_visual_query(self, is_visual_query: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_visual_query = is_visual_query
 
     @property
     def visual_builder_schema_base64(self) -> Optional[str]:
-        return self.attributes.visual_builder_schema_base64
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.visual_builder_schema_base64
+        )
 
     @visual_builder_schema_base64.setter
     def visual_builder_schema_base64(self, visual_builder_schema_base64: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.visual_builder_schema_base64 = visual_builder_schema_base64
 
     @property
     def parent(self) -> Namespace:
-        return self.attributes.parent
+        return None if self.attributes is None else self.attributes.parent
 
     @parent.setter
     def parent(self, parent: Namespace):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent = parent
 
     @property
     def columns(self) -> Optional[list[Column]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def tables(self) -> Optional[list[Table]]:
-        return self.attributes.tables
+        return None if self.attributes is None else self.attributes.tables
 
     @tables.setter
     def tables(self, tables: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tables = tables
 
     @property
     def views(self) -> Optional[list[View]]:
-        return self.attributes.views
+        return None if self.attributes is None else self.attributes.views
 
     @views.setter
     def views(self, views: Optional[list[View]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
@@ -11252,15 +12284,17 @@
         if name in Column._convience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
     _convience_properties: ClassVar[list[str]] = [
         "data_type",
         "sub_data_type",
+        "raw_data_type_definition",
         "order",
+        "nested_column_count",
         "is_partition",
         "partition_order",
         "is_clustered",
         "is_primary",
         "is_foreign",
         "is_indexed",
         "is_sort",
@@ -11270,14 +12304,16 @@
         "pinned_at",
         "precision",
         "default_value",
         "is_nullable",
         "numeric_scale",
         "max_length",
         "validations",
+        "parent_column_qualified_name",
+        "parent_column_name",
         "column_distinct_values_count",
         "column_distinct_values_count_long",
         "column_histogram",
         "column_max",
         "column_min",
         "column_mean",
         "column_sum",
@@ -11295,621 +12331,764 @@
         "column_mins",
         "column_missing_values_count",
         "column_missing_values_count_long",
         "column_missing_values_percentage",
         "column_uniqueness_percentage",
         "column_variance",
         "column_top_values",
+        "column_depth_level",
         "view",
+        "nested_columns",
         "data_quality_metric_dimensions",
         "dbt_model_columns",
         "table",
         "column_dbt_model_columns",
         "materialised_view",
+        "parent_column",
         "queries",
         "metric_timestamps",
         "foreign_key_to",
         "foreign_key_from",
         "dbt_metrics",
         "table_partition",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
-        return self.attributes.data_type
+        return None if self.attributes is None else self.attributes.data_type
 
     @data_type.setter
     def data_type(self, data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_type = data_type
 
     @property
     def sub_data_type(self) -> Optional[str]:
-        return self.attributes.sub_data_type
+        return None if self.attributes is None else self.attributes.sub_data_type
 
     @sub_data_type.setter
     def sub_data_type(self, sub_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sub_data_type = sub_data_type
 
     @property
+    def raw_data_type_definition(self) -> Optional[str]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.raw_data_type_definition
+        )
+
+    @raw_data_type_definition.setter
+    def raw_data_type_definition(self, raw_data_type_definition: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.raw_data_type_definition = raw_data_type_definition
+
+    @property
     def order(self) -> Optional[int]:
-        return self.attributes.order
+        return None if self.attributes is None else self.attributes.order
 
     @order.setter
     def order(self, order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.order = order
 
     @property
+    def nested_column_count(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.nested_column_count
+
+    @nested_column_count.setter
+    def nested_column_count(self, nested_column_count: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.nested_column_count = nested_column_count
+
+    @property
     def is_partition(self) -> Optional[bool]:
-        return self.attributes.is_partition
+        return None if self.attributes is None else self.attributes.is_partition
 
     @is_partition.setter
     def is_partition(self, is_partition: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_partition = is_partition
 
     @property
     def partition_order(self) -> Optional[int]:
-        return self.attributes.partition_order
+        return None if self.attributes is None else self.attributes.partition_order
 
     @partition_order.setter
     def partition_order(self, partition_order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_order = partition_order
 
     @property
     def is_clustered(self) -> Optional[bool]:
-        return self.attributes.is_clustered
+        return None if self.attributes is None else self.attributes.is_clustered
 
     @is_clustered.setter
     def is_clustered(self, is_clustered: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_clustered = is_clustered
 
     @property
     def is_primary(self) -> Optional[bool]:
-        return self.attributes.is_primary
+        return None if self.attributes is None else self.attributes.is_primary
 
     @is_primary.setter
     def is_primary(self, is_primary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_primary = is_primary
 
     @property
     def is_foreign(self) -> Optional[bool]:
-        return self.attributes.is_foreign
+        return None if self.attributes is None else self.attributes.is_foreign
 
     @is_foreign.setter
     def is_foreign(self, is_foreign: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_foreign = is_foreign
 
     @property
     def is_indexed(self) -> Optional[bool]:
-        return self.attributes.is_indexed
+        return None if self.attributes is None else self.attributes.is_indexed
 
     @is_indexed.setter
     def is_indexed(self, is_indexed: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_indexed = is_indexed
 
     @property
     def is_sort(self) -> Optional[bool]:
-        return self.attributes.is_sort
+        return None if self.attributes is None else self.attributes.is_sort
 
     @is_sort.setter
     def is_sort(self, is_sort: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_sort = is_sort
 
     @property
     def is_dist(self) -> Optional[bool]:
-        return self.attributes.is_dist
+        return None if self.attributes is None else self.attributes.is_dist
 
     @is_dist.setter
     def is_dist(self, is_dist: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_dist = is_dist
 
     @property
     def is_pinned(self) -> Optional[bool]:
-        return self.attributes.is_pinned
+        return None if self.attributes is None else self.attributes.is_pinned
 
     @is_pinned.setter
     def is_pinned(self, is_pinned: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_pinned = is_pinned
 
     @property
     def pinned_by(self) -> Optional[str]:
-        return self.attributes.pinned_by
+        return None if self.attributes is None else self.attributes.pinned_by
 
     @pinned_by.setter
     def pinned_by(self, pinned_by: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.pinned_by = pinned_by
 
     @property
     def pinned_at(self) -> Optional[datetime]:
-        return self.attributes.pinned_at
+        return None if self.attributes is None else self.attributes.pinned_at
 
     @pinned_at.setter
     def pinned_at(self, pinned_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.pinned_at = pinned_at
 
     @property
     def precision(self) -> Optional[int]:
-        return self.attributes.precision
+        return None if self.attributes is None else self.attributes.precision
 
     @precision.setter
     def precision(self, precision: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.precision = precision
 
     @property
     def default_value(self) -> Optional[str]:
-        return self.attributes.default_value
+        return None if self.attributes is None else self.attributes.default_value
 
     @default_value.setter
     def default_value(self, default_value: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_value = default_value
 
     @property
     def is_nullable(self) -> Optional[bool]:
-        return self.attributes.is_nullable
+        return None if self.attributes is None else self.attributes.is_nullable
 
     @is_nullable.setter
     def is_nullable(self, is_nullable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_nullable = is_nullable
 
     @property
     def numeric_scale(self) -> Optional[float]:
-        return self.attributes.numeric_scale
+        return None if self.attributes is None else self.attributes.numeric_scale
 
     @numeric_scale.setter
     def numeric_scale(self, numeric_scale: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.numeric_scale = numeric_scale
 
     @property
     def max_length(self) -> Optional[int]:
-        return self.attributes.max_length
+        return None if self.attributes is None else self.attributes.max_length
 
     @max_length.setter
     def max_length(self, max_length: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.max_length = max_length
 
     @property
     def validations(self) -> Optional[dict[str, str]]:
-        return self.attributes.validations
+        return None if self.attributes is None else self.attributes.validations
 
     @validations.setter
     def validations(self, validations: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.validations = validations
 
     @property
+    def parent_column_qualified_name(self) -> Optional[str]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.parent_column_qualified_name
+        )
+
+    @parent_column_qualified_name.setter
+    def parent_column_qualified_name(self, parent_column_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_column_qualified_name = parent_column_qualified_name
+
+    @property
+    def parent_column_name(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.parent_column_name
+
+    @parent_column_name.setter
+    def parent_column_name(self, parent_column_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_column_name = parent_column_name
+
+    @property
     def column_distinct_values_count(self) -> Optional[int]:
-        return self.attributes.column_distinct_values_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_distinct_values_count
+        )
 
     @column_distinct_values_count.setter
     def column_distinct_values_count(self, column_distinct_values_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_distinct_values_count = column_distinct_values_count
 
     @property
     def column_distinct_values_count_long(self) -> Optional[int]:
-        return self.attributes.column_distinct_values_count_long
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_distinct_values_count_long
+        )
 
     @column_distinct_values_count_long.setter
     def column_distinct_values_count_long(
         self, column_distinct_values_count_long: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_distinct_values_count_long = (
             column_distinct_values_count_long
         )
 
     @property
     def column_histogram(self) -> Optional[Histogram]:
-        return self.attributes.column_histogram
+        return None if self.attributes is None else self.attributes.column_histogram
 
     @column_histogram.setter
     def column_histogram(self, column_histogram: Optional[Histogram]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_histogram = column_histogram
 
     @property
     def column_max(self) -> Optional[float]:
-        return self.attributes.column_max
+        return None if self.attributes is None else self.attributes.column_max
 
     @column_max.setter
     def column_max(self, column_max: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_max = column_max
 
     @property
     def column_min(self) -> Optional[float]:
-        return self.attributes.column_min
+        return None if self.attributes is None else self.attributes.column_min
 
     @column_min.setter
     def column_min(self, column_min: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_min = column_min
 
     @property
     def column_mean(self) -> Optional[float]:
-        return self.attributes.column_mean
+        return None if self.attributes is None else self.attributes.column_mean
 
     @column_mean.setter
     def column_mean(self, column_mean: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_mean = column_mean
 
     @property
     def column_sum(self) -> Optional[float]:
-        return self.attributes.column_sum
+        return None if self.attributes is None else self.attributes.column_sum
 
     @column_sum.setter
     def column_sum(self, column_sum: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_sum = column_sum
 
     @property
     def column_median(self) -> Optional[float]:
-        return self.attributes.column_median
+        return None if self.attributes is None else self.attributes.column_median
 
     @column_median.setter
     def column_median(self, column_median: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_median = column_median
 
     @property
     def column_standard_deviation(self) -> Optional[float]:
-        return self.attributes.column_standard_deviation
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_standard_deviation
+        )
 
     @column_standard_deviation.setter
     def column_standard_deviation(self, column_standard_deviation: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_standard_deviation = column_standard_deviation
 
     @property
     def column_unique_values_count(self) -> Optional[int]:
-        return self.attributes.column_unique_values_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_unique_values_count
+        )
 
     @column_unique_values_count.setter
     def column_unique_values_count(self, column_unique_values_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_unique_values_count = column_unique_values_count
 
     @property
     def column_unique_values_count_long(self) -> Optional[int]:
-        return self.attributes.column_unique_values_count_long
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_unique_values_count_long
+        )
 
     @column_unique_values_count_long.setter
     def column_unique_values_count_long(
         self, column_unique_values_count_long: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_unique_values_count_long = (
             column_unique_values_count_long
         )
 
     @property
     def column_average(self) -> Optional[float]:
-        return self.attributes.column_average
+        return None if self.attributes is None else self.attributes.column_average
 
     @column_average.setter
     def column_average(self, column_average: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_average = column_average
 
     @property
     def column_average_length(self) -> Optional[float]:
-        return self.attributes.column_average_length
+        return (
+            None if self.attributes is None else self.attributes.column_average_length
+        )
 
     @column_average_length.setter
     def column_average_length(self, column_average_length: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_average_length = column_average_length
 
     @property
     def column_duplicate_values_count(self) -> Optional[int]:
-        return self.attributes.column_duplicate_values_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_duplicate_values_count
+        )
 
     @column_duplicate_values_count.setter
     def column_duplicate_values_count(
         self, column_duplicate_values_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_duplicate_values_count = column_duplicate_values_count
 
     @property
     def column_duplicate_values_count_long(self) -> Optional[int]:
-        return self.attributes.column_duplicate_values_count_long
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_duplicate_values_count_long
+        )
 
     @column_duplicate_values_count_long.setter
     def column_duplicate_values_count_long(
         self, column_duplicate_values_count_long: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_duplicate_values_count_long = (
             column_duplicate_values_count_long
         )
 
     @property
     def column_maximum_string_length(self) -> Optional[int]:
-        return self.attributes.column_maximum_string_length
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_maximum_string_length
+        )
 
     @column_maximum_string_length.setter
     def column_maximum_string_length(self, column_maximum_string_length: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_maximum_string_length = column_maximum_string_length
 
     @property
     def column_maxs(self) -> Optional[set[str]]:
-        return self.attributes.column_maxs
+        return None if self.attributes is None else self.attributes.column_maxs
 
     @column_maxs.setter
     def column_maxs(self, column_maxs: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_maxs = column_maxs
 
     @property
     def column_minimum_string_length(self) -> Optional[int]:
-        return self.attributes.column_minimum_string_length
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_minimum_string_length
+        )
 
     @column_minimum_string_length.setter
     def column_minimum_string_length(self, column_minimum_string_length: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_minimum_string_length = column_minimum_string_length
 
     @property
     def column_mins(self) -> Optional[set[str]]:
-        return self.attributes.column_mins
+        return None if self.attributes is None else self.attributes.column_mins
 
     @column_mins.setter
     def column_mins(self, column_mins: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_mins = column_mins
 
     @property
     def column_missing_values_count(self) -> Optional[int]:
-        return self.attributes.column_missing_values_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_missing_values_count
+        )
 
     @column_missing_values_count.setter
     def column_missing_values_count(self, column_missing_values_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_missing_values_count = column_missing_values_count
 
     @property
     def column_missing_values_count_long(self) -> Optional[int]:
-        return self.attributes.column_missing_values_count_long
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_missing_values_count_long
+        )
 
     @column_missing_values_count_long.setter
     def column_missing_values_count_long(
         self, column_missing_values_count_long: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_missing_values_count_long = (
             column_missing_values_count_long
         )
 
     @property
     def column_missing_values_percentage(self) -> Optional[float]:
-        return self.attributes.column_missing_values_percentage
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_missing_values_percentage
+        )
 
     @column_missing_values_percentage.setter
     def column_missing_values_percentage(
         self, column_missing_values_percentage: Optional[float]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_missing_values_percentage = (
             column_missing_values_percentage
         )
 
     @property
     def column_uniqueness_percentage(self) -> Optional[float]:
-        return self.attributes.column_uniqueness_percentage
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_uniqueness_percentage
+        )
 
     @column_uniqueness_percentage.setter
     def column_uniqueness_percentage(
         self, column_uniqueness_percentage: Optional[float]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_uniqueness_percentage = column_uniqueness_percentage
 
     @property
     def column_variance(self) -> Optional[float]:
-        return self.attributes.column_variance
+        return None if self.attributes is None else self.attributes.column_variance
 
     @column_variance.setter
     def column_variance(self, column_variance: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_variance = column_variance
 
     @property
     def column_top_values(self) -> Optional[list[ColumnValueFrequencyMap]]:
-        return self.attributes.column_top_values
+        return None if self.attributes is None else self.attributes.column_top_values
 
     @column_top_values.setter
     def column_top_values(
         self, column_top_values: Optional[list[ColumnValueFrequencyMap]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_top_values = column_top_values
 
     @property
+    def column_depth_level(self) -> Optional[int]:
+        return None if self.attributes is None else self.attributes.column_depth_level
+
+    @column_depth_level.setter
+    def column_depth_level(self, column_depth_level: Optional[int]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.column_depth_level = column_depth_level
+
+    @property
     def view(self) -> Optional[View]:
-        return self.attributes.view
+        return None if self.attributes is None else self.attributes.view
 
     @view.setter
     def view(self, view: Optional[View]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view = view
 
     @property
+    def nested_columns(self) -> Optional[list[Column]]:
+        return None if self.attributes is None else self.attributes.nested_columns
+
+    @nested_columns.setter
+    def nested_columns(self, nested_columns: Optional[list[Column]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.nested_columns = nested_columns
+
+    @property
     def data_quality_metric_dimensions(self) -> Optional[list[Metric]]:
-        return self.attributes.data_quality_metric_dimensions
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.data_quality_metric_dimensions
+        )
 
     @data_quality_metric_dimensions.setter
     def data_quality_metric_dimensions(
         self, data_quality_metric_dimensions: Optional[list[Metric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_quality_metric_dimensions = data_quality_metric_dimensions
 
     @property
     def dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
-        return self.attributes.dbt_model_columns
+        return None if self.attributes is None else self.attributes.dbt_model_columns
 
     @dbt_model_columns.setter
     def dbt_model_columns(self, dbt_model_columns: Optional[list[DbtModelColumn]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_model_columns = dbt_model_columns
 
     @property
     def table(self) -> Optional[Table]:
-        return self.attributes.table
+        return None if self.attributes is None else self.attributes.table
 
     @table.setter
     def table(self, table: Optional[Table]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table = table
 
     @property
     def column_dbt_model_columns(self) -> Optional[list[DbtModelColumn]]:
-        return self.attributes.column_dbt_model_columns
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.column_dbt_model_columns
+        )
 
     @column_dbt_model_columns.setter
     def column_dbt_model_columns(
         self, column_dbt_model_columns: Optional[list[DbtModelColumn]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_dbt_model_columns = column_dbt_model_columns
 
     @property
     def materialised_view(self) -> Optional[MaterialisedView]:
-        return self.attributes.materialised_view
+        return None if self.attributes is None else self.attributes.materialised_view
 
     @materialised_view.setter
     def materialised_view(self, materialised_view: Optional[MaterialisedView]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.materialised_view = materialised_view
 
     @property
+    def parent_column(self) -> Optional[Column]:
+        return None if self.attributes is None else self.attributes.parent_column
+
+    @parent_column.setter
+    def parent_column(self, parent_column: Optional[Column]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_column = parent_column
+
+    @property
     def queries(self) -> Optional[list[Query]]:
-        return self.attributes.queries
+        return None if self.attributes is None else self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.queries = queries
 
     @property
     def metric_timestamps(self) -> Optional[list[Metric]]:
-        return self.attributes.metric_timestamps
+        return None if self.attributes is None else self.attributes.metric_timestamps
 
     @metric_timestamps.setter
     def metric_timestamps(self, metric_timestamps: Optional[list[Metric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metric_timestamps = metric_timestamps
 
     @property
     def foreign_key_to(self) -> Optional[list[Column]]:
-        return self.attributes.foreign_key_to
+        return None if self.attributes is None else self.attributes.foreign_key_to
 
     @foreign_key_to.setter
     def foreign_key_to(self, foreign_key_to: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.foreign_key_to = foreign_key_to
 
     @property
     def foreign_key_from(self) -> Optional[Column]:
-        return self.attributes.foreign_key_from
+        return None if self.attributes is None else self.attributes.foreign_key_from
 
     @foreign_key_from.setter
     def foreign_key_from(self, foreign_key_from: Optional[Column]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.foreign_key_from = foreign_key_from
 
     @property
     def dbt_metrics(self) -> Optional[list[DbtMetric]]:
-        return self.attributes.dbt_metrics
+        return None if self.attributes is None else self.attributes.dbt_metrics
 
     @dbt_metrics.setter
     def dbt_metrics(self, dbt_metrics: Optional[list[DbtMetric]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_metrics = dbt_metrics
 
     @property
     def table_partition(self) -> Optional[TablePartition]:
-        return self.attributes.table_partition
+        return None if self.attributes is None else self.attributes.table_partition
 
     @table_partition.setter
     def table_partition(self, table_partition: Optional[TablePartition]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_partition = table_partition
 
@@ -11920,15 +13099,21 @@
         if v != "Column":
             raise ValueError("must be Column")
         return v
 
     class Attributes(SQL.Attributes):
         data_type: Optional[str] = Field(None, description="", alias="dataType")
         sub_data_type: Optional[str] = Field(None, description="", alias="subDataType")
+        raw_data_type_definition: Optional[str] = Field(
+            None, description="", alias="rawDataTypeDefinition"
+        )
         order: Optional[int] = Field(None, description="", alias="order")
+        nested_column_count: Optional[int] = Field(
+            None, description="", alias="nestedColumnCount"
+        )
         is_partition: Optional[bool] = Field(None, description="", alias="isPartition")
         partition_order: Optional[int] = Field(
             None, description="", alias="partitionOrder"
         )
         is_clustered: Optional[bool] = Field(None, description="", alias="isClustered")
         is_primary: Optional[bool] = Field(None, description="", alias="isPrimary")
         is_foreign: Optional[bool] = Field(None, description="", alias="isForeign")
@@ -11944,14 +13129,20 @@
         numeric_scale: Optional[float] = Field(
             None, description="", alias="numericScale"
         )
         max_length: Optional[int] = Field(None, description="", alias="maxLength")
         validations: Optional[dict[str, str]] = Field(
             None, description="", alias="validations"
         )
+        parent_column_qualified_name: Optional[str] = Field(
+            None, description="", alias="parentColumnQualifiedName"
+        )
+        parent_column_name: Optional[str] = Field(
+            None, description="", alias="parentColumnName"
+        )
         column_distinct_values_count: Optional[int] = Field(
             None, description="", alias="columnDistinctValuesCount"
         )
         column_distinct_values_count_long: Optional[int] = Field(
             None, description="", alias="columnDistinctValuesCountLong"
         )
         column_histogram: Optional[Histogram] = Field(
@@ -12011,15 +13202,21 @@
         )
         column_variance: Optional[float] = Field(
             None, description="", alias="columnVariance"
         )
         column_top_values: Optional[list[ColumnValueFrequencyMap]] = Field(
             None, description="", alias="columnTopValues"
         )
+        column_depth_level: Optional[int] = Field(
+            None, description="", alias="columnDepthLevel"
+        )
         view: Optional[View] = Field(None, description="", alias="view")  # relationship
+        nested_columns: Optional[list[Column]] = Field(
+            None, description="", alias="nestedColumns"
+        )  # relationship
         data_quality_metric_dimensions: Optional[list[Metric]] = Field(
             None, description="", alias="dataQualityMetricDimensions"
         )  # relationship
         dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="dbtModelColumns"
         )  # relationship
         table: Optional[Table] = Field(
@@ -12027,14 +13224,17 @@
         )  # relationship
         column_dbt_model_columns: Optional[list[DbtModelColumn]] = Field(
             None, description="", alias="columnDbtModelColumns"
         )  # relationship
         materialised_view: Optional[MaterialisedView] = Field(
             None, description="", alias="materialisedView"
         )  # relationship
+        parent_column: Optional[Column] = Field(
+            None, description="", alias="parentColumn"
+        )  # relationship
         queries: Optional[list[Query]] = Field(
             None, description="", alias="queries"
         )  # relationship
         metric_timestamps: Optional[list[Metric]] = Field(
             None, description="", alias="metricTimestamps"
         )  # relationship
         foreign_key_to: Optional[list[Column]] = Field(
@@ -12051,46 +13251,52 @@
         )  # relationship
 
         @classmethod
         # @validate_arguments()
         def create(
             cls, *, name: str, parent_qualified_name: str, parent_type: type, order: int
         ) -> Column.Attributes:
-            if not name:
-                raise ValueError("name cannot be blank")
-            validate_required_fields(["parent_qualified_name"], [parent_qualified_name])
+            validate_required_fields(
+                ["name", "parent_qualified_name", "parent_type", "order"],
+                [name, parent_qualified_name, parent_type, order],
+            )
             fields = parent_qualified_name.split("/")
             if len(fields) != 6:
                 raise ValueError("Invalid parent_qualified_name")
             try:
                 connector_type = AtlanConnectorType(fields[1])  # type:ignore
             except ValueError as e:
                 raise ValueError("Invalid parent_qualified_name") from e
+            if order < 0:
+                raise ValueError("Order must be be a positive integer")
             ret_value = Column.Attributes(
                 name=name,
                 qualified_name=f"{parent_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 schema_name=fields[4],
                 schema_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}/{fields[4]}",
                 database_name=fields[3],
                 database_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}/{fields[3]}",
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 order=order,
             )
             if parent_type == Table:
                 ret_value.table_qualified_name = parent_qualified_name
                 ret_value.table = Table.ref_by_qualified_name(parent_qualified_name)
+                ret_value.table_name = fields[5]
             elif parent_type == View:
                 ret_value.view_qualified_name = parent_qualified_name
                 ret_value.view = View.ref_by_qualified_name(parent_qualified_name)
+                ret_value.view_name = fields[5]
             elif parent_type == MaterialisedView:
                 ret_value.view_qualified_name = parent_qualified_name
                 ret_value.materialised_view = MaterialisedView.ref_by_qualified_name(
                     parent_qualified_name
                 )
+                ret_value.view_name = fields[5]
             else:
                 raise ValueError(
                     "parent_type must be either Table, View or MaterializeView"
                 )
             return ret_value
 
     @classmethod
@@ -12133,105 +13339,105 @@
         "snowflake_streams",
         "procedures",
         "views",
     ]
 
     @property
     def table_count(self) -> Optional[int]:
-        return self.attributes.table_count
+        return None if self.attributes is None else self.attributes.table_count
 
     @table_count.setter
     def table_count(self, table_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table_count = table_count
 
     @property
     def views_count(self) -> Optional[int]:
-        return self.attributes.views_count
+        return None if self.attributes is None else self.attributes.views_count
 
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
     @property
     def snowflake_tags(self) -> Optional[list[SnowflakeTag]]:
-        return self.attributes.snowflake_tags
+        return None if self.attributes is None else self.attributes.snowflake_tags
 
     @snowflake_tags.setter
     def snowflake_tags(self, snowflake_tags: Optional[list[SnowflakeTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_tags = snowflake_tags
 
     @property
     def materialised_views(self) -> Optional[list[MaterialisedView]]:
-        return self.attributes.materialised_views
+        return None if self.attributes is None else self.attributes.materialised_views
 
     @materialised_views.setter
     def materialised_views(self, materialised_views: Optional[list[MaterialisedView]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.materialised_views = materialised_views
 
     @property
     def tables(self) -> Optional[list[Table]]:
-        return self.attributes.tables
+        return None if self.attributes is None else self.attributes.tables
 
     @tables.setter
     def tables(self, tables: Optional[list[Table]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tables = tables
 
     @property
     def database(self) -> Optional[Database]:
-        return self.attributes.database
+        return None if self.attributes is None else self.attributes.database
 
     @database.setter
     def database(self, database: Optional[Database]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.database = database
 
     @property
     def snowflake_pipes(self) -> Optional[list[SnowflakePipe]]:
-        return self.attributes.snowflake_pipes
+        return None if self.attributes is None else self.attributes.snowflake_pipes
 
     @snowflake_pipes.setter
     def snowflake_pipes(self, snowflake_pipes: Optional[list[SnowflakePipe]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_pipes = snowflake_pipes
 
     @property
     def snowflake_streams(self) -> Optional[list[SnowflakeStream]]:
-        return self.attributes.snowflake_streams
+        return None if self.attributes is None else self.attributes.snowflake_streams
 
     @snowflake_streams.setter
     def snowflake_streams(self, snowflake_streams: Optional[list[SnowflakeStream]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_streams = snowflake_streams
 
     @property
     def procedures(self) -> Optional[list[Procedure]]:
-        return self.attributes.procedures
+        return None if self.attributes is None else self.attributes.procedures
 
     @procedures.setter
     def procedures(self, procedures: Optional[list[Procedure]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.procedures = procedures
 
     @property
     def views(self) -> Optional[list[View]]:
-        return self.attributes.views
+        return None if self.attributes is None else self.attributes.views
 
     @views.setter
     def views(self, views: Optional[list[View]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
@@ -12331,67 +13537,83 @@
         "snowflake_stream_is_stale",
         "snowflake_stream_stale_after",
         "atlan_schema",
     ]
 
     @property
     def snowflake_stream_type(self) -> Optional[str]:
-        return self.attributes.snowflake_stream_type
+        return (
+            None if self.attributes is None else self.attributes.snowflake_stream_type
+        )
 
     @snowflake_stream_type.setter
     def snowflake_stream_type(self, snowflake_stream_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_type = snowflake_stream_type
 
     @property
     def snowflake_stream_source_type(self) -> Optional[str]:
-        return self.attributes.snowflake_stream_source_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_stream_source_type
+        )
 
     @snowflake_stream_source_type.setter
     def snowflake_stream_source_type(self, snowflake_stream_source_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_source_type = snowflake_stream_source_type
 
     @property
     def snowflake_stream_mode(self) -> Optional[str]:
-        return self.attributes.snowflake_stream_mode
+        return (
+            None if self.attributes is None else self.attributes.snowflake_stream_mode
+        )
 
     @snowflake_stream_mode.setter
     def snowflake_stream_mode(self, snowflake_stream_mode: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_mode = snowflake_stream_mode
 
     @property
     def snowflake_stream_is_stale(self) -> Optional[bool]:
-        return self.attributes.snowflake_stream_is_stale
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_stream_is_stale
+        )
 
     @snowflake_stream_is_stale.setter
     def snowflake_stream_is_stale(self, snowflake_stream_is_stale: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_is_stale = snowflake_stream_is_stale
 
     @property
     def snowflake_stream_stale_after(self) -> Optional[datetime]:
-        return self.attributes.snowflake_stream_stale_after
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_stream_stale_after
+        )
 
     @snowflake_stream_stale_after.setter
     def snowflake_stream_stale_after(
         self, snowflake_stream_stale_after: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_stream_stale_after = snowflake_stream_stale_after
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -12443,53 +13665,61 @@
         "snowflake_pipe_is_auto_ingest_enabled",
         "snowflake_pipe_notification_channel_name",
         "atlan_schema",
     ]
 
     @property
     def definition(self) -> Optional[str]:
-        return self.attributes.definition
+        return None if self.attributes is None else self.attributes.definition
 
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
     def snowflake_pipe_is_auto_ingest_enabled(self) -> Optional[bool]:
-        return self.attributes.snowflake_pipe_is_auto_ingest_enabled
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_pipe_is_auto_ingest_enabled
+        )
 
     @snowflake_pipe_is_auto_ingest_enabled.setter
     def snowflake_pipe_is_auto_ingest_enabled(
         self, snowflake_pipe_is_auto_ingest_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_pipe_is_auto_ingest_enabled = (
             snowflake_pipe_is_auto_ingest_enabled
         )
 
     @property
     def snowflake_pipe_notification_channel_name(self) -> Optional[str]:
-        return self.attributes.snowflake_pipe_notification_channel_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_pipe_notification_channel_name
+        )
 
     @snowflake_pipe_notification_channel_name.setter
     def snowflake_pipe_notification_channel_name(
         self, snowflake_pipe_notification_channel_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.snowflake_pipe_notification_channel_name = (
             snowflake_pipe_notification_channel_name
         )
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -12531,25 +13761,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "schema_count",
         "schemas",
     ]
 
     @property
     def schema_count(self) -> Optional[int]:
-        return self.attributes.schema_count
+        return None if self.attributes is None else self.attributes.schema_count
 
     @schema_count.setter
     def schema_count(self, schema_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schema_count = schema_count
 
     @property
     def schemas(self) -> Optional[list[Schema]]:
-        return self.attributes.schemas
+        return None if self.attributes is None else self.attributes.schemas
 
     @schemas.setter
     def schemas(self, schemas: Optional[list[Schema]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.schemas = schemas
 
@@ -12632,25 +13862,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "definition",
         "atlan_schema",
     ]
 
     @property
     def definition(self) -> str:
-        return self.attributes.definition
+        return None if self.attributes is None else self.attributes.definition
 
     @definition.setter
     def definition(self, definition: str):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -12695,115 +13925,115 @@
         "columns",
         "queries",
         "atlan_schema",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
-        return self.attributes.column_count
+        return None if self.attributes is None else self.attributes.column_count
 
     @column_count.setter
     def column_count(self, column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_count = column_count
 
     @property
     def row_count(self) -> Optional[int]:
-        return self.attributes.row_count
+        return None if self.attributes is None else self.attributes.row_count
 
     @row_count.setter
     def row_count(self, row_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_count = row_count
 
     @property
     def size_bytes(self) -> Optional[int]:
-        return self.attributes.size_bytes
+        return None if self.attributes is None else self.attributes.size_bytes
 
     @size_bytes.setter
     def size_bytes(self, size_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.size_bytes = size_bytes
 
     @property
     def is_query_preview(self) -> Optional[bool]:
-        return self.attributes.is_query_preview
+        return None if self.attributes is None else self.attributes.is_query_preview
 
     @is_query_preview.setter
     def is_query_preview(self, is_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_query_preview = is_query_preview
 
     @property
     def query_preview_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.query_preview_config
+        return None if self.attributes is None else self.attributes.query_preview_config
 
     @query_preview_config.setter
     def query_preview_config(self, query_preview_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_preview_config = query_preview_config
 
     @property
     def alias(self) -> Optional[str]:
-        return self.attributes.alias
+        return None if self.attributes is None else self.attributes.alias
 
     @alias.setter
     def alias(self, alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.alias = alias
 
     @property
     def is_temporary(self) -> Optional[bool]:
-        return self.attributes.is_temporary
+        return None if self.attributes is None else self.attributes.is_temporary
 
     @is_temporary.setter
     def is_temporary(self, is_temporary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_temporary = is_temporary
 
     @property
     def definition(self) -> Optional[str]:
-        return self.attributes.definition
+        return None if self.attributes is None else self.attributes.definition
 
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
     def columns(self) -> Optional[list[Column]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def queries(self) -> Optional[list[Query]]:
-        return self.attributes.queries
+        return None if self.attributes is None else self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[Query]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.queries = queries
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -12904,145 +14134,145 @@
         "definition",
         "columns",
         "atlan_schema",
     ]
 
     @property
     def refresh_mode(self) -> Optional[str]:
-        return self.attributes.refresh_mode
+        return None if self.attributes is None else self.attributes.refresh_mode
 
     @refresh_mode.setter
     def refresh_mode(self, refresh_mode: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.refresh_mode = refresh_mode
 
     @property
     def refresh_method(self) -> Optional[str]:
-        return self.attributes.refresh_method
+        return None if self.attributes is None else self.attributes.refresh_method
 
     @refresh_method.setter
     def refresh_method(self, refresh_method: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.refresh_method = refresh_method
 
     @property
     def staleness(self) -> Optional[str]:
-        return self.attributes.staleness
+        return None if self.attributes is None else self.attributes.staleness
 
     @staleness.setter
     def staleness(self, staleness: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.staleness = staleness
 
     @property
     def stale_since_date(self) -> Optional[datetime]:
-        return self.attributes.stale_since_date
+        return None if self.attributes is None else self.attributes.stale_since_date
 
     @stale_since_date.setter
     def stale_since_date(self, stale_since_date: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.stale_since_date = stale_since_date
 
     @property
     def column_count(self) -> Optional[int]:
-        return self.attributes.column_count
+        return None if self.attributes is None else self.attributes.column_count
 
     @column_count.setter
     def column_count(self, column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_count = column_count
 
     @property
     def row_count(self) -> Optional[int]:
-        return self.attributes.row_count
+        return None if self.attributes is None else self.attributes.row_count
 
     @row_count.setter
     def row_count(self, row_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.row_count = row_count
 
     @property
     def size_bytes(self) -> Optional[int]:
-        return self.attributes.size_bytes
+        return None if self.attributes is None else self.attributes.size_bytes
 
     @size_bytes.setter
     def size_bytes(self, size_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.size_bytes = size_bytes
 
     @property
     def is_query_preview(self) -> Optional[bool]:
-        return self.attributes.is_query_preview
+        return None if self.attributes is None else self.attributes.is_query_preview
 
     @is_query_preview.setter
     def is_query_preview(self, is_query_preview: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_query_preview = is_query_preview
 
     @property
     def query_preview_config(self) -> Optional[dict[str, str]]:
-        return self.attributes.query_preview_config
+        return None if self.attributes is None else self.attributes.query_preview_config
 
     @query_preview_config.setter
     def query_preview_config(self, query_preview_config: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_preview_config = query_preview_config
 
     @property
     def alias(self) -> Optional[str]:
-        return self.attributes.alias
+        return None if self.attributes is None else self.attributes.alias
 
     @alias.setter
     def alias(self, alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.alias = alias
 
     @property
     def is_temporary(self) -> Optional[bool]:
-        return self.attributes.is_temporary
+        return None if self.attributes is None else self.attributes.is_temporary
 
     @is_temporary.setter
     def is_temporary(self, is_temporary: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_temporary = is_temporary
 
     @property
     def definition(self) -> Optional[str]:
-        return self.attributes.definition
+        return None if self.attributes is None else self.attributes.definition
 
     @definition.setter
     def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     @property
     def columns(self) -> Optional[list[Column]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def atlan_schema(self) -> Optional[Schema]:
-        return self.attributes.atlan_schema
+        return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
@@ -13148,129 +14378,141 @@
         "google_location_type",
         "google_labels",
         "google_tags",
     ]
 
     @property
     def data_studio_asset_type(self) -> Optional[GoogleDatastudioAssetType]:
-        return self.attributes.data_studio_asset_type
+        return (
+            None if self.attributes is None else self.attributes.data_studio_asset_type
+        )
 
     @data_studio_asset_type.setter
     def data_studio_asset_type(
         self, data_studio_asset_type: Optional[GoogleDatastudioAssetType]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_studio_asset_type = data_studio_asset_type
 
     @property
     def data_studio_asset_title(self) -> Optional[str]:
-        return self.attributes.data_studio_asset_title
+        return (
+            None if self.attributes is None else self.attributes.data_studio_asset_title
+        )
 
     @data_studio_asset_title.setter
     def data_studio_asset_title(self, data_studio_asset_title: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_studio_asset_title = data_studio_asset_title
 
     @property
     def data_studio_asset_owner(self) -> Optional[str]:
-        return self.attributes.data_studio_asset_owner
+        return (
+            None if self.attributes is None else self.attributes.data_studio_asset_owner
+        )
 
     @data_studio_asset_owner.setter
     def data_studio_asset_owner(self, data_studio_asset_owner: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_studio_asset_owner = data_studio_asset_owner
 
     @property
     def is_trashed_data_studio_asset(self) -> Optional[bool]:
-        return self.attributes.is_trashed_data_studio_asset
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.is_trashed_data_studio_asset
+        )
 
     @is_trashed_data_studio_asset.setter
     def is_trashed_data_studio_asset(
         self, is_trashed_data_studio_asset: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_trashed_data_studio_asset = is_trashed_data_studio_asset
 
     @property
     def google_service(self) -> Optional[str]:
-        return self.attributes.google_service
+        return None if self.attributes is None else self.attributes.google_service
 
     @google_service.setter
     def google_service(self, google_service: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_service = google_service
 
     @property
     def google_project_name(self) -> Optional[str]:
-        return self.attributes.google_project_name
+        return None if self.attributes is None else self.attributes.google_project_name
 
     @google_project_name.setter
     def google_project_name(self, google_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_name = google_project_name
 
     @property
     def google_project_id(self) -> Optional[str]:
-        return self.attributes.google_project_id
+        return None if self.attributes is None else self.attributes.google_project_id
 
     @google_project_id.setter
     def google_project_id(self, google_project_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_id = google_project_id
 
     @property
     def google_project_number(self) -> Optional[int]:
-        return self.attributes.google_project_number
+        return (
+            None if self.attributes is None else self.attributes.google_project_number
+        )
 
     @google_project_number.setter
     def google_project_number(self, google_project_number: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_project_number = google_project_number
 
     @property
     def google_location(self) -> Optional[str]:
-        return self.attributes.google_location
+        return None if self.attributes is None else self.attributes.google_location
 
     @google_location.setter
     def google_location(self, google_location: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location = google_location
 
     @property
     def google_location_type(self) -> Optional[str]:
-        return self.attributes.google_location_type
+        return None if self.attributes is None else self.attributes.google_location_type
 
     @google_location_type.setter
     def google_location_type(self, google_location_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_location_type = google_location_type
 
     @property
     def google_labels(self) -> Optional[list[GoogleLabel]]:
-        return self.attributes.google_labels
+        return None if self.attributes is None else self.attributes.google_labels
 
     @google_labels.setter
     def google_labels(self, google_labels: Optional[list[GoogleLabel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_labels = google_labels
 
     @property
     def google_tags(self) -> Optional[list[GoogleTag]]:
-        return self.attributes.google_tags
+        return None if self.attributes is None else self.attributes.google_tags
 
     @google_tags.setter
     def google_tags(self, google_tags: Optional[list[GoogleTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.google_tags = google_tags
 
@@ -13345,101 +14587,133 @@
         "kafka_topic_record_count",
         "kafka_topic_cleanup_policy",
         "kafka_consumer_groups",
     ]
 
     @property
     def kafka_topic_is_internal(self) -> Optional[bool]:
-        return self.attributes.kafka_topic_is_internal
+        return (
+            None if self.attributes is None else self.attributes.kafka_topic_is_internal
+        )
 
     @kafka_topic_is_internal.setter
     def kafka_topic_is_internal(self, kafka_topic_is_internal: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_is_internal = kafka_topic_is_internal
 
     @property
     def kafka_topic_compression_type(self) -> Optional[KafkaTopicCompressionType]:
-        return self.attributes.kafka_topic_compression_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_compression_type
+        )
 
     @kafka_topic_compression_type.setter
     def kafka_topic_compression_type(
         self, kafka_topic_compression_type: Optional[KafkaTopicCompressionType]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_compression_type = kafka_topic_compression_type
 
     @property
     def kafka_topic_replication_factor(self) -> Optional[int]:
-        return self.attributes.kafka_topic_replication_factor
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_replication_factor
+        )
 
     @kafka_topic_replication_factor.setter
     def kafka_topic_replication_factor(
         self, kafka_topic_replication_factor: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_replication_factor = kafka_topic_replication_factor
 
     @property
     def kafka_topic_segment_bytes(self) -> Optional[int]:
-        return self.attributes.kafka_topic_segment_bytes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_segment_bytes
+        )
 
     @kafka_topic_segment_bytes.setter
     def kafka_topic_segment_bytes(self, kafka_topic_segment_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_segment_bytes = kafka_topic_segment_bytes
 
     @property
     def kafka_topic_partitions_count(self) -> Optional[int]:
-        return self.attributes.kafka_topic_partitions_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_partitions_count
+        )
 
     @kafka_topic_partitions_count.setter
     def kafka_topic_partitions_count(self, kafka_topic_partitions_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_partitions_count = kafka_topic_partitions_count
 
     @property
     def kafka_topic_size_in_bytes(self) -> Optional[int]:
-        return self.attributes.kafka_topic_size_in_bytes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_size_in_bytes
+        )
 
     @kafka_topic_size_in_bytes.setter
     def kafka_topic_size_in_bytes(self, kafka_topic_size_in_bytes: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_size_in_bytes = kafka_topic_size_in_bytes
 
     @property
     def kafka_topic_record_count(self) -> Optional[int]:
-        return self.attributes.kafka_topic_record_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_record_count
+        )
 
     @kafka_topic_record_count.setter
     def kafka_topic_record_count(self, kafka_topic_record_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_record_count = kafka_topic_record_count
 
     @property
     def kafka_topic_cleanup_policy(self) -> Optional[PowerbiEndorsement]:
-        return self.attributes.kafka_topic_cleanup_policy
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_cleanup_policy
+        )
 
     @kafka_topic_cleanup_policy.setter
     def kafka_topic_cleanup_policy(
         self, kafka_topic_cleanup_policy: Optional[PowerbiEndorsement]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_cleanup_policy = kafka_topic_cleanup_policy
 
     @property
     def kafka_consumer_groups(self) -> Optional[list[KafkaConsumerGroup]]:
-        return self.attributes.kafka_consumer_groups
+        return (
+            None if self.attributes is None else self.attributes.kafka_consumer_groups
+        )
 
     @kafka_consumer_groups.setter
     def kafka_consumer_groups(
         self, kafka_consumer_groups: Optional[list[KafkaConsumerGroup]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -13505,15 +14779,19 @@
         "kafka_topics",
     ]
 
     @property
     def kafka_consumer_group_topic_consumption_properties(
         self,
     ) -> Optional[list[KafkaTopicConsumption]]:
-        return self.attributes.kafka_consumer_group_topic_consumption_properties
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_consumer_group_topic_consumption_properties
+        )
 
     @kafka_consumer_group_topic_consumption_properties.setter
     def kafka_consumer_group_topic_consumption_properties(
         self,
         kafka_consumer_group_topic_consumption_properties: Optional[
             list[KafkaTopicConsumption]
         ],
@@ -13522,51 +14800,59 @@
             self.attributes = self.Attributes()
         self.attributes.kafka_consumer_group_topic_consumption_properties = (
             kafka_consumer_group_topic_consumption_properties
         )
 
     @property
     def kafka_consumer_group_member_count(self) -> Optional[int]:
-        return self.attributes.kafka_consumer_group_member_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_consumer_group_member_count
+        )
 
     @kafka_consumer_group_member_count.setter
     def kafka_consumer_group_member_count(
         self, kafka_consumer_group_member_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_consumer_group_member_count = (
             kafka_consumer_group_member_count
         )
 
     @property
     def kafka_topic_names(self) -> Optional[set[str]]:
-        return self.attributes.kafka_topic_names
+        return None if self.attributes is None else self.attributes.kafka_topic_names
 
     @kafka_topic_names.setter
     def kafka_topic_names(self, kafka_topic_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_names = kafka_topic_names
 
     @property
     def kafka_topic_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.kafka_topic_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.kafka_topic_qualified_names
+        )
 
     @kafka_topic_qualified_names.setter
     def kafka_topic_qualified_names(
         self, kafka_topic_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topic_qualified_names = kafka_topic_qualified_names
 
     @property
     def kafka_topics(self) -> Optional[list[KafkaTopic]]:
-        return self.attributes.kafka_topics
+        return None if self.attributes is None else self.attributes.kafka_topics
 
     @kafka_topics.setter
     def kafka_topics(self, kafka_topics: Optional[list[KafkaTopic]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.kafka_topics = kafka_topics
 
@@ -13616,37 +14902,41 @@
         "s3_object_count",
         "s3_bucket_versioning_enabled",
         "objects",
     ]
 
     @property
     def s3_object_count(self) -> Optional[int]:
-        return self.attributes.s3_object_count
+        return None if self.attributes is None else self.attributes.s3_object_count
 
     @s3_object_count.setter
     def s3_object_count(self, s3_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_count = s3_object_count
 
     @property
     def s3_bucket_versioning_enabled(self) -> Optional[bool]:
-        return self.attributes.s3_bucket_versioning_enabled
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.s3_bucket_versioning_enabled
+        )
 
     @s3_bucket_versioning_enabled.setter
     def s3_bucket_versioning_enabled(
         self, s3_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_bucket_versioning_enabled = s3_bucket_versioning_enabled
 
     @property
     def objects(self) -> Optional[list[S3Object]]:
-        return self.attributes.objects
+        return None if self.attributes is None else self.attributes.objects
 
     @objects.setter
     def objects(self, objects: Optional[list[S3Object]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.objects = objects
 
@@ -13739,109 +15029,125 @@
         "s3_object_content_disposition",
         "s3_object_version_id",
         "bucket",
     ]
 
     @property
     def s3_object_last_modified_time(self) -> Optional[datetime]:
-        return self.attributes.s3_object_last_modified_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.s3_object_last_modified_time
+        )
 
     @s3_object_last_modified_time.setter
     def s3_object_last_modified_time(
         self, s3_object_last_modified_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_last_modified_time = s3_object_last_modified_time
 
     @property
     def s3_bucket_name(self) -> Optional[str]:
-        return self.attributes.s3_bucket_name
+        return None if self.attributes is None else self.attributes.s3_bucket_name
 
     @s3_bucket_name.setter
     def s3_bucket_name(self, s3_bucket_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_bucket_name = s3_bucket_name
 
     @property
     def s3_bucket_qualified_name(self) -> Optional[str]:
-        return self.attributes.s3_bucket_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.s3_bucket_qualified_name
+        )
 
     @s3_bucket_qualified_name.setter
     def s3_bucket_qualified_name(self, s3_bucket_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_bucket_qualified_name = s3_bucket_qualified_name
 
     @property
     def s3_object_size(self) -> Optional[int]:
-        return self.attributes.s3_object_size
+        return None if self.attributes is None else self.attributes.s3_object_size
 
     @s3_object_size.setter
     def s3_object_size(self, s3_object_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_size = s3_object_size
 
     @property
     def s3_object_storage_class(self) -> Optional[str]:
-        return self.attributes.s3_object_storage_class
+        return (
+            None if self.attributes is None else self.attributes.s3_object_storage_class
+        )
 
     @s3_object_storage_class.setter
     def s3_object_storage_class(self, s3_object_storage_class: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_storage_class = s3_object_storage_class
 
     @property
     def s3_object_key(self) -> Optional[str]:
-        return self.attributes.s3_object_key
+        return None if self.attributes is None else self.attributes.s3_object_key
 
     @s3_object_key.setter
     def s3_object_key(self, s3_object_key: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_key = s3_object_key
 
     @property
     def s3_object_content_type(self) -> Optional[str]:
-        return self.attributes.s3_object_content_type
+        return (
+            None if self.attributes is None else self.attributes.s3_object_content_type
+        )
 
     @s3_object_content_type.setter
     def s3_object_content_type(self, s3_object_content_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_content_type = s3_object_content_type
 
     @property
     def s3_object_content_disposition(self) -> Optional[str]:
-        return self.attributes.s3_object_content_disposition
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.s3_object_content_disposition
+        )
 
     @s3_object_content_disposition.setter
     def s3_object_content_disposition(
         self, s3_object_content_disposition: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_content_disposition = s3_object_content_disposition
 
     @property
     def s3_object_version_id(self) -> Optional[str]:
-        return self.attributes.s3_object_version_id
+        return None if self.attributes is None else self.attributes.s3_object_version_id
 
     @s3_object_version_id.setter
     def s3_object_version_id(self, s3_object_version_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.s3_object_version_id = s3_object_version_id
 
     @property
     def bucket(self) -> Optional[S3Bucket]:
-        return self.attributes.bucket
+        return None if self.attributes is None else self.attributes.bucket
 
     @bucket.setter
     def bucket(self, bucket: Optional[S3Bucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.bucket = bucket
 
@@ -13966,125 +15272,151 @@
         "adls_account_provision_state",
         "adls_account_access_tier",
         "adls_containers",
     ]
 
     @property
     def adls_e_tag(self) -> Optional[str]:
-        return self.attributes.adls_e_tag
+        return None if self.attributes is None else self.attributes.adls_e_tag
 
     @adls_e_tag.setter
     def adls_e_tag(self, adls_e_tag: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_e_tag = adls_e_tag
 
     @property
     def adls_encryption_type(self) -> Optional[ADLSEncryptionTypes]:
-        return self.attributes.adls_encryption_type
+        return None if self.attributes is None else self.attributes.adls_encryption_type
 
     @adls_encryption_type.setter
     def adls_encryption_type(self, adls_encryption_type: Optional[ADLSEncryptionTypes]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_encryption_type = adls_encryption_type
 
     @property
     def adls_account_resource_group(self) -> Optional[str]:
-        return self.attributes.adls_account_resource_group
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_resource_group
+        )
 
     @adls_account_resource_group.setter
     def adls_account_resource_group(self, adls_account_resource_group: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_resource_group = adls_account_resource_group
 
     @property
     def adls_account_subscription(self) -> Optional[str]:
-        return self.attributes.adls_account_subscription
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_subscription
+        )
 
     @adls_account_subscription.setter
     def adls_account_subscription(self, adls_account_subscription: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_subscription = adls_account_subscription
 
     @property
     def adls_account_performance(self) -> Optional[ADLSPerformance]:
-        return self.attributes.adls_account_performance
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_performance
+        )
 
     @adls_account_performance.setter
     def adls_account_performance(
         self, adls_account_performance: Optional[ADLSPerformance]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_performance = adls_account_performance
 
     @property
     def adls_account_replication(self) -> Optional[ADLSReplicationType]:
-        return self.attributes.adls_account_replication
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_replication
+        )
 
     @adls_account_replication.setter
     def adls_account_replication(
         self, adls_account_replication: Optional[ADLSReplicationType]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_replication = adls_account_replication
 
     @property
     def adls_account_kind(self) -> Optional[ADLSStorageKind]:
-        return self.attributes.adls_account_kind
+        return None if self.attributes is None else self.attributes.adls_account_kind
 
     @adls_account_kind.setter
     def adls_account_kind(self, adls_account_kind: Optional[ADLSStorageKind]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_kind = adls_account_kind
 
     @property
     def adls_primary_disk_state(self) -> Optional[ADLSAccountStatus]:
-        return self.attributes.adls_primary_disk_state
+        return (
+            None if self.attributes is None else self.attributes.adls_primary_disk_state
+        )
 
     @adls_primary_disk_state.setter
     def adls_primary_disk_state(
         self, adls_primary_disk_state: Optional[ADLSAccountStatus]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_primary_disk_state = adls_primary_disk_state
 
     @property
     def adls_account_provision_state(self) -> Optional[ADLSProvisionState]:
-        return self.attributes.adls_account_provision_state
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_provision_state
+        )
 
     @adls_account_provision_state.setter
     def adls_account_provision_state(
         self, adls_account_provision_state: Optional[ADLSProvisionState]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_provision_state = adls_account_provision_state
 
     @property
     def adls_account_access_tier(self) -> Optional[ADLSAccessTier]:
-        return self.attributes.adls_account_access_tier
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_account_access_tier
+        )
 
     @adls_account_access_tier.setter
     def adls_account_access_tier(
         self, adls_account_access_tier: Optional[ADLSAccessTier]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account_access_tier = adls_account_access_tier
 
     @property
     def adls_containers(self) -> Optional[list[ADLSContainer]]:
-        return self.attributes.adls_containers
+        return None if self.attributes is None else self.attributes.adls_containers
 
     @adls_containers.setter
     def adls_containers(self, adls_containers: Optional[list[ADLSContainer]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_containers = adls_containers
 
@@ -14153,97 +15485,113 @@
         "adls_object_count",
         "adls_objects",
         "adls_account",
     ]
 
     @property
     def adls_container_url(self) -> Optional[str]:
-        return self.attributes.adls_container_url
+        return None if self.attributes is None else self.attributes.adls_container_url
 
     @adls_container_url.setter
     def adls_container_url(self, adls_container_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_url = adls_container_url
 
     @property
     def adls_container_lease_state(self) -> Optional[ADLSLeaseState]:
-        return self.attributes.adls_container_lease_state
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_container_lease_state
+        )
 
     @adls_container_lease_state.setter
     def adls_container_lease_state(
         self, adls_container_lease_state: Optional[ADLSLeaseState]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_lease_state = adls_container_lease_state
 
     @property
     def adls_container_lease_status(self) -> Optional[ADLSLeaseStatus]:
-        return self.attributes.adls_container_lease_status
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_container_lease_status
+        )
 
     @adls_container_lease_status.setter
     def adls_container_lease_status(
         self, adls_container_lease_status: Optional[ADLSLeaseStatus]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_lease_status = adls_container_lease_status
 
     @property
     def adls_container_encryption_scope(self) -> Optional[str]:
-        return self.attributes.adls_container_encryption_scope
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_container_encryption_scope
+        )
 
     @adls_container_encryption_scope.setter
     def adls_container_encryption_scope(
         self, adls_container_encryption_scope: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_encryption_scope = (
             adls_container_encryption_scope
         )
 
     @property
     def adls_container_version_level_immutability_support(self) -> Optional[bool]:
-        return self.attributes.adls_container_version_level_immutability_support
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_container_version_level_immutability_support
+        )
 
     @adls_container_version_level_immutability_support.setter
     def adls_container_version_level_immutability_support(
         self, adls_container_version_level_immutability_support: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_version_level_immutability_support = (
             adls_container_version_level_immutability_support
         )
 
     @property
     def adls_object_count(self) -> Optional[int]:
-        return self.attributes.adls_object_count
+        return None if self.attributes is None else self.attributes.adls_object_count
 
     @adls_object_count.setter
     def adls_object_count(self, adls_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_count = adls_object_count
 
     @property
     def adls_objects(self) -> Optional[list[ADLSObject]]:
-        return self.attributes.adls_objects
+        return None if self.attributes is None else self.attributes.adls_objects
 
     @adls_objects.setter
     def adls_objects(self, adls_objects: Optional[list[ADLSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_objects = adls_objects
 
     @property
     def adls_account(self) -> Optional[ADLSAccount]:
-        return self.attributes.adls_account
+        return None if self.attributes is None else self.attributes.adls_account
 
     @adls_account.setter
     def adls_account(self, adls_account: Optional[ADLSAccount]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_account = adls_account
 
@@ -14315,207 +15663,253 @@
         "adls_object_metadata",
         "adls_container_qualified_name",
         "adls_container",
     ]
 
     @property
     def adls_object_url(self) -> Optional[str]:
-        return self.attributes.adls_object_url
+        return None if self.attributes is None else self.attributes.adls_object_url
 
     @adls_object_url.setter
     def adls_object_url(self, adls_object_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_url = adls_object_url
 
     @property
     def adls_object_version_id(self) -> Optional[str]:
-        return self.attributes.adls_object_version_id
+        return (
+            None if self.attributes is None else self.attributes.adls_object_version_id
+        )
 
     @adls_object_version_id.setter
     def adls_object_version_id(self, adls_object_version_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_version_id = adls_object_version_id
 
     @property
     def adls_object_type(self) -> Optional[ADLSObjectType]:
-        return self.attributes.adls_object_type
+        return None if self.attributes is None else self.attributes.adls_object_type
 
     @adls_object_type.setter
     def adls_object_type(self, adls_object_type: Optional[ADLSObjectType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_type = adls_object_type
 
     @property
     def adls_object_size(self) -> Optional[int]:
-        return self.attributes.adls_object_size
+        return None if self.attributes is None else self.attributes.adls_object_size
 
     @adls_object_size.setter
     def adls_object_size(self, adls_object_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_size = adls_object_size
 
     @property
     def adls_object_access_tier(self) -> Optional[ADLSAccessTier]:
-        return self.attributes.adls_object_access_tier
+        return (
+            None if self.attributes is None else self.attributes.adls_object_access_tier
+        )
 
     @adls_object_access_tier.setter
     def adls_object_access_tier(
         self, adls_object_access_tier: Optional[ADLSAccessTier]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_access_tier = adls_object_access_tier
 
     @property
     def adls_object_access_tier_last_modified_time(self) -> Optional[datetime]:
-        return self.attributes.adls_object_access_tier_last_modified_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_access_tier_last_modified_time
+        )
 
     @adls_object_access_tier_last_modified_time.setter
     def adls_object_access_tier_last_modified_time(
         self, adls_object_access_tier_last_modified_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_access_tier_last_modified_time = (
             adls_object_access_tier_last_modified_time
         )
 
     @property
     def adls_object_archive_status(self) -> Optional[ADLSObjectArchiveStatus]:
-        return self.attributes.adls_object_archive_status
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_archive_status
+        )
 
     @adls_object_archive_status.setter
     def adls_object_archive_status(
         self, adls_object_archive_status: Optional[ADLSObjectArchiveStatus]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_archive_status = adls_object_archive_status
 
     @property
     def adls_object_server_encrypted(self) -> Optional[bool]:
-        return self.attributes.adls_object_server_encrypted
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_server_encrypted
+        )
 
     @adls_object_server_encrypted.setter
     def adls_object_server_encrypted(
         self, adls_object_server_encrypted: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_server_encrypted = adls_object_server_encrypted
 
     @property
     def adls_object_version_level_immutability_support(self) -> Optional[bool]:
-        return self.attributes.adls_object_version_level_immutability_support
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_version_level_immutability_support
+        )
 
     @adls_object_version_level_immutability_support.setter
     def adls_object_version_level_immutability_support(
         self, adls_object_version_level_immutability_support: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_version_level_immutability_support = (
             adls_object_version_level_immutability_support
         )
 
     @property
     def adls_object_cache_control(self) -> Optional[str]:
-        return self.attributes.adls_object_cache_control
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_cache_control
+        )
 
     @adls_object_cache_control.setter
     def adls_object_cache_control(self, adls_object_cache_control: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_cache_control = adls_object_cache_control
 
     @property
     def adls_object_content_type(self) -> Optional[str]:
-        return self.attributes.adls_object_content_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_content_type
+        )
 
     @adls_object_content_type.setter
     def adls_object_content_type(self, adls_object_content_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_content_type = adls_object_content_type
 
     @property
     def adls_object_content_m_d5_hash(self) -> Optional[str]:
-        return self.attributes.adls_object_content_m_d5_hash
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_content_m_d5_hash
+        )
 
     @adls_object_content_m_d5_hash.setter
     def adls_object_content_m_d5_hash(
         self, adls_object_content_m_d5_hash: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_content_m_d5_hash = adls_object_content_m_d5_hash
 
     @property
     def adls_object_content_language(self) -> Optional[str]:
-        return self.attributes.adls_object_content_language
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_content_language
+        )
 
     @adls_object_content_language.setter
     def adls_object_content_language(self, adls_object_content_language: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_content_language = adls_object_content_language
 
     @property
     def adls_object_lease_status(self) -> Optional[ADLSLeaseStatus]:
-        return self.attributes.adls_object_lease_status
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_object_lease_status
+        )
 
     @adls_object_lease_status.setter
     def adls_object_lease_status(
         self, adls_object_lease_status: Optional[ADLSLeaseStatus]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_lease_status = adls_object_lease_status
 
     @property
     def adls_object_lease_state(self) -> Optional[ADLSLeaseState]:
-        return self.attributes.adls_object_lease_state
+        return (
+            None if self.attributes is None else self.attributes.adls_object_lease_state
+        )
 
     @adls_object_lease_state.setter
     def adls_object_lease_state(
         self, adls_object_lease_state: Optional[ADLSLeaseState]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_lease_state = adls_object_lease_state
 
     @property
     def adls_object_metadata(self) -> Optional[dict[str, str]]:
-        return self.attributes.adls_object_metadata
+        return None if self.attributes is None else self.attributes.adls_object_metadata
 
     @adls_object_metadata.setter
     def adls_object_metadata(self, adls_object_metadata: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_object_metadata = adls_object_metadata
 
     @property
     def adls_container_qualified_name(self) -> Optional[str]:
-        return self.attributes.adls_container_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.adls_container_qualified_name
+        )
 
     @adls_container_qualified_name.setter
     def adls_container_qualified_name(
         self, adls_container_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container_qualified_name = adls_container_qualified_name
 
     @property
     def adls_container(self) -> Optional[ADLSContainer]:
-        return self.attributes.adls_container
+        return None if self.attributes is None else self.attributes.adls_container
 
     @adls_container.setter
     def adls_container(self, adls_container: Optional[ADLSContainer]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.adls_container = adls_container
 
@@ -14615,175 +16009,211 @@
         "gcs_object_content_language",
         "gcs_object_retention_expiration_date",
         "gcs_bucket",
     ]
 
     @property
     def gcs_bucket_name(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_name
+        return None if self.attributes is None else self.attributes.gcs_bucket_name
 
     @gcs_bucket_name.setter
     def gcs_bucket_name(self, gcs_bucket_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_name = gcs_bucket_name
 
     @property
     def gcs_bucket_qualified_name(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_qualified_name
+        )
 
     @gcs_bucket_qualified_name.setter
     def gcs_bucket_qualified_name(self, gcs_bucket_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_qualified_name = gcs_bucket_qualified_name
 
     @property
     def gcs_object_size(self) -> Optional[int]:
-        return self.attributes.gcs_object_size
+        return None if self.attributes is None else self.attributes.gcs_object_size
 
     @gcs_object_size.setter
     def gcs_object_size(self, gcs_object_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_size = gcs_object_size
 
     @property
     def gcs_object_key(self) -> Optional[str]:
-        return self.attributes.gcs_object_key
+        return None if self.attributes is None else self.attributes.gcs_object_key
 
     @gcs_object_key.setter
     def gcs_object_key(self, gcs_object_key: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_key = gcs_object_key
 
     @property
     def gcs_object_media_link(self) -> Optional[str]:
-        return self.attributes.gcs_object_media_link
+        return (
+            None if self.attributes is None else self.attributes.gcs_object_media_link
+        )
 
     @gcs_object_media_link.setter
     def gcs_object_media_link(self, gcs_object_media_link: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_media_link = gcs_object_media_link
 
     @property
     def gcs_object_hold_type(self) -> Optional[str]:
-        return self.attributes.gcs_object_hold_type
+        return None if self.attributes is None else self.attributes.gcs_object_hold_type
 
     @gcs_object_hold_type.setter
     def gcs_object_hold_type(self, gcs_object_hold_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_hold_type = gcs_object_hold_type
 
     @property
     def gcs_object_generation_id(self) -> Optional[int]:
-        return self.attributes.gcs_object_generation_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_generation_id
+        )
 
     @gcs_object_generation_id.setter
     def gcs_object_generation_id(self, gcs_object_generation_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_generation_id = gcs_object_generation_id
 
     @property
     def gcs_object_c_r_c32_c_hash(self) -> Optional[str]:
-        return self.attributes.gcs_object_c_r_c32_c_hash
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_c_r_c32_c_hash
+        )
 
     @gcs_object_c_r_c32_c_hash.setter
     def gcs_object_c_r_c32_c_hash(self, gcs_object_c_r_c32_c_hash: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_c_r_c32_c_hash = gcs_object_c_r_c32_c_hash
 
     @property
     def gcs_object_m_d5_hash(self) -> Optional[str]:
-        return self.attributes.gcs_object_m_d5_hash
+        return None if self.attributes is None else self.attributes.gcs_object_m_d5_hash
 
     @gcs_object_m_d5_hash.setter
     def gcs_object_m_d5_hash(self, gcs_object_m_d5_hash: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_m_d5_hash = gcs_object_m_d5_hash
 
     @property
     def gcs_object_data_last_modified_time(self) -> Optional[datetime]:
-        return self.attributes.gcs_object_data_last_modified_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_data_last_modified_time
+        )
 
     @gcs_object_data_last_modified_time.setter
     def gcs_object_data_last_modified_time(
         self, gcs_object_data_last_modified_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_data_last_modified_time = (
             gcs_object_data_last_modified_time
         )
 
     @property
     def gcs_object_content_type(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_type
+        return (
+            None if self.attributes is None else self.attributes.gcs_object_content_type
+        )
 
     @gcs_object_content_type.setter
     def gcs_object_content_type(self, gcs_object_content_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_content_type = gcs_object_content_type
 
     @property
     def gcs_object_content_encoding(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_encoding
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_content_encoding
+        )
 
     @gcs_object_content_encoding.setter
     def gcs_object_content_encoding(self, gcs_object_content_encoding: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_content_encoding = gcs_object_content_encoding
 
     @property
     def gcs_object_content_disposition(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_disposition
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_content_disposition
+        )
 
     @gcs_object_content_disposition.setter
     def gcs_object_content_disposition(
         self, gcs_object_content_disposition: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_content_disposition = gcs_object_content_disposition
 
     @property
     def gcs_object_content_language(self) -> Optional[str]:
-        return self.attributes.gcs_object_content_language
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_content_language
+        )
 
     @gcs_object_content_language.setter
     def gcs_object_content_language(self, gcs_object_content_language: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_content_language = gcs_object_content_language
 
     @property
     def gcs_object_retention_expiration_date(self) -> Optional[datetime]:
-        return self.attributes.gcs_object_retention_expiration_date
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_object_retention_expiration_date
+        )
 
     @gcs_object_retention_expiration_date.setter
     def gcs_object_retention_expiration_date(
         self, gcs_object_retention_expiration_date: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_retention_expiration_date = (
             gcs_object_retention_expiration_date
         )
 
     @property
     def gcs_bucket(self) -> Optional[GCSBucket]:
-        return self.attributes.gcs_bucket
+        return None if self.attributes is None else self.attributes.gcs_bucket
 
     @gcs_bucket.setter
     def gcs_bucket(self, gcs_bucket: Optional[GCSBucket]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket = gcs_bucket
 
@@ -14869,91 +16299,115 @@
         "gcs_bucket_lifecycle_rules",
         "gcs_bucket_retention_policy",
         "gcs_objects",
     ]
 
     @property
     def gcs_object_count(self) -> Optional[int]:
-        return self.attributes.gcs_object_count
+        return None if self.attributes is None else self.attributes.gcs_object_count
 
     @gcs_object_count.setter
     def gcs_object_count(self, gcs_object_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_object_count = gcs_object_count
 
     @property
     def gcs_bucket_versioning_enabled(self) -> Optional[bool]:
-        return self.attributes.gcs_bucket_versioning_enabled
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_versioning_enabled
+        )
 
     @gcs_bucket_versioning_enabled.setter
     def gcs_bucket_versioning_enabled(
         self, gcs_bucket_versioning_enabled: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_versioning_enabled = gcs_bucket_versioning_enabled
 
     @property
     def gcs_bucket_retention_locked(self) -> Optional[bool]:
-        return self.attributes.gcs_bucket_retention_locked
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_retention_locked
+        )
 
     @gcs_bucket_retention_locked.setter
     def gcs_bucket_retention_locked(self, gcs_bucket_retention_locked: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_locked = gcs_bucket_retention_locked
 
     @property
     def gcs_bucket_retention_period(self) -> Optional[int]:
-        return self.attributes.gcs_bucket_retention_period
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_retention_period
+        )
 
     @gcs_bucket_retention_period.setter
     def gcs_bucket_retention_period(self, gcs_bucket_retention_period: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_period = gcs_bucket_retention_period
 
     @property
     def gcs_bucket_retention_effective_time(self) -> Optional[datetime]:
-        return self.attributes.gcs_bucket_retention_effective_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_retention_effective_time
+        )
 
     @gcs_bucket_retention_effective_time.setter
     def gcs_bucket_retention_effective_time(
         self, gcs_bucket_retention_effective_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_effective_time = (
             gcs_bucket_retention_effective_time
         )
 
     @property
     def gcs_bucket_lifecycle_rules(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_lifecycle_rules
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_lifecycle_rules
+        )
 
     @gcs_bucket_lifecycle_rules.setter
     def gcs_bucket_lifecycle_rules(self, gcs_bucket_lifecycle_rules: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_lifecycle_rules = gcs_bucket_lifecycle_rules
 
     @property
     def gcs_bucket_retention_policy(self) -> Optional[str]:
-        return self.attributes.gcs_bucket_retention_policy
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.gcs_bucket_retention_policy
+        )
 
     @gcs_bucket_retention_policy.setter
     def gcs_bucket_retention_policy(self, gcs_bucket_retention_policy: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_bucket_retention_policy = gcs_bucket_retention_policy
 
     @property
     def gcs_objects(self) -> Optional[list[GCSObject]]:
-        return self.attributes.gcs_objects
+        return None if self.attributes is None else self.attributes.gcs_objects
 
     @gcs_objects.setter
     def gcs_objects(self, gcs_objects: Optional[list[GCSObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.gcs_objects = gcs_objects
 
@@ -15015,85 +16469,89 @@
         "mc_incident_warehouse",
         "mc_incident_assets",
         "mc_monitor",
     ]
 
     @property
     def mc_incident_id(self) -> Optional[str]:
-        return self.attributes.mc_incident_id
+        return None if self.attributes is None else self.attributes.mc_incident_id
 
     @mc_incident_id.setter
     def mc_incident_id(self, mc_incident_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_id = mc_incident_id
 
     @property
     def mc_incident_type(self) -> Optional[str]:
-        return self.attributes.mc_incident_type
+        return None if self.attributes is None else self.attributes.mc_incident_type
 
     @mc_incident_type.setter
     def mc_incident_type(self, mc_incident_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_type = mc_incident_type
 
     @property
     def mc_incident_sub_types(self) -> Optional[set[str]]:
-        return self.attributes.mc_incident_sub_types
+        return (
+            None if self.attributes is None else self.attributes.mc_incident_sub_types
+        )
 
     @mc_incident_sub_types.setter
     def mc_incident_sub_types(self, mc_incident_sub_types: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_sub_types = mc_incident_sub_types
 
     @property
     def mc_incident_severity(self) -> Optional[str]:
-        return self.attributes.mc_incident_severity
+        return None if self.attributes is None else self.attributes.mc_incident_severity
 
     @mc_incident_severity.setter
     def mc_incident_severity(self, mc_incident_severity: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_severity = mc_incident_severity
 
     @property
     def mc_incident_state(self) -> Optional[str]:
-        return self.attributes.mc_incident_state
+        return None if self.attributes is None else self.attributes.mc_incident_state
 
     @mc_incident_state.setter
     def mc_incident_state(self, mc_incident_state: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_state = mc_incident_state
 
     @property
     def mc_incident_warehouse(self) -> Optional[str]:
-        return self.attributes.mc_incident_warehouse
+        return (
+            None if self.attributes is None else self.attributes.mc_incident_warehouse
+        )
 
     @mc_incident_warehouse.setter
     def mc_incident_warehouse(self, mc_incident_warehouse: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_warehouse = mc_incident_warehouse
 
     @property
     def mc_incident_assets(self) -> Optional[list[Asset]]:
-        return self.attributes.mc_incident_assets
+        return None if self.attributes is None else self.attributes.mc_incident_assets
 
     @mc_incident_assets.setter
     def mc_incident_assets(self, mc_incident_assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_incident_assets = mc_incident_assets
 
     @property
     def mc_monitor(self) -> Optional[MCMonitor]:
-        return self.attributes.mc_monitor
+        return None if self.attributes is None else self.attributes.mc_monitor
 
     @mc_monitor.setter
     def mc_monitor(self, mc_monitor: Optional[MCMonitor]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor = mc_monitor
 
@@ -15165,203 +16623,245 @@
         "mc_monitor_breach_rate",
         "mc_monitor_incident_count",
         "mc_monitor_assets",
     ]
 
     @property
     def mc_monitor_id(self) -> Optional[str]:
-        return self.attributes.mc_monitor_id
+        return None if self.attributes is None else self.attributes.mc_monitor_id
 
     @mc_monitor_id.setter
     def mc_monitor_id(self, mc_monitor_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_id = mc_monitor_id
 
     @property
     def mc_monitor_status(self) -> Optional[str]:
-        return self.attributes.mc_monitor_status
+        return None if self.attributes is None else self.attributes.mc_monitor_status
 
     @mc_monitor_status.setter
     def mc_monitor_status(self, mc_monitor_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_status = mc_monitor_status
 
     @property
     def mc_monitor_type(self) -> Optional[str]:
-        return self.attributes.mc_monitor_type
+        return None if self.attributes is None else self.attributes.mc_monitor_type
 
     @mc_monitor_type.setter
     def mc_monitor_type(self, mc_monitor_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_type = mc_monitor_type
 
     @property
     def mc_monitor_warehouse(self) -> Optional[str]:
-        return self.attributes.mc_monitor_warehouse
+        return None if self.attributes is None else self.attributes.mc_monitor_warehouse
 
     @mc_monitor_warehouse.setter
     def mc_monitor_warehouse(self, mc_monitor_warehouse: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_warehouse = mc_monitor_warehouse
 
     @property
     def mc_monitor_schedule_type(self) -> Optional[str]:
-        return self.attributes.mc_monitor_schedule_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_schedule_type
+        )
 
     @mc_monitor_schedule_type.setter
     def mc_monitor_schedule_type(self, mc_monitor_schedule_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_schedule_type = mc_monitor_schedule_type
 
     @property
     def mc_monitor_namespace(self) -> Optional[str]:
-        return self.attributes.mc_monitor_namespace
+        return None if self.attributes is None else self.attributes.mc_monitor_namespace
 
     @mc_monitor_namespace.setter
     def mc_monitor_namespace(self, mc_monitor_namespace: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_namespace = mc_monitor_namespace
 
     @property
     def mc_monitor_rule_type(self) -> Optional[str]:
-        return self.attributes.mc_monitor_rule_type
+        return None if self.attributes is None else self.attributes.mc_monitor_rule_type
 
     @mc_monitor_rule_type.setter
     def mc_monitor_rule_type(self, mc_monitor_rule_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_type = mc_monitor_rule_type
 
     @property
     def mc_monitor_rule_custom_sql(self) -> Optional[str]:
-        return self.attributes.mc_monitor_rule_custom_sql
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_custom_sql
+        )
 
     @mc_monitor_rule_custom_sql.setter
     def mc_monitor_rule_custom_sql(self, mc_monitor_rule_custom_sql: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_custom_sql = mc_monitor_rule_custom_sql
 
     @property
     def mc_monitor_rule_schedule_config(self) -> Optional[MCRuleSchedule]:
-        return self.attributes.mc_monitor_rule_schedule_config
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_schedule_config
+        )
 
     @mc_monitor_rule_schedule_config.setter
     def mc_monitor_rule_schedule_config(
         self, mc_monitor_rule_schedule_config: Optional[MCRuleSchedule]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_schedule_config = (
             mc_monitor_rule_schedule_config
         )
 
     @property
     def mc_monitor_rule_schedule_config_humanized(self) -> Optional[str]:
-        return self.attributes.mc_monitor_rule_schedule_config_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_schedule_config_humanized
+        )
 
     @mc_monitor_rule_schedule_config_humanized.setter
     def mc_monitor_rule_schedule_config_humanized(
         self, mc_monitor_rule_schedule_config_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_schedule_config_humanized = (
             mc_monitor_rule_schedule_config_humanized
         )
 
     @property
     def mc_monitor_alert_condition(self) -> Optional[str]:
-        return self.attributes.mc_monitor_alert_condition
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_alert_condition
+        )
 
     @mc_monitor_alert_condition.setter
     def mc_monitor_alert_condition(self, mc_monitor_alert_condition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_alert_condition = mc_monitor_alert_condition
 
     @property
     def mc_monitor_rule_next_execution_time(self) -> Optional[datetime]:
-        return self.attributes.mc_monitor_rule_next_execution_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_next_execution_time
+        )
 
     @mc_monitor_rule_next_execution_time.setter
     def mc_monitor_rule_next_execution_time(
         self, mc_monitor_rule_next_execution_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_next_execution_time = (
             mc_monitor_rule_next_execution_time
         )
 
     @property
     def mc_monitor_rule_previous_execution_time(self) -> Optional[datetime]:
-        return self.attributes.mc_monitor_rule_previous_execution_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_previous_execution_time
+        )
 
     @mc_monitor_rule_previous_execution_time.setter
     def mc_monitor_rule_previous_execution_time(
         self, mc_monitor_rule_previous_execution_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_previous_execution_time = (
             mc_monitor_rule_previous_execution_time
         )
 
     @property
     def mc_monitor_rule_comparisons(self) -> Optional[list[MCRuleComparison]]:
-        return self.attributes.mc_monitor_rule_comparisons
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_comparisons
+        )
 
     @mc_monitor_rule_comparisons.setter
     def mc_monitor_rule_comparisons(
         self, mc_monitor_rule_comparisons: Optional[list[MCRuleComparison]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_comparisons = mc_monitor_rule_comparisons
 
     @property
     def mc_monitor_rule_is_snoozed(self) -> Optional[bool]:
-        return self.attributes.mc_monitor_rule_is_snoozed
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_rule_is_snoozed
+        )
 
     @mc_monitor_rule_is_snoozed.setter
     def mc_monitor_rule_is_snoozed(self, mc_monitor_rule_is_snoozed: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_rule_is_snoozed = mc_monitor_rule_is_snoozed
 
     @property
     def mc_monitor_breach_rate(self) -> Optional[float]:
-        return self.attributes.mc_monitor_breach_rate
+        return (
+            None if self.attributes is None else self.attributes.mc_monitor_breach_rate
+        )
 
     @mc_monitor_breach_rate.setter
     def mc_monitor_breach_rate(self, mc_monitor_breach_rate: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_breach_rate = mc_monitor_breach_rate
 
     @property
     def mc_monitor_incident_count(self) -> Optional[int]:
-        return self.attributes.mc_monitor_incident_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mc_monitor_incident_count
+        )
 
     @mc_monitor_incident_count.setter
     def mc_monitor_incident_count(self, mc_monitor_incident_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_incident_count = mc_monitor_incident_count
 
     @property
     def mc_monitor_assets(self) -> Optional[list[Asset]]:
-        return self.attributes.mc_monitor_assets
+        return None if self.attributes is None else self.attributes.mc_monitor_assets
 
     @mc_monitor_assets.setter
     def mc_monitor_assets(self, mc_monitor_assets: Optional[list[Asset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mc_monitor_assets = mc_monitor_assets
 
@@ -15446,39 +16946,45 @@
         "preset_chart_description_markdown",
         "preset_chart_form_data",
         "preset_dashboard",
     ]
 
     @property
     def preset_chart_description_markdown(self) -> Optional[str]:
-        return self.attributes.preset_chart_description_markdown
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_chart_description_markdown
+        )
 
     @preset_chart_description_markdown.setter
     def preset_chart_description_markdown(
         self, preset_chart_description_markdown: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_chart_description_markdown = (
             preset_chart_description_markdown
         )
 
     @property
     def preset_chart_form_data(self) -> Optional[dict[str, str]]:
-        return self.attributes.preset_chart_form_data
+        return (
+            None if self.attributes is None else self.attributes.preset_chart_form_data
+        )
 
     @preset_chart_form_data.setter
     def preset_chart_form_data(self, preset_chart_form_data: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_chart_form_data = preset_chart_form_data
 
     @property
     def preset_dashboard(self) -> Optional[PresetDashboard]:
-        return self.attributes.preset_dashboard
+        return None if self.attributes is None else self.attributes.preset_dashboard
 
     @preset_dashboard.setter
     def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard = preset_dashboard
 
@@ -15521,47 +17027,51 @@
         "preset_dataset_id",
         "preset_dataset_type",
         "preset_dashboard",
     ]
 
     @property
     def preset_dataset_datasource_name(self) -> Optional[str]:
-        return self.attributes.preset_dataset_datasource_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dataset_datasource_name
+        )
 
     @preset_dataset_datasource_name.setter
     def preset_dataset_datasource_name(
         self, preset_dataset_datasource_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dataset_datasource_name = preset_dataset_datasource_name
 
     @property
     def preset_dataset_id(self) -> Optional[int]:
-        return self.attributes.preset_dataset_id
+        return None if self.attributes is None else self.attributes.preset_dataset_id
 
     @preset_dataset_id.setter
     def preset_dataset_id(self, preset_dataset_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dataset_id = preset_dataset_id
 
     @property
     def preset_dataset_type(self) -> Optional[str]:
-        return self.attributes.preset_dataset_type
+        return None if self.attributes is None else self.attributes.preset_dataset_type
 
     @preset_dataset_type.setter
     def preset_dataset_type(self, preset_dataset_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dataset_type = preset_dataset_type
 
     @property
     def preset_dashboard(self) -> Optional[PresetDashboard]:
-        return self.attributes.preset_dashboard
+        return None if self.attributes is None else self.attributes.preset_dashboard
 
     @preset_dashboard.setter
     def preset_dashboard(self, preset_dashboard: Optional[PresetDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard = preset_dashboard
 
@@ -15612,111 +17122,135 @@
         "preset_datasets",
         "preset_charts",
         "preset_workspace",
     ]
 
     @property
     def preset_dashboard_changed_by_name(self) -> Optional[str]:
-        return self.attributes.preset_dashboard_changed_by_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_changed_by_name
+        )
 
     @preset_dashboard_changed_by_name.setter
     def preset_dashboard_changed_by_name(
         self, preset_dashboard_changed_by_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_changed_by_name = (
             preset_dashboard_changed_by_name
         )
 
     @property
     def preset_dashboard_changed_by_url(self) -> Optional[str]:
-        return self.attributes.preset_dashboard_changed_by_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_changed_by_url
+        )
 
     @preset_dashboard_changed_by_url.setter
     def preset_dashboard_changed_by_url(
         self, preset_dashboard_changed_by_url: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_changed_by_url = (
             preset_dashboard_changed_by_url
         )
 
     @property
     def preset_dashboard_is_managed_externally(self) -> Optional[bool]:
-        return self.attributes.preset_dashboard_is_managed_externally
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_is_managed_externally
+        )
 
     @preset_dashboard_is_managed_externally.setter
     def preset_dashboard_is_managed_externally(
         self, preset_dashboard_is_managed_externally: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_is_managed_externally = (
             preset_dashboard_is_managed_externally
         )
 
     @property
     def preset_dashboard_is_published(self) -> Optional[bool]:
-        return self.attributes.preset_dashboard_is_published
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_is_published
+        )
 
     @preset_dashboard_is_published.setter
     def preset_dashboard_is_published(
         self, preset_dashboard_is_published: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_is_published = preset_dashboard_is_published
 
     @property
     def preset_dashboard_thumbnail_url(self) -> Optional[str]:
-        return self.attributes.preset_dashboard_thumbnail_url
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_thumbnail_url
+        )
 
     @preset_dashboard_thumbnail_url.setter
     def preset_dashboard_thumbnail_url(
         self, preset_dashboard_thumbnail_url: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_thumbnail_url = preset_dashboard_thumbnail_url
 
     @property
     def preset_dashboard_chart_count(self) -> Optional[int]:
-        return self.attributes.preset_dashboard_chart_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_dashboard_chart_count
+        )
 
     @preset_dashboard_chart_count.setter
     def preset_dashboard_chart_count(self, preset_dashboard_chart_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboard_chart_count = preset_dashboard_chart_count
 
     @property
     def preset_datasets(self) -> Optional[list[PresetDataset]]:
-        return self.attributes.preset_datasets
+        return None if self.attributes is None else self.attributes.preset_datasets
 
     @preset_datasets.setter
     def preset_datasets(self, preset_datasets: Optional[list[PresetDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_datasets = preset_datasets
 
     @property
     def preset_charts(self) -> Optional[list[PresetChart]]:
-        return self.attributes.preset_charts
+        return None if self.attributes is None else self.attributes.preset_charts
 
     @preset_charts.setter
     def preset_charts(self, preset_charts: Optional[list[PresetChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_charts = preset_charts
 
     @property
     def preset_workspace(self) -> Optional[PresetWorkspace]:
-        return self.attributes.preset_workspace
+        return None if self.attributes is None else self.attributes.preset_workspace
 
     @preset_workspace.setter
     def preset_workspace(self, preset_workspace: Optional[PresetWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace = preset_workspace
 
@@ -15783,121 +17317,153 @@
         "preset_workspace_dashboard_count",
         "preset_workspace_dataset_count",
         "preset_dashboards",
     ]
 
     @property
     def preset_workspace_public_dashboards_allowed(self) -> Optional[bool]:
-        return self.attributes.preset_workspace_public_dashboards_allowed
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_public_dashboards_allowed
+        )
 
     @preset_workspace_public_dashboards_allowed.setter
     def preset_workspace_public_dashboards_allowed(
         self, preset_workspace_public_dashboards_allowed: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_public_dashboards_allowed = (
             preset_workspace_public_dashboards_allowed
         )
 
     @property
     def preset_workspace_cluster_id(self) -> Optional[int]:
-        return self.attributes.preset_workspace_cluster_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_cluster_id
+        )
 
     @preset_workspace_cluster_id.setter
     def preset_workspace_cluster_id(self, preset_workspace_cluster_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_cluster_id = preset_workspace_cluster_id
 
     @property
     def preset_workspace_hostname(self) -> Optional[str]:
-        return self.attributes.preset_workspace_hostname
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_hostname
+        )
 
     @preset_workspace_hostname.setter
     def preset_workspace_hostname(self, preset_workspace_hostname: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_hostname = preset_workspace_hostname
 
     @property
     def preset_workspace_is_in_maintenance_mode(self) -> Optional[bool]:
-        return self.attributes.preset_workspace_is_in_maintenance_mode
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_is_in_maintenance_mode
+        )
 
     @preset_workspace_is_in_maintenance_mode.setter
     def preset_workspace_is_in_maintenance_mode(
         self, preset_workspace_is_in_maintenance_mode: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_is_in_maintenance_mode = (
             preset_workspace_is_in_maintenance_mode
         )
 
     @property
     def preset_workspace_region(self) -> Optional[str]:
-        return self.attributes.preset_workspace_region
+        return (
+            None if self.attributes is None else self.attributes.preset_workspace_region
+        )
 
     @preset_workspace_region.setter
     def preset_workspace_region(self, preset_workspace_region: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_region = preset_workspace_region
 
     @property
     def preset_workspace_status(self) -> Optional[str]:
-        return self.attributes.preset_workspace_status
+        return (
+            None if self.attributes is None else self.attributes.preset_workspace_status
+        )
 
     @preset_workspace_status.setter
     def preset_workspace_status(self, preset_workspace_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_status = preset_workspace_status
 
     @property
     def preset_workspace_deployment_id(self) -> Optional[int]:
-        return self.attributes.preset_workspace_deployment_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_deployment_id
+        )
 
     @preset_workspace_deployment_id.setter
     def preset_workspace_deployment_id(
         self, preset_workspace_deployment_id: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_deployment_id = preset_workspace_deployment_id
 
     @property
     def preset_workspace_dashboard_count(self) -> Optional[int]:
-        return self.attributes.preset_workspace_dashboard_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_dashboard_count
+        )
 
     @preset_workspace_dashboard_count.setter
     def preset_workspace_dashboard_count(
         self, preset_workspace_dashboard_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_dashboard_count = (
             preset_workspace_dashboard_count
         )
 
     @property
     def preset_workspace_dataset_count(self) -> Optional[int]:
-        return self.attributes.preset_workspace_dataset_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.preset_workspace_dataset_count
+        )
 
     @preset_workspace_dataset_count.setter
     def preset_workspace_dataset_count(
         self, preset_workspace_dataset_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_workspace_dataset_count = preset_workspace_dataset_count
 
     @property
     def preset_dashboards(self) -> Optional[list[PresetDashboard]]:
-        return self.attributes.preset_dashboards
+        return None if self.attributes is None else self.attributes.preset_dashboards
 
     @preset_dashboards.setter
     def preset_dashboards(self, preset_dashboards: Optional[list[PresetDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.preset_dashboards = preset_dashboards
 
@@ -15966,95 +17532,101 @@
         "mode_is_shared",
         "mode_collections",
         "mode_queries",
     ]
 
     @property
     def mode_collection_token(self) -> Optional[str]:
-        return self.attributes.mode_collection_token
+        return (
+            None if self.attributes is None else self.attributes.mode_collection_token
+        )
 
     @mode_collection_token.setter
     def mode_collection_token(self, mode_collection_token: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_token = mode_collection_token
 
     @property
     def mode_report_published_at(self) -> Optional[datetime]:
-        return self.attributes.mode_report_published_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mode_report_published_at
+        )
 
     @mode_report_published_at.setter
     def mode_report_published_at(self, mode_report_published_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_published_at = mode_report_published_at
 
     @property
     def mode_query_count(self) -> Optional[int]:
-        return self.attributes.mode_query_count
+        return None if self.attributes is None else self.attributes.mode_query_count
 
     @mode_query_count.setter
     def mode_query_count(self, mode_query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_count = mode_query_count
 
     @property
     def mode_chart_count(self) -> Optional[int]:
-        return self.attributes.mode_chart_count
+        return None if self.attributes is None else self.attributes.mode_chart_count
 
     @mode_chart_count.setter
     def mode_chart_count(self, mode_chart_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_chart_count = mode_chart_count
 
     @property
     def mode_query_preview(self) -> Optional[str]:
-        return self.attributes.mode_query_preview
+        return None if self.attributes is None else self.attributes.mode_query_preview
 
     @mode_query_preview.setter
     def mode_query_preview(self, mode_query_preview: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query_preview = mode_query_preview
 
     @property
     def mode_is_public(self) -> Optional[bool]:
-        return self.attributes.mode_is_public
+        return None if self.attributes is None else self.attributes.mode_is_public
 
     @mode_is_public.setter
     def mode_is_public(self, mode_is_public: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_is_public = mode_is_public
 
     @property
     def mode_is_shared(self) -> Optional[bool]:
-        return self.attributes.mode_is_shared
+        return None if self.attributes is None else self.attributes.mode_is_shared
 
     @mode_is_shared.setter
     def mode_is_shared(self, mode_is_shared: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_is_shared = mode_is_shared
 
     @property
     def mode_collections(self) -> Optional[list[ModeCollection]]:
-        return self.attributes.mode_collections
+        return None if self.attributes is None else self.attributes.mode_collections
 
     @mode_collections.setter
     def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collections = mode_collections
 
     @property
     def mode_queries(self) -> Optional[list[ModeQuery]]:
-        return self.attributes.mode_queries
+        return None if self.attributes is None else self.attributes.mode_queries
 
     @mode_queries.setter
     def mode_queries(self, mode_queries: Optional[list[ModeQuery]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_queries = mode_queries
 
@@ -16115,45 +17687,49 @@
         "mode_report_import_count",
         "mode_charts",
         "mode_report",
     ]
 
     @property
     def mode_raw_query(self) -> Optional[str]:
-        return self.attributes.mode_raw_query
+        return None if self.attributes is None else self.attributes.mode_raw_query
 
     @mode_raw_query.setter
     def mode_raw_query(self, mode_raw_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_raw_query = mode_raw_query
 
     @property
     def mode_report_import_count(self) -> Optional[int]:
-        return self.attributes.mode_report_import_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.mode_report_import_count
+        )
 
     @mode_report_import_count.setter
     def mode_report_import_count(self, mode_report_import_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report_import_count = mode_report_import_count
 
     @property
     def mode_charts(self) -> Optional[list[ModeChart]]:
-        return self.attributes.mode_charts
+        return None if self.attributes is None else self.attributes.mode_charts
 
     @mode_charts.setter
     def mode_charts(self, mode_charts: Optional[list[ModeChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_charts = mode_charts
 
     @property
     def mode_report(self) -> Optional[ModeReport]:
-        return self.attributes.mode_report
+        return None if self.attributes is None else self.attributes.mode_report
 
     @mode_report.setter
     def mode_report(self, mode_report: Optional[ModeReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_report = mode_report
 
@@ -16197,25 +17773,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "mode_chart_type",
         "mode_query",
     ]
 
     @property
     def mode_chart_type(self) -> Optional[str]:
-        return self.attributes.mode_chart_type
+        return None if self.attributes is None else self.attributes.mode_chart_type
 
     @mode_chart_type.setter
     def mode_chart_type(self, mode_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_chart_type = mode_chart_type
 
     @property
     def mode_query(self) -> Optional[ModeQuery]:
-        return self.attributes.mode_query
+        return None if self.attributes is None else self.attributes.mode_query
 
     @mode_query.setter
     def mode_query(self, mode_query: Optional[ModeQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_query = mode_query
 
@@ -16253,25 +17829,27 @@
     _convience_properties: ClassVar[list[str]] = [
         "mode_collection_count",
         "mode_collections",
     ]
 
     @property
     def mode_collection_count(self) -> Optional[int]:
-        return self.attributes.mode_collection_count
+        return (
+            None if self.attributes is None else self.attributes.mode_collection_count
+        )
 
     @mode_collection_count.setter
     def mode_collection_count(self, mode_collection_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_count = mode_collection_count
 
     @property
     def mode_collections(self) -> Optional[list[ModeCollection]]:
-        return self.attributes.mode_collections
+        return None if self.attributes is None else self.attributes.mode_collections
 
     @mode_collections.setter
     def mode_collections(self, mode_collections: Optional[list[ModeCollection]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collections = mode_collections
 
@@ -16311,45 +17889,47 @@
         "mode_collection_state",
         "mode_workspace",
         "mode_reports",
     ]
 
     @property
     def mode_collection_type(self) -> Optional[str]:
-        return self.attributes.mode_collection_type
+        return None if self.attributes is None else self.attributes.mode_collection_type
 
     @mode_collection_type.setter
     def mode_collection_type(self, mode_collection_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_type = mode_collection_type
 
     @property
     def mode_collection_state(self) -> Optional[str]:
-        return self.attributes.mode_collection_state
+        return (
+            None if self.attributes is None else self.attributes.mode_collection_state
+        )
 
     @mode_collection_state.setter
     def mode_collection_state(self, mode_collection_state: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_collection_state = mode_collection_state
 
     @property
     def mode_workspace(self) -> Optional[ModeWorkspace]:
-        return self.attributes.mode_workspace
+        return None if self.attributes is None else self.attributes.mode_workspace
 
     @mode_workspace.setter
     def mode_workspace(self, mode_workspace: Optional[ModeWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_workspace = mode_workspace
 
     @property
     def mode_reports(self) -> Optional[list[ModeReport]]:
-        return self.attributes.mode_reports
+        return None if self.attributes is None else self.attributes.mode_reports
 
     @mode_reports.setter
     def mode_reports(self, mode_reports: Optional[list[ModeReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.mode_reports = mode_reports
 
@@ -16394,35 +17974,39 @@
         "sigma_dataset_qualified_name",
         "sigma_dataset_name",
         "sigma_dataset",
     ]
 
     @property
     def sigma_dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.sigma_dataset_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_dataset_qualified_name
+        )
 
     @sigma_dataset_qualified_name.setter
     def sigma_dataset_qualified_name(self, sigma_dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_qualified_name = sigma_dataset_qualified_name
 
     @property
     def sigma_dataset_name(self) -> Optional[str]:
-        return self.attributes.sigma_dataset_name
+        return None if self.attributes is None else self.attributes.sigma_dataset_name
 
     @sigma_dataset_name.setter
     def sigma_dataset_name(self, sigma_dataset_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_name = sigma_dataset_name
 
     @property
     def sigma_dataset(self) -> Optional[SigmaDataset]:
-        return self.attributes.sigma_dataset
+        return None if self.attributes is None else self.attributes.sigma_dataset
 
     @sigma_dataset.setter
     def sigma_dataset(self, sigma_dataset: Optional[SigmaDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset = sigma_dataset
 
@@ -16463,25 +18047,31 @@
     _convience_properties: ClassVar[list[str]] = [
         "sigma_dataset_column_count",
         "sigma_dataset_columns",
     ]
 
     @property
     def sigma_dataset_column_count(self) -> Optional[int]:
-        return self.attributes.sigma_dataset_column_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_dataset_column_count
+        )
 
     @sigma_dataset_column_count.setter
     def sigma_dataset_column_count(self, sigma_dataset_column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_dataset_column_count = sigma_dataset_column_count
 
     @property
     def sigma_dataset_columns(self) -> Optional[list[SigmaDatasetColumn]]:
-        return self.attributes.sigma_dataset_columns
+        return (
+            None if self.attributes is None else self.attributes.sigma_dataset_columns
+        )
 
     @sigma_dataset_columns.setter
     def sigma_dataset_columns(
         self, sigma_dataset_columns: Optional[list[SigmaDatasetColumn]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -16521,25 +18111,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "sigma_page_count",
         "sigma_pages",
     ]
 
     @property
     def sigma_page_count(self) -> Optional[int]:
-        return self.attributes.sigma_page_count
+        return None if self.attributes is None else self.attributes.sigma_page_count
 
     @sigma_page_count.setter
     def sigma_page_count(self, sigma_page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page_count = sigma_page_count
 
     @property
     def sigma_pages(self) -> Optional[list[SigmaPage]]:
-        return self.attributes.sigma_pages
+        return None if self.attributes is None else self.attributes.sigma_pages
 
     @sigma_pages.setter
     def sigma_pages(self, sigma_pages: Optional[list[SigmaPage]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_pages = sigma_pages
 
@@ -16578,43 +18168,51 @@
         "sigma_data_element_field_is_hidden",
         "sigma_data_element_field_formula",
         "sigma_data_element",
     ]
 
     @property
     def sigma_data_element_field_is_hidden(self) -> Optional[bool]:
-        return self.attributes.sigma_data_element_field_is_hidden
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_field_is_hidden
+        )
 
     @sigma_data_element_field_is_hidden.setter
     def sigma_data_element_field_is_hidden(
         self, sigma_data_element_field_is_hidden: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_is_hidden = (
             sigma_data_element_field_is_hidden
         )
 
     @property
     def sigma_data_element_field_formula(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_field_formula
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_field_formula
+        )
 
     @sigma_data_element_field_formula.setter
     def sigma_data_element_field_formula(
         self, sigma_data_element_field_formula: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_formula = (
             sigma_data_element_field_formula
         )
 
     @property
     def sigma_data_element(self) -> Optional[SigmaDataElement]:
-        return self.attributes.sigma_data_element
+        return None if self.attributes is None else self.attributes.sigma_data_element
 
     @sigma_data_element.setter
     def sigma_data_element(self, sigma_data_element: Optional[SigmaDataElement]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element = sigma_data_element
 
@@ -16656,37 +18254,41 @@
         "sigma_data_element_count",
         "sigma_data_elements",
         "sigma_workbook",
     ]
 
     @property
     def sigma_data_element_count(self) -> Optional[int]:
-        return self.attributes.sigma_data_element_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_count
+        )
 
     @sigma_data_element_count.setter
     def sigma_data_element_count(self, sigma_data_element_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_count = sigma_data_element_count
 
     @property
     def sigma_data_elements(self) -> Optional[list[SigmaDataElement]]:
-        return self.attributes.sigma_data_elements
+        return None if self.attributes is None else self.attributes.sigma_data_elements
 
     @sigma_data_elements.setter
     def sigma_data_elements(
         self, sigma_data_elements: Optional[list[SigmaDataElement]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_elements = sigma_data_elements
 
     @property
     def sigma_workbook(self) -> Optional[SigmaWorkbook]:
-        return self.attributes.sigma_workbook
+        return None if self.attributes is None else self.attributes.sigma_workbook
 
     @sigma_workbook.setter
     def sigma_workbook(self, sigma_workbook: Optional[SigmaWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_workbook = sigma_workbook
 
@@ -16730,57 +18332,71 @@
         "sigma_data_element_field_count",
         "sigma_page",
         "sigma_data_element_fields",
     ]
 
     @property
     def sigma_data_element_query(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_query
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_query
+        )
 
     @sigma_data_element_query.setter
     def sigma_data_element_query(self, sigma_data_element_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_query = sigma_data_element_query
 
     @property
     def sigma_data_element_type(self) -> Optional[str]:
-        return self.attributes.sigma_data_element_type
+        return (
+            None if self.attributes is None else self.attributes.sigma_data_element_type
+        )
 
     @sigma_data_element_type.setter
     def sigma_data_element_type(self, sigma_data_element_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_type = sigma_data_element_type
 
     @property
     def sigma_data_element_field_count(self) -> Optional[int]:
-        return self.attributes.sigma_data_element_field_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_field_count
+        )
 
     @sigma_data_element_field_count.setter
     def sigma_data_element_field_count(
         self, sigma_data_element_field_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_data_element_field_count = sigma_data_element_field_count
 
     @property
     def sigma_page(self) -> Optional[SigmaPage]:
-        return self.attributes.sigma_page
+        return None if self.attributes is None else self.attributes.sigma_page
 
     @sigma_page.setter
     def sigma_page(self, sigma_page: Optional[SigmaPage]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sigma_page = sigma_page
 
     @property
     def sigma_data_element_fields(self) -> Optional[list[SigmaDataElementField]]:
-        return self.attributes.sigma_data_element_fields
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.sigma_data_element_fields
+        )
 
     @sigma_data_element_fields.setter
     def sigma_data_element_fields(
         self, sigma_data_element_fields: Optional[list[SigmaDataElementField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -16836,99 +18452,107 @@
         "dashboards",
         "worksheets",
         "datasources",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_name
+        return (
+            None if self.attributes is None else self.attributes.top_level_project_name
+        )
 
     @top_level_project_name.setter
     def top_level_project_name(self, top_level_project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_name = top_level_project_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def project(self) -> Optional[TableauProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def dashboards(self) -> Optional[list[TableauDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[TableauDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
     @property
     def worksheets(self) -> Optional[list[TableauWorksheet]]:
-        return self.attributes.worksheets
+        return None if self.attributes is None else self.attributes.worksheets
 
     @worksheets.setter
     def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.worksheets = worksheets
 
     @property
     def datasources(self) -> Optional[list[TableauDatasource]]:
-        return self.attributes.datasources
+        return None if self.attributes is None else self.attributes.datasources
 
     @datasources.setter
     def datasources(self, datasources: Optional[list[TableauDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasources = datasources
 
@@ -17003,207 +18627,241 @@
         "datasource_field_type",
         "worksheets",
         "datasource",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.workbook_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.workbook_qualified_name
+        )
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
     def datasource_qualified_name(self) -> Optional[str]:
-        return self.attributes.datasource_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.datasource_qualified_name
+        )
 
     @datasource_qualified_name.setter
     def datasource_qualified_name(self, datasource_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_qualified_name = datasource_qualified_name
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def fully_qualified_name(self) -> Optional[str]:
-        return self.attributes.fully_qualified_name
+        return None if self.attributes is None else self.attributes.fully_qualified_name
 
     @fully_qualified_name.setter
     def fully_qualified_name(self, fully_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fully_qualified_name = fully_qualified_name
 
     @property
     def tableau_datasource_field_data_category(self) -> Optional[str]:
-        return self.attributes.tableau_datasource_field_data_category
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.tableau_datasource_field_data_category
+        )
 
     @tableau_datasource_field_data_category.setter
     def tableau_datasource_field_data_category(
         self, tableau_datasource_field_data_category: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_datasource_field_data_category = (
             tableau_datasource_field_data_category
         )
 
     @property
     def tableau_datasource_field_role(self) -> Optional[str]:
-        return self.attributes.tableau_datasource_field_role
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.tableau_datasource_field_role
+        )
 
     @tableau_datasource_field_role.setter
     def tableau_datasource_field_role(
         self, tableau_datasource_field_role: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_datasource_field_role = tableau_datasource_field_role
 
     @property
     def tableau_datasource_field_data_type(self) -> Optional[str]:
-        return self.attributes.tableau_datasource_field_data_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.tableau_datasource_field_data_type
+        )
 
     @tableau_datasource_field_data_type.setter
     def tableau_datasource_field_data_type(
         self, tableau_datasource_field_data_type: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_datasource_field_data_type = (
             tableau_datasource_field_data_type
         )
 
     @property
     def upstream_tables(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_tables
+        return None if self.attributes is None else self.attributes.upstream_tables
 
     @upstream_tables.setter
     def upstream_tables(self, upstream_tables: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_tables = upstream_tables
 
     @property
     def tableau_datasource_field_formula(self) -> Optional[str]:
-        return self.attributes.tableau_datasource_field_formula
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.tableau_datasource_field_formula
+        )
 
     @tableau_datasource_field_formula.setter
     def tableau_datasource_field_formula(
         self, tableau_datasource_field_formula: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_datasource_field_formula = (
             tableau_datasource_field_formula
         )
 
     @property
     def tableau_datasource_field_bin_size(self) -> Optional[str]:
-        return self.attributes.tableau_datasource_field_bin_size
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.tableau_datasource_field_bin_size
+        )
 
     @tableau_datasource_field_bin_size.setter
     def tableau_datasource_field_bin_size(
         self, tableau_datasource_field_bin_size: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_datasource_field_bin_size = (
             tableau_datasource_field_bin_size
         )
 
     @property
     def upstream_columns(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_columns
+        return None if self.attributes is None else self.attributes.upstream_columns
 
     @upstream_columns.setter
     def upstream_columns(self, upstream_columns: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_columns = upstream_columns
 
     @property
     def upstream_fields(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_fields
+        return None if self.attributes is None else self.attributes.upstream_fields
 
     @upstream_fields.setter
     def upstream_fields(self, upstream_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_fields = upstream_fields
 
     @property
     def datasource_field_type(self) -> Optional[str]:
-        return self.attributes.datasource_field_type
+        return (
+            None if self.attributes is None else self.attributes.datasource_field_type
+        )
 
     @datasource_field_type.setter
     def datasource_field_type(self, datasource_field_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_field_type = datasource_field_type
 
     @property
     def worksheets(self) -> Optional[list[TableauWorksheet]]:
-        return self.attributes.worksheets
+        return None if self.attributes is None else self.attributes.worksheets
 
     @worksheets.setter
     def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.worksheets = worksheets
 
     @property
     def datasource(self) -> Optional[TableauDatasource]:
-        return self.attributes.datasource
+        return None if self.attributes is None else self.attributes.datasource
 
     @datasource.setter
     def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource = datasource
 
@@ -17300,139 +18958,151 @@
         "upstream_fields",
         "worksheets",
         "datasource",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.workbook_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.workbook_qualified_name
+        )
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
     def datasource_qualified_name(self) -> Optional[str]:
-        return self.attributes.datasource_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.datasource_qualified_name
+        )
 
     @datasource_qualified_name.setter
     def datasource_qualified_name(self, datasource_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_qualified_name = datasource_qualified_name
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def data_category(self) -> Optional[str]:
-        return self.attributes.data_category
+        return None if self.attributes is None else self.attributes.data_category
 
     @data_category.setter
     def data_category(self, data_category: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_category = data_category
 
     @property
     def role(self) -> Optional[str]:
-        return self.attributes.role
+        return None if self.attributes is None else self.attributes.role
 
     @role.setter
     def role(self, role: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.role = role
 
     @property
     def tableau_data_type(self) -> Optional[str]:
-        return self.attributes.tableau_data_type
+        return None if self.attributes is None else self.attributes.tableau_data_type
 
     @tableau_data_type.setter
     def tableau_data_type(self, tableau_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tableau_data_type = tableau_data_type
 
     @property
     def formula(self) -> Optional[str]:
-        return self.attributes.formula
+        return None if self.attributes is None else self.attributes.formula
 
     @formula.setter
     def formula(self, formula: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.formula = formula
 
     @property
     def upstream_fields(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_fields
+        return None if self.attributes is None else self.attributes.upstream_fields
 
     @upstream_fields.setter
     def upstream_fields(self, upstream_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_fields = upstream_fields
 
     @property
     def worksheets(self) -> Optional[list[TableauWorksheet]]:
-        return self.attributes.worksheets
+        return None if self.attributes is None else self.attributes.worksheets
 
     @worksheets.setter
     def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.worksheets = worksheets
 
     @property
     def datasource(self) -> Optional[TableauDatasource]:
-        return self.attributes.datasource
+        return None if self.attributes is None else self.attributes.datasource
 
     @datasource.setter
     def datasource(self, datasource: Optional[TableauDatasource]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource = datasource
 
@@ -17505,109 +19175,113 @@
         "datasources",
         "flows",
         "child_projects",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def is_top_level_project(self) -> Optional[bool]:
-        return self.attributes.is_top_level_project
+        return None if self.attributes is None else self.attributes.is_top_level_project
 
     @is_top_level_project.setter
     def is_top_level_project(self, is_top_level_project: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_top_level_project = is_top_level_project
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def parent_project(self) -> Optional[TableauProject]:
-        return self.attributes.parent_project
+        return None if self.attributes is None else self.attributes.parent_project
 
     @parent_project.setter
     def parent_project(self, parent_project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_project = parent_project
 
     @property
     def workbooks(self) -> Optional[list[TableauWorkbook]]:
-        return self.attributes.workbooks
+        return None if self.attributes is None else self.attributes.workbooks
 
     @workbooks.setter
     def workbooks(self, workbooks: Optional[list[TableauWorkbook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbooks = workbooks
 
     @property
     def site(self) -> Optional[TableauSite]:
-        return self.attributes.site
+        return None if self.attributes is None else self.attributes.site
 
     @site.setter
     def site(self, site: Optional[TableauSite]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site = site
 
     @property
     def datasources(self) -> Optional[list[TableauDatasource]]:
-        return self.attributes.datasources
+        return None if self.attributes is None else self.attributes.datasources
 
     @datasources.setter
     def datasources(self, datasources: Optional[list[TableauDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasources = datasources
 
     @property
     def flows(self) -> Optional[list[TableauFlow]]:
-        return self.attributes.flows
+        return None if self.attributes is None else self.attributes.flows
 
     @flows.setter
     def flows(self, flows: Optional[list[TableauFlow]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.flows = flows
 
     @property
     def child_projects(self) -> Optional[list[TableauProject]]:
-        return self.attributes.child_projects
+        return None if self.attributes is None else self.attributes.child_projects
 
     @child_projects.setter
     def child_projects(self, child_projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.child_projects = child_projects
 
@@ -17672,59 +19346,65 @@
         "top_level_project_qualified_name",
         "project_hierarchy",
         "project",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def project(self) -> Optional[TableauProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
@@ -17770,15 +19450,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "projects",
     ]
 
     @property
     def projects(self) -> Optional[list[TableauProject]]:
-        return self.attributes.projects
+        return None if self.attributes is None else self.attributes.projects
 
     @projects.setter
     def projects(self, projects: Optional[list[TableauProject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.projects = projects
 
@@ -17827,171 +19507,181 @@
         "workbook",
         "project",
         "fields",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.workbook_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.workbook_qualified_name
+        )
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def is_published(self) -> Optional[bool]:
-        return self.attributes.is_published
+        return None if self.attributes is None else self.attributes.is_published
 
     @is_published.setter
     def is_published(self, is_published: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_published = is_published
 
     @property
     def has_extracts(self) -> Optional[bool]:
-        return self.attributes.has_extracts
+        return None if self.attributes is None else self.attributes.has_extracts
 
     @has_extracts.setter
     def has_extracts(self, has_extracts: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.has_extracts = has_extracts
 
     @property
     def is_certified(self) -> Optional[bool]:
-        return self.attributes.is_certified
+        return None if self.attributes is None else self.attributes.is_certified
 
     @is_certified.setter
     def is_certified(self, is_certified: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_certified = is_certified
 
     @property
     def certifier(self) -> Optional[dict[str, str]]:
-        return self.attributes.certifier
+        return None if self.attributes is None else self.attributes.certifier
 
     @certifier.setter
     def certifier(self, certifier: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certifier = certifier
 
     @property
     def certification_note(self) -> Optional[str]:
-        return self.attributes.certification_note
+        return None if self.attributes is None else self.attributes.certification_note
 
     @certification_note.setter
     def certification_note(self, certification_note: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certification_note = certification_note
 
     @property
     def certifier_display_name(self) -> Optional[str]:
-        return self.attributes.certifier_display_name
+        return (
+            None if self.attributes is None else self.attributes.certifier_display_name
+        )
 
     @certifier_display_name.setter
     def certifier_display_name(self, certifier_display_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.certifier_display_name = certifier_display_name
 
     @property
     def upstream_tables(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_tables
+        return None if self.attributes is None else self.attributes.upstream_tables
 
     @upstream_tables.setter
     def upstream_tables(self, upstream_tables: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_tables = upstream_tables
 
     @property
     def upstream_datasources(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.upstream_datasources
+        return None if self.attributes is None else self.attributes.upstream_datasources
 
     @upstream_datasources.setter
     def upstream_datasources(
         self, upstream_datasources: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.upstream_datasources = upstream_datasources
 
     @property
     def workbook(self) -> Optional[TableauWorkbook]:
-        return self.attributes.workbook
+        return None if self.attributes is None else self.attributes.workbook
 
     @workbook.setter
     def workbook(self, workbook: Optional[TableauWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook = workbook
 
     @property
     def project(self) -> Optional[TableauProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def fields(self) -> Optional[list[TableauDatasourceField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[TableauDatasourceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
@@ -18070,79 +19760,87 @@
         "project_hierarchy",
         "workbook",
         "worksheets",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.workbook_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.workbook_qualified_name
+        )
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def workbook(self) -> Optional[TableauWorkbook]:
-        return self.attributes.workbook
+        return None if self.attributes is None else self.attributes.workbook
 
     @workbook.setter
     def workbook(self, workbook: Optional[TableauWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook = workbook
 
     @property
     def worksheets(self) -> Optional[list[TableauWorksheet]]:
-        return self.attributes.worksheets
+        return None if self.attributes is None else self.attributes.worksheets
 
     @worksheets.setter
     def worksheets(self, worksheets: Optional[list[TableauWorksheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.worksheets = worksheets
 
@@ -18201,89 +19899,95 @@
         "output_fields",
         "output_steps",
         "project",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def input_fields(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.input_fields
+        return None if self.attributes is None else self.attributes.input_fields
 
     @input_fields.setter
     def input_fields(self, input_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.input_fields = input_fields
 
     @property
     def output_fields(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.output_fields
+        return None if self.attributes is None else self.attributes.output_fields
 
     @output_fields.setter
     def output_fields(self, output_fields: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_fields = output_fields
 
     @property
     def output_steps(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.output_steps
+        return None if self.attributes is None else self.attributes.output_steps
 
     @output_steps.setter
     def output_steps(self, output_steps: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_steps = output_steps
 
     @property
     def project(self) -> Optional[TableauProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[TableauProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
@@ -18346,103 +20050,111 @@
         "datasource_fields",
         "calculated_fields",
         "dashboards",
     ]
 
     @property
     def site_qualified_name(self) -> Optional[str]:
-        return self.attributes.site_qualified_name
+        return None if self.attributes is None else self.attributes.site_qualified_name
 
     @site_qualified_name.setter
     def site_qualified_name(self, site_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.site_qualified_name = site_qualified_name
 
     @property
     def project_qualified_name(self) -> Optional[str]:
-        return self.attributes.project_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.project_qualified_name
+        )
 
     @project_qualified_name.setter
     def project_qualified_name(self, project_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_qualified_name = project_qualified_name
 
     @property
     def top_level_project_qualified_name(self) -> Optional[str]:
-        return self.attributes.top_level_project_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.top_level_project_qualified_name
+        )
 
     @top_level_project_qualified_name.setter
     def top_level_project_qualified_name(
         self, top_level_project_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.top_level_project_qualified_name = (
             top_level_project_qualified_name
         )
 
     @property
     def project_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.project_hierarchy
+        return None if self.attributes is None else self.attributes.project_hierarchy
 
     @project_hierarchy.setter
     def project_hierarchy(self, project_hierarchy: Optional[list[dict[str, str]]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_hierarchy = project_hierarchy
 
     @property
     def workbook_qualified_name(self) -> Optional[str]:
-        return self.attributes.workbook_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.workbook_qualified_name
+        )
 
     @workbook_qualified_name.setter
     def workbook_qualified_name(self, workbook_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook_qualified_name = workbook_qualified_name
 
     @property
     def workbook(self) -> Optional[TableauWorkbook]:
-        return self.attributes.workbook
+        return None if self.attributes is None else self.attributes.workbook
 
     @workbook.setter
     def workbook(self, workbook: Optional[TableauWorkbook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workbook = workbook
 
     @property
     def datasource_fields(self) -> Optional[list[TableauDatasourceField]]:
-        return self.attributes.datasource_fields
+        return None if self.attributes is None else self.attributes.datasource_fields
 
     @datasource_fields.setter
     def datasource_fields(
         self, datasource_fields: Optional[list[TableauDatasourceField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasource_fields = datasource_fields
 
     @property
     def calculated_fields(self) -> Optional[list[TableauCalculatedField]]:
-        return self.attributes.calculated_fields
+        return None if self.attributes is None else self.attributes.calculated_fields
 
     @calculated_fields.setter
     def calculated_fields(
         self, calculated_fields: Optional[list[TableauCalculatedField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.calculated_fields = calculated_fields
 
     @property
     def dashboards(self) -> Optional[list[TableauDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[TableauDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
@@ -18513,145 +20225,155 @@
         "tile",
         "model",
         "dashboard",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
-        return self.attributes.folder_name
+        return None if self.attributes is None else self.attributes.folder_name
 
     @folder_name.setter
     def folder_name(self, folder_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.folder_name = folder_name
 
     @property
     def source_user_id(self) -> Optional[int]:
-        return self.attributes.source_user_id
+        return None if self.attributes is None else self.attributes.source_user_id
 
     @source_user_id.setter
     def source_user_id(self, source_user_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_user_id = source_user_id
 
     @property
     def source_view_count(self) -> Optional[int]:
-        return self.attributes.source_view_count
+        return None if self.attributes is None else self.attributes.source_view_count
 
     @source_view_count.setter
     def source_view_count(self, source_view_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_view_count = source_view_count
 
     @property
     def sourcelast_updater_id(self) -> Optional[int]:
-        return self.attributes.sourcelast_updater_id
+        return (
+            None if self.attributes is None else self.attributes.sourcelast_updater_id
+        )
 
     @sourcelast_updater_id.setter
     def sourcelast_updater_id(self, sourcelast_updater_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sourcelast_updater_id = sourcelast_updater_id
 
     @property
     def source_last_accessed_at(self) -> Optional[datetime]:
-        return self.attributes.source_last_accessed_at
+        return (
+            None if self.attributes is None else self.attributes.source_last_accessed_at
+        )
 
     @source_last_accessed_at.setter
     def source_last_accessed_at(self, source_last_accessed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_accessed_at = source_last_accessed_at
 
     @property
     def source_last_viewed_at(self) -> Optional[datetime]:
-        return self.attributes.source_last_viewed_at
+        return (
+            None if self.attributes is None else self.attributes.source_last_viewed_at
+        )
 
     @source_last_viewed_at.setter
     def source_last_viewed_at(self, source_last_viewed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_viewed_at = source_last_viewed_at
 
     @property
     def source_content_metadata_id(self) -> Optional[int]:
-        return self.attributes.source_content_metadata_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_content_metadata_id
+        )
 
     @source_content_metadata_id.setter
     def source_content_metadata_id(self, source_content_metadata_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_content_metadata_id = source_content_metadata_id
 
     @property
     def source_query_id(self) -> Optional[int]:
-        return self.attributes.source_query_id
+        return None if self.attributes is None else self.attributes.source_query_id
 
     @source_query_id.setter
     def source_query_id(self, source_query_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_query_id = source_query_id
 
     @property
     def model_name(self) -> Optional[str]:
-        return self.attributes.model_name
+        return None if self.attributes is None else self.attributes.model_name
 
     @model_name.setter
     def model_name(self, model_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model_name = model_name
 
     @property
     def query(self) -> Optional[LookerQuery]:
-        return self.attributes.query
+        return None if self.attributes is None else self.attributes.query
 
     @query.setter
     def query(self, query: Optional[LookerQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query = query
 
     @property
     def folder(self) -> Optional[LookerFolder]:
-        return self.attributes.folder
+        return None if self.attributes is None else self.attributes.folder
 
     @folder.setter
     def folder(self, folder: Optional[LookerFolder]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.folder = folder
 
     @property
     def tile(self) -> Optional[LookerTile]:
-        return self.attributes.tile
+        return None if self.attributes is None else self.attributes.tile
 
     @tile.setter
     def tile(self, tile: Optional[LookerTile]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tile = tile
 
     @property
     def model(self) -> Optional[LookerModel]:
-        return self.attributes.model
+        return None if self.attributes is None else self.attributes.model
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
     @property
     def dashboard(self) -> Optional[LookerDashboard]:
-        return self.attributes.dashboard
+        return None if self.attributes is None else self.attributes.dashboard
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[LookerDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
@@ -18729,105 +20451,111 @@
         "tiles",
         "looks",
         "folder",
     ]
 
     @property
     def folder_name(self) -> Optional[str]:
-        return self.attributes.folder_name
+        return None if self.attributes is None else self.attributes.folder_name
 
     @folder_name.setter
     def folder_name(self, folder_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.folder_name = folder_name
 
     @property
     def source_user_id(self) -> Optional[int]:
-        return self.attributes.source_user_id
+        return None if self.attributes is None else self.attributes.source_user_id
 
     @source_user_id.setter
     def source_user_id(self, source_user_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_user_id = source_user_id
 
     @property
     def source_view_count(self) -> Optional[int]:
-        return self.attributes.source_view_count
+        return None if self.attributes is None else self.attributes.source_view_count
 
     @source_view_count.setter
     def source_view_count(self, source_view_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_view_count = source_view_count
 
     @property
     def source_metadata_id(self) -> Optional[int]:
-        return self.attributes.source_metadata_id
+        return None if self.attributes is None else self.attributes.source_metadata_id
 
     @source_metadata_id.setter
     def source_metadata_id(self, source_metadata_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_metadata_id = source_metadata_id
 
     @property
     def sourcelast_updater_id(self) -> Optional[int]:
-        return self.attributes.sourcelast_updater_id
+        return (
+            None if self.attributes is None else self.attributes.sourcelast_updater_id
+        )
 
     @sourcelast_updater_id.setter
     def sourcelast_updater_id(self, sourcelast_updater_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sourcelast_updater_id = sourcelast_updater_id
 
     @property
     def source_last_accessed_at(self) -> Optional[datetime]:
-        return self.attributes.source_last_accessed_at
+        return (
+            None if self.attributes is None else self.attributes.source_last_accessed_at
+        )
 
     @source_last_accessed_at.setter
     def source_last_accessed_at(self, source_last_accessed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_accessed_at = source_last_accessed_at
 
     @property
     def source_last_viewed_at(self) -> Optional[datetime]:
-        return self.attributes.source_last_viewed_at
+        return (
+            None if self.attributes is None else self.attributes.source_last_viewed_at
+        )
 
     @source_last_viewed_at.setter
     def source_last_viewed_at(self, source_last_viewed_at: Optional[datetime]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_last_viewed_at = source_last_viewed_at
 
     @property
     def tiles(self) -> Optional[list[LookerTile]]:
-        return self.attributes.tiles
+        return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[list[LookerTile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tiles = tiles
 
     @property
     def looks(self) -> Optional[list[LookerLook]]:
-        return self.attributes.looks
+        return None if self.attributes is None else self.attributes.looks
 
     @looks.setter
     def looks(self, looks: Optional[list[LookerLook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looks = looks
 
     @property
     def folder(self) -> Optional[LookerFolder]:
-        return self.attributes.folder
+        return None if self.attributes is None else self.attributes.folder
 
     @folder.setter
     def folder(self, folder: Optional[LookerFolder]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.folder = folder
 
@@ -18891,65 +20619,69 @@
         "source_parent_i_d",
         "looks",
         "dashboards",
     ]
 
     @property
     def source_content_metadata_id(self) -> Optional[int]:
-        return self.attributes.source_content_metadata_id
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_content_metadata_id
+        )
 
     @source_content_metadata_id.setter
     def source_content_metadata_id(self, source_content_metadata_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_content_metadata_id = source_content_metadata_id
 
     @property
     def source_creator_id(self) -> Optional[int]:
-        return self.attributes.source_creator_id
+        return None if self.attributes is None else self.attributes.source_creator_id
 
     @source_creator_id.setter
     def source_creator_id(self, source_creator_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_creator_id = source_creator_id
 
     @property
     def source_child_count(self) -> Optional[int]:
-        return self.attributes.source_child_count
+        return None if self.attributes is None else self.attributes.source_child_count
 
     @source_child_count.setter
     def source_child_count(self, source_child_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_child_count = source_child_count
 
     @property
     def source_parent_i_d(self) -> Optional[int]:
-        return self.attributes.source_parent_i_d
+        return None if self.attributes is None else self.attributes.source_parent_i_d
 
     @source_parent_i_d.setter
     def source_parent_i_d(self, source_parent_i_d: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_parent_i_d = source_parent_i_d
 
     @property
     def looks(self) -> Optional[list[LookerLook]]:
-        return self.attributes.looks
+        return None if self.attributes is None else self.attributes.looks
 
     @looks.setter
     def looks(self, looks: Optional[list[LookerLook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looks = looks
 
     @property
     def dashboards(self) -> Optional[list[LookerDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[LookerDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
@@ -19007,105 +20739,105 @@
         "query",
         "look",
         "dashboard",
     ]
 
     @property
     def lookml_link_id(self) -> Optional[str]:
-        return self.attributes.lookml_link_id
+        return None if self.attributes is None else self.attributes.lookml_link_id
 
     @lookml_link_id.setter
     def lookml_link_id(self, lookml_link_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.lookml_link_id = lookml_link_id
 
     @property
     def merge_result_id(self) -> Optional[str]:
-        return self.attributes.merge_result_id
+        return None if self.attributes is None else self.attributes.merge_result_id
 
     @merge_result_id.setter
     def merge_result_id(self, merge_result_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.merge_result_id = merge_result_id
 
     @property
     def note_text(self) -> Optional[str]:
-        return self.attributes.note_text
+        return None if self.attributes is None else self.attributes.note_text
 
     @note_text.setter
     def note_text(self, note_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.note_text = note_text
 
     @property
     def query_i_d(self) -> Optional[int]:
-        return self.attributes.query_i_d
+        return None if self.attributes is None else self.attributes.query_i_d
 
     @query_i_d.setter
     def query_i_d(self, query_i_d: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query_i_d = query_i_d
 
     @property
     def result_maker_i_d(self) -> Optional[int]:
-        return self.attributes.result_maker_i_d
+        return None if self.attributes is None else self.attributes.result_maker_i_d
 
     @result_maker_i_d.setter
     def result_maker_i_d(self, result_maker_i_d: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.result_maker_i_d = result_maker_i_d
 
     @property
     def subtitle_text(self) -> Optional[str]:
-        return self.attributes.subtitle_text
+        return None if self.attributes is None else self.attributes.subtitle_text
 
     @subtitle_text.setter
     def subtitle_text(self, subtitle_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.subtitle_text = subtitle_text
 
     @property
     def look_id(self) -> Optional[int]:
-        return self.attributes.look_id
+        return None if self.attributes is None else self.attributes.look_id
 
     @look_id.setter
     def look_id(self, look_id: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.look_id = look_id
 
     @property
     def query(self) -> Optional[LookerQuery]:
-        return self.attributes.query
+        return None if self.attributes is None else self.attributes.query
 
     @query.setter
     def query(self, query: Optional[LookerQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.query = query
 
     @property
     def look(self) -> Optional[LookerLook]:
-        return self.attributes.look
+        return None if self.attributes is None else self.attributes.look
 
     @look.setter
     def look(self, look: Optional[LookerLook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.look = look
 
     @property
     def dashboard(self) -> Optional[LookerDashboard]:
-        return self.attributes.dashboard
+        return None if self.attributes is None else self.attributes.dashboard
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[LookerDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
@@ -19163,65 +20895,65 @@
         "look",
         "queries",
         "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
-        return self.attributes.project_name
+        return None if self.attributes is None else self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
     def explores(self) -> Optional[list[LookerExplore]]:
-        return self.attributes.explores
+        return None if self.attributes is None else self.attributes.explores
 
     @explores.setter
     def explores(self, explores: Optional[list[LookerExplore]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.explores = explores
 
     @property
     def project(self) -> Optional[LookerProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def look(self) -> Optional[LookerLook]:
-        return self.attributes.look
+        return None if self.attributes is None else self.attributes.look
 
     @look.setter
     def look(self, look: Optional[LookerLook]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.look = look
 
     @property
     def queries(self) -> Optional[list[LookerQuery]]:
-        return self.attributes.queries
+        return None if self.attributes is None else self.attributes.queries
 
     @queries.setter
     def queries(self, queries: Optional[list[LookerQuery]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.queries = queries
 
     @property
     def fields(self) -> Optional[list[LookerField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
@@ -19275,85 +21007,87 @@
         "project",
         "model",
         "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
-        return self.attributes.project_name
+        return None if self.attributes is None else self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
     def model_name(self) -> Optional[str]:
-        return self.attributes.model_name
+        return None if self.attributes is None else self.attributes.model_name
 
     @model_name.setter
     def model_name(self, model_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model_name = model_name
 
     @property
     def source_connection_name(self) -> Optional[str]:
-        return self.attributes.source_connection_name
+        return (
+            None if self.attributes is None else self.attributes.source_connection_name
+        )
 
     @source_connection_name.setter
     def source_connection_name(self, source_connection_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_connection_name = source_connection_name
 
     @property
     def view_name(self) -> Optional[str]:
-        return self.attributes.view_name
+        return None if self.attributes is None else self.attributes.view_name
 
     @view_name.setter
     def view_name(self, view_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view_name = view_name
 
     @property
     def sql_table_name(self) -> Optional[str]:
-        return self.attributes.sql_table_name
+        return None if self.attributes is None else self.attributes.sql_table_name
 
     @sql_table_name.setter
     def sql_table_name(self, sql_table_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.sql_table_name = sql_table_name
 
     @property
     def project(self) -> Optional[LookerProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def model(self) -> Optional[LookerModel]:
-        return self.attributes.model
+        return None if self.attributes is None else self.attributes.model
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
     @property
     def fields(self) -> Optional[list[LookerField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
@@ -19405,45 +21139,45 @@
         "explores",
         "fields",
         "views",
     ]
 
     @property
     def models(self) -> Optional[list[LookerModel]]:
-        return self.attributes.models
+        return None if self.attributes is None else self.attributes.models
 
     @models.setter
     def models(self, models: Optional[list[LookerModel]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.models = models
 
     @property
     def explores(self) -> Optional[list[LookerExplore]]:
-        return self.attributes.explores
+        return None if self.attributes is None else self.attributes.explores
 
     @explores.setter
     def explores(self, explores: Optional[list[LookerExplore]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.explores = explores
 
     @property
     def fields(self) -> Optional[list[LookerField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
     @property
     def views(self) -> Optional[list[LookerView]]:
-        return self.attributes.views
+        return None if self.attributes is None else self.attributes.views
 
     @views.setter
     def views(self, views: Optional[list[LookerView]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views = views
 
@@ -19492,75 +21226,83 @@
         "tiles",
         "looks",
         "model",
     ]
 
     @property
     def source_definition(self) -> Optional[str]:
-        return self.attributes.source_definition
+        return None if self.attributes is None else self.attributes.source_definition
 
     @source_definition.setter
     def source_definition(self, source_definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_definition = source_definition
 
     @property
     def source_definition_database(self) -> Optional[str]:
-        return self.attributes.source_definition_database
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_definition_database
+        )
 
     @source_definition_database.setter
     def source_definition_database(self, source_definition_database: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_definition_database = source_definition_database
 
     @property
     def source_definition_schema(self) -> Optional[str]:
-        return self.attributes.source_definition_schema
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.source_definition_schema
+        )
 
     @source_definition_schema.setter
     def source_definition_schema(self, source_definition_schema: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_definition_schema = source_definition_schema
 
     @property
     def fields(self) -> Optional[set[str]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
     @property
     def tiles(self) -> Optional[list[LookerTile]]:
-        return self.attributes.tiles
+        return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[list[LookerTile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tiles = tiles
 
     @property
     def looks(self) -> Optional[list[LookerLook]]:
-        return self.attributes.looks
+        return None if self.attributes is None else self.attributes.looks
 
     @looks.setter
     def looks(self, looks: Optional[list[LookerLook]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looks = looks
 
     @property
     def model(self) -> Optional[LookerModel]:
-        return self.attributes.model
+        return None if self.attributes is None else self.attributes.model
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
@@ -19620,117 +21362,127 @@
         "project",
         "view",
         "model",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
-        return self.attributes.project_name
+        return None if self.attributes is None else self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
     def looker_explore_qualified_name(self) -> Optional[str]:
-        return self.attributes.looker_explore_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.looker_explore_qualified_name
+        )
 
     @looker_explore_qualified_name.setter
     def looker_explore_qualified_name(
         self, looker_explore_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_explore_qualified_name = looker_explore_qualified_name
 
     @property
     def looker_view_qualified_name(self) -> Optional[str]:
-        return self.attributes.looker_view_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.looker_view_qualified_name
+        )
 
     @looker_view_qualified_name.setter
     def looker_view_qualified_name(self, looker_view_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_view_qualified_name = looker_view_qualified_name
 
     @property
     def model_name(self) -> Optional[str]:
-        return self.attributes.model_name
+        return None if self.attributes is None else self.attributes.model_name
 
     @model_name.setter
     def model_name(self, model_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model_name = model_name
 
     @property
     def source_definition(self) -> Optional[str]:
-        return self.attributes.source_definition
+        return None if self.attributes is None else self.attributes.source_definition
 
     @source_definition.setter
     def source_definition(self, source_definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_definition = source_definition
 
     @property
     def looker_field_data_type(self) -> Optional[str]:
-        return self.attributes.looker_field_data_type
+        return (
+            None if self.attributes is None else self.attributes.looker_field_data_type
+        )
 
     @looker_field_data_type.setter
     def looker_field_data_type(self, looker_field_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_field_data_type = looker_field_data_type
 
     @property
     def looker_times_used(self) -> Optional[int]:
-        return self.attributes.looker_times_used
+        return None if self.attributes is None else self.attributes.looker_times_used
 
     @looker_times_used.setter
     def looker_times_used(self, looker_times_used: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.looker_times_used = looker_times_used
 
     @property
     def explore(self) -> Optional[LookerExplore]:
-        return self.attributes.explore
+        return None if self.attributes is None else self.attributes.explore
 
     @explore.setter
     def explore(self, explore: Optional[LookerExplore]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.explore = explore
 
     @property
     def project(self) -> Optional[LookerProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def view(self) -> Optional[LookerView]:
-        return self.attributes.view
+        return None if self.attributes is None else self.attributes.view
 
     @view.setter
     def view(self, view: Optional[LookerView]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.view = view
 
     @property
     def model(self) -> Optional[LookerModel]:
-        return self.attributes.model
+        return None if self.attributes is None else self.attributes.model
 
     @model.setter
     def model(self, model: Optional[LookerModel]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.model = model
 
@@ -19792,35 +21544,35 @@
         "project_name",
         "project",
         "fields",
     ]
 
     @property
     def project_name(self) -> Optional[str]:
-        return self.attributes.project_name
+        return None if self.attributes is None else self.attributes.project_name
 
     @project_name.setter
     def project_name(self, project_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project_name = project_name
 
     @property
     def project(self) -> Optional[LookerProject]:
-        return self.attributes.project
+        return None if self.attributes is None else self.attributes.project
 
     @project.setter
     def project(self, project: Optional[LookerProject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.project = project
 
     @property
     def fields(self) -> Optional[list[LookerField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[LookerField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
@@ -19858,15 +21610,19 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "redash_dashboard_widget_count",
     ]
 
     @property
     def redash_dashboard_widget_count(self) -> Optional[int]:
-        return self.attributes.redash_dashboard_widget_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_dashboard_widget_count
+        )
 
     @redash_dashboard_widget_count.setter
     def redash_dashboard_widget_count(
         self, redash_dashboard_widget_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -19908,85 +21664,103 @@
         "redash_query_last_executed_at",
         "redash_query_schedule_humanized",
         "redash_visualizations",
     ]
 
     @property
     def redash_query_s_q_l(self) -> Optional[str]:
-        return self.attributes.redash_query_s_q_l
+        return None if self.attributes is None else self.attributes.redash_query_s_q_l
 
     @redash_query_s_q_l.setter
     def redash_query_s_q_l(self, redash_query_s_q_l: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_s_q_l = redash_query_s_q_l
 
     @property
     def redash_query_parameters(self) -> Optional[str]:
-        return self.attributes.redash_query_parameters
+        return (
+            None if self.attributes is None else self.attributes.redash_query_parameters
+        )
 
     @redash_query_parameters.setter
     def redash_query_parameters(self, redash_query_parameters: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_parameters = redash_query_parameters
 
     @property
     def redash_query_schedule(self) -> Optional[dict[str, str]]:
-        return self.attributes.redash_query_schedule
+        return (
+            None if self.attributes is None else self.attributes.redash_query_schedule
+        )
 
     @redash_query_schedule.setter
     def redash_query_schedule(self, redash_query_schedule: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_schedule = redash_query_schedule
 
     @property
     def redash_query_last_execution_runtime(self) -> Optional[float]:
-        return self.attributes.redash_query_last_execution_runtime
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_query_last_execution_runtime
+        )
 
     @redash_query_last_execution_runtime.setter
     def redash_query_last_execution_runtime(
         self, redash_query_last_execution_runtime: Optional[float]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_last_execution_runtime = (
             redash_query_last_execution_runtime
         )
 
     @property
     def redash_query_last_executed_at(self) -> Optional[datetime]:
-        return self.attributes.redash_query_last_executed_at
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_query_last_executed_at
+        )
 
     @redash_query_last_executed_at.setter
     def redash_query_last_executed_at(
         self, redash_query_last_executed_at: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_last_executed_at = redash_query_last_executed_at
 
     @property
     def redash_query_schedule_humanized(self) -> Optional[str]:
-        return self.attributes.redash_query_schedule_humanized
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_query_schedule_humanized
+        )
 
     @redash_query_schedule_humanized.setter
     def redash_query_schedule_humanized(
         self, redash_query_schedule_humanized: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_schedule_humanized = (
             redash_query_schedule_humanized
         )
 
     @property
     def redash_visualizations(self) -> Optional[list[RedashVisualization]]:
-        return self.attributes.redash_visualizations
+        return (
+            None if self.attributes is None else self.attributes.redash_visualizations
+        )
 
     @redash_visualizations.setter
     def redash_visualizations(
         self, redash_visualizations: Optional[list[RedashVisualization]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -20043,45 +21817,53 @@
         "redash_query_name",
         "redash_query_qualified_name",
         "redash_query",
     ]
 
     @property
     def redash_visualization_type(self) -> Optional[str]:
-        return self.attributes.redash_visualization_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_visualization_type
+        )
 
     @redash_visualization_type.setter
     def redash_visualization_type(self, redash_visualization_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_visualization_type = redash_visualization_type
 
     @property
     def redash_query_name(self) -> Optional[str]:
-        return self.attributes.redash_query_name
+        return None if self.attributes is None else self.attributes.redash_query_name
 
     @redash_query_name.setter
     def redash_query_name(self, redash_query_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_name = redash_query_name
 
     @property
     def redash_query_qualified_name(self) -> Optional[str]:
-        return self.attributes.redash_query_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.redash_query_qualified_name
+        )
 
     @redash_query_qualified_name.setter
     def redash_query_qualified_name(self, redash_query_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query_qualified_name = redash_query_qualified_name
 
     @property
     def redash_query(self) -> Optional[RedashQuery]:
-        return self.attributes.redash_query
+        return None if self.attributes is None else self.attributes.redash_query
 
     @redash_query.setter
     def redash_query(self, redash_query: Optional[RedashQuery]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_query = redash_query
 
@@ -20128,57 +21910,61 @@
         "metabase_query",
         "metabase_dashboards",
         "metabase_collection",
     ]
 
     @property
     def metabase_dashboard_count(self) -> Optional[int]:
-        return self.attributes.metabase_dashboard_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metabase_dashboard_count
+        )
 
     @metabase_dashboard_count.setter
     def metabase_dashboard_count(self, metabase_dashboard_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_dashboard_count = metabase_dashboard_count
 
     @property
     def metabase_query_type(self) -> Optional[str]:
-        return self.attributes.metabase_query_type
+        return None if self.attributes is None else self.attributes.metabase_query_type
 
     @metabase_query_type.setter
     def metabase_query_type(self, metabase_query_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_query_type = metabase_query_type
 
     @property
     def metabase_query(self) -> Optional[str]:
-        return self.attributes.metabase_query
+        return None if self.attributes is None else self.attributes.metabase_query
 
     @metabase_query.setter
     def metabase_query(self, metabase_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_query = metabase_query
 
     @property
     def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
-        return self.attributes.metabase_dashboards
+        return None if self.attributes is None else self.attributes.metabase_dashboards
 
     @metabase_dashboards.setter
     def metabase_dashboards(
         self, metabase_dashboards: Optional[list[MetabaseDashboard]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_dashboards = metabase_dashboards
 
     @property
     def metabase_collection(self) -> Optional[MetabaseCollection]:
-        return self.attributes.metabase_collection
+        return None if self.attributes is None else self.attributes.metabase_collection
 
     @metabase_collection.setter
     def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection = metabase_collection
 
@@ -20229,71 +22015,75 @@
         "metabase_is_personal_collection",
         "metabase_dashboards",
         "metabase_questions",
     ]
 
     @property
     def metabase_slug(self) -> Optional[str]:
-        return self.attributes.metabase_slug
+        return None if self.attributes is None else self.attributes.metabase_slug
 
     @metabase_slug.setter
     def metabase_slug(self, metabase_slug: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_slug = metabase_slug
 
     @property
     def metabase_color(self) -> Optional[str]:
-        return self.attributes.metabase_color
+        return None if self.attributes is None else self.attributes.metabase_color
 
     @metabase_color.setter
     def metabase_color(self, metabase_color: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_color = metabase_color
 
     @property
     def metabase_namespace(self) -> Optional[str]:
-        return self.attributes.metabase_namespace
+        return None if self.attributes is None else self.attributes.metabase_namespace
 
     @metabase_namespace.setter
     def metabase_namespace(self, metabase_namespace: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_namespace = metabase_namespace
 
     @property
     def metabase_is_personal_collection(self) -> Optional[bool]:
-        return self.attributes.metabase_is_personal_collection
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.metabase_is_personal_collection
+        )
 
     @metabase_is_personal_collection.setter
     def metabase_is_personal_collection(
         self, metabase_is_personal_collection: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_is_personal_collection = (
             metabase_is_personal_collection
         )
 
     @property
     def metabase_dashboards(self) -> Optional[list[MetabaseDashboard]]:
-        return self.attributes.metabase_dashboards
+        return None if self.attributes is None else self.attributes.metabase_dashboards
 
     @metabase_dashboards.setter
     def metabase_dashboards(
         self, metabase_dashboards: Optional[list[MetabaseDashboard]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_dashboards = metabase_dashboards
 
     @property
     def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
-        return self.attributes.metabase_questions
+        return None if self.attributes is None else self.attributes.metabase_questions
 
     @metabase_questions.setter
     def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_questions = metabase_questions
 
@@ -20342,35 +22132,37 @@
         "metabase_question_count",
         "metabase_questions",
         "metabase_collection",
     ]
 
     @property
     def metabase_question_count(self) -> Optional[int]:
-        return self.attributes.metabase_question_count
+        return (
+            None if self.attributes is None else self.attributes.metabase_question_count
+        )
 
     @metabase_question_count.setter
     def metabase_question_count(self, metabase_question_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_question_count = metabase_question_count
 
     @property
     def metabase_questions(self) -> Optional[list[MetabaseQuestion]]:
-        return self.attributes.metabase_questions
+        return None if self.attributes is None else self.attributes.metabase_questions
 
     @metabase_questions.setter
     def metabase_questions(self, metabase_questions: Optional[list[MetabaseQuestion]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_questions = metabase_questions
 
     @property
     def metabase_collection(self) -> Optional[MetabaseCollection]:
-        return self.attributes.metabase_collection
+        return None if self.attributes is None else self.attributes.metabase_collection
 
     @metabase_collection.setter
     def metabase_collection(self, metabase_collection: Optional[MetabaseCollection]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.metabase_collection = metabase_collection
 
@@ -20414,63 +22206,71 @@
         "quick_sight_dashboards",
         "quick_sight_analyses",
         "quick_sight_datasets",
     ]
 
     @property
     def quick_sight_folder_type(self) -> Optional[QuickSightFolderType]:
-        return self.attributes.quick_sight_folder_type
+        return (
+            None if self.attributes is None else self.attributes.quick_sight_folder_type
+        )
 
     @quick_sight_folder_type.setter
     def quick_sight_folder_type(
         self, quick_sight_folder_type: Optional[QuickSightFolderType]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_folder_type = quick_sight_folder_type
 
     @property
     def quick_sight_folder_hierarchy(self) -> Optional[list[dict[str, str]]]:
-        return self.attributes.quick_sight_folder_hierarchy
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_folder_hierarchy
+        )
 
     @quick_sight_folder_hierarchy.setter
     def quick_sight_folder_hierarchy(
         self, quick_sight_folder_hierarchy: Optional[list[dict[str, str]]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_folder_hierarchy = quick_sight_folder_hierarchy
 
     @property
     def quick_sight_dashboards(self) -> Optional[list[QuickSightDashboard]]:
-        return self.attributes.quick_sight_dashboards
+        return (
+            None if self.attributes is None else self.attributes.quick_sight_dashboards
+        )
 
     @quick_sight_dashboards.setter
     def quick_sight_dashboards(
         self, quick_sight_dashboards: Optional[list[QuickSightDashboard]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboards = quick_sight_dashboards
 
     @property
     def quick_sight_analyses(self) -> Optional[list[QuickSightAnalysis]]:
-        return self.attributes.quick_sight_analyses
+        return None if self.attributes is None else self.attributes.quick_sight_analyses
 
     @quick_sight_analyses.setter
     def quick_sight_analyses(
         self, quick_sight_analyses: Optional[list[QuickSightAnalysis]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analyses = quick_sight_analyses
 
     @property
     def quick_sight_datasets(self) -> Optional[list[QuickSightDataset]]:
-        return self.attributes.quick_sight_datasets
+        return None if self.attributes is None else self.attributes.quick_sight_datasets
 
     @quick_sight_datasets.setter
     def quick_sight_datasets(
         self, quick_sight_datasets: Optional[list[QuickSightDataset]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -20519,29 +22319,35 @@
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_dashboard_qualified_name",
         "quick_sight_dashboard",
     ]
 
     @property
     def quick_sight_dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_dashboard_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dashboard_qualified_name
+        )
 
     @quick_sight_dashboard_qualified_name.setter
     def quick_sight_dashboard_qualified_name(
         self, quick_sight_dashboard_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_qualified_name = (
             quick_sight_dashboard_qualified_name
         )
 
     @property
     def quick_sight_dashboard(self) -> Optional[QuickSightDashboard]:
-        return self.attributes.quick_sight_dashboard
+        return (
+            None if self.attributes is None else self.attributes.quick_sight_dashboard
+        )
 
     @quick_sight_dashboard.setter
     def quick_sight_dashboard(
         self, quick_sight_dashboard: Optional[QuickSightDashboard]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -20581,29 +22387,33 @@
     _convience_properties: ClassVar[list[str]] = [
         "quick_sight_analysis_qualified_name",
         "quick_sight_analysis",
     ]
 
     @property
     def quick_sight_analysis_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_analysis_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_qualified_name
+        )
 
     @quick_sight_analysis_qualified_name.setter
     def quick_sight_analysis_qualified_name(
         self, quick_sight_analysis_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_qualified_name = (
             quick_sight_analysis_qualified_name
         )
 
     @property
     def quick_sight_analysis(self) -> Optional[QuickSightAnalysis]:
-        return self.attributes.quick_sight_analysis
+        return None if self.attributes is None else self.attributes.quick_sight_analysis
 
     @quick_sight_analysis.setter
     def quick_sight_analysis(self, quick_sight_analysis: Optional[QuickSightAnalysis]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis = quick_sight_analysis
 
@@ -20642,41 +22452,49 @@
         "quick_sight_dataset_field_type",
         "quick_sight_dataset_qualified_name",
         "quick_sight_dataset",
     ]
 
     @property
     def quick_sight_dataset_field_type(self) -> Optional[QuickSightDatasetFieldType]:
-        return self.attributes.quick_sight_dataset_field_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_field_type
+        )
 
     @quick_sight_dataset_field_type.setter
     def quick_sight_dataset_field_type(
         self, quick_sight_dataset_field_type: Optional[QuickSightDatasetFieldType]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_field_type = quick_sight_dataset_field_type
 
     @property
     def quick_sight_dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.quick_sight_dataset_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_qualified_name
+        )
 
     @quick_sight_dataset_qualified_name.setter
     def quick_sight_dataset_qualified_name(
         self, quick_sight_dataset_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_qualified_name = (
             quick_sight_dataset_qualified_name
         )
 
     @property
     def quick_sight_dataset(self) -> Optional[QuickSightDataset]:
-        return self.attributes.quick_sight_dataset
+        return None if self.attributes is None else self.attributes.quick_sight_dataset
 
     @quick_sight_dataset.setter
     def quick_sight_dataset(self, quick_sight_dataset: Optional[QuickSightDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset = quick_sight_dataset
 
@@ -20721,81 +22539,105 @@
         "quick_sight_analysis_filter_groups",
         "quick_sight_analysis_visuals",
         "quick_sight_analysis_folders",
     ]
 
     @property
     def quick_sight_analysis_status(self) -> Optional[QuickSightAnalysisStatus]:
-        return self.attributes.quick_sight_analysis_status
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_status
+        )
 
     @quick_sight_analysis_status.setter
     def quick_sight_analysis_status(
         self, quick_sight_analysis_status: Optional[QuickSightAnalysisStatus]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_status = quick_sight_analysis_status
 
     @property
     def quick_sight_analysis_calculated_fields(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_calculated_fields
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_calculated_fields
+        )
 
     @quick_sight_analysis_calculated_fields.setter
     def quick_sight_analysis_calculated_fields(
         self, quick_sight_analysis_calculated_fields: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_calculated_fields = (
             quick_sight_analysis_calculated_fields
         )
 
     @property
     def quick_sight_analysis_parameter_declarations(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_parameter_declarations
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_parameter_declarations
+        )
 
     @quick_sight_analysis_parameter_declarations.setter
     def quick_sight_analysis_parameter_declarations(
         self, quick_sight_analysis_parameter_declarations: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_parameter_declarations = (
             quick_sight_analysis_parameter_declarations
         )
 
     @property
     def quick_sight_analysis_filter_groups(self) -> Optional[set[str]]:
-        return self.attributes.quick_sight_analysis_filter_groups
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_filter_groups
+        )
 
     @quick_sight_analysis_filter_groups.setter
     def quick_sight_analysis_filter_groups(
         self, quick_sight_analysis_filter_groups: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_filter_groups = (
             quick_sight_analysis_filter_groups
         )
 
     @property
     def quick_sight_analysis_visuals(self) -> Optional[list[QuickSightAnalysisVisual]]:
-        return self.attributes.quick_sight_analysis_visuals
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_visuals
+        )
 
     @quick_sight_analysis_visuals.setter
     def quick_sight_analysis_visuals(
         self, quick_sight_analysis_visuals: Optional[list[QuickSightAnalysisVisual]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_analysis_visuals = quick_sight_analysis_visuals
 
     @property
     def quick_sight_analysis_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_analysis_folders
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_analysis_folders
+        )
 
     @quick_sight_analysis_folders.setter
     def quick_sight_analysis_folders(
         self, quick_sight_analysis_folders: Optional[list[QuickSightFolder]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -20849,57 +22691,73 @@
         "quick_sight_dashboard_last_published_time",
         "quick_sight_dashboard_folders",
         "quick_sight_dashboard_visuals",
     ]
 
     @property
     def quick_sight_dashboard_published_version_number(self) -> Optional[int]:
-        return self.attributes.quick_sight_dashboard_published_version_number
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dashboard_published_version_number
+        )
 
     @quick_sight_dashboard_published_version_number.setter
     def quick_sight_dashboard_published_version_number(
         self, quick_sight_dashboard_published_version_number: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_published_version_number = (
             quick_sight_dashboard_published_version_number
         )
 
     @property
     def quick_sight_dashboard_last_published_time(self) -> Optional[datetime]:
-        return self.attributes.quick_sight_dashboard_last_published_time
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dashboard_last_published_time
+        )
 
     @quick_sight_dashboard_last_published_time.setter
     def quick_sight_dashboard_last_published_time(
         self, quick_sight_dashboard_last_published_time: Optional[datetime]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_last_published_time = (
             quick_sight_dashboard_last_published_time
         )
 
     @property
     def quick_sight_dashboard_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_dashboard_folders
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dashboard_folders
+        )
 
     @quick_sight_dashboard_folders.setter
     def quick_sight_dashboard_folders(
         self, quick_sight_dashboard_folders: Optional[list[QuickSightFolder]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dashboard_folders = quick_sight_dashboard_folders
 
     @property
     def quick_sight_dashboard_visuals(
         self,
     ) -> Optional[list[QuickSightDashboardVisual]]:
-        return self.attributes.quick_sight_dashboard_visuals
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dashboard_visuals
+        )
 
     @quick_sight_dashboard_visuals.setter
     def quick_sight_dashboard_visuals(
         self, quick_sight_dashboard_visuals: Optional[list[QuickSightDashboardVisual]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -20949,55 +22807,71 @@
         "quick_sight_dataset_column_count",
         "quick_sight_dataset_folders",
         "quick_sight_dataset_fields",
     ]
 
     @property
     def quick_sight_dataset_import_mode(self) -> Optional[QuickSightDatasetImportMode]:
-        return self.attributes.quick_sight_dataset_import_mode
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_import_mode
+        )
 
     @quick_sight_dataset_import_mode.setter
     def quick_sight_dataset_import_mode(
         self, quick_sight_dataset_import_mode: Optional[QuickSightDatasetImportMode]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_import_mode = (
             quick_sight_dataset_import_mode
         )
 
     @property
     def quick_sight_dataset_column_count(self) -> Optional[int]:
-        return self.attributes.quick_sight_dataset_column_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_column_count
+        )
 
     @quick_sight_dataset_column_count.setter
     def quick_sight_dataset_column_count(
         self, quick_sight_dataset_column_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_column_count = (
             quick_sight_dataset_column_count
         )
 
     @property
     def quick_sight_dataset_folders(self) -> Optional[list[QuickSightFolder]]:
-        return self.attributes.quick_sight_dataset_folders
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_folders
+        )
 
     @quick_sight_dataset_folders.setter
     def quick_sight_dataset_folders(
         self, quick_sight_dataset_folders: Optional[list[QuickSightFolder]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.quick_sight_dataset_folders = quick_sight_dataset_folders
 
     @property
     def quick_sight_dataset_fields(self) -> Optional[list[QuickSightDatasetField]]:
-        return self.attributes.quick_sight_dataset_fields
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.quick_sight_dataset_fields
+        )
 
     @quick_sight_dataset_fields.setter
     def quick_sight_dataset_fields(
         self, quick_sight_dataset_fields: Optional[list[QuickSightDatasetField]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -21042,15 +22916,15 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "thoughtspot_dashlets",
     ]
 
     @property
     def thoughtspot_dashlets(self) -> Optional[list[ThoughtspotDashlet]]:
-        return self.attributes.thoughtspot_dashlets
+        return None if self.attributes is None else self.attributes.thoughtspot_dashlets
 
     @thoughtspot_dashlets.setter
     def thoughtspot_dashlets(
         self, thoughtspot_dashlets: Optional[list[ThoughtspotDashlet]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -21088,39 +22962,49 @@
         "thoughtspot_liveboard_name",
         "thoughtspot_liveboard_qualified_name",
         "thoughtspot_liveboard",
     ]
 
     @property
     def thoughtspot_liveboard_name(self) -> Optional[str]:
-        return self.attributes.thoughtspot_liveboard_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.thoughtspot_liveboard_name
+        )
 
     @thoughtspot_liveboard_name.setter
     def thoughtspot_liveboard_name(self, thoughtspot_liveboard_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_liveboard_name = thoughtspot_liveboard_name
 
     @property
     def thoughtspot_liveboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.thoughtspot_liveboard_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.thoughtspot_liveboard_qualified_name
+        )
 
     @thoughtspot_liveboard_qualified_name.setter
     def thoughtspot_liveboard_qualified_name(
         self, thoughtspot_liveboard_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.thoughtspot_liveboard_qualified_name = (
             thoughtspot_liveboard_qualified_name
         )
 
     @property
     def thoughtspot_liveboard(self) -> Optional[ThoughtspotLiveboard]:
-        return self.attributes.thoughtspot_liveboard
+        return (
+            None if self.attributes is None else self.attributes.thoughtspot_liveboard
+        )
 
     @thoughtspot_liveboard.setter
     def thoughtspot_liveboard(
         self, thoughtspot_liveboard: Optional[ThoughtspotLiveboard]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -21188,85 +23072,91 @@
         "tiles",
         "pages",
         "dataset",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.dataset_qualified_name
+        )
 
     @dataset_qualified_name.setter
     def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset_qualified_name = dataset_qualified_name
 
     @property
     def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
+        return None if self.attributes is None else self.attributes.web_url
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
     def page_count(self) -> Optional[int]:
-        return self.attributes.page_count
+        return None if self.attributes is None else self.attributes.page_count
 
     @page_count.setter
     def page_count(self, page_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.page_count = page_count
 
     @property
     def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
+        return None if self.attributes is None else self.attributes.workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
     @property
     def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
+        return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[list[PowerBITile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tiles = tiles
 
     @property
     def pages(self) -> Optional[list[PowerBIPage]]:
-        return self.attributes.pages
+        return None if self.attributes is None else self.attributes.pages
 
     @pages.setter
     def pages(self, pages: Optional[list[PowerBIPage]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.pages = pages
 
     @property
     def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
+        return None if self.attributes is None else self.attributes.dataset
 
     @dataset.setter
     def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset = dataset
 
@@ -21321,57 +23211,71 @@
         "power_b_i_measure_expression",
         "power_b_i_is_external_measure",
         "table",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.dataset_qualified_name
+        )
 
     @dataset_qualified_name.setter
     def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset_qualified_name = dataset_qualified_name
 
     @property
     def power_b_i_measure_expression(self) -> Optional[str]:
-        return self.attributes.power_b_i_measure_expression
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_measure_expression
+        )
 
     @power_b_i_measure_expression.setter
     def power_b_i_measure_expression(self, power_b_i_measure_expression: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_measure_expression = power_b_i_measure_expression
 
     @property
     def power_b_i_is_external_measure(self) -> Optional[bool]:
-        return self.attributes.power_b_i_is_external_measure
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_is_external_measure
+        )
 
     @power_b_i_is_external_measure.setter
     def power_b_i_is_external_measure(
         self, power_b_i_is_external_measure: Optional[bool]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_is_external_measure = power_b_i_is_external_measure
 
     @property
     def table(self) -> Optional[PowerBITable]:
-        return self.attributes.table
+        return None if self.attributes is None else self.attributes.table
 
     @table.setter
     def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table = table
 
@@ -21423,79 +23327,101 @@
         "power_b_i_sort_by_column",
         "power_b_i_column_summarize_by",
         "table",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.dataset_qualified_name
+        )
 
     @dataset_qualified_name.setter
     def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset_qualified_name = dataset_qualified_name
 
     @property
     def power_b_i_column_data_category(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_data_category
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_column_data_category
+        )
 
     @power_b_i_column_data_category.setter
     def power_b_i_column_data_category(
         self, power_b_i_column_data_category: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_column_data_category = power_b_i_column_data_category
 
     @property
     def power_b_i_column_data_type(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_data_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_column_data_type
+        )
 
     @power_b_i_column_data_type.setter
     def power_b_i_column_data_type(self, power_b_i_column_data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_column_data_type = power_b_i_column_data_type
 
     @property
     def power_b_i_sort_by_column(self) -> Optional[str]:
-        return self.attributes.power_b_i_sort_by_column
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_sort_by_column
+        )
 
     @power_b_i_sort_by_column.setter
     def power_b_i_sort_by_column(self, power_b_i_sort_by_column: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_sort_by_column = power_b_i_sort_by_column
 
     @property
     def power_b_i_column_summarize_by(self) -> Optional[str]:
-        return self.attributes.power_b_i_column_summarize_by
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_column_summarize_by
+        )
 
     @power_b_i_column_summarize_by.setter
     def power_b_i_column_summarize_by(
         self, power_b_i_column_summarize_by: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_column_summarize_by = power_b_i_column_summarize_by
 
     @property
     def table(self) -> Optional[PowerBITable]:
-        return self.attributes.table
+        return None if self.attributes is None else self.attributes.table
 
     @table.setter
     def table(self, table: Optional[PowerBITable]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.table = table
 
@@ -21554,91 +23480,109 @@
         "measures",
         "columns",
         "dataset",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def dataset_qualified_name(self) -> Optional[str]:
-        return self.attributes.dataset_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.dataset_qualified_name
+        )
 
     @dataset_qualified_name.setter
     def dataset_qualified_name(self, dataset_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset_qualified_name = dataset_qualified_name
 
     @property
     def power_b_i_table_source_expressions(self) -> Optional[set[str]]:
-        return self.attributes.power_b_i_table_source_expressions
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_table_source_expressions
+        )
 
     @power_b_i_table_source_expressions.setter
     def power_b_i_table_source_expressions(
         self, power_b_i_table_source_expressions: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_source_expressions = (
             power_b_i_table_source_expressions
         )
 
     @property
     def power_b_i_table_column_count(self) -> Optional[int]:
-        return self.attributes.power_b_i_table_column_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_table_column_count
+        )
 
     @power_b_i_table_column_count.setter
     def power_b_i_table_column_count(self, power_b_i_table_column_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_column_count = power_b_i_table_column_count
 
     @property
     def power_b_i_table_measure_count(self) -> Optional[int]:
-        return self.attributes.power_b_i_table_measure_count
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.power_b_i_table_measure_count
+        )
 
     @power_b_i_table_measure_count.setter
     def power_b_i_table_measure_count(
         self, power_b_i_table_measure_count: Optional[int]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.power_b_i_table_measure_count = power_b_i_table_measure_count
 
     @property
     def measures(self) -> Optional[list[PowerBIMeasure]]:
-        return self.attributes.measures
+        return None if self.attributes is None else self.attributes.measures
 
     @measures.setter
     def measures(self, measures: Optional[list[PowerBIMeasure]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.measures = measures
 
     @property
     def columns(self) -> Optional[list[PowerBIColumn]]:
-        return self.attributes.columns
+        return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[list[PowerBIColumn]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
     def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
+        return None if self.attributes is None else self.attributes.dataset
 
     @dataset.setter
     def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset = dataset
 
@@ -21697,55 +23641,63 @@
         "report",
         "dataset",
         "dashboard",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def dashboard_qualified_name(self) -> Optional[str]:
-        return self.attributes.dashboard_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.dashboard_qualified_name
+        )
 
     @dashboard_qualified_name.setter
     def dashboard_qualified_name(self, dashboard_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard_qualified_name = dashboard_qualified_name
 
     @property
     def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
+        return None if self.attributes is None else self.attributes.report
 
     @report.setter
     def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report = report
 
     @property
     def dataset(self) -> Optional[PowerBIDataset]:
-        return self.attributes.dataset
+        return None if self.attributes is None else self.attributes.dataset
 
     @dataset.setter
     def dataset(self, dataset: Optional[PowerBIDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset = dataset
 
     @property
     def dashboard(self) -> Optional[PowerBIDashboard]:
-        return self.attributes.dashboard
+        return None if self.attributes is None else self.attributes.dashboard
 
     @dashboard.setter
     def dashboard(self, dashboard: Optional[PowerBIDashboard]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard = dashboard
 
@@ -21792,25 +23744,25 @@
     _convience_properties: ClassVar[list[str]] = [
         "connection_details",
         "datasets",
     ]
 
     @property
     def connection_details(self) -> Optional[dict[str, str]]:
-        return self.attributes.connection_details
+        return None if self.attributes is None else self.attributes.connection_details
 
     @connection_details.setter
     def connection_details(self, connection_details: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.connection_details = connection_details
 
     @property
     def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
+        return None if self.attributes is None else self.attributes.datasets
 
     @datasets.setter
     def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasets = datasets
 
@@ -21855,95 +23807,95 @@
         "datasets",
         "dashboards",
         "dataflows",
     ]
 
     @property
     def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
+        return None if self.attributes is None else self.attributes.web_url
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
     def report_count(self) -> Optional[int]:
-        return self.attributes.report_count
+        return None if self.attributes is None else self.attributes.report_count
 
     @report_count.setter
     def report_count(self, report_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_count = report_count
 
     @property
     def dashboard_count(self) -> Optional[int]:
-        return self.attributes.dashboard_count
+        return None if self.attributes is None else self.attributes.dashboard_count
 
     @dashboard_count.setter
     def dashboard_count(self, dashboard_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard_count = dashboard_count
 
     @property
     def dataset_count(self) -> Optional[int]:
-        return self.attributes.dataset_count
+        return None if self.attributes is None else self.attributes.dataset_count
 
     @dataset_count.setter
     def dataset_count(self, dataset_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataset_count = dataset_count
 
     @property
     def dataflow_count(self) -> Optional[int]:
-        return self.attributes.dataflow_count
+        return None if self.attributes is None else self.attributes.dataflow_count
 
     @dataflow_count.setter
     def dataflow_count(self, dataflow_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflow_count = dataflow_count
 
     @property
     def reports(self) -> Optional[list[PowerBIReport]]:
-        return self.attributes.reports
+        return None if self.attributes is None else self.attributes.reports
 
     @reports.setter
     def reports(self, reports: Optional[list[PowerBIReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.reports = reports
 
     @property
     def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
+        return None if self.attributes is None else self.attributes.datasets
 
     @datasets.setter
     def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasets = datasets
 
     @property
     def dashboards(self) -> Optional[list[PowerBIDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[PowerBIDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
     @property
     def dataflows(self) -> Optional[list[PowerBIDataflow]]:
-        return self.attributes.dataflows
+        return None if self.attributes is None else self.attributes.dataflows
 
     @dataflows.setter
     def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflows = dataflows
 
@@ -22002,85 +23954,89 @@
         "tiles",
         "tables",
         "datasources",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
+        return None if self.attributes is None else self.attributes.web_url
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
     def reports(self) -> Optional[list[PowerBIReport]]:
-        return self.attributes.reports
+        return None if self.attributes is None else self.attributes.reports
 
     @reports.setter
     def reports(self, reports: Optional[list[PowerBIReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.reports = reports
 
     @property
     def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
+        return None if self.attributes is None else self.attributes.workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
     @property
     def dataflows(self) -> Optional[list[PowerBIDataflow]]:
-        return self.attributes.dataflows
+        return None if self.attributes is None else self.attributes.dataflows
 
     @dataflows.setter
     def dataflows(self, dataflows: Optional[list[PowerBIDataflow]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dataflows = dataflows
 
     @property
     def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
+        return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[list[PowerBITile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tiles = tiles
 
     @property
     def tables(self) -> Optional[list[PowerBITable]]:
-        return self.attributes.tables
+        return None if self.attributes is None else self.attributes.tables
 
     @tables.setter
     def tables(self, tables: Optional[list[PowerBITable]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tables = tables
 
     @property
     def datasources(self) -> Optional[list[PowerBIDatasource]]:
-        return self.attributes.datasources
+        return None if self.attributes is None else self.attributes.datasources
 
     @datasources.setter
     def datasources(self, datasources: Optional[list[PowerBIDatasource]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasources = datasources
 
@@ -22137,55 +24093,59 @@
         "tile_count",
         "tiles",
         "workspace",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
+        return None if self.attributes is None else self.attributes.web_url
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
     def tile_count(self) -> Optional[int]:
-        return self.attributes.tile_count
+        return None if self.attributes is None else self.attributes.tile_count
 
     @tile_count.setter
     def tile_count(self, tile_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tile_count = tile_count
 
     @property
     def tiles(self) -> Optional[list[PowerBITile]]:
-        return self.attributes.tiles
+        return None if self.attributes is None else self.attributes.tiles
 
     @tiles.setter
     def tiles(self, tiles: Optional[list[PowerBITile]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.tiles = tiles
 
     @property
     def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
+        return None if self.attributes is None else self.attributes.workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
@@ -22230,45 +24190,49 @@
         "web_url",
         "workspace",
         "datasets",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def web_url(self) -> Optional[str]:
-        return self.attributes.web_url
+        return None if self.attributes is None else self.attributes.web_url
 
     @web_url.setter
     def web_url(self, web_url: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.web_url = web_url
 
     @property
     def workspace(self) -> Optional[PowerBIWorkspace]:
-        return self.attributes.workspace
+        return None if self.attributes is None else self.attributes.workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[PowerBIWorkspace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace = workspace
 
     @property
     def datasets(self) -> Optional[list[PowerBIDataset]]:
-        return self.attributes.datasets
+        return None if self.attributes is None else self.attributes.datasets
 
     @datasets.setter
     def datasets(self, datasets: Optional[list[PowerBIDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.datasets = datasets
 
@@ -22311,35 +24275,41 @@
         "workspace_qualified_name",
         "report_qualified_name",
         "report",
     ]
 
     @property
     def workspace_qualified_name(self) -> Optional[str]:
-        return self.attributes.workspace_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.workspace_qualified_name
+        )
 
     @workspace_qualified_name.setter
     def workspace_qualified_name(self, workspace_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.workspace_qualified_name = workspace_qualified_name
 
     @property
     def report_qualified_name(self) -> Optional[str]:
-        return self.attributes.report_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.report_qualified_name
+        )
 
     @report_qualified_name.setter
     def report_qualified_name(self, report_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_qualified_name = report_qualified_name
 
     @property
     def report(self) -> Optional[PowerBIReport]:
-        return self.attributes.report
+        return None if self.attributes is None else self.attributes.report
 
     @report.setter
     def report(self, report: Optional[PowerBIReport]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report = report
 
@@ -22382,49 +24352,61 @@
         "micro_strategy_metrics",
         "micro_strategy_project",
         "micro_strategy_attributes",
     ]
 
     @property
     def micro_strategy_report_type(self) -> Optional[str]:
-        return self.attributes.micro_strategy_report_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_report_type
+        )
 
     @micro_strategy_report_type.setter
     def micro_strategy_report_type(self, micro_strategy_report_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_report_type = micro_strategy_report_type
 
     @property
     def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metrics
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_metrics
+        )
 
     @micro_strategy_metrics.setter
     def micro_strategy_metrics(
         self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metrics = micro_strategy_metrics
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
     @property
     def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
-        return self.attributes.micro_strategy_attributes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attributes
+        )
 
     @micro_strategy_attributes.setter
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -22476,101 +24458,119 @@
         "micro_strategy_cubes",
         "micro_strategy_dossiers",
         "micro_strategy_attributes",
     ]
 
     @property
     def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
-        return self.attributes.micro_strategy_reports
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_reports
+        )
 
     @micro_strategy_reports.setter
     def micro_strategy_reports(
         self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_reports = micro_strategy_reports
 
     @property
     def micro_strategy_facts(self) -> Optional[list[MicroStrategyFact]]:
-        return self.attributes.micro_strategy_facts
+        return None if self.attributes is None else self.attributes.micro_strategy_facts
 
     @micro_strategy_facts.setter
     def micro_strategy_facts(
         self, micro_strategy_facts: Optional[list[MicroStrategyFact]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_facts = micro_strategy_facts
 
     @property
     def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metrics
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_metrics
+        )
 
     @micro_strategy_metrics.setter
     def micro_strategy_metrics(
         self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metrics = micro_strategy_metrics
 
     @property
     def micro_strategy_visualizations(
         self,
     ) -> Optional[list[MicroStrategyVisualization]]:
-        return self.attributes.micro_strategy_visualizations
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_visualizations
+        )
 
     @micro_strategy_visualizations.setter
     def micro_strategy_visualizations(
         self, micro_strategy_visualizations: Optional[list[MicroStrategyVisualization]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_visualizations = micro_strategy_visualizations
 
     @property
     def micro_strategy_documents(self) -> Optional[list[MicroStrategyDocument]]:
-        return self.attributes.micro_strategy_documents
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_documents
+        )
 
     @micro_strategy_documents.setter
     def micro_strategy_documents(
         self, micro_strategy_documents: Optional[list[MicroStrategyDocument]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_documents = micro_strategy_documents
 
     @property
     def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
-        return self.attributes.micro_strategy_cubes
+        return None if self.attributes is None else self.attributes.micro_strategy_cubes
 
     @micro_strategy_cubes.setter
     def micro_strategy_cubes(
         self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cubes = micro_strategy_cubes
 
     @property
     def micro_strategy_dossiers(self) -> Optional[list[MicroStrategyDossier]]:
-        return self.attributes.micro_strategy_dossiers
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_dossiers
+        )
 
     @micro_strategy_dossiers.setter
     def micro_strategy_dossiers(
         self, micro_strategy_dossiers: Optional[list[MicroStrategyDossier]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_dossiers = micro_strategy_dossiers
 
     @property
     def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
-        return self.attributes.micro_strategy_attributes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attributes
+        )
 
     @micro_strategy_attributes.setter
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -22642,179 +24642,223 @@
         "micro_strategy_metric_children",
         "micro_strategy_project",
         "micro_strategy_attributes",
     ]
 
     @property
     def micro_strategy_metric_expression(self) -> Optional[str]:
-        return self.attributes.micro_strategy_metric_expression
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_metric_expression
+        )
 
     @micro_strategy_metric_expression.setter
     def micro_strategy_metric_expression(
         self, micro_strategy_metric_expression: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metric_expression = (
             micro_strategy_metric_expression
         )
 
     @property
     def micro_strategy_attribute_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_attribute_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attribute_qualified_names
+        )
 
     @micro_strategy_attribute_qualified_names.setter
     def micro_strategy_attribute_qualified_names(
         self, micro_strategy_attribute_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attribute_qualified_names = (
             micro_strategy_attribute_qualified_names
         )
 
     @property
     def micro_strategy_attribute_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_attribute_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attribute_names
+        )
 
     @micro_strategy_attribute_names.setter
     def micro_strategy_attribute_names(
         self, micro_strategy_attribute_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attribute_names = micro_strategy_attribute_names
 
     @property
     def micro_strategy_fact_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_fact_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_fact_qualified_names
+        )
 
     @micro_strategy_fact_qualified_names.setter
     def micro_strategy_fact_qualified_names(
         self, micro_strategy_fact_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_fact_qualified_names = (
             micro_strategy_fact_qualified_names
         )
 
     @property
     def micro_strategy_fact_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_fact_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_fact_names
+        )
 
     @micro_strategy_fact_names.setter
     def micro_strategy_fact_names(self, micro_strategy_fact_names: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_fact_names = micro_strategy_fact_names
 
     @property
     def micro_strategy_metric_parent_qualified_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_metric_parent_qualified_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_metric_parent_qualified_names
+        )
 
     @micro_strategy_metric_parent_qualified_names.setter
     def micro_strategy_metric_parent_qualified_names(
         self, micro_strategy_metric_parent_qualified_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metric_parent_qualified_names = (
             micro_strategy_metric_parent_qualified_names
         )
 
     @property
     def micro_strategy_metric_parent_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_metric_parent_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_metric_parent_names
+        )
 
     @micro_strategy_metric_parent_names.setter
     def micro_strategy_metric_parent_names(
         self, micro_strategy_metric_parent_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metric_parent_names = (
             micro_strategy_metric_parent_names
         )
 
     @property
     def micro_strategy_metric_parents(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metric_parents
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_metric_parents
+        )
 
     @micro_strategy_metric_parents.setter
     def micro_strategy_metric_parents(
         self, micro_strategy_metric_parents: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metric_parents = micro_strategy_metric_parents
 
     @property
     def micro_strategy_facts(self) -> Optional[list[MicroStrategyFact]]:
-        return self.attributes.micro_strategy_facts
+        return None if self.attributes is None else self.attributes.micro_strategy_facts
 
     @micro_strategy_facts.setter
     def micro_strategy_facts(
         self, micro_strategy_facts: Optional[list[MicroStrategyFact]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_facts = micro_strategy_facts
 
     @property
     def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
-        return self.attributes.micro_strategy_reports
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_reports
+        )
 
     @micro_strategy_reports.setter
     def micro_strategy_reports(
         self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_reports = micro_strategy_reports
 
     @property
     def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
-        return self.attributes.micro_strategy_cubes
+        return None if self.attributes is None else self.attributes.micro_strategy_cubes
 
     @micro_strategy_cubes.setter
     def micro_strategy_cubes(
         self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cubes = micro_strategy_cubes
 
     @property
     def micro_strategy_metric_children(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metric_children
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_metric_children
+        )
 
     @micro_strategy_metric_children.setter
     def micro_strategy_metric_children(
         self, micro_strategy_metric_children: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metric_children = micro_strategy_metric_children
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
     @property
     def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
-        return self.attributes.micro_strategy_attributes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attributes
+        )
 
     @micro_strategy_attributes.setter
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -22893,59 +24937,75 @@
         "micro_strategy_metrics",
         "micro_strategy_project",
         "micro_strategy_attributes",
     ]
 
     @property
     def micro_strategy_cube_type(self) -> Optional[str]:
-        return self.attributes.micro_strategy_cube_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_cube_type
+        )
 
     @micro_strategy_cube_type.setter
     def micro_strategy_cube_type(self, micro_strategy_cube_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cube_type = micro_strategy_cube_type
 
     @property
     def micro_strategy_cube_query(self) -> Optional[str]:
-        return self.attributes.micro_strategy_cube_query
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_cube_query
+        )
 
     @micro_strategy_cube_query.setter
     def micro_strategy_cube_query(self, micro_strategy_cube_query: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cube_query = micro_strategy_cube_query
 
     @property
     def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metrics
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_metrics
+        )
 
     @micro_strategy_metrics.setter
     def micro_strategy_metrics(
         self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metrics = micro_strategy_metrics
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
     @property
     def micro_strategy_attributes(self) -> Optional[list[MicroStrategyAttribute]]:
-        return self.attributes.micro_strategy_attributes
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attributes
+        )
 
     @micro_strategy_attributes.setter
     def micro_strategy_attributes(
         self, micro_strategy_attributes: Optional[list[MicroStrategyAttribute]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -22995,43 +25055,53 @@
         "micro_strategy_dossier_chapter_names",
         "micro_strategy_project",
         "micro_strategy_visualizations",
     ]
 
     @property
     def micro_strategy_dossier_chapter_names(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_dossier_chapter_names
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_dossier_chapter_names
+        )
 
     @micro_strategy_dossier_chapter_names.setter
     def micro_strategy_dossier_chapter_names(
         self, micro_strategy_dossier_chapter_names: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_dossier_chapter_names = (
             micro_strategy_dossier_chapter_names
         )
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_project = micro_strategy_project
 
     @property
     def micro_strategy_visualizations(
         self,
     ) -> Optional[list[MicroStrategyVisualization]]:
-        return self.attributes.micro_strategy_visualizations
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_visualizations
+        )
 
     @micro_strategy_visualizations.setter
     def micro_strategy_visualizations(
         self, micro_strategy_visualizations: Optional[list[MicroStrategyVisualization]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -23077,41 +25147,49 @@
         "micro_strategy_fact_expressions",
         "micro_strategy_metrics",
         "micro_strategy_project",
     ]
 
     @property
     def micro_strategy_fact_expressions(self) -> Optional[set[str]]:
-        return self.attributes.micro_strategy_fact_expressions
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_fact_expressions
+        )
 
     @micro_strategy_fact_expressions.setter
     def micro_strategy_fact_expressions(
         self, micro_strategy_fact_expressions: Optional[set[str]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_fact_expressions = (
             micro_strategy_fact_expressions
         )
 
     @property
     def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metrics
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_metrics
+        )
 
     @micro_strategy_metrics.setter
     def micro_strategy_metrics(
         self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metrics = micro_strategy_metrics
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -23153,15 +25231,17 @@
 
     _convience_properties: ClassVar[list[str]] = [
         "micro_strategy_project",
     ]
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -23201,63 +25281,73 @@
         "micro_strategy_metrics",
         "micro_strategy_cubes",
         "micro_strategy_project",
     ]
 
     @property
     def micro_strategy_attribute_forms(self) -> Optional[str]:
-        return self.attributes.micro_strategy_attribute_forms
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_attribute_forms
+        )
 
     @micro_strategy_attribute_forms.setter
     def micro_strategy_attribute_forms(
         self, micro_strategy_attribute_forms: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_attribute_forms = micro_strategy_attribute_forms
 
     @property
     def micro_strategy_reports(self) -> Optional[list[MicroStrategyReport]]:
-        return self.attributes.micro_strategy_reports
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_reports
+        )
 
     @micro_strategy_reports.setter
     def micro_strategy_reports(
         self, micro_strategy_reports: Optional[list[MicroStrategyReport]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_reports = micro_strategy_reports
 
     @property
     def micro_strategy_metrics(self) -> Optional[list[MicroStrategyMetric]]:
-        return self.attributes.micro_strategy_metrics
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_metrics
+        )
 
     @micro_strategy_metrics.setter
     def micro_strategy_metrics(
         self, micro_strategy_metrics: Optional[list[MicroStrategyMetric]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_metrics = micro_strategy_metrics
 
     @property
     def micro_strategy_cubes(self) -> Optional[list[MicroStrategyCube]]:
-        return self.attributes.micro_strategy_cubes
+        return None if self.attributes is None else self.attributes.micro_strategy_cubes
 
     @micro_strategy_cubes.setter
     def micro_strategy_cubes(
         self, micro_strategy_cubes: Optional[list[MicroStrategyCube]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_cubes = micro_strategy_cubes
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -23309,65 +25399,81 @@
         "micro_strategy_dossier_name",
         "micro_strategy_dossier",
         "micro_strategy_project",
     ]
 
     @property
     def micro_strategy_visualization_type(self) -> Optional[str]:
-        return self.attributes.micro_strategy_visualization_type
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_visualization_type
+        )
 
     @micro_strategy_visualization_type.setter
     def micro_strategy_visualization_type(
         self, micro_strategy_visualization_type: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_visualization_type = (
             micro_strategy_visualization_type
         )
 
     @property
     def micro_strategy_dossier_qualified_name(self) -> Optional[str]:
-        return self.attributes.micro_strategy_dossier_qualified_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_dossier_qualified_name
+        )
 
     @micro_strategy_dossier_qualified_name.setter
     def micro_strategy_dossier_qualified_name(
         self, micro_strategy_dossier_qualified_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_dossier_qualified_name = (
             micro_strategy_dossier_qualified_name
         )
 
     @property
     def micro_strategy_dossier_name(self) -> Optional[str]:
-        return self.attributes.micro_strategy_dossier_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.micro_strategy_dossier_name
+        )
 
     @micro_strategy_dossier_name.setter
     def micro_strategy_dossier_name(self, micro_strategy_dossier_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_dossier_name = micro_strategy_dossier_name
 
     @property
     def micro_strategy_dossier(self) -> Optional[MicroStrategyDossier]:
-        return self.attributes.micro_strategy_dossier
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_dossier
+        )
 
     @micro_strategy_dossier.setter
     def micro_strategy_dossier(
         self, micro_strategy_dossier: Optional[MicroStrategyDossier]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.micro_strategy_dossier = micro_strategy_dossier
 
     @property
     def micro_strategy_project(self) -> Optional[MicroStrategyProject]:
-        return self.attributes.micro_strategy_project
+        return (
+            None if self.attributes is None else self.attributes.micro_strategy_project
+        )
 
     @micro_strategy_project.setter
     def micro_strategy_project(
         self, micro_strategy_project: Optional[MicroStrategyProject]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -23417,35 +25523,35 @@
         "qlik_space_type",
         "qlik_datasets",
         "qlik_apps",
     ]
 
     @property
     def qlik_space_type(self) -> Optional[str]:
-        return self.attributes.qlik_space_type
+        return None if self.attributes is None else self.attributes.qlik_space_type
 
     @qlik_space_type.setter
     def qlik_space_type(self, qlik_space_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space_type = qlik_space_type
 
     @property
     def qlik_datasets(self) -> Optional[list[QlikDataset]]:
-        return self.attributes.qlik_datasets
+        return None if self.attributes is None else self.attributes.qlik_datasets
 
     @qlik_datasets.setter
     def qlik_datasets(self, qlik_datasets: Optional[list[QlikDataset]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_datasets = qlik_datasets
 
     @property
     def qlik_apps(self) -> Optional[list[QlikApp]]:
-        return self.attributes.qlik_apps
+        return None if self.attributes is None else self.attributes.qlik_apps
 
     @qlik_apps.setter
     def qlik_apps(self, qlik_apps: Optional[list[QlikApp]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_apps = qlik_apps
 
@@ -23491,75 +25597,85 @@
         "qlik_app_static_byte_size",
         "qlik_space",
         "qlik_sheets",
     ]
 
     @property
     def qlik_has_section_access(self) -> Optional[bool]:
-        return self.attributes.qlik_has_section_access
+        return (
+            None if self.attributes is None else self.attributes.qlik_has_section_access
+        )
 
     @qlik_has_section_access.setter
     def qlik_has_section_access(self, qlik_has_section_access: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_has_section_access = qlik_has_section_access
 
     @property
     def qlik_origin_app_id(self) -> Optional[str]:
-        return self.attributes.qlik_origin_app_id
+        return None if self.attributes is None else self.attributes.qlik_origin_app_id
 
     @qlik_origin_app_id.setter
     def qlik_origin_app_id(self, qlik_origin_app_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_origin_app_id = qlik_origin_app_id
 
     @property
     def qlik_is_encrypted(self) -> Optional[bool]:
-        return self.attributes.qlik_is_encrypted
+        return None if self.attributes is None else self.attributes.qlik_is_encrypted
 
     @qlik_is_encrypted.setter
     def qlik_is_encrypted(self, qlik_is_encrypted: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_encrypted = qlik_is_encrypted
 
     @property
     def qlik_is_direct_query_mode(self) -> Optional[bool]:
-        return self.attributes.qlik_is_direct_query_mode
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.qlik_is_direct_query_mode
+        )
 
     @qlik_is_direct_query_mode.setter
     def qlik_is_direct_query_mode(self, qlik_is_direct_query_mode: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_is_direct_query_mode = qlik_is_direct_query_mode
 
     @property
     def qlik_app_static_byte_size(self) -> Optional[int]:
-        return self.attributes.qlik_app_static_byte_size
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.qlik_app_static_byte_size
+        )
 
     @qlik_app_static_byte_size.setter
     def qlik_app_static_byte_size(self, qlik_app_static_byte_size: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app_static_byte_size = qlik_app_static_byte_size
 
     @property
     def qlik_space(self) -> Optional[QlikSpace]:
-        return self.attributes.qlik_space
+        return None if self.attributes is None else self.attributes.qlik_space
 
     @qlik_space.setter
     def qlik_space(self, qlik_space: Optional[QlikSpace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space = qlik_space
 
     @property
     def qlik_sheets(self) -> Optional[list[QlikSheet]]:
-        return self.attributes.qlik_sheets
+        return None if self.attributes is None else self.attributes.qlik_sheets
 
     @qlik_sheets.setter
     def qlik_sheets(self, qlik_sheets: Optional[list[QlikSheet]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheets = qlik_sheets
 
@@ -23615,55 +25731,57 @@
         "qlik_chart_orientation",
         "qlik_chart_type",
         "qlik_sheet",
     ]
 
     @property
     def qlik_chart_subtitle(self) -> Optional[str]:
-        return self.attributes.qlik_chart_subtitle
+        return None if self.attributes is None else self.attributes.qlik_chart_subtitle
 
     @qlik_chart_subtitle.setter
     def qlik_chart_subtitle(self, qlik_chart_subtitle: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_subtitle = qlik_chart_subtitle
 
     @property
     def qlik_chart_footnote(self) -> Optional[str]:
-        return self.attributes.qlik_chart_footnote
+        return None if self.attributes is None else self.attributes.qlik_chart_footnote
 
     @qlik_chart_footnote.setter
     def qlik_chart_footnote(self, qlik_chart_footnote: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_footnote = qlik_chart_footnote
 
     @property
     def qlik_chart_orientation(self) -> Optional[str]:
-        return self.attributes.qlik_chart_orientation
+        return (
+            None if self.attributes is None else self.attributes.qlik_chart_orientation
+        )
 
     @qlik_chart_orientation.setter
     def qlik_chart_orientation(self, qlik_chart_orientation: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_orientation = qlik_chart_orientation
 
     @property
     def qlik_chart_type(self) -> Optional[str]:
-        return self.attributes.qlik_chart_type
+        return None if self.attributes is None else self.attributes.qlik_chart_type
 
     @qlik_chart_type.setter
     def qlik_chart_type(self, qlik_chart_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_chart_type = qlik_chart_type
 
     @property
     def qlik_sheet(self) -> Optional[QlikSheet]:
-        return self.attributes.qlik_sheet
+        return None if self.attributes is None else self.attributes.qlik_sheet
 
     @qlik_sheet.setter
     def qlik_sheet(self, qlik_sheet: Optional[QlikSheet]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheet = qlik_sheet
 
@@ -23713,55 +25831,59 @@
         "qlik_dataset_uri",
         "qlik_dataset_subtype",
         "qlik_space",
     ]
 
     @property
     def qlik_dataset_technical_name(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_technical_name
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.qlik_dataset_technical_name
+        )
 
     @qlik_dataset_technical_name.setter
     def qlik_dataset_technical_name(self, qlik_dataset_technical_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_technical_name = qlik_dataset_technical_name
 
     @property
     def qlik_dataset_type(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_type
+        return None if self.attributes is None else self.attributes.qlik_dataset_type
 
     @qlik_dataset_type.setter
     def qlik_dataset_type(self, qlik_dataset_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_type = qlik_dataset_type
 
     @property
     def qlik_dataset_uri(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_uri
+        return None if self.attributes is None else self.attributes.qlik_dataset_uri
 
     @qlik_dataset_uri.setter
     def qlik_dataset_uri(self, qlik_dataset_uri: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_uri = qlik_dataset_uri
 
     @property
     def qlik_dataset_subtype(self) -> Optional[str]:
-        return self.attributes.qlik_dataset_subtype
+        return None if self.attributes is None else self.attributes.qlik_dataset_subtype
 
     @qlik_dataset_subtype.setter
     def qlik_dataset_subtype(self, qlik_dataset_subtype: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_dataset_subtype = qlik_dataset_subtype
 
     @property
     def qlik_space(self) -> Optional[QlikSpace]:
-        return self.attributes.qlik_space
+        return None if self.attributes is None else self.attributes.qlik_space
 
     @qlik_space.setter
     def qlik_space(self, qlik_space: Optional[QlikSpace]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_space = qlik_space
 
@@ -23809,35 +25931,37 @@
         "qlik_sheet_is_approved",
         "qlik_app",
         "qlik_charts",
     ]
 
     @property
     def qlik_sheet_is_approved(self) -> Optional[bool]:
-        return self.attributes.qlik_sheet_is_approved
+        return (
+            None if self.attributes is None else self.attributes.qlik_sheet_is_approved
+        )
 
     @qlik_sheet_is_approved.setter
     def qlik_sheet_is_approved(self, qlik_sheet_is_approved: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_sheet_is_approved = qlik_sheet_is_approved
 
     @property
     def qlik_app(self) -> Optional[QlikApp]:
-        return self.attributes.qlik_app
+        return None if self.attributes is None else self.attributes.qlik_app
 
     @qlik_app.setter
     def qlik_app(self, qlik_app: Optional[QlikApp]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_app = qlik_app
 
     @property
     def qlik_charts(self) -> Optional[list[QlikChart]]:
-        return self.attributes.qlik_charts
+        return None if self.attributes is None else self.attributes.qlik_charts
 
     @qlik_charts.setter
     def qlik_charts(self, qlik_charts: Optional[list[QlikChart]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.qlik_charts = qlik_charts
 
@@ -23883,75 +26007,75 @@
         "organization",
         "lookup_fields",
         "fields",
     ]
 
     @property
     def is_custom(self) -> Optional[bool]:
-        return self.attributes.is_custom
+        return None if self.attributes is None else self.attributes.is_custom
 
     @is_custom.setter
     def is_custom(self, is_custom: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_custom = is_custom
 
     @property
     def is_mergable(self) -> Optional[bool]:
-        return self.attributes.is_mergable
+        return None if self.attributes is None else self.attributes.is_mergable
 
     @is_mergable.setter
     def is_mergable(self, is_mergable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_mergable = is_mergable
 
     @property
     def is_queryable(self) -> Optional[bool]:
-        return self.attributes.is_queryable
+        return None if self.attributes is None else self.attributes.is_queryable
 
     @is_queryable.setter
     def is_queryable(self, is_queryable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_queryable = is_queryable
 
     @property
     def field_count(self) -> Optional[int]:
-        return self.attributes.field_count
+        return None if self.attributes is None else self.attributes.field_count
 
     @field_count.setter
     def field_count(self, field_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.field_count = field_count
 
     @property
     def organization(self) -> Optional[SalesforceOrganization]:
-        return self.attributes.organization
+        return None if self.attributes is None else self.attributes.organization
 
     @organization.setter
     def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.organization = organization
 
     @property
     def lookup_fields(self) -> Optional[list[SalesforceField]]:
-        return self.attributes.lookup_fields
+        return None if self.attributes is None else self.attributes.lookup_fields
 
     @lookup_fields.setter
     def lookup_fields(self, lookup_fields: Optional[list[SalesforceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.lookup_fields = lookup_fields
 
     @property
     def fields(self) -> Optional[list[SalesforceField]]:
-        return self.attributes.fields
+        return None if self.attributes is None else self.attributes.fields
 
     @fields.setter
     def fields(self, fields: Optional[list[SalesforceField]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.fields = fields
 
@@ -24012,185 +26136,193 @@
         "default_value_formula",
         "lookup_objects",
         "object",
     ]
 
     @property
     def data_type(self) -> Optional[str]:
-        return self.attributes.data_type
+        return None if self.attributes is None else self.attributes.data_type
 
     @data_type.setter
     def data_type(self, data_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.data_type = data_type
 
     @property
     def object_qualified_name(self) -> Optional[str]:
-        return self.attributes.object_qualified_name
+        return (
+            None if self.attributes is None else self.attributes.object_qualified_name
+        )
 
     @object_qualified_name.setter
     def object_qualified_name(self, object_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.object_qualified_name = object_qualified_name
 
     @property
     def order(self) -> Optional[int]:
-        return self.attributes.order
+        return None if self.attributes is None else self.attributes.order
 
     @order.setter
     def order(self, order: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.order = order
 
     @property
     def inline_help_text(self) -> Optional[str]:
-        return self.attributes.inline_help_text
+        return None if self.attributes is None else self.attributes.inline_help_text
 
     @inline_help_text.setter
     def inline_help_text(self, inline_help_text: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.inline_help_text = inline_help_text
 
     @property
     def is_calculated(self) -> Optional[bool]:
-        return self.attributes.is_calculated
+        return None if self.attributes is None else self.attributes.is_calculated
 
     @is_calculated.setter
     def is_calculated(self, is_calculated: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_calculated = is_calculated
 
     @property
     def formula(self) -> Optional[str]:
-        return self.attributes.formula
+        return None if self.attributes is None else self.attributes.formula
 
     @formula.setter
     def formula(self, formula: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.formula = formula
 
     @property
     def is_case_sensitive(self) -> Optional[bool]:
-        return self.attributes.is_case_sensitive
+        return None if self.attributes is None else self.attributes.is_case_sensitive
 
     @is_case_sensitive.setter
     def is_case_sensitive(self, is_case_sensitive: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_case_sensitive = is_case_sensitive
 
     @property
     def is_encrypted(self) -> Optional[bool]:
-        return self.attributes.is_encrypted
+        return None if self.attributes is None else self.attributes.is_encrypted
 
     @is_encrypted.setter
     def is_encrypted(self, is_encrypted: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_encrypted = is_encrypted
 
     @property
     def max_length(self) -> Optional[int]:
-        return self.attributes.max_length
+        return None if self.attributes is None else self.attributes.max_length
 
     @max_length.setter
     def max_length(self, max_length: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.max_length = max_length
 
     @property
     def is_nullable(self) -> Optional[bool]:
-        return self.attributes.is_nullable
+        return None if self.attributes is None else self.attributes.is_nullable
 
     @is_nullable.setter
     def is_nullable(self, is_nullable: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_nullable = is_nullable
 
     @property
     def precision(self) -> Optional[int]:
-        return self.attributes.precision
+        return None if self.attributes is None else self.attributes.precision
 
     @precision.setter
     def precision(self, precision: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.precision = precision
 
     @property
     def numeric_scale(self) -> Optional[float]:
-        return self.attributes.numeric_scale
+        return None if self.attributes is None else self.attributes.numeric_scale
 
     @numeric_scale.setter
     def numeric_scale(self, numeric_scale: Optional[float]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.numeric_scale = numeric_scale
 
     @property
     def is_unique(self) -> Optional[bool]:
-        return self.attributes.is_unique
+        return None if self.attributes is None else self.attributes.is_unique
 
     @is_unique.setter
     def is_unique(self, is_unique: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_unique = is_unique
 
     @property
     def picklist_values(self) -> Optional[set[str]]:
-        return self.attributes.picklist_values
+        return None if self.attributes is None else self.attributes.picklist_values
 
     @picklist_values.setter
     def picklist_values(self, picklist_values: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.picklist_values = picklist_values
 
     @property
     def is_polymorphic_foreign_key(self) -> Optional[bool]:
-        return self.attributes.is_polymorphic_foreign_key
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.is_polymorphic_foreign_key
+        )
 
     @is_polymorphic_foreign_key.setter
     def is_polymorphic_foreign_key(self, is_polymorphic_foreign_key: Optional[bool]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.is_polymorphic_foreign_key = is_polymorphic_foreign_key
 
     @property
     def default_value_formula(self) -> Optional[str]:
-        return self.attributes.default_value_formula
+        return (
+            None if self.attributes is None else self.attributes.default_value_formula
+        )
 
     @default_value_formula.setter
     def default_value_formula(self, default_value_formula: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.default_value_formula = default_value_formula
 
     @property
     def lookup_objects(self) -> Optional[list[SalesforceObject]]:
-        return self.attributes.lookup_objects
+        return None if self.attributes is None else self.attributes.lookup_objects
 
     @lookup_objects.setter
     def lookup_objects(self, lookup_objects: Optional[list[SalesforceObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.lookup_objects = lookup_objects
 
     @property
     def object(self) -> Optional[SalesforceObject]:
-        return self.attributes.object
+        return None if self.attributes is None else self.attributes.object
 
     @object.setter
     def object(self, object: Optional[SalesforceObject]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.object = object
 
@@ -24262,45 +26394,45 @@
         "reports",
         "objects",
         "dashboards",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
-        return self.attributes.source_id
+        return None if self.attributes is None else self.attributes.source_id
 
     @source_id.setter
     def source_id(self, source_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_id = source_id
 
     @property
     def reports(self) -> Optional[list[SalesforceReport]]:
-        return self.attributes.reports
+        return None if self.attributes is None else self.attributes.reports
 
     @reports.setter
     def reports(self, reports: Optional[list[SalesforceReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.reports = reports
 
     @property
     def objects(self) -> Optional[list[SalesforceObject]]:
-        return self.attributes.objects
+        return None if self.attributes is None else self.attributes.objects
 
     @objects.setter
     def objects(self, objects: Optional[list[SalesforceObject]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.objects = objects
 
     @property
     def dashboards(self) -> Optional[list[SalesforceDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
 
@@ -24345,55 +26477,55 @@
         "report_count",
         "reports",
         "organization",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
-        return self.attributes.source_id
+        return None if self.attributes is None else self.attributes.source_id
 
     @source_id.setter
     def source_id(self, source_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_id = source_id
 
     @property
     def dashboard_type(self) -> Optional[str]:
-        return self.attributes.dashboard_type
+        return None if self.attributes is None else self.attributes.dashboard_type
 
     @dashboard_type.setter
     def dashboard_type(self, dashboard_type: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboard_type = dashboard_type
 
     @property
     def report_count(self) -> Optional[int]:
-        return self.attributes.report_count
+        return None if self.attributes is None else self.attributes.report_count
 
     @report_count.setter
     def report_count(self, report_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_count = report_count
 
     @property
     def reports(self) -> Optional[list[SalesforceReport]]:
-        return self.attributes.reports
+        return None if self.attributes is None else self.attributes.reports
 
     @reports.setter
     def reports(self, reports: Optional[list[SalesforceReport]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.reports = reports
 
     @property
     def organization(self) -> Optional[SalesforceOrganization]:
-        return self.attributes.organization
+        return None if self.attributes is None else self.attributes.organization
 
     @organization.setter
     def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.organization = organization
 
@@ -24439,55 +26571,55 @@
         "detail_columns",
         "organization",
         "dashboards",
     ]
 
     @property
     def source_id(self) -> Optional[str]:
-        return self.attributes.source_id
+        return None if self.attributes is None else self.attributes.source_id
 
     @source_id.setter
     def source_id(self, source_id: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.source_id = source_id
 
     @property
     def report_type(self) -> Optional[dict[str, str]]:
-        return self.attributes.report_type
+        return None if self.attributes is None else self.attributes.report_type
 
     @report_type.setter
     def report_type(self, report_type: Optional[dict[str, str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.report_type = report_type
 
     @property
     def detail_columns(self) -> Optional[set[str]]:
-        return self.attributes.detail_columns
+        return None if self.attributes is None else self.attributes.detail_columns
 
     @detail_columns.setter
     def detail_columns(self, detail_columns: Optional[set[str]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.detail_columns = detail_columns
 
     @property
     def organization(self) -> Optional[SalesforceOrganization]:
-        return self.attributes.organization
+        return None if self.attributes is None else self.attributes.organization
 
     @organization.setter
     def organization(self, organization: Optional[SalesforceOrganization]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.organization = organization
 
     @property
     def dashboards(self) -> Optional[list[SalesforceDashboard]]:
-        return self.attributes.dashboards
+        return None if self.attributes is None else self.attributes.dashboards
 
     @dashboards.setter
     def dashboards(self, dashboards: Optional[list[SalesforceDashboard]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dashboards = dashboards
```

### Comparing `pyatlan-0.1.2/pyatlan/model/atlan_image.py` & `pyatlan-0.1.3/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/core.py` & `pyatlan-0.1.3/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/custom_metadata.py` & `pyatlan-0.1.3/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/enums.py` & `pyatlan-0.1.3/pyatlan/model/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,14 +395,22 @@
     DENY = "deny"
     ALLOWEXCEPTIONS = "allowExceptions"
     DENYEXCEPTIONS = "denyExceptions"
     DATAMASK = "dataMask"
     ROWFILTER = "rowFilter"
 
 
+class DataMaskingType(str, Enum):
+    SHOW_FIRST_4 = "MASK_SHOW_FIRST_4"
+    SHOW_LAST_4 = "MASK_SHOW_LAST_4"
+    HASH = "MASK_HASH"
+    NULLIFY = "MASK_NULL"
+    REDACT = "MASK_REDACT"
+
+
 class AuthPolicyCategory(str, Enum):
     BOOTSTRAP = "bootstrap"
     PERSONA = "persona"
     PURPOSE = "purpose"
 
 
 class AuthPolicyResourceCategory(str, Enum):
@@ -410,14 +418,77 @@
     RELATIONSHIP = "RELATIONSHIP"
     TAG = "TAG"
     CUSTOM = "CUSTOM"
     TYPEDEFS = "TYPEDEFS"
     ADMIN = "ADMIN"
 
 
+class AssetSidebarTab(str, Enum):
+    INCIDENTS = "Incidents"
+    VISUALS = "Visuals"
+    COLUMNS = "Columns"
+    RUNS = "Runs"
+    TASKS = "Tasks"
+    USAGE = "Usage"
+    OBJECTS = "Objects"
+    LINEAGE = "Lineage"
+    FIELDS = "Fields"
+    VISUALIZATIONS = "Visualizations"
+    RELATIONS = "Relations"
+    PROFILE = "Profile"
+    ASSETS = "Assets"
+    ACTIVITY = "Activity"
+    SCHEDULES = "Schedules"
+    RESOURCES = "Resources"
+    QUERIES = "Queries"
+    REQUESTS = "Requests"
+    PROPERTIES = "Properties"
+    MONTE_CARLO = "Monte Carlo"
+
+
+class DataAction(str, Enum):
+    SELECT = "select"
+
+
+class PurposeMetadataAction(str, Enum):
+    CREATE = "entity-create"
+    READ = "entity-read"
+    UPDATE = "entity-update"
+    DELETE = "entity-delete"
+    UPDATE_CUSTOM_METADATA = "entity-update-business-metadata"
+    ADD_ATLAN_TAG = "entity-add-classification"
+    READ_ATLAN_TAG = "entity-read-classification"
+    UPDATE_ATLAN_TAG = "entity-update-classification"
+    REMOVE_ATLAN_TAG = "entity-remove-classification"
+
+
+class PersonaMetadataAction(str, Enum):
+    CREATE = "persona-api-create"
+    READ = "persona-asset-read"
+    UPDATE = "persona-asset-update"
+    DELETE = "persona-api-delete"
+    UPDATE_CUSTOM_METADATA = "persona-business-update-metadata"
+    ADD_ATLAN_TAG = "persona-entity-add-classification"
+    UPDATE_ATLAN_TAG = "persona-entity-update-classification"
+    REMOVE_ATLAN_TAG = "persona-entity-remove-classification"
+    ATTACH_TERMS = "persona-add-terms"
+    DETACH_TERMS = "persona-remove-terms"
+
+
+class PersonaGlossaryAction(str, Enum):
+    CREATE = "persona-glossary-create"
+    READ = "persona-glossary-read"
+    UPDATE = "persona-glossary-update"
+    DELETE = "persona-glossary-delete"
+    UPDATE_CUSTOM_METADATA = "persona-glossary-update-custom-metadata"
+    ADD_ATLAN_TAG = "persona-glossary-add-classifications"
+    UPDATE_ATLAN_TAG = "persona-glossary-update-classifications"
+    REMOVE_ATLAN_TAG = "persona-glossary-delete-classifications"
+
+
 class AtlanIcon(str, Enum):
     ATLAN_TAG = "atlanTags"
     ATLAN_SHIELD = "atlanShield"
     ADDRESS_BOOK = "PhAddressBook"
     AIR_TRAFFIC_CONTROL = "PhAirTrafficControl"
     AIRPLANE = "PhAirplane"
     AIRPLANE_IN_FLIGHT = "PhAirplaneInFlight"
```

### Comparing `pyatlan-0.1.2/pyatlan/model/group.py` & `pyatlan-0.1.3/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/lineage.py` & `pyatlan-0.1.3/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/query.py` & `pyatlan-0.1.3/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/response.py` & `pyatlan-0.1.3/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/role.py` & `pyatlan-0.1.3/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/search.py` & `pyatlan-0.1.3/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/structs.py` & `pyatlan-0.1.3/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/typedef.py` & `pyatlan-0.1.3/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/model/user.py` & `pyatlan-0.1.3/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/multipart_data_generator.py` & `pyatlan-0.1.3/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan/utils.py` & `pyatlan-0.1.3/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.1.3/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.1.2/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.1.3/pyatlan.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -50,22 +50,43 @@
 tests/integration/classification_test.py
 tests/integration/client.py
 tests/integration/conftest.py
 tests/integration/connection_test.py
 tests/integration/custom_metadata_test.py
 tests/integration/glossary_test.py
 tests/integration/lineage_test.py
+tests/integration/persona_test.py
+tests/integration/purpose_test.py
 tests/integration/query_parser_test.py
 tests/integration/s3_asset_test.py
 tests/integration/test_client.py
 tests/integration/test_index_search.py
 tests/integration/test_sql_assets.py
 tests/unit/__init__.py
+tests/unit/conftest.py
 tests/unit/test_classification_name.py
 tests/unit/test_client.py
 tests/unit/test_custom_metadata.py
 tests/unit/test_glossary_term.py
 tests/unit/test_lineage.py
 tests/unit/test_model.py
 tests/unit/test_search_model.py
 tests/unit/test_typedef_model.py
-tests/unit/test_utils.py
+tests/unit/test_utils.py
+tests/unit/model/__init__.py
+tests/unit/model/badge_condition_test.py
+tests/unit/model/badge_test.py
+tests/unit/model/column_test.py
+tests/unit/model/connection_test.py
+tests/unit/model/constants.py
+tests/unit/model/database_test.py
+tests/unit/model/glossary_category_test.py
+tests/unit/model/glossary_term_test.py
+tests/unit/model/glossary_test.py
+tests/unit/model/materialised_view_test.py
+tests/unit/model/process_test.py
+tests/unit/model/readme_test.py
+tests/unit/model/s3_bucket_test.py
+tests/unit/model/s3object_test.py
+tests/unit/model/schema_test.py
+tests/unit/model/table_test.py
+tests/unit/model/view_test.py
```

### Comparing `pyatlan-0.1.2/setup.py` & `pyatlan-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/admin_test.py` & `pyatlan-0.1.3/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/classification_test.py` & `pyatlan-0.1.3/tests/integration/classification_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/client.py` & `pyatlan-0.1.3/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/connection_test.py` & `pyatlan-0.1.3/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/custom_metadata_test.py` & `pyatlan-0.1.3/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/glossary_test.py` & `pyatlan-0.1.3/tests/integration/glossary_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -110,7 +110,28 @@
     assert isinstance(g, AtlasGlossary)
     assert g.guid == glossary.guid
     assert g.qualified_name == glossary.qualified_name
     assert g.name == glossary.name
     terms = g.terms
     assert terms
     assert len(terms) == 2
+
+
+@pytest.mark.order(after="test_read_glossary")
+def test_trim_to_required_glossary(
+    client: AtlanClient,
+    glossary: AtlasGlossary,
+):
+    glossary = glossary.trim_to_required()
+    response = client.upsert(glossary)
+    assert response.mutated_entities is None
+
+
+@pytest.mark.order(after="test_term1")
+def test_term_trim_to_required(
+    client: AtlanClient,
+    term1: AtlasGlossaryTerm,
+):
+    term1 = client.get_asset_by_guid(guid=term1.guid, asset_type=AtlasGlossaryTerm)
+    term1 = term1.trim_to_required()
+    response = client.upsert(term1)
+    assert response.mutated_entities is None
```

### Comparing `pyatlan-0.1.2/tests/integration/lineage_test.py` & `pyatlan-0.1.3/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/query_parser_test.py` & `pyatlan-0.1.3/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/s3_asset_test.py` & `pyatlan-0.1.3/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/test_client.py` & `pyatlan-0.1.3/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/test_index_search.py` & `pyatlan-0.1.3/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/integration/test_sql_assets.py` & `pyatlan-0.1.3/tests/integration/test_sql_assets.py`

 * *Files 14% similar despite different names*

```diff
@@ -99,14 +99,23 @@
             qualified_name=TestConnection.connection.qualified_name,
             name=TestConnection.connection.name,
         )
         connection.description = description
         response = upsert(connection)
         verify_asset_updated(response, Connection)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestConnection.connection
+        connection = TestConnection.connection.trim_to_required()
+        response = upsert(connection)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestConnection")
 class TestDatabase:
     database: Optional[Database] = None
 
     def test_create(
         self,
@@ -140,14 +149,23 @@
             name=TestDatabase.database.name,
         )
         description = f"{TestDatabase.database.description} more stuff"
         database.description = description
         response = upsert(database)
         verify_asset_updated(response, Database)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestDatabase.database
+        database = TestDatabase.database.trim_to_required()
+        response = upsert(database)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestDatabase")
 class TestSchema:
     schema: Optional[Schema] = None
 
     def test_create(
         self,
@@ -183,14 +201,23 @@
         schema = Schema.create_for_modification(
             qualified_name=schema.qualified_name, name=schema.name
         )
         schema.description = description
         response = upsert(schema)
         verify_asset_updated(response, Schema)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestSchema.schema
+        schema = TestSchema.schema.trim_to_required()
+        response = upsert(schema)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestSchema")
 class TestTable:
     table: Optional[Table] = None
 
     def test_create(
         self,
@@ -226,14 +253,23 @@
         table = Table.create_for_modification(
             qualified_name=table.qualified_name, name=table.name
         )
         table.description = description
         response = upsert(table)
         verify_asset_updated(response, Table)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestTable.table
+        table = TestTable.table.trim_to_required()
+        response = upsert(table)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestTable")
 class TestView:
     view: Optional[View] = None
 
     def test_create(
         self,
@@ -265,14 +301,23 @@
         view = View.create_for_modification(
             qualified_name=view.qualified_name, name=view.name
         )
         view.description = description
         response = upsert(view)
         verify_asset_updated(response, View)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestView.view
+        view = TestView.view.trim_to_required()
+        response = upsert(view)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestView")
 class TestColumn:
     column: Optional[Column] = None
 
     def test_create(
         self,
@@ -308,14 +353,23 @@
         column = Column.create_for_modification(
             qualified_name=column.qualified_name, name=column.name
         )
         column.description = description
         response = upsert(column)
         verify_asset_updated(response, Column)
 
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestColumn.column
+        column = TestColumn.column.trim_to_required()
+        response = upsert(column)
+        assert response.mutated_entities is None
+
 
 @pytest.mark.order(after="TestColumn")
 class TestReadme:
     readme: Optional[Readme] = None
 
     def test_create(
         self,
@@ -341,7 +395,17 @@
         description = f"{readme.description} more stuff"
         readme = Readme.create_for_modification(
             qualified_name=readme.qualified_name, name=readme.name
         )
         readme.description = description
         response = upsert(readme)
         verify_asset_updated(response, Readme)
+
+    @pytest.mark.order(after="test_create")
+    def test_trim_to_required(
+        self, client: AtlanClient, upsert: Callable[[Asset], AssetMutationResponse]
+    ):
+        assert TestReadme.readme
+        readme = TestReadme.readme
+        readme = readme.trim_to_required()
+        response = upsert(readme)
+        assert response.mutated_entities is None
```

### Comparing `pyatlan-0.1.2/tests/unit/test_classification_name.py` & `pyatlan-0.1.3/tests/unit/test_classification_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_client.py` & `pyatlan-0.1.3/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_custom_metadata.py` & `pyatlan-0.1.3/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_glossary_term.py` & `pyatlan-0.1.3/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_lineage.py` & `pyatlan-0.1.3/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_search_model.py` & `pyatlan-0.1.3/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.1.2/tests/unit/test_typedef_model.py` & `pyatlan-0.1.3/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

