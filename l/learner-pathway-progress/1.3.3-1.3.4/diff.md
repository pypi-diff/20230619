# Comparing `tmp/learner-pathway-progress-1.3.3.tar.gz` & `tmp/learner-pathway-progress-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learner-pathway-progress-1.3.3.tar", last modified: Tue Oct 11 08:42:28 2022, max compression
+gzip compressed data, was "learner-pathway-progress-1.3.4.tar", last modified: Mon Jun 19 09:17:04 2023, max compression
```

## Comparing `learner-pathway-progress-1.3.3.tar` & `learner-pathway-progress-1.3.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35139 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8854 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4226 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     7271 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/management/commands/update_all_pathways_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/management/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5545 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/management/tests/test_update_all_pathways_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0002_historicallearnerpathwayprogress_learnerpathwayprogress.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0003_auto_20220901_0616.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0004_auto_20220907_0316.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0005_auto_20221007_0758.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/learner_pathway_progress/templates/learner_pathway_progress/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/templates/learner_pathway_progress/base.html
--rw-r--r--   0 runner    (1001) docker     (121)    11705 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/learner_pathway_progress/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.266024 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8854 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-11 08:42:28.000000 learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-10-11 08:42:28.270025 learner-pathway-progress-1.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     5203 2022-10-11 08:42:25.000000 learner-pathway-progress-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     2326 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.269362 learner-pathway-progress-1.3.4/learner_pathway_progress/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7271 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/commands/update_all_pathways_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/commands/update_existing_pathways_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/management/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/tests/test_update_all_pathways_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/management/tests/test_update_existing_pathways_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0002_historicallearnerpathwayprogress_learnerpathwayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0003_auto_20220901_0616.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0004_auto_20220907_0316.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0005_auto_20221007_0758.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.269362 learner-pathway-progress-1.3.4/learner_pathway_progress/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress/templates/learner_pathway_progress/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/templates/learner_pathway_progress/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)    12040 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/learner_pathway_progress/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9032 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-19 09:17:04.000000 learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-19 09:17:04.273362 learner-pathway-progress-1.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5203 2023-06-19 09:16:56.000000 learner-pathway-progress-1.3.4/setup.py
```

### Comparing `learner-pathway-progress-1.3.3/CHANGELOG.rst` & `learner-pathway-progress-1.3.4/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[1.3.4]- 2023-06-16
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added management command to update existing LearnerPathwayProgress table.
+
 [1.3.3]- 2022-10-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Added a data migration to delete data for LearnerEnterprisePathwayMembership and LearnerPathwayProgress table.
 
 [1.3.2]- 2022-09-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Added enterprise with learner pathway membership.
```

### Comparing `learner-pathway-progress-1.3.3/LICENSE.txt` & `learner-pathway-progress-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/PKG-INFO` & `learner-pathway-progress-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: learner-pathway-progress
-Version: 1.3.3
+Version: 1.3.4
 Summary: A plugin to track learners progress in pathways.
 Home-page: https://github.com/edx/learner-pathway-progress
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: Learner Pathway Progress
         =============================
