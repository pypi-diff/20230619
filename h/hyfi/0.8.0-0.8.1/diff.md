# Comparing `tmp/hyfi-0.8.0.tar.gz` & `tmp/hyfi-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.8.0.tar", max compression
+gzip compressed data, was "hyfi-0.8.1.tar", max compression
```

## Comparing `hyfi-0.8.0.tar` & `hyfi-0.8.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1071 2023-06-18 12:24:27.497927 hyfi-0.8.0/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-18 12:24:27.497927 hyfi-0.8.0/README.md
--rw-r--r--   0        0        0     4592 2023-06-18 12:24:55.180192 hyfi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3804 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      647 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9858 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      735 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-18 12:24:55.096186 hyfi-0.8.0/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3182 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-18 12:24:55.096186 hyfi-0.8.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      407 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      396 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      132 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      195 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3045 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8363 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4535 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     6610 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    22023 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7618 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3487 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2636 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30789 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      219 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     3220 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     1897 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     4649 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5874 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     4544 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5234 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     6948 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/dataframe.py
--rw-r--r--   0        0        0     5667 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     6215 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/file.py
--rw-r--r--   0        0        0    10015 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3766 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4162 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     2002 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9981 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5584 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 08:19:13.066612 hyfi-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-19 08:19:13.066612 hyfi-0.8.1/README.md
+-rw-r--r--   0        0        0     4608 2023-06-19 08:19:36.907040 hyfi-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      647 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9823 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      735 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-19 08:19:36.835039 hyfi-0.8.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3339 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-19 08:19:36.835039 hyfi-0.8.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      153 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3045 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8363 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4535 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     6610 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    20944 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7618 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3512 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2636 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30789 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2365 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      949 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     3758 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5335 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4013 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5089 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     6948 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/dataframe.py
+-rw-r--r--   0        0        0     5667 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     6215 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0    10015 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3767 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4162 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     2002 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9981 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5584 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 hyfi-0.8.1/PKG-INFO
```

### Comparing `hyfi-0.8.0/LICENSE` & `hyfi-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/README.md` & `hyfi-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/pyproject.toml` & `hyfi-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.8.0"
+version = "0.8.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -15,38 +15,38 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
 pydantic = "^1.10.7"
 chardet = "<=5.1.0"
-pandas = "^1.5.3"
+pandas = ">=1.5.3,<=2.0.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
-numpy = "<1.24"
+numpy = "<=1.24.3"
 python-dotenv = "^1.0.0"
 requests = "^2.27.1"
 tqdm = "^4.64.1"
 colorama = "^0.4.3"
 pathspec = ">=0.9.0"
-filelock = ">=3.4,<3.10"
+filelock = ">=3.4,<=3.12.2"
 rich = ">=12.1,<14.0"
 gdown = "<=4.6.6"
