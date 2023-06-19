# Comparing `tmp/duqtools-1.8.0.tar.gz` & `tmp/duqtools-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duqtools-1.8.0.tar", last modified: Tue May  9 08:25:41 2023, max compression
+gzip compressed data, was "duqtools-1.9.0.tar", last modified: Mon Jun 19 12:44:00 2023, max compression
```

## Comparing `duqtools-1.8.0.tar` & `duqtools-1.9.0.tar`

### file list

```diff
@@ -1,101 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 08:25:33.000000 duqtools-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 08:25:33.000000 duqtools-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-09 08:25:41.388682 duqtools-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 08:25:33.000000 duqtools-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-09 08:25:33.000000 duqtools-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-09 08:25:41.392682 duqtools-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:25:33.000000 duqtools-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.376681 duqtools-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_click_opt_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/apply_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools/config/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/config/_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/dash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/dash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/data/dash/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/pages/1_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/dash/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/duqtools.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/jetto_tools_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_core-profiles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_core-sources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_equilibrium.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/data/variables_ids2jetto.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/duqmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/ids/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_apply_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_imas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/ids/_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/jetto/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_batchfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_jettovar_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/jetto/_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.384682 duqtools-1.8.0/src/duqtools/large_scale_validation/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/large_scale_validation/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/list_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/matrix_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/src/duqtools/models/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/models/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.388682 duqtools-1.8.0/src/duqtools/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_description_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_imas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_jetto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/matrix_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/schema/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-09 08:25:33.000000 duqtools-1.8.0/src/duqtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:25:41.380682 duqtools-1.8.0/src/duqtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:25:40.000000 duqtools-1.8.0/src/duqtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 08:25:41.000000 duqtools-1.8.0/src/duqtools.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.260220 duqtools-1.9.0/
+-rw-r--r--   0 stef      (1000) stef      (1000)    11357 2023-06-19 08:09:55.000000 duqtools-1.9.0/LICENSE
+-rw-r--r--   0 stef      (1000) stef      (1000)       86 2023-06-19 08:09:55.000000 duqtools-1.9.0/MANIFEST.in
+-rw-r--r--   0 stef      (1000) stef      (1000)     3196 2023-06-19 12:44:00.260220 duqtools-1.9.0/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)     1908 2023-06-19 08:09:55.000000 duqtools-1.9.0/README.md
+-rw-r--r--   0 stef      (1000) stef      (1000)     5148 2023-06-19 12:43:12.000000 duqtools-1.9.0/pyproject.toml
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-19 12:44:00.260220 duqtools-1.9.0/setup.cfg
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.248220 duqtools-1.9.0/src/
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.252220 duqtools-1.9.0/src/duqtools/
+-rw-r--r--   0 stef      (1000) stef      (1000)      677 2023-06-19 12:43:12.000000 duqtools-1.9.0/src/duqtools/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1588 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/_click_opt_groups.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1808 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/_logging_utils.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     6458 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/_plot_utils.py
+-rw-r--r--   0 stef      (1000) stef      (1000)       87 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/_types.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1581 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/api.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1173 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/apply_model.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2187 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/cleanup.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    15621 2023-06-19 12:43:12.000000 duqtools-1.9.0/src/duqtools/cli.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.253220 duqtools-1.9.0/src/duqtools/config/
+-rw-r--r--   0 stef      (1000) stef      (1000)      190 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/config/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1659 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/config/_config.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     5475 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/config/_variables.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    11065 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/create.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      791 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/dash.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.253220 duqtools-1.9.0/src/duqtools/dashboard/
+-rw-r--r--   0 stef      (1000) stef      (1000)     2274 2023-06-19 09:19:58.000000 duqtools-1.9.0/src/duqtools/dashboard/Plotting.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3176 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/dashboard/_shared.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.253220 duqtools-1.9.0/src/duqtools/dashboard/pages/
+-rw-r--r--   0 stef      (1000) stef      (1000)     3786 2023-06-19 09:19:58.000000 duqtools-1.9.0/src/duqtools/dashboard/pages/1_Merging.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      149 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/dashboard/readme.md
+-rw-r--r--   0 stef      (1000) stef      (1000)       41 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/dashboard/requirements.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.254220 duqtools-1.9.0/src/duqtools/data/
+-rw-r--r--   0 stef      (1000) stef      (1000)      513 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/duqtools.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)     1687 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/jetto_tools_lookup.json
+-rw-r--r--   0 stef      (1000) stef      (1000)      579 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/variables.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)     2748 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/variables_core-profiles.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)     1309 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/variables_core-sources.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)     3157 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/variables_equilibrium.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)      703 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/data/variables_ids2jetto.yaml
+-rw-r--r--   0 stef      (1000) stef      (1000)     2974 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/duqmap.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.254220 duqtools-1.9.0/src/duqtools/ets/
+-rw-r--r--   0 stef      (1000) stef      (1000)      130 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ets/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     6424 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ets/_system.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.255220 duqtools-1.9.0/src/duqtools/ids/
+-rw-r--r--   0 stef      (1000) stef      (1000)      624 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2971 2023-06-19 12:43:12.000000 duqtools-1.9.0/src/duqtools/ids/_apply_model.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     4145 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_copy.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    10579 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_handle.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1459 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_imas.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    11418 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_mapping.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2902 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_merge.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     6428 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/ids/_rebase.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1278 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/init.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.256220 duqtools-1.9.0/src/duqtools/jetto/
+-rw-r--r--   0 stef      (1000) stef      (1000)      401 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/jetto/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3188 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/jetto/_batchfile.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1189 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/jetto/_jettovar_to_json.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    14281 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/jetto/_system.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.257220 duqtools-1.9.0/src/duqtools/large_scale_validation/
+-rw-r--r--   0 stef      (1000) stef      (1000)      100 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     4789 2023-06-19 12:43:12.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/cli.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1300 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/create.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1953 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/merge.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      492 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/setup.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1515 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/status.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2589 2023-06-19 09:19:15.000000 duqtools-1.9.0/src/duqtools/large_scale_validation/submit.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1503 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/list_variables.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3336 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/matrix_samplers.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2836 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/merge.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.257220 duqtools-1.9.0/src/duqtools/models/
+-rw-r--r--   0 stef      (1000) stef      (1000)      236 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/models/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     5034 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/models/_job.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1246 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/models/_locations.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1587 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/models/_run.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     4298 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/models/_system.py
+-rw-r--r--   0 stef      (1000) stef      (1000)    11579 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/operations.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2165 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/plot.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.259220 duqtools-1.9.0/src/duqtools/schema/
+-rw-r--r--   0 stef      (1000) stef      (1000)      919 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      244 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_basemodel.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      144 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_description_helpers.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     7689 2023-06-19 12:43:12.000000 duqtools-1.9.0/src/duqtools/schema/_dimensions.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      869 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_imas.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1445 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_jetto.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1325 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_ranges.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     5210 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_systems.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3200 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/_variable.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     5010 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/cli.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1631 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/data_location.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1007 2023-06-19 09:19:58.000000 duqtools-1.9.0/src/duqtools/schema/matrix_samplers.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      574 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/schema/variables.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     7146 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/setup.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     6706 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/status.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     7581 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/submit.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     1626 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/system.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3966 2023-06-19 08:09:55.000000 duqtools-1.9.0/src/duqtools/utils.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.252220 duqtools-1.9.0/src/duqtools.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)     3196 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)     2924 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)      107 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/entry_points.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-19 08:14:56.000000 duqtools-1.9.0/src/duqtools.egg-info/not-zip-safe
+-rw-r--r--   0 stef      (1000) stef      (1000)      515 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/requires.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        9 2023-06-19 12:44:00.000000 duqtools-1.9.0/src/duqtools.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-19 12:44:00.260220 duqtools-1.9.0/tests/
+-rw-r--r--   0 stef      (1000) stef      (1000)     3742 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_api.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      542 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_cmdline.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      731 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_duqmap.py
+-rw-r--r--   0 stef      (1000) stef      (1000)       71 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_duqtools.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2307 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_ids2jetto_variables.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     3023 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_operations.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      932 2023-06-19 08:09:55.000000 duqtools-1.9.0/tests/test_samplers.py
```

### Comparing `duqtools-1.8.0/LICENSE` & `duqtools-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/PKG-INFO` & `duqtools-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: duqtools
-Version: 1.8.0
+Version: 1.9.0
 Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