@@ -145,14 +145,18 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [1.3.4]- 2023-06-16
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        * Added management command to update existing LearnerPathwayProgress table.
+        
         [1.3.3]- 2022-10-07
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         * Added a data migration to delete data for LearnerEnterprisePathwayMembership and LearnerPathwayProgress table.
         
         [1.3.2]- 2022-09-07
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         * Added enterprise with learner pathway membership.
```

### Comparing `learner-pathway-progress-1.3.3/README.rst` & `learner-pathway-progress-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/admin.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/admin.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/api/filters.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/api/filters.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/api/serializers.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/api/serializers.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/api/v1/views.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/apps.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/apps.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/management/commands/update_all_pathways_progress.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/management/commands/update_all_pathways_progress.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/management/tests/test_update_all_pathways_progress.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/management/tests/test_update_all_pathways_progress.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0001_initial.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0002_historicallearnerpathwayprogress_learnerpathwayprogress.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0002_historicallearnerpathwayprogress_learnerpathwayprogress.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0003_auto_20220901_0616.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0003_auto_20220901_0616.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0004_auto_20220907_0316.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0004_auto_20220907_0316.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/migrations/0005_auto_20221007_0758.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/migrations/0005_auto_20221007_0758.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/models.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/models.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/signals.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/signals.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/templates/learner_pathway_progress/base.html` & `learner-pathway-progress-1.3.4/learner_pathway_progress/templates/learner_pathway_progress/base.html`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/utilities.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 )
 from openedx.core.djangoapps.catalog.utils import get_catalog_api_client as create_catalog_api_client
 from openedx.core.djangoapps.catalog.utils import get_programs
 from requests.exceptions import HTTPError
 
 from learner_pathway_progress import models
 from learner_pathway_progress.constants import CHUNK_SIZE, PATHWAY_LOGS_IDENTIFIER
+from learner_pathway_progress.models import LearnerPathwayProgress
 
 log = getLogger(__name__)
 
 User = get_user_model()
 
 
 def get_learner_pathways_associated_with_course(user, course_key):
@@ -222,14 +223,21 @@
         program_courses = program.get('courses') or []
         for program_course in program_courses:
             program_course_runs = program_course.get('course_runs') or []
             for program_course_run in program_course_runs:
                 pathway_course_runs.append(program_course_run['key'])
 
 
+def update_existing_pathways_progress():
+    """Update progress of all existing pathways."""
+    learner_pathway_progress = LearnerPathwayProgress.objects.all()
+    for pathway_progress in learner_pathway_progress:
+        pathway_progress.update_pathway_progress()
+
+
 def update_progress_all_pathways():
     """Update progress of all pathways."""
     user, _ = check_catalog_integration_and_get_user(
         error_message_field='Call to fetch pathways from pathway progress management command'
     )
     if user:
         learner_pathways = get_all_learner_pathways(user.id)
```

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress/waffle.py` & `learner-pathway-progress-1.3.4/learner_pathway_progress/waffle.py`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/PKG-INFO` & `learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: learner-pathway-progress
-Version: 1.3.3
+Version: 1.3.4
 Summary: A plugin to track learners progress in pathways.
 Home-page: https://github.com/edx/learner-pathway-progress
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: Learner Pathway Progress
         =============================
@@ -145,14 +145,18 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [1.3.4]- 2023-06-16
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        * Added management command to update existing LearnerPathwayProgress table.
+        
         [1.3.3]- 2022-10-07
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         * Added a data migration to delete data for LearnerEnterprisePathwayMembership and LearnerPathwayProgress table.
         
         [1.3.2]- 2022-09-07
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         * Added enterprise with learner pathway membership.
```

### Comparing `learner-pathway-progress-1.3.3/learner_pathway_progress.egg-info/SOURCES.txt` & `learner-pathway-progress-1.3.4/learner_pathway_progress.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 learner_pathway_progress/api/urls.py
 learner_pathway_progress/api/v1/__init__.py
 learner_pathway_progress/api/v1/urls.py
 learner_pathway_progress/api/v1/views.py
 learner_pathway_progress/management/__init__.py
 learner_pathway_progress/management/commands/__init__.py
 learner_pathway_progress/management/commands/update_all_pathways_progress.py
+learner_pathway_progress/management/commands/update_existing_pathways_progress.py
 learner_pathway_progress/management/tests/__init__.py
 learner_pathway_progress/management/tests/test_update_all_pathways_progress.py
+learner_pathway_progress/management/tests/test_update_existing_pathways_progress.py
 learner_pathway_progress/migrations/0001_initial.py
 learner_pathway_progress/migrations/0002_historicallearnerpathwayprogress_learnerpathwayprogress.py
 learner_pathway_progress/migrations/0003_auto_20220901_0616.py
 learner_pathway_progress/migrations/0004_auto_20220907_0316.py
 learner_pathway_progress/migrations/0005_auto_20221007_0758.py
 learner_pathway_progress/migrations/__init__.py
 learner_pathway_progress/templates/learner_pathway_progress/base.html
```

### Comparing `learner-pathway-progress-1.3.3/requirements/constraints.txt` & `learner-pathway-progress-1.3.4/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `learner-pathway-progress-1.3.3/setup.py` & `learner-pathway-progress-1.3.4/setup.py`

 * *Files identical despite different names*