-huggingface-hub = ">=0.8.1,<0.13.0"
+huggingface-hub = ">=0.8.1,<=0.15.1"
 # google-cloud-storage = ">=1.32.0,<3.0"
 # boto3 = ">=1.0,<2.0"
 click = "^8.1.3"
 
 [tool.poetry.group.ipython]
 optional = true
 
 [tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
-ipython = "<=8.12.0"
+ipython = "<=8.12.2"
 ipython-autotime = "^0.3.1"
 ipywidgets = "^8.0.6"
 
 [tool.poetry.extras]
 ipython = ["ipython", "ipython-autotime", "ipywidgets"]
 
 [tool.poetry.group.mkdocs]
```

### Comparing `hyfi-0.8.0/src/hyfi/__cli__.py` & `hyfi-0.8.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/__click__.py` & `hyfi-0.8.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/__global__/__init__.py` & `hyfi-0.8.1/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/__global__/config.py` & `hyfi-0.8.1/src/hyfi/__global__/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from omegaconf import DictConfig
 from pydantic import BaseModel, root_validator, validator
 
 from hyfi.__global__ import __about__, __hydra_config__
 from hyfi.about import AboutConfig
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import _compose
+from hyfi.hydra import Composer
 from hyfi.project import ProjectConfig
 from hyfi.task import TaskConfig
 from hyfi.utils.env import check_and_set_osenv, expand_posix_vars
 from hyfi.utils.logging import getLogger, setLogger
 from hyfi.utils.notebook import load_extentions, set_matplotlib_formats
 
 logger = getLogger(__name__)
@@ -196,15 +196,15 @@
         # Set the retina matplotlib formats.
         if retina:
             set_matplotlib_formats("retina")
         self.initialize()
 
     def initialize(self, config: Union[DictConfig, Dict, None] = None):
         """
-        Initialize hyfi. This is called by : meth : ` __init__ ` to perform initialisation.
+        Initialize hyfi.
 
         Args:
                 config: Configuration dictionary or None.
 
         Returns:
                 A boolean indicating whether initialization was successful
         """
@@ -214,18 +214,19 @@
             return
         __hydra_config__.hyfi_config_module = self.hyfi_config_module
         __hydra_config__.hyfi_config_path = self.hyfi_config_path
         __hydra_config__.hyfi_user_config_path = self.hyfi_user_config_path
 
         # If config is not set the default config is used.
         if config is None:
-            config = _compose(
-                overrides=["+project=__init__"], config_module=__about__.config_module
-            )
             logger.debug("Using default config.")
+            config = Composer(
+                overrides=["+project=__init__"],
+                config_module=__about__.config_module,
+            ).config_as_dict
 
         # Skip project config initialization.
         if "project" not in config:
             logger.info("No project config found, skip project config initialization.")
             return
         self.project = ProjectConfig(**config["project"])
         # self.project.init_project()
```

### Comparing `hyfi-0.8.0/src/hyfi/__init__.py` & `hyfi-0.8.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/about/__init__.py` & `hyfi-0.8.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/batch/__init__.py` & `hyfi-0.8.1/src/hyfi/batch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 import random
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Union
 
-from pydantic import BaseModel, validator
+from pydantic import validator
 
-from hyfi.hydra import _compose
+from hyfi.hydra import BaseConfig, Composer
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class BatchConfig(BaseModel):
+class BatchConfig(BaseConfig):
     config_name: str = "__init__"
+    config_group: str = "batch"
+
     batch_name: str
-    batch_num: Optional[int] = None
+    batch_num: int = -1
     batch_root: str = "outputs"
     output_suffix: str = ""
-    output_extention: Optional[str] = ""
+    output_extention: str = ""
     random_seed: bool = True
     seed: int = -1
     resume_run: bool = False
     resume_latest: bool = False
     device: str = "cpu"
     num_devices: int = 1
     num_workers: int = 1
     config_yaml = "config.yaml"
     config_json = "config.json"
     config_dirname = "configs"
     verbose: Union[bool, int] = False
 
-    def __init__(
-        self,
-        config_name: str = "__init__",
-        **data: Any,
-    ):
-        data = _compose(
-            f"batch={config_name}",
-            config_data=data,
-        )  # type: ignore
-        super().__init__(**data)
+    def initialize_configs(self, **data):
+        super().initialize_configs(**data)
         self.init_batch_num()
 
     def init_batch_num(self):
         if self.batch_num is None:
+            self.batch_num = -1
+        if self.batch_num < 0:
             num_files = len(list(self.config_dir.glob(self.config_filepattern)))
             self.batch_num = num_files - 1 if self.resume_latest else num_files
         if self.verbose:
             logger.info(
                 "Init batch - Batch name: %s, Batch num: %s",
                 self.batch_name,
                 self.batch_num,
@@ -58,15 +54,23 @@
             random.seed()
             seed = random.randint(0, 2**32 - 1)
             if values.get("verbose"):
                 logger.info(f"Setting seed to {seed}")
             return seed
         return v
 
-    @validator("output_extention")
+    @validator("batch_num", pre=True, always=True)
+    def _validate_batch_num(cls, v):
+        return v or -1
+
+    @validator("output_suffix", pre=True, always=True)
+    def _validate_output_suffix(cls, v):
+        return v or ""
+
+    @validator("output_extention", pre=True, always=True)
     def _validate_output_extention(cls, v):
         return v.strip(".") if v else ""
 
     @property
     def root_dir(self):
         return Path(self.batch_root)
```

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/__init__.py` & `hyfi-0.8.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.8.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.8.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.8.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.8.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.8.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.8.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/copier/__init__.py` & `hyfi-0.8.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/dotenv/__init__.py` & `hyfi-0.8.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/graphics/collage.py` & `hyfi-0.8.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/graphics/motion.py` & `hyfi-0.8.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/graphics/utils.py` & `hyfi-0.8.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/hydra/__init__.py` & `hyfi-0.8.1/src/hyfi/hydra/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 
 from hyfi.__global__ import (
     __about__,
     __hydra_config__,
     __hydra_default_config_group_value__,
     __hydra_version_base__,
 )
-from hyfi.utils.logging import getLogger
+from hyfi.utils.logging import getLogger, setLogger
 
+if level := os.environ.get("HYFI_LOG_LEVEL"):
+    setLogger(level)
 logger = getLogger(__name__)
 
 DictKeyType = Union[str, int, Enum, float, bool]
 
 
 class SpecialKeys(str, Enum):
     """Special keys in configs used by hyfi."""
@@ -232,15 +234,15 @@
             cfg: The config to convert.
 
         Returns:
             The dict representation of the config.
         """
         # Convert a config object to a config object.
         if isinstance(cfg, dict):
-            cfg = _to_config(cfg)
+            cfg = Composer.to_config(cfg)
         # Returns a container for the given config.
         if isinstance(cfg, (DictConfig, ListConfig)):
             return OmegaConf.to_container(
                 cfg,
                 resolve=True,
                 throw_on_missing=False,
                 structured_config_mode=SCMode.DICT,
@@ -330,15 +332,15 @@
         if group_key and group_value:
             # Initialize hydra configuration module.
             cfg = Composer.hydra_compose(
                 root_config_name=root_config_name,
                 config_module=config_module,
                 overrides=overrides,
             )
-            cfg = _select(
+            cfg = Composer.select(
                 cfg,
                 key=group_key,
                 default=None,
                 throw_on_missing=False,
                 throw_on_resolution_failure=False,
             )
             override = config_group if cfg is not None else f"+{config_group}"
@@ -393,15 +395,15 @@
 
     @staticmethod
     def print(cfg: Any, resolve: bool = True, **kwargs):
         import pprint
 
         if Composer.is_config(cfg):
             if resolve:
-                pprint.pprint(_to_dict(cfg), **kwargs)
+                pprint.pprint(Composer.to_dict(cfg), **kwargs)
             else:
                 pprint.pprint(cfg, **kwargs)
         else:
             print(cfg)
 
     @staticmethod
     def is_config(
@@ -484,15 +486,15 @@
         :return: the merged config object.
         """
         return OmegaConf.merge(*configs)
 
     @staticmethod
     def to_yaml(cfg: Any, resolve: bool = False, sort_keys: bool = False) -> str:
         if resolve:
-            cfg = _to_dict(cfg)
+            cfg = Composer.to_dict(cfg)
         return OmegaConf.to_yaml(cfg, resolve=resolve, sort_keys=sort_keys)
 
     @staticmethod
     def to_container(
         cfg: Any,
         resolve: bool = False,
         throw_on_missing: bool = False,
@@ -581,77 +583,48 @@
         if callable(_fn):
             args = getargspec(_fn).args
             logger.info(f"args of {_fn}: {args}")
             return {k: v for k, v in _kwargs.items() if k in args}
         return _kwargs
 
 
-def _compose(
-    config_group: Union[str, None] = None,
-    overrides: Union[List[str], None] = None,
-    config_data: Union[Dict[str, Any], DictConfig, None] = None,
-    return_as_dict: bool = True,
-    throw_on_resolution_failure: bool = True,
-    throw_on_missing: bool = False,
-    root_config_name: Union[str, None] = None,
-    config_module: Union[str, None] = None,
-    global_package: bool = False,
-    verbose: bool = False,
-) -> Union[DictConfig, Dict]:  # sourcery skip: low-code-quality
-    """
-    Compose a configuration by applying overrides
+class BaseConfig(BaseModel):
+    config_name: str = "__init__"
+    config_group: str = ""
 
-    Args:
-        config_group: Name of the config group to compose (`config_group=name`)
-        overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
-        config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
-        return_as_dict: Return the result as a dict
-        throw_on_resolution_failure: If True throw an exception if resolution fails
-        throw_on_missing: If True throw an exception if config_group doesn't exist
-        root_config_name: Name of the root config to be used (e.g. `hconf`)
-        config_module: Module of the config to be used (e.g. `hyfi.conf`)
-        global_package: If True, the config assumed to be a global package
-        verbose: If True print configuration to stdout
+    class Config:
+        arbitrary_types_allowed = True
+        extra = "allow"
+        validate_assignment = True
+        exclude = {}
+        include = {}
+        underscore_attrs_are_private = True
+        property_set_methods = {}
 
-    Returns:
-        A config object or a dictionary with the composed config
-    """
-    cmpsr = Composer(
-        config_group=config_group,
-        overrides=overrides,
-        config_data=config_data,
-        throw_on_resolution_failure=throw_on_resolution_failure,
-        throw_on_missing=throw_on_missing,
-        config_name=root_config_name,
-        config_module=config_module,
-        global_package=global_package,
-        verbose=verbose,
-    )
-    return cmpsr.config_as_dict if return_as_dict else cmpsr.config
-
-
-def _select(
-    cfg: Any,
-    key: str,
-    default: Any = None,
-    throw_on_resolution_failure: bool = True,
-    throw_on_missing: bool = False,
-):
-    return Composer.select(
-        cfg=cfg,
-        key=key,
-        default=default,
-        throw_on_resolution_failure=throw_on_resolution_failure,
-        throw_on_missing=throw_on_missing,
-    )
-
-
-def _to_dict(
-    cfg: Any,
-) -> Any:
-    return Composer.to_dict(cfg)
-
-
-def _to_config(
-    cfg: Any,
-) -> Union[DictConfig, ListConfig]:
-    return Composer.to_config(cfg)
+    def __init__(self, **data):
+        super().__init__(**data)
+        self.initialize_configs(**data)
+
+    def __setattr__(self, key, val):
+        super().__setattr__(key, val)
+        if method := self.__config__.property_set_methods.get(key):  # type: ignore
+            getattr(self, method)(val)
+
+    def initialize_configs(
+        self,
+        **data,
+    ):
+        if not self.config_group:
+            logger.info("There is no config group specified.")
+            return
+        # Initialize the config with the given config_name.
+        logger.info(
+            "Initializing `%s` class with `%s` config in `%s` group.",
+            self.__class__.__name__,
+            self.config_name,
+            self.config_group,
+        )
+        data = Composer(
+            config_group=f"{self.config_group}={self.config_name}",
+            config_data=data,
+        ).config_as_dict
+        self.__dict__.update(data)
```

### Comparing `hyfi-0.8.0/src/hyfi/hydra/main.py` & `hyfi-0.8.1/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/joblib/__init__.py` & `hyfi-0.8.1/src/hyfi/joblib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 
 from pydantic import BaseModel
 
 from hyfi.__global__ import __about__
-from hyfi.hydra import _compose
+from hyfi.hydra import BaseConfig, Composer
 from hyfi.joblib.batch import batcher
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class DistFramwork(BaseModel):
+class DistFramworkConfig(BaseModel):
     """Distributed Framework Configuration"""
 
     backend: str = "joblib"
     initialize: bool = False
     num_workers: int = 1
 
 
@@ -25,38 +25,35 @@
     minibatch_size: int = 1_000
     backend: str = "joblib"
     task_num_cpus: int = 1
     task_num_gpus: int = 0
     verbose: int = 10
 
 
-class JobLibConfig(BaseModel):
+class JobLibConfig(BaseConfig):
     """JobLib Configuration"""
 
     config_name: str = "__init__"
+    config_group: str = "joblib"
+
     num_workers: int = 1
-    distributed_framework: DistFramwork = DistFramwork()
+    distributed_framework: DistFramworkConfig = DistFramworkConfig()
     batcher: BatcherConfig = BatcherConfig()
     __initilized__: bool = False
 
     class Config:
         extra = "allow"
         underscore_attrs_are_private = True
 
-    def __init__(
-        self,
-        config_name: str = "__init__",
-        **data: Any,
-    ):
-        data = _compose(
-            f"joblib={config_name}",
-            config_data=data,
-            config_module=__about__.config_module,
-        )  # type: ignore
-        super().__init__(config_name=config_name, **data)
+    def initialize_configs(self, **data):
+        super().initialize_configs(**data)
+        self.batcher = BatcherConfig.parse_obj(self.__dict__["batcher"])
+        self.distributed_framework = DistFramworkConfig.parse_obj(
+            self.__dict__["distributed_framework"]
+        )
 
     def init_backend(
         self,
     ):
         """Initialize the backend for joblib"""
         if self.distributed_framework.initialize:
             backend_handle = None
```

### Comparing `hyfi-0.8.0/src/hyfi/joblib/batch/apply.py` & `hyfi-0.8.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.8.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.8.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/joblib/pipe.py` & `hyfi-0.8.1/src/hyfi/joblib/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/main/__init__.py` & `hyfi-0.8.1/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/project/__init__.py` & `hyfi-0.8.1/src/hyfi/project/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 from pathlib import Path
 from typing import Any, Union
 
-from pydantic import BaseModel, validator
+from pydantic import validator
 
 from hyfi.__global__ import __about__
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import Composer
+from hyfi.hydra import BaseConfig
 from hyfi.joblib import JobLibConfig
 from hyfi.path import PathConfig
 from hyfi.utils.logging import getLogger
 from hyfi.utils.notebook import is_notebook
 
 logger = getLogger(__name__)
 
 
-class ProjectConfig(BaseModel):
+class ProjectConfig(BaseConfig):
     """Project Config"""
 
     config_name: str = "__init__"
+    config_group: str = "project"
+    # Project Config
     project_name: str = "hyfi-project"
     task_name: str = ""
     project_description: str = ""
     project_root: str = ""
     project_workspace_name: str = "workspace"
     global_hyfi_root: str = ""
     global_workspace_name: str = "workspace"
@@ -52,43 +54,20 @@
                 v = True
             elif v.lower() in {"false", "0"}:
                 v = False
             else:
                 raise ValueError("verbose must be a boolean or a string of 0 or 1")
         return v
 
-    def __init__(
-        self,
-        config_name: str = "__init__",
-        config_group: str = "project",
-        **data: Any,
-    ):
-        super().__init__(**data)
-        self.initialize_configs(
-            config_name=config_name,
-            config_group=config_group,
-            **data,
-        )
-
-    def initialize_configs(
-        self,
-        config_name: str = "__init__",
-        config_group: str = "project",
-        **data,
-    ):
-        # Initialize the config with the given config_name.
-        data = Composer(
-            config_group=f"{config_group}={config_name}",
-            config_data=data,
-        ).config_as_dict
-        self.__dict__.update(data)
+    def initialize_configs(self, **data):
+        super().initialize_configs(**data)
 
         self.dotenv = DotEnvConfig()
-        self.path = PathConfig(**self.__dict__["path"])
-        self.joblib = JobLibConfig(**self.__dict__["joblib"])
+        self.path = PathConfig.parse_obj(self.__dict__["path"])
+        self.joblib = JobLibConfig.parse_obj(self.__dict__["joblib"])
 
         self.dotenv.HYFI_PROJECT_NAME = self.project_name
         self.dotenv.HYFI_TASK_NAME = self.task_name
         self.dotenv.HYFI_PROJECT_DESC = self.project_description
         self.dotenv.HYFI_PROJECT_ROOT = self.project_root
         self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
         self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
```

### Comparing `hyfi-0.8.0/src/hyfi/task/__init__.py` & `hyfi-0.8.1/src/hyfi/task/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from pathlib import Path
 from typing import Union
 
-from pydantic import BaseModel
-
-from hyfi.hydra import Composer
+from hyfi.hydra import BaseConfig, Composer
 from hyfi.module import ModuleConfig
 from hyfi.path.batch import BatchPathConfig
 from hyfi.project import ProjectConfig
 from hyfi.utils.lib import ensure_import_module
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class TaskConfig(BaseModel):
+class TaskConfig(BaseConfig):
     config_name: str = "__init__"
     config_group: str = "task"
+
     task_name: str = "demo-task"
     task_root: str = "tmp/task"
     autoload: bool = False
     version: str = "0.0.0"
     module: ModuleConfig = None  # type: ignore
     path: BatchPathConfig = None  # type: ignore
     project: ProjectConfig = None  # type: ignore
@@ -37,58 +36,35 @@
         include = {}
         underscore_attrs_are_private = True
         property_set_methods = {
             "task_name": "set_task_name",
             "task_root": "set_task_root",
         }
 
-    def __init__(
-        self,
-        config_name: str = "__init__",
-        config_group: str = "task",
-        **data,
-    ):
-        super().__init__(**data)
-        self.initialize_configs(
-            config_name=config_name,
-            config_group=config_group,
-            **data,
-        )
-
     def __setattr__(self, key, val):
         super().__setattr__(key, val)
         if method := self.__config__.property_set_methods.get(key):  # type: ignore
             getattr(self, method)(val)
 
     def set_task_root(self, val: Union[str, Path]):
         if not self.task_root or self.task_root != val:
             self.initialize_configs(task_root=val)
 
     def set_task_name(self, val):
         if not self.task_name or self.task_name != val:
             self.initialize_configs(task_name=val)
 
-    def initialize_configs(
-        self,
-        config_name: str = "__init__",
-        config_group: str = "task",
-        **data,
-    ):
-        # Initialize the config with the given config_name.
-        data = Composer(
-            config_group=f"{config_group}={config_name}",
-            config_data=data,
-        ).config_as_dict
-        self.__dict__.update(data)
-        if "module" in data:
-            self.module = ModuleConfig(**data["module"])
-        if "path" in data:
-            self.path = BatchPathConfig(**data["path"])
-        if "project" in data:
-            self.project = ProjectConfig(**data["project"])
+    def initialize_configs(self, **data):
+        super().initialize_configs(**data)
+        if "module" in self.__dict__:
+            self.module = ModuleConfig.parse_obj(self.__dict__["module"])
+        if "path" in self.__dict__:
+            self.path = BatchPathConfig.parse_obj(self.__dict__["path"])
+        if "project" in self.__dict__:
+            self.project = ProjectConfig.parse_obj(self.__dict__["project"])
 
     @property
     def config(self):
         return self.dict()
 
     @property
     def root_dir(self) -> Path:
```

### Comparing `hyfi-0.8.0/src/hyfi/task/batch.py` & `hyfi-0.8.1/src/hyfi/task/batch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,63 @@
+from typing import Dict, List, Union
+
 from omegaconf import DictConfig
 
 from hyfi.batch import BatchConfig
 from hyfi.hydra.main import XC
 from hyfi.task import TaskConfig
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class BatchTaskConfig(TaskConfig):
+    config_name: str = "__batch__"
+    config_group: str = "task"
+
     batch_name: str = "demo"
     batch: BatchConfig = None  # type: ignore
 
     class Config:
         arbitrary_types_allowed = True
         extra = "allow"
         validate_assignment = False
         exclude = {
             "_config_",
             "_initial_config_",
             "__data__",
             "path",
             "module",
-            "secret",
-            "auto",
             "project",
         }
         include = {}
         underscore_attrs_are_private = True
         property_set_methods = {
-            "name": "set_name",
-            "batch_name": "set_name",
+            "task_name": "set_task_name",
+            "task_root": "set_task_root",
+            "batch_name": "set_batch_name",
             "batch_num": "set_batch_num",
-            "root_dir": "set_root_dir",
         }
 
-    def __init__(self, **args):
-        super().__init__(**args)
-
     def set_batch_name(self, val):
-        super().set_task_name(val)
-        self._config_.batch.batch_name = val
-        self.batch.batch_name = val
-        self.initialize_configs(name=val)
+        self.initialize_configs(batch_name=val)
 
     def set_batch_num(self, val):
-        self._config_.batch.batch_num = val
         self.batch.batch_num = val
 
-    def initialize_configs(
-        self,
-        task_root: str = "",
-        batch_config_class=BatchConfig,
-        **kwargs,
-    ):
-        super().initialize_configs(task_root=task_root, **kwargs)
-
-        self.batch = batch_config_class(**self.config.batch)
-        self.batch_num = self.batch.batch_num
-        # if self.project.use_huggingface_hub:
-        #     self.secrets.init_huggingface_hub()
-        if self.verbose:
-            logger.info(
-                f"Initalized batch: {self.batch_name}({self.batch_num}) in {self.root_dir}"
-            )
+    def initialize_configs(self, **data):
+        super().initialize_configs(**data)
+        if "batch" in self.__dict__ and self.__dict__["batch"]:
+            self.batch = BatchConfig.parse_obj(self.__dict__["batch"])
+        logger.info(
+            "Initalized batch: %s(%s) in %s",
+            self.batch_name,
+            self.batch_num,
+            self.batch_dir,
+        )
 
     @property
     def batch_num(self):
         return self.batch.batch_num
 
     @property
     def seed(self):
@@ -79,101 +69,108 @@
 
     @property
     def dataset_dir(self):
         return self.path.dataset_dir
 
     @property
     def verbose(self):
-        return self.batch.verbose
+        return self.project.verbose
 
     @property
     def device(self):
         return self.batch.device
 
     @property
     def num_devices(self):
         return self.batch.num_devices
 
     def save_config(
         self,
-        config=None,
-        exclude=None,
-        include=None,
+        config: Union[DictConfig, Dict, None] = None,
+        exclude: Union[str, List[str], None] = None,
+        include: Union[str, List[str], None] = None,
     ):
         """Save the batch config"""
-        if config is not None:
-            self._config_ = config
-        logger.info(f"Saving config to {self.batch.config_filepath}")
-        cfg = XC.to_dict(self.config)
-        if exclude is None:
-            exclude = self.__config__.exclude
+        if not config:
+            config = self.__dict__
+        logger.info(
+            "Saving config to %s",
+            self.batch.config_filepath,
+        )
+        cfg = XC.to_dict(config)
+        if not exclude:
+            exclude = self.__config__.exclude  # type: ignore
 
         if include:
             if isinstance(include, str):
                 include = [include]
-            args = {key: cfg[key] for key in include}
+            config_to_save = {key: cfg[key] for key in include}
         else:
-            args = cfg
+            config_to_save = cfg
             if exclude:
                 if isinstance(exclude, str):
                     exclude = [exclude]
                 for key in exclude:
-                    args.pop(key, None)
-        XC.save(args, self.batch.config_filepath)
+                    config_to_save.pop(key, None)
+        XC.save(config_to_save, self.batch.config_filepath)
         self.save_settings(exclude=exclude)
         return self.batch.config_filename
 
     def save_settings(self, exclude=None, exclude_none=True):
         def dumper(obj):
             return XC.to_dict(obj) if isinstance(obj, DictConfig) else str(obj)
 
         if exclude is None:
-            exclude = self.__config__.exclude
+            exclude = self.__config__.exclude  # type: ignore
         config = self.dict(exclude=exclude, exclude_none=exclude_none)
         if self.verbose:
-            logger.info(f"Saving config to {self.batch.config_jsonpath}")
+            logger.info(
+                "Saving config to %s",
+                self.batch.config_jsonpath,
+            )
         XC.save_json(config, self.batch.config_jsonpath, default=dumper)
 
     def load_config(
         self,
-        batch_name=None,
-        batch_num=None,
-        **args,
+        batch_name: str = "",
+        batch_num: int = -1,
+        **data,
     ):
         """Load the config from the batch config file"""
         if self.verbose:
             logger.info(
-                f"> Loading config for batch_name: {batch_name} batch_num: {batch_num}"
+                "> Loading config for batch_name: %s batch_num: %s",
+                batch_name,
+                batch_num,
             )
-        # self.config.batch.batch_num = batch_num
-        if batch_name is None:
+        if not batch_name:
             batch_name = self.batch_name
 
-        if batch_num is not None:
-            cfg = self._initial_config_.copy()
-            self.batch.batch_name = batch_name
-            self.batch.batch_num = batch_num
-            _path = self.batch.config_filepath
+        if batch_num is None:
+            batch_num = -1
+        cfg = self.__dict__.copy()
+        if batch_num >= 0:
+            batch = BatchConfig(batch_name=batch_name, batch_num=batch_num)
+            _path = batch.config_filepath
             if _path.is_file():
-                logger.info(f"Loading config from {_path}")
+                logger.info("Loading config from %s", _path)
                 batch_cfg = XC.load(_path)
-                if self.verbose:
-                    logger.info("Merging config with the loaded config")
+                logger.info("Merging config with the loaded config")
                 cfg = XC.merge(cfg, batch_cfg)
             else:
-                logger.info(f"No config file found at {_path}")
-                batch_num = None
-        else:
-            cfg = self.config
-
+                logger.info("No config file found at %s", _path)
+                batch_num = -1
         if self.verbose:
-            logger.info(f"Merging config with args: {args}")
-        self._config_ = XC.merge(cfg, args)
+            logger.info("Merging config with args: %s", data)
+        cfg = XC.to_dict(XC.merge(cfg, data))
 
-        self.batch_num = batch_num
-        self.batch_name = batch_name
+        self.initialize_configs(**cfg)
 
         return self.config
 
-    def show_config(self, batch_name=None, batch_num=None):
+    def print_config(
+        self,
+        batch_name: str = "",
+        batch_num: int = -1,
+    ):
         self.load_config(batch_name, batch_num)
         XC.print(self.dict())
```

### Comparing `hyfi-0.8.0/src/hyfi/utils/dataframe.py` & `hyfi-0.8.1/src/hyfi/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/env.py` & `hyfi-0.8.1/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/file.py` & `hyfi-0.8.1/src/hyfi/utils/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/func.py` & `hyfi-0.8.1/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/google.py` & `hyfi-0.8.1/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/gpu.py` & `hyfi-0.8.1/src/hyfi/utils/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from hyfi.utils.notebook import clear_output
 
 logger = getLogger(__name__)
 
 try:
     import GPUtil  # type: ignore
 except ImportError:
-    logger.info("GPUtil not found. Please install it to use GPU utilities.")
+    logger.debug("GPUtil not found. Please install it to use GPU utilities.")
 
 
 class GPUMon(Thread):
     """Monitor GPU usage in a separate thread"""
 
     def __init__(self, delay=10, show_current_time=True, clear_output=True):
         super(GPUMon, self).__init__()
```

### Comparing `hyfi-0.8.0/src/hyfi/utils/lib.py` & `hyfi-0.8.1/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/logging.py` & `hyfi-0.8.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/notebook.py` & `hyfi-0.8.1/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/src/hyfi/utils/tools.py` & `hyfi-0.8.1/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.0/PKG-INFO` & `hyfi-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.8.0
+Version: 0.8.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -12,22 +12,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ipython
 Requires-Dist: chardet (<=5.1.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
-Requires-Dist: filelock (>=3.4,<3.10)
+Requires-Dist: filelock (>=3.4,<=3.12.2)
 Requires-Dist: gdown (<=4.6.6)
-Requires-Dist: huggingface-hub (>=0.8.1,<0.13.0)
+Requires-Dist: huggingface-hub (>=0.8.1,<=0.15.1)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (<1.24)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: numpy (<=1.24.3)
+Requires-Dist: pandas (>=1.5.3,<=2.0.2)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.1,<14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
```