-Home-page: https://github.com/duqtools/duqtools
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
-Project-URL: Documentation, https://duqtools.readthedocs.io
+Author: Victor Azizi, Aaron Ho
+Author-email: Stef Smeets <s.smeets@esciencecenter.nl>
+License: Apache 2.0 License
+Project-URL: homepage, https://github.com/duqtools/duqtools
+Project-URL: issues, https://github.com/duqtools/duqtools/issues
+Project-URL: documentation, https://duqtools.readthedocs.io
+Project-URL: changelog, https://github.com/duqtools/duqtools/releases
 Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: docs
 Provides-Extra: publishing
 Provides-Extra: imas
 License-File: LICENSE
 
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest)
+[![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/)
+[![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/)
+[![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json)
+
+
+![Duqtools banner](https://raw.githubusercontent.com/duqtools/duqtools/main/src/duqtools/data/logo.png)
 
 # Duqtools
 
 *Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
 
 Features:
 
@@ -61,9 +64,7 @@
 
 Suggestions, improvements, and edits are most welcome.
 
 
 ## Development
 
 Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
-
-
```

### Comparing `duqtools-1.8.0/README.md` & `duqtools-1.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest)
+[![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/)
+[![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/)
+[![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json)
+
+
+![Duqtools banner](https://raw.githubusercontent.com/duqtools/duqtools/main/src/duqtools/data/logo.png)
 
 # Duqtools
 
 *Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
 
 Features:
```

### Comparing `duqtools-1.8.0/src/duqtools/__init__.py` & `duqtools-1.9.0/src/duqtools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     import pkg_resources  # noqa
 
 
 fix_dependencies()
 
 __author__ = 'Stef Smeets'
 __email__ = 's.smeets@esciencecenter.nl'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 import logging  # noqa
 import warnings  # noqa
 
 # https://github.com/duqtools/duqtools/issues/264
 warnings.filterwarnings(
     'ignore',
```

### Comparing `duqtools-1.8.0/src/duqtools/_click_opt_groups.py` & `duqtools-1.9.0/src/duqtools/_click_opt_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class GroupCmd(click.Command):
 
     def format_options(self, ctx, formatter):
         """Writes all the options into the formatter if they exist.
 
         Implementation based on:
-            https://github.com/pallets/click/issues/373#issuecomment-515293746
+        https://github.com/pallets/click/issues/373#issuecomment-515293746
         """
         sections = defaultdict(list)
 
         for param in self.get_params(ctx):
             option = param.get_help_record(ctx)
             if option:
                 try:
```

### Comparing `duqtools-1.8.0/src/duqtools/_logging_utils.py` & `duqtools-1.9.0/src/duqtools/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/_plot_utils.py` & `duqtools-1.9.0/src/duqtools/_plot_utils.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/apply_model.py` & `duqtools-1.9.0/src/duqtools/apply_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from collections import abc
 from functools import singledispatch
 from pathlib import Path
 
+from .jetto import BaseJettoSystem
 from .schema import BaseModel, JettoOperation
 
 
 @singledispatch
 def apply_model(model: BaseModel, **kwargs):
     """Apply operation in model to target. Data are modified in-place.
 
@@ -30,12 +31,16 @@
         apply_model(submodel, **kwargs)
 
 
 from .ids._apply_model import _apply_ids  # noqa: E402, F401
 
 
 @apply_model.register
-def _apply_jetto(model: JettoOperation, run_dir: Path, **kwargs):
-    from .system import get_system
-    system = get_system()
+def _apply_jetto(model: JettoOperation, run_dir: Path, system: BaseJettoSystem,
+                 **kwargs):
     system.set_jetto_variable(run_dir, model.variable.name, model.value,
                               model.variable.lookup)
+
+
+#@apply_model.register
+#def _apply_ets6(model: JettoOperation, run_dir: Path, **kwargs):
+#    pass
```

### Comparing `duqtools-1.8.0/src/duqtools/cleanup.py` & `duqtools-1.9.0/src/duqtools/cleanup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 from pathlib import Path
 
+from .config import Config
 from .ids import ImasHandle
 from .models import Locations, Run
 from .operations import op_queue
 
 logger = logging.getLogger(__name__)
 
 
@@ -27,29 +28,35 @@
             action=shutil.rmtree,
             args=(model.dirname, ),
             description='Removing run dir',
             extra_description=f'{model.dirname}',
         )
 
 
-def cleanup(out, force, **kwargs):
+def cleanup(*, cfg: Config, out: bool, force: bool, **kwargs):
     """Read runs.yaml and clean the current directory.
 
     Parameters
     ----------
+    cfg : Config
+        Duqtools config.
     out : bool
         Remove output IDS.
+    force : bool
+        Force overwriting of old files.
     """
+    locations = Locations(cfg=cfg)
+
     try:
-        runs = Locations().runs
+        runs = locations.runs
     except OSError:
-        runs = ()
+        runs = []
     else:
-        if Locations().runs_yaml.exists() and not force:
-            if Locations().runs_yaml_old.exists():
+        if locations.runs_yaml.exists() and not force:
+            if locations.runs_yaml_old.exists():
                 raise OSError(
                     '`runs.yaml.old` exists, use --force to overwrite anyway')
 
     for run in runs:
         data_in = ImasHandle.parse_obj(run.data_in)
         data_out = ImasHandle.parse_obj(run.data_out)
 
@@ -61,17 +68,17 @@
             op_queue.add_no_op(description='NOT Removing',
                                extra_description=f'{data_out}')
 
         remove_run(run)
 
     op_queue.add(
         action=shutil.move,
-        args=(Locations().runs_yaml, Locations().runs_yaml_old),
+        args=(locations.runs_yaml, locations.runs_yaml_old),
         description='Moving runs.yaml',
-        extra_description=f'{Locations().runs_yaml_old}',
+        extra_description=f'{locations.runs_yaml_old}',
     )
 
     op_queue.add(
         action=remove_files,
         args=(
             'duqtools_slurm_array.err',
             'duqtools_slurm_array.out',
```

### Comparing `duqtools-1.8.0/src/duqtools/cli.py` & `duqtools-1.9.0/src/duqtools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,17 +278,17 @@
               help='Overwrite existing run directories and IDS data.')
 @click.option('--no-sampling',
               is_flag=True,
               help='Create base run (ignores `dimensions`/`sampler`).')
 @common_options(*all_options)
 def cli_create(**kwargs):
     """Create the UQ run files."""
-    from .create import create_entry
+    from .create import create
     with op_queue_context():
-        create_entry(**kwargs)
+        create(cfg=CFG, **kwargs)
 
 
 @cli.command('recreate', cls=GroupCmd)
 @click.argument('runs', type=Path, nargs=-1)
 @common_options(*all_options)
 def cli_recreate(**kwargs):
     """Read `runs.yaml` and re-create the given runs.
@@ -296,37 +296,46 @@
     \b
     Example:
 
     - `duqtools recreate run_0003 run_0004 --force`
     """
     from .create import recreate
     with op_queue_context():
-        recreate(**kwargs)
+        recreate(cfg=CFG, **kwargs)
 
 
 @cli.command('submit', cls=GroupCmd)
 @click.option('--force',
               is_flag=True,
               help='Re-submit running or completed jobs.')
 @click.option(
     '--schedule',
     is_flag=True,
-    help='Schedule and submit jobs automatically. `max_jobs` must be defined.')
-@click.option(
-    '-j',
-    '--max_jobs',
-    type=int,
-    help=
-    'Maximum number of jobs to submit (simultaneously for array submission).')
+    help=(
+        'Schedule and submit jobs automatically.'
+        '`max_jobs` defines the total number of jobs running simultaneiously.'
+    ))
+@click.option('-j',
+              '--max_jobs',
+              type=int,
+              help='Maximum number of running jobs.',
+              default=10)
 @click.option(
     '--max_array_size',
     type=int,
     default=100,
     help='Maximum array size for slurm (usually 1001, default = 100).')
-@click.option('-a', '--array', is_flag=True, help='Submit jobs as array.')
+@click.option(
+    '-a',
+    '--array',
+    is_flag=True,
+    help=(
+        'Submit jobs as array. '
+        '`max_jobs` defines the total number of jobs running simultaneiously.'
+    ))
 @click.option('-r',
               '--resubmit',
               multiple=True,
               default=tuple(),
               type=Path,
               help='Case to re-submit, can be specified multiple times')
 @click.option('-s',
@@ -335,34 +344,36 @@
               type=str,
               multiple=True,
               help='Only submit jobs with this status.')
 @common_options(*all_options)
 def cli_submit(**kwargs):
     """Submit the UQ runs.
 
-    This subcommand will read `runs.yaml`, and start all runs which are not yet
-    running. By default, It will not re-submit running or finished jobs.
-
-    There is a scheduler that will continue to submit jobs until the specified
-    maximum number of jobs is running. Once a job has completed, a new job will
-    be submitted from the queue to fill the spot.
+    This subcommand will read `runs.yaml`, and start all runs which are
+    not yet running. By default, It will not re-submit running or
+    finished jobs.
+
+    There is a scheduler that will continue to submit jobs until the
+    specified maximum number of jobs is running. Once a job has
+    completed, a new job will be submitted from the queue to fill the
+    spot.
     """
     from .submit import submit
     with op_queue_context():
-        submit(**kwargs)
+        submit(cfg=CFG, **kwargs)
 
 
 @cli.command('status', cls=GroupCmd)
 @click.option('--detailed', is_flag=True, help='Detailed info on progress')
 @click.option('--progress', is_flag=True, help='Fancy progress bar')
 @common_options(*all_options)
 def cli_status(**kwargs):
     """Print the status of the UQ runs."""
     from .status import status
-    status(**kwargs)
+    status(cfg=CFG, **kwargs)
 
 
 @cli.command('plot')
 @handles_option
 @variables_option
 @click.option('-o',
               '--format',
@@ -399,15 +410,15 @@
               is_flag=True,
               help='Overwrite backup file if necessary.')
 @common_options(*all_options)
 def cli_clean(**kwargs):
     """Delete generated IDS data and the run dir."""
     from .cleanup import cleanup
     with op_queue_context():
-        cleanup(**kwargs)
+        cleanup(cfg=CFG, **kwargs)
 
 
 @cli.command('go', cls=GroupCmd)
 @click.option('--force', is_flag=True, help='Overwrite files when necessary.')
 @common_options(*all_options)
 def cli_go(**kwargs):
     """Run create, submit, status, dash in succession.
@@ -415,26 +426,27 @@
     Useful for existing tested and working pipelines.
     """
     from .create import create
     from .dash import dash
     from .status import status
     from .submit import submit
     with op_queue_context():
-        create(**kwargs)
+        create(cfg=CFG, **kwargs)
     with op_queue_context():
-        submit(max_jobs=None,
+        submit(cfg=CFG,
+               max_jobs=None,
                array=True,
                schedule=None,
                resubmit=tuple(),
                **kwargs)
 
     skwargs = kwargs.copy()
     skwargs['detailed'] = True
     skwargs['progress'] = False
-    status(**skwargs)
+    status(cfg=CFG, **skwargs)
 
     dash(**kwargs)
 
 
 @cli.command('yolo')
 @click.pass_context
 def cli_yolo(ctx, **kwargs):
@@ -501,22 +513,27 @@
     from .merge import merge
     with op_queue_context():
         merge(**kwargs)
 
 
 @cli.command('list-variables')
 @config_option
-def cli_list_variables(**kwargs):
+def cli_list_variables(config, **kwargs):
     """List available variables.
 
     Picks up variables from `duqtools.yaml` if it exists in the local
     directory.
     """
     from .list_variables import list_variables
-    list_variables(**kwargs)
+    try:
+        cfg = load_config(config)
+    except FileNotFoundError:
+        print(f'Cannot find `{config}`.')
+        cfg = CFG
+    list_variables(cfg=cfg, **kwargs)
 
 
 @cli.command('version')
 def cli_version(**kwargs):
     """Print the version and exit."""
     import git
```

### Comparing `duqtools-1.8.0/src/duqtools/config/_config.py` & `duqtools-1.9.0/src/duqtools/config/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Config class containing all configs, can be used with:
 
-    from duqtools.config import CFG
-    CFG.<variable you want>
+```
+from duqtools.config import CFG
+CFG.<variable you want>
+```
 
 To update the config:
 
-    load_config('duqtools.yaml')
+```
+load_config('duqtools.yaml')
+```
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Union
```

### Comparing `duqtools-1.8.0/src/duqtools/config/_variables.py` & `duqtools-1.9.0/src/duqtools/config/_variables.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/create.py` & `duqtools-1.9.0/src/duqtools/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,26 @@
 
 
 class CreateManager:
     """Docstring for CreateManager."""
 
     def __init__(self, cfg: Config):
         self.cfg = cfg
-
         if not self.cfg.create:
             logger.warning('No create options specified.')
             raise CreateError('No create options specified in config.')
 
         self.options = self.cfg.create
 
         self.template_drc = self.options.template
-        self.system = get_system()
+        self.system = get_system(cfg=cfg)
         self.runs_dir = self.system.get_runs_dir()
         self.source = self._get_source_handle()
 
-        locations = Locations()
+        locations = Locations(cfg=cfg)
         self.runs_yaml = locations.runs_yaml
         self.data_csv = locations.data_csv
 
     def _get_source_handle(self) -> ImasHandle:
         if not self.options.template_data:
             source = self.system.imas_from_path(self.template_drc)
         else:
@@ -157,15 +156,18 @@
                          extra_description='Some targets already exist, '
                          'use --force to override')
 
     @add_to_op_queue('Setting inital condition of', '{data_in}', quiet=True)
     def apply_operations(self, data_in: ImasHandle, run_dir: Path,
                          operations: list[Any]):
         for model in operations:
-            apply_model(model, run_dir=run_dir, ids_mapping=data_in)
+            apply_model(model,
+                        run_dir=run_dir,
+                        ids_mapping=data_in,
+                        system=self.system)
 
     @add_to_op_queue('Writing runs', '{self.runs_yaml}', quiet=True)
     def write_runs_file(self, runs: Sequence[Run]) -> None:
         runs = Runs.parse_obj(runs)
 
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
@@ -219,25 +221,26 @@
                      kwargs={
                          'parents': True,
                          'exist_ok': force
                      },
                      description='Creating run',
                      extra_description=f'{model.dirname}')
 
-        self.source.copy_data_to(model.data_in)
+        self.source.copy_data_to(ImasHandle.parse_obj(model.data_in))
 
         self.system.copy_from_template(self.template_drc, model.dirname)
 
         self.apply_operations(model.data_in, model.dirname, model.operations)
 
-        self.system.write_batchfile(model.dirname, self.cfg)
+        self.system.write_batchfile(model.dirname)
 
         self.system.update_imas_locations(run=model.dirname,
                                           inp=model.data_in,
-                                          out=model.data_out)
+                                          out=model.data_out,
+                                          cfg_filename=self.template_drc.name)
 
 
 def create(*,
            cfg: Config,
            force: bool = False,
            no_sampling: bool = False,
            absolute_dirpath: bool = False,
@@ -283,50 +286,43 @@
     create_mgr.write_runs_file(runs)
     create_mgr.write_runs_csv(runs)
     create_mgr.copy_config()
 
     return runs
 
 
-def create_entry(*args, **kwargs):
-    """Entry point for duqtools cli."""
-    from .config import CFG
-    create(cfg=CFG, *args, **kwargs)
-
-
-def create_api(config: dict, **kwargs) -> tuple[Job, Run]:
+def create_api(config: dict, **kwargs) -> dict[str, tuple[Job, Run]]:
     """Wrapper around create for python api."""
     cfg = Config.from_dict(config)
     runs = create(cfg=cfg, **kwargs)
 
     if len(runs) == 0:
         raise CreateError('No runs were created, check logs for errors.')
-    elif len(runs) > 1:
-        raise NotImplementedError('Multiple runs in single call not supported')
-
-    run = runs[0]
-    job = Job(run.dirname, cfg=cfg)
 
-    return job, run
+    return {
+        str(run.shortname): (Job(run.dirname, cfg=cfg), run)
+        for run in runs
+    }
 
 
-def recreate(*, runs: Sequence[Path], **kwargs):
+def recreate(*, cfg: Config, runs: Sequence[Path], **kwargs):
     """Create input for jetto and IDS data structures.
 
     Parameters
     ----------
+    cfg : Config
+        Duqtools config.
     runs : Sequence[Path]
         Run names to recreate.
     **kwargs
         Unused.
     """
-    from .config import CFG
-    create_mgr = CreateManager(CFG)
+    create_mgr = CreateManager(cfg)
 
-    run_dict = {run.shortname: run for run in Locations().runs}
+    run_dict = {run.shortname: run for run in Locations(cfg=cfg).runs}
 
     run_models = []
     for run in runs:
         if run not in run_dict:
             raise ValueError(f'`{run}` not in `runs.yaml`.')
 
         model = run_dict[run]
@@ -336,7 +332,24 @@
         model.data_in.delete()
         remove_run(model)
 
         run_models.append(model)
 
     for model in run_models:
         create_mgr.create_run(model)
+
+    return run_models
+
+
+def recreate_api(config: dict, runs: Sequence[Path],
+                 **kwargs) -> dict[str, tuple[Job, Run]]:
+    """Wrapper around create for python api."""
+    cfg = Config.from_dict(config)
+    runs = recreate(cfg=cfg, runs=runs, **kwargs)
+
+    if len(runs) == 0:
+        raise CreateError('No runs were recreated, check logs for errors.')
+
+    return {
+        str(run.shortname): (Job(run.dirname, cfg=cfg), run)
+        for run in runs
+    }
```

### Comparing `duqtools-1.8.0/src/duqtools/data/dash/dash.py` & `duqtools-1.9.0/src/duqtools/dashboard/Plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from pathlib import Path
 
 import pandas as pd
 import streamlit as st
-from _shared import default_workdir, get_dataset
+from _shared import add_sidebar_logo, default_workdir, get_dataset
 
 from duqtools._plot_utils import alt_errorband_chart, alt_line_chart
 from duqtools.config import var_lookup
 from duqtools.utils import read_imas_handles_from_file
 
+add_sidebar_logo()
+
 st.title('Plot IDS')
 
 with st.sidebar:
     st.header('Input data')
     work_dir = st.text_input('Work directory', default_workdir)
     data_file = st.text_input('Data file', 'data.csv')
```

### Comparing `duqtools-1.8.0/src/duqtools/data/dash/pages/1_merge.py` & `duqtools-1.9.0/src/duqtools/dashboard/pages/1_Merging.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 from duqtools.config import var_lookup
 from duqtools.ids import ImasHandle, merge_data
 from duqtools.utils import read_imas_handles_from_file
 
 sys.path.insert(0, str(Path(__file__).parent))
 
-from _shared import get_var_options  # noqa
+from _shared import get_var_options, add_sidebar_logo  # noqa
 from _shared import default_workdir, get_ids_options, get_variables  # noqa
 
+add_sidebar_logo()
+
 st.markdown('# Merge IMAS data')
 
 with st.sidebar:
     st.header('Input data')
     work_dir = st.text_input('Work directory', default_workdir)
     data_file = st.text_input('Data file', 'data.csv')
```

### Comparing `duqtools-1.8.0/src/duqtools/data/duqtools.yaml` & `duqtools-1.9.0/src/duqtools/data/duqtools.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Check out the documentation for more info:
 # https://duqtools.readthedocs.io/en/latest/config/
 tag: duqtools
-system: jetto
 create:
   runs_dir: ./runs_dir # change to output directory
   template: ./template # change to directory with template
   dimensions:
   - variable: t_e
     operator: multiply
     values: [0.9, 1.0, 1.1]
@@ -13,10 +12,9 @@
   - variable: zeff
     operator: multiply
     values: [0.9, 1.0, 1.1]
     scale_to_error: false
   sampler:
     method: latin-hypercube
     n_samples: 3
-submit:
-  submit_command: sbatch
-  submit_script_name: .llcmd
+system:
+  name: jetto
```

### Comparing `duqtools-1.8.0/src/duqtools/data/jetto_tools_lookup.json` & `duqtools-1.9.0/src/duqtools/data/jetto_tools_lookup.json`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/data/variables.yaml` & `duqtools-1.9.0/src/duqtools/data/variables.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/data/variables_core-profiles.yaml` & `duqtools-1.9.0/src/duqtools/data/variables_core-profiles.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/data/variables_core-sources.yaml` & `duqtools-1.9.0/src/duqtools/data/variables_core-sources.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/data/variables_equilibrium.yaml` & `duqtools-1.9.0/src/duqtools/data/variables_equilibrium.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/data/variables_ids2jetto.yaml` & `duqtools-1.9.0/src/duqtools/data/variables_ids2jetto.yaml`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/duqmap.py` & `duqtools-1.9.0/src/duqtools/duqmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,25 +28,26 @@
 
 
 def duqmap_run(function: Callable[[Run], Any], **kwargs) -> List[Any]:
     return _duqmap(function, lambda x: x, **kwargs)  # Identity
 
 
 def duqmap_imas(function: Callable[[ImasHandle], Any], **kwargs) -> List[Any]:
+
     def to_imas_handle(run):
         return run.to_imas_handle()
 
     return _duqmap(function, to_imas_handle, **kwargs)
 
 
 def duqmap(function: Callable[[Run | ImasHandle], Any],
            *,
            runs: Optional[List[Run | Path]] = None,
            **kwargs) -> List[Any]:
-    """duqmap is a mapping function which can be used to map a user defined
+    """Duqmap is a mapping function which can be used to map a user defined
     function `function` over either the runs created by duqtools, or the runs
     specified by the user in `runs`.
 
     An important gotcha is that when `Paths` are used to define the runs, duqtools
     does not know how to associate the corresponding ImasHandles, as that information
     is not available.  So when using it in this way, it is not possible to provide a
     function which takes an `ImasHandle` as input.
```

### Comparing `duqtools-1.8.0/src/duqtools/ids/__init__.py` & `duqtools-1.9.0/src/duqtools/ids/__init__.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/ids/_apply_model.py` & `duqtools-1.9.0/src/duqtools/ids/_apply_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 import logging
+from functools import partial
 from typing import Union
 
 import numpy as np
 
 from .._logging_utils import duqlog_screen
 from ..apply_model import apply_model
 from ..schema import IDSOperation
 from ._handle import ImasHandle
 from ._mapping import IDSMapping
 
 logger = logging.getLogger(__name__)
 
 
+def _custom_function(data: np.ndarray, value, *, out: np.ndarray, code: str):
+    """Mimick np.ufunc for custom functions."""
+    out[:] = eval(code)
+
+
 @apply_model.register  # type: ignore
 def _apply_ids(model: IDSOperation, *,
                ids_mapping: Union[ImasHandle, IDSMapping], **kwargs) -> None:
     """Implementation for IDS operations.
 
     Parameters
     ----------
@@ -34,15 +40,18 @@
     if isinstance(ids_mapping, ImasHandle):
         target_in = ids_mapping
         ids_mapping = ids_mapping.get(model.variable.ids)
 
     if isinstance(model.variable, str):
         raise TypeError('`model.variable` must have a `path` attribute.')
 
-    npfunc = getattr(np, model.operator)
+    if model.operator == 'custom':
+        npfunc = partial(_custom_function, code=model.custom_code)
+    else:
+        npfunc = getattr(np, model.operator)
 
     data_map = ids_mapping.findall(model.variable.path)
 
     if len(data_map) == 0:
         # TODO this should be 'raise Error' but that breaks our tests,
         # leave it as a message until we can fix it with a Jetto-IMAS container
         duqlog_screen.error(
@@ -67,14 +76,23 @@
             value = sigma * model.value
         else:
 
             value = model.value
 
         logger.info('Apply %s', model)
 
+        if model.linear_ramp is not None:
+            a, b = model.linear_ramp
+            value = np.linspace(a, b, len(data)) * value
+
         logger.debug('data range before: %s - %s', data.min(), data.max())
+
         npfunc(data, value, out=data)
+
+        if model.clip_max is not None or model.clip_min is not None:
+            np.clip(data, a_min=model.clip_min, a_max=model.clip_max, out=data)
+
         logger.debug('data range after: %s - %s', data.min(), data.max())
 
     if target_in:
         logger.info('Writing data entry: %s', target_in)
         ids_mapping.sync(target_in)
```

### Comparing `duqtools-1.8.0/src/duqtools/ids/_copy.py` & `duqtools-1.9.0/src/duqtools/ids/_copy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 import logging
+import os
+import shutil
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from packaging import version
 
 from .._logging_utils import LoggingContext
 from ..operations import add_to_op_queue
@@ -13,20 +15,25 @@
 if TYPE_CHECKING:
     from .ids import ImasHandle
 
 
 def get_imas_ual_version():
     """Get imas/ual versions.
 
-    Parsed from a string like: `imas_3_34_0_ual_4_9_3`
+    Parsed from a string like:
+    - `imas_3_34_0_ual_4_9_3`
+    - `imas_3_38_0_dev1_ual_4_11_0`
     """
     vsplit = imas.names[0].split('_')
 
-    imas_version = version.parse('.'.join(vsplit[1:4]))
-    ual_version = version.parse('.'.join(vsplit[5:8]))
+    ual_start = vsplit.index('ual')
+    imas_start = vsplit.index('imas')
+
+    imas_version = version.parse('.'.join(vsplit[imas_start + 1:ual_start]))
+    ual_version = version.parse('.'.join(vsplit[ual_start + 1:]))
 
     return imas_version, ual_version
 
 
 def add_provenance_info(handle: ImasHandle, ids: str = 'core_profiles'):
     """Add provenance information to handle.
 
@@ -64,32 +71,31 @@
 
         # The repository, always set to duqtools
         entry.code.repository = 'https://github.com/duqtools/duqtools/'
 
         entry.put(db_entry=data_entry_target)
 
 
-@add_to_op_queue('Copy ids from template to', '{target}', quiet=True)
-def copy_ids_entry(source: ImasHandle, target: ImasHandle):
-    """Copies the ids entry to a new location.
+def copy_ids_entry_complex(source: ImasHandle, target: ImasHandle):
+    """Old way of copying by reading and writing via IMAS.
+
+    Copies the ids entry to a new location.
 
     Parameters
     ----------
     source : ImasHandle
         Source ids entry
     target : ImasHandle
         Target ids entry
 
     Raises
     ------
     KeyError
         If the IDS entry you are trying to copy does not exist.
     """
-    target.validate()
-
     imas_version, _ = get_imas_ual_version()
 
     idss_in = imas.ids(source.shot, source.run)
     op = idss_in.open_env(source.user, source.db, str(imas_version.major))
 
     ids_not_found = op[0] < 0
     if ids_not_found:
@@ -117,8 +123,33 @@
                 ids.get(i)
                 ids.setExpIdx(idx)  # this line sets the index to the output
                 ids.put(i)
 
     idss_in.close()
     idss_out.close()
 
+
+@add_to_op_queue('Copy ids from template to', '{target}', quiet=True)
+def copy_ids_entry(source: ImasHandle, target: ImasHandle):
+    """Copies the ids entry to a new location.
+
+    Parameters
+    ----------
+    source : ImasHandle
+        Source ids entry
+    target : ImasHandle
+        Target ids entry
+
+    Raises
+    ------
+    KeyError
+        If the IDS entry you are trying to copy does not exist.
+    """
+    target.validate()
+
+    if os.environ.get('SIMPLE_IDS_COPY'):
+        for src_file, dst_file in zip(source.paths(), target.paths()):
+            shutil.copyfile(src_file, dst_file)
+    else:
+        copy_ids_entry_complex(source, target)
+
     add_provenance_info(handle=target)
```

### Comparing `duqtools-1.8.0/src/duqtools/ids/_handle.py` & `duqtools-1.9.0/src/duqtools/ids/_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import os
 import re
 from contextlib import contextmanager
 from getpass import getuser
 from pathlib import Path
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, List, Sequence
 
 from pydantic import validator
 
 from ..config import lookup_vars, var_lookup
 from ..operations import add_to_op_queue
 from ..schema import IDSVariableModel, ImasBaseModel
 from ._copy import copy_ids_entry
@@ -25,14 +25,15 @@
 
 _FILENAME = 'ids_{shot}{run:04d}{suffix}'
 _IMASDB = ('{db}', '3', '0')
 GLOBAL_PATH_TEMPLATE = str(Path.home().parent.joinpath('{user}', 'public',
                                                        'imasdb', *_IMASDB,
                                                        _FILENAME))
 LOCAL_PATH_TEMPLATE = str(Path('{user}', *_IMASDB, _FILENAME))
+PUBLIC_PATH_TEMPLATE = str(Path('shared', 'imasdb', *_IMASDB, _FILENAME))
 
 SUFFIXES = (
     '.datafile',
     '.characteristics',
     '.tree',
 )
 
@@ -124,27 +125,35 @@
         return f'{self.user}/{self.db}/{self.shot}/{self.run}'
 
     @property
     def is_local_db(self):
         """Return True if the handle points to a local imas database."""
         return self.user.startswith('/')
 
-    def path(self) -> Path:
+    def path(self, suffix=SUFFIXES[0]) -> Path:
         """Return location as Path."""
+        imas_home = os.environ.get('IMAS_HOME')
+
         if self.is_local_db:
             template = LOCAL_PATH_TEMPLATE
+        elif imas_home and self.user == 'public':
+            template = imas_home + '/' + PUBLIC_PATH_TEMPLATE
         else:
             template = GLOBAL_PATH_TEMPLATE
 
         return Path(
             template.format(user=self.user,
                             db=self.db,
                             shot=self.shot,
                             run=self.run,
-                            suffix=SUFFIXES[0]))
+                            suffix=suffix))
+
+    def paths(self) -> List[Path]:
+        """Return location of all files as a list of Paths."""
+        return [self.path(suffix) for suffix in SUFFIXES]
 
     def imasdb_path(self) -> Path:
         """Return path to imasdb."""
         return self.path().parents[2]
 
     def exists(self) -> bool:
         """Return true if the directory exists.
```

### Comparing `duqtools-1.8.0/src/duqtools/ids/_imas.py` & `duqtools-1.9.0/src/duqtools/ids/_imas.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/ids/_mapping.py` & `duqtools-1.9.0/src/duqtools/ids/_mapping.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/ids/_merge.py` & `duqtools-1.9.0/src/duqtools/ids/_merge.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/ids/_rebase.py` & `duqtools-1.9.0/src/duqtools/ids/_rebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import xarray as xr
 
 logger = logging.getLogger(__name__)
 
 
 def rezero_time(ds: xr.Dataset, *, start: int = 0) -> None:
-    """Standardize the time within a dataset by setting the first timestep to 0.
+    """Standardize the time within a dataset by setting the first timestep to
+    0.
 
     Simply subtracts time[0] from all time entries and adds `start`
     Note: this does not interpolate the times between different datasets
 
     Parameters
     ----------
     ds : xr.Dataset
```

### Comparing `duqtools-1.8.0/src/duqtools/init.py` & `duqtools-1.9.0/src/duqtools/init.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/jetto/_batchfile.py` & `duqtools-1.9.0/src/duqtools/jetto/_batchfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,41 +4,46 @@
 import stat
 from os.path import commonpath
 from pathlib import Path
 from typing import TYPE_CHECKING, Sequence
 
 import jetto_tools
 
-from ..models import Locations
+from ..config import Config
 
 if TYPE_CHECKING:
     from ..models import Job
 
 
-def write_batchfile(run_dir: Path,
-                    jset: jetto_tools.jset.JSET,
-                    tag: str | None = None):
+def write_batchfile(
+    run_dir: Path,
+    jset: jetto_tools.jset.JSET,
+    *,
+    cfg: Config,
+    jruns_path: Path,
+):
     """Write batchfile (`.llcmd`) to start jetto.
 
     Parameters
     ----------
     run_dir : Path
         Directory to place batch file into.
     jset: JSET
         Jetto settings object (from jetto-pythontools)
-    tag : str | None
-        Tag the job, defaults to 'jetto'.
+    cfg : Config
+        Duqtools config.
+    jruns_path : Path
+        Path where runs can be run with slurm
     """
-    if not tag:
-        tag = 'jetto'
+    tag = cfg.tag if cfg.tag else 'jetto'
 
     llcmd_path = run_dir / '.llcmd'
 
     rjettov_path = (run_dir / 'rjettov').resolve()
-    rel_path = run_dir.resolve().relative_to(Locations().jruns_path.resolve())
+    rel_path = run_dir.resolve().relative_to(jruns_path.resolve())
 
     build_name = jset['JobProcessingPanel.name']
     build_user_name = jset['JobProcessingPanel.userid']
     machine_number = jset['JobProcessingPanel.machineNumber']
     num_proc = jset['JobProcessingPanel.numProcessors']
     wall_time = jset['JobProcessingPanel.wallTime']
```

### Comparing `duqtools-1.8.0/src/duqtools/jetto/_jettovar_to_json.py` & `duqtools-1.9.0/src/duqtools/jetto/_jettovar_to_json.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/jetto/_system.py` & `duqtools-1.9.0/src/duqtools/jetto/_system.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 from pathlib import Path
 from typing import Any, List, Optional
 
 from jetto_tools import config, jset, lookup, namelist, template
 from jetto_tools import job as jetto_job
 from jetto_tools.template import _EXTRA_FILE_REGEXES
 
-from ..config import CFG, Config
 from ..ids import ImasHandle
-from ..models import AbstractSystem, Job, Locations
+from ..models import AbstractSystem, Job
 from ..operations import add_to_op_queue
-from ..schema import JettoVar
+from ..schema import JettoSystemModel, JettoVar
 from ._batchfile import write_array_batchfile as _write_array_batchfile
 from ._batchfile import write_batchfile as _write_batchfile
 from ._jettovar_to_json import jettovar_to_json
 
 if sys.version_info < (3, 10):
     from importlib_resources import files
 else:
@@ -50,25 +49,41 @@
                 'Please remove these or turn "restart off" in JAMS'
                 'before running duqtools again.'
                 'More info: https://github.com/duqtools/duqtools/issues/498')
 
     return jetto_extra
 
 
-class BaseJettoSystem(AbstractSystem):
+class BaseJettoSystem(AbstractSystem, JettoSystemModel):
     """System that can be used to create runs for jetto.
 
     This system can submit to various backends like docker, prominence
     and the gateway.
     """
 
-    @staticmethod
-    def get_runs_dir() -> Path:
-        path = Locations().jruns_path
-        runs_dir = CFG.create.runs_dir  # type: ignore
+    @property
+    def jruns_path(self) -> Path:
+        """Return the Path specified in the system>jruns config variable, or,
+        if that is empty, the `$JRUNS` environment variable, or, if `$JRUNS`
+        does not exists, return the current directory `./`.
+
+        Returns
+        -------
+        Path
+        """
+        if self.jruns:  # type: ignore
+            return self.jruns  # type: ignore
+        elif os.getenv('JRUNS'):
+            return Path(os.getenv('JRUNS'))  # type: ignore
+        else:
+            return Path()
+
+    def get_runs_dir(self) -> Path:
+        path = self.jruns_path
+        runs_dir = self.cfg.create.runs_dir  # type: ignore
         if not runs_dir:
             abs_cwd = str(Path.cwd().resolve())
             abs_jruns = str(path.resolve())
             # Check if jruns is parent dir of current dir
             if abs_cwd.startswith(abs_jruns):
                 runs_dir = Path()
             else:  # jruns is somewhere else
@@ -76,57 +91,56 @@
                 while True:  # find the next free folder
                     runs_dir = f'duqtools_experiment_{count:04d}'
                     if not (path / runs_dir).exists():
                         break
                     count = count + 1
         return path / runs_dir
 
-    @staticmethod
     @add_to_op_queue('Writing new batchfile', '{run_dir.name}', quiet=True)
-    def write_batchfile(run_dir: Path, cfg: Config):
+    def write_batchfile(self, run_dir: Path):
         jetto_jset = jset.read(run_dir / 'jetto.jset')
-        _write_batchfile(run_dir, jetto_jset, tag=cfg.tag)
+        _write_batchfile(run_dir,
+                         jetto_jset,
+                         cfg=self.cfg,
+                         jruns_path=self.jruns_path)
 
-    @staticmethod
-    def submit_job(job: Job):
+    def submit_job(self, job: Job):
         # Make sure we get a new correct status
         if (job.path / 'jetto.status').exists():
             os.remove(job.path / 'jetto.status')
 
-        submit_system = job.cfg.submit.submit_system
+        submit_system = self.submit_system
 
         if submit_system == 'slurm':
-            submit = JettoSystem.submit_slurm
+            submit = self.submit_slurm
         elif submit_system == 'docker':
-            submit = JettoSystem.submit_docker
+            submit = self.submit_docker
         elif submit_system == 'prominence':
-            submit = JettoSystem.submit_prominence
+            submit = self.submit_prominence
         else:
             raise NotImplementedError(f'submission type {submit_system}'
                                       ' not implemented')
 
         submit(job)
 
-    @staticmethod
-    def submit_slurm(job: Job):
+    def submit_slurm(self, job: Job):
         if not job.has_submit_script:
             raise FileNotFoundError(job.submit_script)
 
-        submit_cmd = job.cfg.submit.submit_command.split()
+        submit_cmd = self.submit_command.split()
         cmd: list[Any] = [*submit_cmd, str(job.submit_script)]
 
         logger.info(f'submitting script via slurm {cmd}')
 
         ret = sp.run(cmd, check=True, capture_output=True)
         logger.info('submission returned: ' + str(ret.stdout))
         with open(job.lockfile, 'wb') as f:
             f.write(ret.stdout)
 
-    @staticmethod
-    def submit_docker(job: Job):
+    def submit_docker(self, job: Job):
         jetto_template = template.from_directory(job.path)
         jetto_config = config.RunConfig(jetto_template)
         jetto_manager = jetto_job.JobManager()
         extra_volumes = {
             job.path.parent / 'imasdb': {
                 'bind': '/opt/imas/shared/imasdb',
                 'mode': 'rw'
@@ -134,72 +148,90 @@
         }
 
         os.environ['RUNS_HOME'] = os.getcwd()
         os.environ['JINTRAC_IMAS_BACKEND'] = 'MDSPLUS'
         container = jetto_manager.submit_job_to_docker(
             jetto_config,
             job.path,
-            image=job.cfg.submit.docker_image,
+            image=self.docker_image,
             extra_volumes=extra_volumes)
         job.lockfile.touch()
         with open(job.lockfile, 'w') as f:
             f.write(container.name)
 
-    @staticmethod
-    def submit_prominence(job: Job):
+    def submit_prominence(self, job: Job):
         jetto_template = template.from_directory(job.path)
-        jetto_config = config.RunConfig(jetto_template)
-        jetto_manager = jetto_job.JobManager()
+        config.RunConfig(jetto_template)
+        jetto_job.JobManager()
+        jetto_jset = jset.read(job.path / 'jetto.jset')
+
+        # Jetto tools decided to be weird, so we use jams/prom-submit.py
+        cmd = [
+            'prom-submit.py', '--rundir',
+            str(job.path), '--image', self.prominence_image, '--cpus',
+            str(jetto_jset['JobProcessingPanel.numProcessors']), '--walltime',
+            '24.0', '--name', f'duqtools_{job.path.name}', '--cmd',
+            '/docker-entrypoint.sh rjettov -I -xmpi -x64'
+        ]
 
-        os.environ['RUNS_HOME'] = os.getcwd()
-        _ = jetto_manager.submit_job_to_prominence(jetto_config, job.path)
+        ret = sp.run(cmd, check=True, capture_output=True)
+        with open(job.lockfile, 'wb') as f:
+            f.write(ret.stdout)
 
-    @staticmethod
-    def submit_array(jobs: Sequence[Job],
-                     max_jobs: int,
-                     max_array_size: int = 100):
-        if jobs[0].cfg.submit.submit_system == 'slurm':
-            JettoSystem.submit_array_slurm(jobs, max_jobs, max_array_size)
+    def submit_array(
+        self,
+        jobs: Sequence[Job],
+        *,
+        max_jobs: int = 10,
+        max_array_size: int = 100,
+        **kwargs,
+    ):
+        if self.submit_system == 'slurm':
+            self.submit_array_slurm(jobs,
+                                    max_jobs=max_jobs,
+                                    max_array_size=max_array_size)
         else:
             raise NotImplementedError(
-                f'array submission type {jobs[0].cfg.submit.submit_system}'
+                f'array submission type {self.submit_system}'
                 ' not implemented')
 
-    @staticmethod
     @add_to_op_queue('Submit single array job', 'duqtools_slurm_array.sh')
-    def submit_array_slurm(jobs: Sequence[Job], max_jobs: int,
-                           max_array_size: int):
+    def submit_array_slurm(
+        self,
+        jobs: Sequence[Job],
+        max_jobs: int,
+        max_array_size: int,
+        **kwargs,
+    ):
         for job in jobs:
             job.lockfile.touch()
 
         logger.info('writing duqtools_slurm_array.sh file')
         _write_array_batchfile(jobs, max_jobs, max_array_size)
 
-        submit_cmd = jobs[0].cfg.submit.submit_command.split()
+        submit_cmd = self.submit_command.split()
         cmd: list[Any] = [*submit_cmd, 'duqtools_slurm_array.sh']
 
         logger.info(f'Submitting script via: {cmd}')
 
         ret = sp.run(cmd, check=True, capture_output=True)
         logger.info('submission returned: ' + str(ret.stdout))
 
         for job in jobs:
             with open(job.lockfile, 'wb') as f:
                 f.write(ret.stdout)
 
-    @staticmethod
-    def _apply_patches_to_template(jetto_template: template.Template):
+    def _apply_patches_to_template(self, jetto_template: template.Template):
         """Apply settings that are necessary for duqtools to function."""
         # Force output of IDS data
         # https://github.com/duqtools/duqtools/issues/343
         jetto_template.jset._settings['JobProcessingPanel.selIdsRunid'] = True
 
-    @staticmethod
     @add_to_op_queue('Copying template to', '{target_drc}', quiet=True)
-    def copy_from_template(source_drc: Path, target_drc: Path):
+    def copy_from_template(self, source_drc: Path, target_drc: Path):
         jetto_jset = jset.read(source_drc / 'jetto.jset')
         jetto_namelist = namelist.read(source_drc / 'jetto.in')
 
         jetto_sanco = None
         if (source_drc / 'jetto.sin').exists():
             jetto_sanco = namelist.read(source_drc / 'jetto.sin')
 
@@ -211,15 +243,15 @@
 
         jetto_template = template.Template(jset=jetto_jset,
                                            namelist=jetto_namelist,
                                            lookup=jetto_lookup,
                                            sanco_namelist=jetto_sanco,
                                            extra_files=jetto_extra)
 
-        JettoSystem._apply_patches_to_template(jetto_template)
+        self._apply_patches_to_template(jetto_template)
 
         jetto_config = config.RunConfig(jetto_template)
 
         jetto_config.export(target_drc)
         lookup.to_file(jetto_lookup, target_drc /
                        'lookup.json')  # TODO, this should be copied as well
 
@@ -228,43 +260,47 @@
                 'utils_jetto',
         ):
             src = source_drc / filename
             dst = target_drc / filename
             shutil.copyfile(src, dst)
             dst.chmod(dst.stat().st_mode | stat.S_IXUSR)
 
-    @staticmethod
-    def imas_from_path(template_drc: Path) -> ImasHandle:
+    def imas_from_path(self, template_drc: Path) -> ImasHandle:
         jetto_jset = jset.read(template_drc / 'jetto.jset')
 
         return ImasHandle(
             db=jetto_jset['SetUpPanel.idsIMASDBMachine'],  # type: ignore
             user=jetto_jset['SetUpPanel.idsIMASDBUser'],  # type: ignore
             run=jetto_jset['SetUpPanel.idsIMASDBRunid'],  # type: ignore
             shot=jetto_jset['SetUpPanel.idsIMASDBShot'])  # type: ignore
 
-    @staticmethod
     @add_to_op_queue('Updating imas locations of', '{run}', quiet=True)
-    def update_imas_locations(run: Path, inp: ImasHandle, out: ImasHandle):
+    def update_imas_locations(
+        self,
+        run: Path,
+        inp: ImasHandle,
+        out: ImasHandle,
+        **kwargs,
+    ):
         jetto_template = template.from_directory(run)
         jetto_config = config.RunConfig(jetto_template)
 
         jetto_config['user_in'] = inp.user
         jetto_config['machine_in'] = inp.db
         jetto_config['shot_in'] = inp.shot
         jetto_config['run_in'] = inp.run
 
         jetto_config['machine_out'] = out.db
         jetto_config['shot_out'] = out.shot
         jetto_config['run_out'] = out.run
 
         jetto_config.export(run)  # Just overwrite the poor files
 
-    @staticmethod
-    def set_jetto_variable(run: Path,
+    def set_jetto_variable(self,
+                           run: Path,
                            key: str,
                            value,
                            variable: Optional[JettoVar] = None):
         jetto_template = template.from_directory(run)
 
         if variable:
             extra_lookup = lookup.from_json(jettovar_to_json(variable))
@@ -287,38 +323,38 @@
 
     The backend that is  assumed is jetto-v210921.
 
     This system can submit to various backends like docker, prominence
     and the gateway.
 
     ```yaml title="duqtools.yaml"
-    system: jetto-v210921
-    submit:
+    system:
+      name: jetto-v210921
       submit_system: prominence
     ```
     """
 
-    @staticmethod
     def get_data_in_handle(
+        self,
         *,
         dirname: Path,
         source: ImasHandle,
         seq_number: int,
         options,
     ):
         """Get handle for data input."""
         return ImasHandle(
             user=options.user,
             db=options.imasdb,
             shot=source.shot,
             run=options.run_in_start_at + seq_number,
         )
 
-    @staticmethod
     def get_data_out_handle(
+        self,
         *,
         dirname: Path,
         source: ImasHandle,
         seq_number: int,
         options,
     ):
         """Get handle for data output."""
@@ -337,22 +373,22 @@
     difference with v210921 is that the IMAS data is handled locally
     instead of via a public `imasdb`
 
     This system can submit to various backends like docker, prominence
     and the gateway.
 
     ```yaml title="duqtools.yaml"
-    system: jetto-v220922
-    submit:
+    system:
+      name: jetto-v220922
       submit_system: docker
     ```
     """
 
-    @staticmethod
     def get_data_in_handle(
+        self,
         *,
         dirname: Path,
         source: ImasHandle,
         seq_number: int,
         options,
     ):
         relative_location: Optional[str] = str(
@@ -363,16 +399,16 @@
         """Get handle for data input."""
         return ImasHandle(user=str((dirname / 'imasdb').resolve()),
                           db=source.db,
                           shot=source.shot,
                           run=1,
                           relative_location=relative_location)
 
-    @staticmethod
     def get_data_out_handle(
+        self,
         *,
         dirname: Path,
         source: ImasHandle,
         seq_number: int,
         options,
     ):
         relative_location: Optional[str] = str(
```

### Comparing `duqtools-1.8.0/src/duqtools/large_scale_validation/cli.py` & `duqtools-1.9.0/src/duqtools/large_scale_validation/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,19 +94,23 @@
 @cli.command('submit')
 @click.option('--force',
               is_flag=True,
               help='Re-submit running or completed jobs.')
 @click.option(
     '--schedule',
     is_flag=True,
-    help='Schedule and submit jobs automatically. `max_jobs` must be defined.')
+    help=(
+        'Schedule and submit jobs automatically. '
+        '`max_jobs` defines the total number of jobs running simultaneiously.'
+    ))
 @click.option('-j',
               '--max_jobs',
               type=int,
-              help='Maximum number of jobs to submit.')
+              help='Maximum number of running jobs.',
+              default=10)
 @click.option('-s',
               '--status',
               'status_filter',
               type=str,
               multiple=True,
               help='Only submit jobs with this status.')
 @click.option(
@@ -119,15 +123,22 @@
     '-i',
     '--input',
     'input_file',
     type=str,
     help=
     'Only submit jobs for configs where `template_data` matches a handle in this data.csv.'
 )
-@click.option('-a', '--array', is_flag=True, help='Submit jobs as array.')
+@click.option(
+    '-a',
+    '--array',
+    is_flag=True,
+    help=(
+        'Submit jobs as array. '
+        '`max_jobs` defines the total number of jobs running simultaneiously.'
+    ))
 @click.option(
     '--max_array_size',
     type=int,
     default=100,
     help='Maximum array size for slurm (usually 1001, default = 100).')
 @common_options(*logging_options, yes_option, dry_run_option)
 def cli_submit(**kwargs):
```

### Comparing `duqtools-1.8.0/src/duqtools/large_scale_validation/create.py` & `duqtools-1.9.0/src/duqtools/large_scale_validation/create.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/large_scale_validation/merge.py` & `duqtools-1.9.0/src/duqtools/large_scale_validation/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         cfg = load_config(config_file)
 
         assert cfg.create
         assert cfg.create.runs_dir
 
         config_dir = config_file.parent
 
-        runs = Locations(config_dir).runs
-        runs = (run for run in runs if Job(run.dirname).is_completed)
+        runs = Locations(parent_dir=config_dir, cfg=cfg).runs
+        runs = (run for run in runs if Job(run.dirname, cfg=cfg).is_completed)
         handles = (ImasHandle.parse_obj(run.data_out) for run in runs)
         handles = [handle for handle in handles if handle.exists()]
 
         if not handles:
             op_queue.warning(run_name, 'No data to merge.')
             continue
```

### Comparing `duqtools-1.8.0/src/duqtools/large_scale_validation/status.py` & `duqtools-1.9.0/src/duqtools/large_scale_validation/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,21 +30,24 @@
 
     click.echo(Job.status_symbol_help())
     click.echo()
 
     for config_file in config_files:
         cfg = load_config(config_file)
 
-        if not cfg.status:
+        if not cfg.system:
             raise StatusError(
                 f'Status field required in config file: {config_file}')
 
         config_dir = config_file.parent
 
-        jobs = [Job(run.dirname) for run in Locations(config_dir).runs]
+        jobs = [
+            Job(run.dirname, cfg=cfg)
+            for run in Locations(parent_dir=config_dir, cfg=cfg).runs
+        ]
         all_jobs.extend(jobs)
 
         dirname = config_file.parent.relative_to(cwd)
         tag = cfg.tag
         status = ''.join(job.status_symbol for job in jobs)
 
         click.echo(f'{dirname} ({tag}): {status}')
```

### Comparing `duqtools-1.8.0/src/duqtools/large_scale_validation/submit.py` & `duqtools-1.9.0/src/duqtools/large_scale_validation/submit.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,32 +51,42 @@
     jobs: list[Job] = []
 
     for drc in dirs:
         config_file = drc / 'duqtools.yaml'
         cfg = load_config(config_file)
 
         assert cfg.create
-        assert cfg.submit
+        assert cfg.system
 
         if handles and (cfg.create.template_data not in handles):
             continue
 
         config_dir = config_file.parent
 
-        jobs.extend(Job(run.dirname) for run in Locations(config_dir).runs)
+        jobs.extend(
+            Job(run.dirname, cfg=cfg)
+            for run in Locations(parent_dir=config_dir, cfg=cfg).runs)
 
     job_queue: Deque[Job] = deque()
 
     for job in jobs:
         status = job.status()
 
         if status_filter and (status not in status_filter):
             continue
         if not status_file_ok(job, force=force):
             continue
         if not lockfile_ok(job, force=force):
             continue
         job_queue.append(job)
 
-    submitter = job_scheduler if schedule else job_submitter
-    submitter = job_array_submitter if array else submitter
-    submitter(job_queue, max_jobs=max_jobs, max_array_size=max_array_size)
+    if schedule:
+        job_scheduler(job_queue, max_jobs=max_jobs)
+    elif array:
+        job_array_submitter(job_queue,
+                            max_jobs=max_jobs,
+                            max_array_size=max_array_size,
+                            cfg=cfg)
+    else:
+        job_submitter(job_queue, max_jobs=max_jobs)
+
+    return job_queue
```

### Comparing `duqtools-1.8.0/src/duqtools/list_variables.py` & `duqtools-1.9.0/src/duqtools/list_variables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import typing
+
 import click
-from pydantic import ValidationError
 
-from duqtools.config import load_config, var_lookup
+from duqtools.config import Config, var_lookup
 
 cs = click.style
 
 ST_ITEMS = {'fg': 'green', 'bold': True}
 ST_HEADER = {'fg': 'red', 'bold': True}
 ST_INFO = {'fg': 'white', 'bold': False}
 
 
+@typing.no_type_check
 def list_group(group: list, extra_variables: dict):
     group = sorted(group, key=lambda var: var.name)
 
     for var in group:
         star = cs('*', **ST_HEADER) if var.name in extra_variables else ''
 
         name = cs(f'{var.name}', **ST_ITEMS)
@@ -22,35 +24,28 @@
             sub = cs(f'({var.path})', **ST_INFO)
         except AttributeError:
             sub = cs(f'({var.type})', **ST_INFO)
 
         click.echo(f'    - {star}{name} {sub}')
 
 
-def list_variables(*, config, **kwargs):
+@typing.no_type_check
+def list_variables(*, cfg: Config, **kwargs):
     """List variables in `variables.yaml` and config/`duqtools.yaml` if
     present.
 
     Parameters
     ----------
-    config : str
-        Name of the config file to use
+    config : Config
+        Duqtools config.
     **kwargs
         Unused.
     """
-    try:
-        cfg = load_config(config)
-    except FileNotFoundError:
-        print(f'Could not find: {config}')
-    except ValidationError as e:
-        exit(e)
-        print(f'*: defined by {config}')
-    finally:
-        extra_variables = cfg.extra_variables.to_variable_dict(
-        ) if cfg.extra_variables else {}
+    extra_variables = cfg.extra_variables.to_variable_dict(
+    ) if cfg.extra_variables else {}
 
     grouped_ids_vars = var_lookup.groupby_ids()
 
     for root_ids, group in grouped_ids_vars.items():
         click.secho(f'\nIDS-variable - {root_ids}:', **ST_HEADER)
         list_group(group, extra_variables)
```

### Comparing `duqtools-1.8.0/src/duqtools/matrix_samplers.py` & `duqtools-1.9.0/src/duqtools/matrix_samplers.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/merge.py` & `duqtools-1.9.0/src/duqtools/merge.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/models/_job.py` & `duqtools-1.9.0/src/duqtools/models/_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import time
 from enum import Enum
 from pathlib import Path
-from typing import Optional
 
 import click
 
-from ..config import CFG, Config
+from ..config import Config
 
 logger = logging.getLogger(__name__)
 info, debug = logger.info, logger.debug
 
 cs = click.style
 
 STATUS_SYMBOLS = {
@@ -40,27 +39,26 @@
         s = ', '.join(f'{code} : {status}'
                       for status, code in STATUS_SYMBOLS.items())
         return f'Status codes:\n{s}'
 
 
 class Job:
 
-    def __init__(self, path: Path, *, cfg: Optional[Config] = None):
+    def __init__(self, path: Path, *, cfg: Config):
         """Summary.
 
         Parameters
         ----------
         path : Path
             Directory for simulation or model run.
         cfg : Optional[Config], optional
             Duqtools config, defaults to global config if unspecified.
         """
         self.path = Path(path).resolve()
-
-        self.cfg = cfg if cfg is not None else CFG
+        self.cfg = cfg
 
     def __repr__(self):
         run = str(self.path)
         return f'{self.__class__.__name__}({run!r})'
 
     @staticmethod
     def status_symbol_help():
@@ -91,19 +89,19 @@
         """Return the status of the job."""
         if not self.has_status:
             return JobStatus.NOSTATUS
 
         sf = self.status_file
         with open(sf) as f:
             content = f.read()
-            if self.cfg.status.msg_completed in content:
+            if self.cfg.system.msg_completed in content:
                 return JobStatus.COMPLETED
-            elif self.cfg.status.msg_failed in content:
+            elif self.cfg.system.msg_failed in content:
                 return JobStatus.FAILED
-            elif self.cfg.status.msg_running in content:
+            elif self.cfg.system.msg_running in content:
                 return JobStatus.RUNNING
 
         if self.is_submitted:
             return JobStatus.SUBMITTED
 
         return JobStatus.UNKNOWN
 
@@ -126,43 +124,43 @@
     def is_done(self) -> bool:
         """Return true if the job is done (completed or failed)."""
         return self.status() in (JobStatus.COMPLETED or JobStatus.FAILED)
 
     @property
     def in_file(self) -> Path:
         """Return path to the input file for the job."""
-        return self.path / self.cfg.status.in_file
+        return self.path / self.cfg.system.in_file
 
     @property
     def out_file(self) -> Path:
         """Return path to the output file for the job."""
-        return self.path / self.cfg.status.out_file
+        return self.path / self.cfg.system.out_file
 
     @property
     def status_file(self) -> Path:
         """Return the path of the status file."""
-        return self.path / self.cfg.status.status_file
+        return self.path / self.cfg.system.status_file
 
     @property
     def submit_script(self) -> Path:
         """Return the path of the submit script."""
-        return self.path / self.cfg.submit.submit_script_name
+        return self.path / self.cfg.system.submit_script_name
 
     @property
     def lockfile(self) -> Path:
         """Return the path of the lockfile."""
         return self.path / 'duqtools.submit.lock'
 
     def submit(self):
         """Submit job."""
         from ..system import get_system
         debug(f'Put lockfile in place for {self.lockfile}')
         self.lockfile.touch()
 
-        get_system().submit_job(self)
+        get_system(self.cfg).submit_job(self)
 
     def start(self):
         """Submit job and return generate that raises StopIteration when
         done."""
         click.echo(f'Submitting {self}\033[K')
         self.submit()
```

### Comparing `duqtools-1.8.0/src/duqtools/models/_run.py` & `duqtools-1.9.0/src/duqtools/models/_run.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/operations.py` & `duqtools-1.9.0/src/duqtools/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     def warning(self, description: str, extra_description: str):
         self.warnings.add(
             Warning(description=description,
                     extra_description=extra_description))
 
     def put(self, item: Operation):
-        """synonym for append."""
+        """Synonym for append."""
         self.append(item)
 
     def append(self, item: Operation):  # type: ignore
         """Restrict our diet to Operation objects only."""
         if self.enabled:
             logger.debug(
                 f'Appended {item.description} to the operations queue')
```

### Comparing `duqtools-1.8.0/src/duqtools/plot.py` & `duqtools-1.9.0/src/duqtools/plot.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/_imas.py` & `duqtools-1.9.0/src/duqtools/schema/_imas.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/_jetto.py` & `duqtools-1.9.0/src/duqtools/schema/_jetto.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/_ranges.py` & `duqtools-1.9.0/src/duqtools/schema/_ranges.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/_variable.py` & `duqtools-1.9.0/src/duqtools/schema/_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,26 @@
         The fields are separated by forward slashes (`\\`).
     """))
 
 
 class IDSVariableModel(IDSPath):
     """Variable for describing data within a IMAS database.
 
-    The variable can be given a name, which will be used in the rest of the config
-    to reference the variable. It will also be used as the column labels or
-    on plots.
-
-    The dimensions for each variable must be specified. This ensures the the data
-    will be self-consistent. For example for 1D data, you can use `[x]` and for 2D data,
-    `[x, y]`.
-
-    The IDS path may contain indices. You can point to a single index, by simply giving the
-    complete path (i.e. `profiles_1d/0/t_i_ave` for the 0th time slice).
-    To retrieve all time slices, you can use `profiles_1d/*/t_i_ave`.
+    The variable can be given a name, which will be used in the rest of
+    the config to reference the variable. It will also be used as the
+    column labels or on plots.
+
+    The dimensions for each variable must be specified. This ensures the
+    the data will be self-consistent. For example for 1D data, you can
+    use `[x]` and for 2D data, `[x, y]`.
+
+    The IDS path may contain indices. You can point to a single index,
+    by simply giving the complete path (i.e. `profiles_1d/0/t_i_ave` for
+    the 0th time slice). To retrieve all time slices, you can use
+    `profiles_1d/*/t_i_ave`.
     """
     type: str = Field('IDS-variable',
                       description='discriminator for the variable type')
 
     name: str = Field(description=f("""
         Name of the variable.
         This will be used to reference this variable.
```

### Comparing `duqtools-1.8.0/src/duqtools/schema/data_location.py` & `duqtools-1.9.0/src/duqtools/schema/data_location.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/matrix_samplers.py` & `duqtools-1.9.0/src/duqtools/schema/matrix_samplers.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/schema/variables.py` & `duqtools-1.9.0/src/duqtools/schema/variables.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools/setup.py` & `duqtools-1.9.0/src/duqtools/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from .utils import no_op
 
 if TYPE_CHECKING:
     import jinja2
 
     from duqtools.api import IDSMapping
 
+    from .schema import IDS2JettoVariableModel
+
 logger = logging.getLogger(__name__)
 
 
 class SetupError(Exception):
     ...
 
 
@@ -121,15 +123,16 @@
         elif isinstance(value, complex):
             return value == imasdef.EMPTY_COMPLEX
 
         return False
 
     def __getattr__(self, key: str):
         try:
-            spec = self.lookup[f'ids-{key}']
+            spec: IDS2JettoVariableModel = self.lookup[
+                f'ids-{key}']  # type: ignore
         except KeyError as exc:
             msg = f'Cannot find {key!r} in your variable listing (i.e. `variables.yaml`).'
             raise AttributeError(msg) from exc
 
         value = spec.default
 
         for item in spec.paths:
```

### Comparing `duqtools-1.8.0/src/duqtools/status.py` & `duqtools-1.9.0/src/duqtools/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess as sp
 from collections import Counter
 from time import sleep
 from typing import Sequence
 
 from jetto_tools import config, template
 
-from .config import CFG
+from .config import Config
 from .jetto._system import jetto_lookup
 from .models import Job, JobStatus, Locations
 
 logger = logging.getLogger(__name__)
 info, debug = logger.info, logger.debug
 stream = logging.StreamHandler()
 stream.setFormatter(logging.Formatter('%(message)s'))
@@ -48,15 +48,15 @@
         self.n_submitted = counter[JobStatus.SUBMITTED]
         self.n_completed = counter[JobStatus.COMPLETED]
         self.n_running = counter[JobStatus.RUNNING]
         self.n_failed = counter[JobStatus.FAILED]
         self.n_unknown = counter[JobStatus.UNKNOWN]
 
     def simple_status(self):
-        """stateless status."""
+        """Stateless status."""
         self.update_status()
 
         msg = 'Total number of directories with %-17s : %i'
 
         info(msg, 'submit script', self.n_submit_script)
         info(msg, 'unsubmitted jobs', self.n_submit_script - self.n_status)
         info(msg, 'status script', self.n_status)
@@ -132,15 +132,16 @@
         self.set_status()
 
     def check_kwmain_flag(self, jetto_config):
         """Check for NLIST2/KWMAIN in jetto.jset. If this flag is not set, the
         output in `job.out_file` does not contain the output that is grepped
         for the progress.
 
-        More info: https://github.com/duqtools/duqtools/issues/337
+        More info:
+        https://github.com/duqtools/duqtools/issues/337
         """
         msg = ('Cannot show detailed status, `nlist2.KWMAIN` flag'
                ' is not set to 1 in `{self.job.status_file}`')
         if jetto_config['kwmain'] != 1:
             raise StatusError(msg)
 
     def set_status(self):
@@ -179,30 +180,42 @@
             self.time = steptime
 
         self.pbar.n = int(100 * (self.time - self.start) /
                           (self.end - self.start))
         self.pbar.refresh()
 
 
-def status(*, progress: bool, detailed: bool, **kwargs):
+def status(*,
+           cfg: Config,
+           progress: bool = False,
+           detailed: bool = False,
+           **kwargs):
     """Show status of runs.
 
     Parameters
     ----------
     progress : bool
         Show progress bar.
     detailed : bool
         Show detailed progress for every job.
     """
-    debug('Submit config: %s', CFG.submit)
+    debug('Submit config: %s', cfg.system)
 
-    runs = Locations().runs
-    jobs = [Job(run.dirname) for run in runs]
+    runs = Locations(cfg=cfg).runs
+    jobs = [Job(run.dirname, cfg=cfg) for run in runs]
 
     tracker = Status(jobs)
 
     if detailed:
         tracker.detailed_status()
     elif progress:
         tracker.progress_status()
     else:
         tracker.simple_status()
+
+    return tracker
+
+
+def status_api(config: dict, **kwargs):
+    """Wrapper around status for python api."""
+    cfg = Config.from_dict(config)
+    return status(cfg=cfg, **kwargs)
```

### Comparing `duqtools-1.8.0/src/duqtools/submit.py` & `duqtools-1.9.0/src/duqtools/submit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 import time
 from collections import deque
 from itertools import cycle
 from pathlib import Path
-from typing import Deque, Sequence
+from typing import Deque, Optional, Sequence
 
 from ._logging_utils import duqlog_screen
-from .config import CFG
+from .config import Config
+from .create import CreateError
 from .models import Job, Locations
 from .operations import add_to_op_queue, op_queue
 from .system import get_system
 
 logger = logging.getLogger(__name__)
 info, debug = logger.info, logger.debug
 
@@ -34,25 +35,25 @@
         This causes issues with slurm, for example.
     """
     if delay:
         time.sleep(delay)
     job.submit()
 
 
-def job_submitter(jobs: Sequence[Job], *, max_jobs, **kwargs):
+def job_submitter(jobs: Sequence[Job], *, max_jobs: int, **kwargs):
     for n, job in enumerate(jobs):
         if max_jobs and (n >= max_jobs):
             info(f'Max jobs ({max_jobs}) reached.')
             break
 
         _submit_job(job, delay=0.1)
 
 
 @add_to_op_queue('Start job scheduler')
-def job_scheduler(queue: Deque[Job], max_jobs=10, **kwargs):
+def job_scheduler(queue: Deque[Job], *, max_jobs: int = 10, **kwargs):
     interval = 1.0
 
     s = Spinner()
 
     tasks: Deque[Job] = deque()
     completed: Deque[Job] = deque()
 
@@ -75,43 +76,49 @@
         print(
             f' {next(s)} Running: {len(tasks)},'
             f' queue: {len(queue)}, completed: {len(completed)}',
             end='\033[K\r',
         )
 
 
-def job_array_submitter(jobs: Sequence[Job], *, max_jobs, max_array_size,
-                        **kwargs):
+def job_array_submitter(
+    jobs: Sequence[Job],
+    *,
+    max_jobs: int = 10,
+    max_array_size: int = 100,
+    cfg: Config,
+):
     if len(jobs) == 0:
         duqlog_screen.error('No jobs to submit, not creating array ...')
         return
 
     for job in jobs:
         op_queue.add(action=lambda: None,
                      description='Adding to array',
                      extra_description=f'{job}')
 
-    if not max_jobs:
-        logger.info('Max jobs not specified, defaulting to 10')
-        max_jobs = 10
+    if not cfg.create:
+        raise CreateError('Create field required in config file')
 
-    get_system().submit_array(jobs, max_jobs, max_array_size)
+    get_system(cfg=cfg).submit_array(jobs,
+                                     max_jobs=max_jobs,
+                                     max_array_size=max_array_size)
 
 
-def submission_script_ok(job):
+def submission_script_ok(job) -> bool:
     submission_script = job.submit_script
     if not submission_script.is_file():
         info('Did not found submission script %s ; Skipping directory...',
              submission_script)
         return False
 
     return True
 
 
-def status_file_ok(job, *, force):
+def status_file_ok(job, *, force: bool) -> bool:
     status_file = job.status_file
     if job.has_status and not force:
         if not status_file.is_file():
             logger.warning('Status file %s is not a file', status_file)
         with open(status_file) as f:
             info('Status of %s: %s. To rerun enable the --force flag',
                  status_file, f.read())
@@ -119,59 +126,67 @@
             description='Not Submitting',
             extra_description=f'{job} (reason: status file exists)')
         return False
 
     return True
 
 
-def lockfile_ok(job, *, force):
+def lockfile_ok(job: Job, *, force: bool) -> bool:
     lockfile = job.lockfile
     if lockfile.exists() and not force:
         op_queue.add_no_op(
             description='Not Submitting',
             extra_description=f'{job} (reason: {lockfile} exists)')
         return False
 
     return True
 
 
-def get_resubmit_jobs(resubmit_names: Sequence[Path]) -> list[Job]:
-    """get_resubmit_jobs.
+def get_resubmit_jobs(cfg: Config, *, resubmit_names: Sequence[Path],
+                      locations: Locations) -> list[Job]:
+    """Get list of jobs to resubmit.
 
     Parameters
     ----------
+    cfg: Config
+        Duqtools config.
     resubmit_names : Sequence[Path]
         The names (short or full path) of the jobs that need to be resubmitted
+    locations : Locations
+        Instance of Locations, use these to search for jobs
 
     Returns
     -------
     list[Job]
     """
     jobs: list[Job] = []
-    run_dict = {run.shortname: run for run in Locations().runs}
+    run_dict = {run.shortname: run for run in locations.runs}
     for name in resubmit_names:
         if name in run_dict:  # check for shortname
-            jobs.append(Job(run_dict[name].dirname))
+            name = run_dict[name].dirname
         else:
             # It's not a short name, use the argument as the full path to the job
-            jobs.append(Job(Path(name)))
+            name = Path(name)
+
+        jobs.append(Job(name, cfg=cfg))
     return jobs
 
 
 def submit(*,
-           force: bool,
-           max_jobs: int,
-           max_array_size: int,
-           schedule: bool,
-           array: bool,
+           cfg: Config,
+           force: bool = False,
+           max_jobs: int = 10,
+           max_array_size: int = 100,
+           schedule: bool = False,
+           array: bool = False,
            resubmit: Sequence[Path] = (),
-           status_filter: Sequence[str],
+           status_filter: Sequence[str] = (),
+           parent_dir: Optional[Path] = None,
            **kwargs):
-    """submit. Function which implements the functionality to submit jobs to
-    the cluster.
+    """Submit jobs to the cluster.
 
     Parameters
     ----------
     force : bool
         Force the submission even in the presence of lockfiles
     max_jobs : int
         Maximum number of jobs to submit at once
@@ -184,45 +199,61 @@
         Submit the jobs as a single array
     resubmit : Sequence[Path]
         If any jobs need to be resubmitted, this is has a nonzero length, and
         contains a Sequence of Paths which either are the full Path to the run
         that needs to be resubmitted, or the shortname
     status_filter : list[str]
         Only submit jobs with this status.
+    parent_dir : Path
+        Search for jobs in this directory.
     """
-    if not CFG.submit:
-        raise SubmitError('Submit field required in config file')
 
-    debug('Submit config: %s', CFG.submit)
+    locations = Locations(parent_dir=parent_dir, cfg=cfg)
 
     if resubmit:
-        jobs = get_resubmit_jobs(resubmit)
+        jobs = get_resubmit_jobs(cfg=cfg,
+                                 resubmit_names=resubmit,
+                                 locations=locations)
         force = True
     else:
-        jobs = [Job(run.dirname) for run in Locations().runs]
+        jobs = [Job(run.dirname, cfg=cfg) for run in locations.runs]
 
     debug('Case directories: %s', jobs)
 
     job_queue: Deque[Job] = deque()
 
+    if array and Path('./duqtools_slurm_array.sh').exists() and not force:
+        op_queue.add_no_op(
+            description='Not Creating Array',
+            extra_description='(reason: duqtools_slurm_array.sh exists)')
+        op_queue.add_no_op(description='Not Submitting Array',
+                           extra_description='use --force to override')
+        return job_queue
+
     for job in jobs:
         status = job.status()
 
         if status_filter and (status not in status_filter):
             continue
         if not status_file_ok(job, force=force):
             continue
         if not lockfile_ok(job, force=force):
             continue
         job_queue.append(job)
 
-    if array and Path('./duqtools_slurm_array.sh').exists() and not force:
-        op_queue.add_no_op(
-            description='Not Creating Array',
-            extra_description='(reason: duqtools_slurm_array.sh exists)')
-        op_queue.add_no_op(description='Not Submitting Array',
-                           extra_description='use --force to override')
-        return
+    if schedule:
+        job_scheduler(job_queue, max_jobs=max_jobs)
+    elif array:
+        job_array_submitter(job_queue,
+                            max_jobs=max_jobs,
+                            max_array_size=max_array_size,
+                            cfg=cfg)
+    else:
+        job_submitter(job_queue, max_jobs=max_jobs)
+
+    return job_queue
+
 
-    submitter = job_scheduler if schedule else job_submitter
-    submitter = job_array_submitter if array else submitter
-    submitter(job_queue, max_jobs=max_jobs, max_array_size=max_array_size)
+def submit_api(config: dict, **kwargs):
+    """Wrapper around submit for python api."""
+    cfg = Config.from_dict(config)
+    return submit(cfg=cfg, **kwargs)
```

### Comparing `duqtools-1.8.0/src/duqtools/utils.py` & `duqtools-1.9.0/src/duqtools/utils.py`

 * *Files identical despite different names*

### Comparing `duqtools-1.8.0/src/duqtools.egg-info/PKG-INFO` & `duqtools-1.9.0/src/duqtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: duqtools
-Version: 1.8.0
+Version: 1.9.0
 Summary: Dynamic uncertainty quantification for Tokamak reactor simulations modelling
-Home-page: https://github.com/duqtools/duqtools
-Author: Stef Smeets
-Author-email: s.smeets@esciencecenter.nl
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/duqtools/duqtools/issues
-Project-URL: Documentation, https://duqtools.readthedocs.io
+Author: Victor Azizi, Aaron Ho
+Author-email: Stef Smeets <s.smeets@esciencecenter.nl>
+License: Apache 2.0 License
+Project-URL: homepage, https://github.com/duqtools/duqtools
+Project-URL: issues, https://github.com/duqtools/duqtools/issues
+Project-URL: documentation, https://duqtools.readthedocs.io
+Project-URL: changelog, https://github.com/duqtools/duqtools/releases
 Keywords: modelling,uncertainty-quantification,tokamak,fusion-reactor
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 Provides-Extra: docs
 Provides-Extra: publishing
 Provides-Extra: imas
 License-File: LICENSE
 
-| Source | Badges |
-| --- | --- |
-| ReadTheDocs |[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest) |
-| Github | [![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml) ![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json) |
-| PyPI | [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/) [![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/) |
-| SonarCloud | [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=duqtools_duqtools&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=duqtools_duqtools) |
-| Zenodo | [![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189) |
+[![Documentation Status](https://readthedocs.org/projects/duqtools/badge/?version=latest)](https://duqtools.readthedocs.io/en/latest/?badge=latest)
+[![Tests](https://github.com/duqtools/duqtools/actions/workflows/test.yaml/badge.svg)](https://github.com/duqtools/duqtools/actions/workflows/test.yaml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/duqtools)](https://pypi.org/project/duqtools/)
+[![PyPI](https://img.shields.io/pypi/v/duqtools.svg?style=flat)](https://pypi.org/project/duqtools/)
+[![DOI](https://zenodo.org/badge/492734189.svg)](https://zenodo.org/badge/latestdoi/492734189)
+![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/stefsmeets/ea916a5b3c3d9bc59065a7304e4ca707/raw/covbadge.json)
+
+
+![Duqtools banner](https://raw.githubusercontent.com/duqtools/duqtools/main/src/duqtools/data/logo.png)
 
 # Duqtools
 
 *Duqtools* is a tool for **D**ynamic **U**ndertainty **Q**uantification for Tokamak reactor simulations modelling.
 
 Features:
 
@@ -61,9 +64,7 @@
 
 Suggestions, improvements, and edits are most welcome.
 
 
 ## Development
 
 Check out our [Contributing Guidelines](CONTRIBUTING.md#Getting-started-with-development) to get started with development.
-
-
```

### Comparing `duqtools-1.8.0/src/duqtools.egg-info/SOURCES.txt` & `duqtools-1.9.0/src/duqtools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 src/duqtools/__init__.py
 src/duqtools/_click_opt_groups.py
 src/duqtools/_logging_utils.py
 src/duqtools/_plot_utils.py
 src/duqtools/_types.py
 src/duqtools/api.py
 src/duqtools/apply_model.py
@@ -33,26 +31,28 @@
 src/duqtools.egg-info/entry_points.txt
 src/duqtools.egg-info/not-zip-safe
 src/duqtools.egg-info/requires.txt
 src/duqtools.egg-info/top_level.txt
 src/duqtools/config/__init__.py
 src/duqtools/config/_config.py
 src/duqtools/config/_variables.py
+src/duqtools/dashboard/Plotting.py
+src/duqtools/dashboard/_shared.py
+src/duqtools/dashboard/readme.md
+src/duqtools/dashboard/requirements.txt
+src/duqtools/dashboard/pages/1_Merging.py
 src/duqtools/data/duqtools.yaml
 src/duqtools/data/jetto_tools_lookup.json
 src/duqtools/data/variables.yaml
 src/duqtools/data/variables_core-profiles.yaml
 src/duqtools/data/variables_core-sources.yaml
 src/duqtools/data/variables_equilibrium.yaml
 src/duqtools/data/variables_ids2jetto.yaml
-src/duqtools/data/dash/_shared.py
-src/duqtools/data/dash/dash.py
-src/duqtools/data/dash/readme.md
-src/duqtools/data/dash/requirements.txt
-src/duqtools/data/dash/pages/1_merge.py
+src/duqtools/ets/__init__.py
+src/duqtools/ets/_system.py
 src/duqtools/ids/__init__.py
 src/duqtools/ids/_apply_model.py
 src/duqtools/ids/_copy.py
 src/duqtools/ids/_handle.py
 src/duqtools/ids/_imas.py
 src/duqtools/ids/_mapping.py
 src/duqtools/ids/_merge.py
@@ -76,12 +76,20 @@
 src/duqtools/schema/__init__.py
 src/duqtools/schema/_basemodel.py
 src/duqtools/schema/_description_helpers.py
 src/duqtools/schema/_dimensions.py
 src/duqtools/schema/_imas.py
 src/duqtools/schema/_jetto.py
 src/duqtools/schema/_ranges.py
+src/duqtools/schema/_systems.py
 src/duqtools/schema/_variable.py
 src/duqtools/schema/cli.py
 src/duqtools/schema/data_location.py
 src/duqtools/schema/matrix_samplers.py
-src/duqtools/schema/variables.py
+src/duqtools/schema/variables.py
+tests/test_api.py
+tests/test_cmdline.py
+tests/test_duqmap.py
+tests/test_duqtools.py
+tests/test_ids2jetto_variables.py
+tests/test_operations.py
+tests/test_samplers.py
```

### Comparing `duqtools-1.8.0/src/duqtools.egg-info/requires.txt` & `duqtools-1.9.0/src/duqtools.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,33 +4,29 @@
 jinja2>=3.0
 numpy
 pandas
 pydantic!=1.10.3,!=1.10.4,!=1.10.5
 pydantic-yaml
 scipy>=1.09
 tqdm
+typing-extensions!=4.6.0
 xarray
 jetto-tools>=1.8.8
-
-[:python_full_version != "3.9.7"]
 streamlit>=1.12
 
-[:python_full_version == "3.9.7"]
-streamlit==1.11
-
 [:python_version < "3.10"]
 importlib_resources
 
 [develop]
 bump2version
 ruff
 pre-commit
 yapf
 mypy
-coverage
+coverage[toml]
 nbmake
 pytest
 pytest-dependency
 pycodestyle
 
 [docs]
 matplotlib
```

