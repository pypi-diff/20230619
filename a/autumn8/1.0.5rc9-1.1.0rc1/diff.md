# Comparing `tmp/autumn8-1.0.5rc9.tar.gz` & `tmp/autumn8-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc9.tar", last modified: Tue May 16 16:05:51 2023, max compression
+gzip compressed data, was "autumn8-1.1.0rc1.tar", last modified: Mon Jun 19 13:20:56 2023, max compression
```

## Comparing `autumn8-1.0.5rc9.tar` & `autumn8-1.1.0rc1.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc9/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.100751 autumn8-1.0.5rc9/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13527 2023-05-16 14:35:59.000000 autumn8-1.0.5rc9/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16235 2023-05-16 16:03:09.000000 autumn8-1.0.5rc9/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-05-16 14:28:29.000000 autumn8-1.0.5rc9/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 16:04:29.000000 autumn8-1.0.5rc9/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc9/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc9/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc9/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc9/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc9/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/tensorflow_custom_layers.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-05-16 16:01:30.000000 autumn8-1.0.5rc9/autumn8/exceptions.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-05-16 14:26:52.000000 autumn8-1.0.5rc9/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc9/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc9/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-05-16 16:01:57.000000 autumn8-1.0.5rc9/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc9/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/types/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1112 2023-05-16 14:30:08.000000 autumn8-1.0.5rc9/autumn8/types/deployment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.100751 autumn8-1.0.5rc9/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1486 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     8030 2023-06-19 12:42:47.000000 autumn8-1.1.0rc1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12773 2023-06-19 12:49:40.000000 autumn8-1.1.0rc1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17485 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-06-19 13:20:04.000000 autumn8-1.1.0rc1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7161 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-24 15:09:02.000000 autumn8-1.1.0rc1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.1.0rc1/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.1.0rc1/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.1.0rc1/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.1.0rc1/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.1.0rc1/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/tensorflow_custom_layers.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/exceptions.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       71 2023-06-19 12:42:33.000000 autumn8-1.1.0rc1/autumn8/i18n.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12004 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.1.0rc1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3606 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/service.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       69 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/libenv.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/types/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1924 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/types/deployment.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      464 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/types/router.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1544 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc9/PKG-INFO` & `autumn8-1.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc9
+Version: 1.1.0rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc9/README.md` & `autumn8-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/analyze.py` & `autumn8-1.1.0rc1/autumn8/cli/analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from pathlib import Path, PurePosixPath
 
 from click import ClickException
 
 import autumn8
 from autumn8.lib import logging
 
+from autumn8.i18n import PLEASE_CONTACT_OUR_SUPPORT
+
 sys.path.append(os.getcwd())
 
 PYTHON_FILE_EXTENSION = ".py"
 
 logger = logging.getLogger(__name__)
 
 
@@ -211,20 +213,20 @@
         ".tflite"
     ]:  # TODO - add this extension also to the UI autofiller
         framework = "TFLITE"
         raise ClickException(f"Files with '{extension}' are not supported yet")
 
     elif extension in [".pt", ".pth"]:
         raise ClickException(
-            f"Files with '{extension}' are not supported - please contact us at support@autumn8.ai to add the support."
+            f"Files with '{extension}' are not supported - {PLEASE_CONTACT_OUR_SUPPORT} to add the support."
         )
 
     else:
         raise ClickException(
-            f"Files with '{extension}' are not supported - please contact us at support@autumn8.ai to add the support."
+            f"Files with '{extension}' are not supported - {PLEASE_CONTACT_OUR_SUPPORT} to add the support."
         )
 
     return (
         model_filepath_or_url,
         inferred_model_name,
         framework,
         inferred_quantization,
```

### Comparing `autumn8-1.0.5rc9/autumn8/cli/cli_environment.py` & `autumn8-1.1.0rc1/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/commands/cloud.py` & `autumn8-1.1.0rc1/autumn8/cli/commands/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     coro_click_command,
     get_deployment,
     normalize_args,
     validate_and_ask_about_docker_image_name,
     validate_and_ask_about_schedule,
 )
 from autumn8.common.config.settings import CloudServiceProvider
-from autumn8.common.types import Sla
 from autumn8.lib import api, logging
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(context_settings={"token_normalize_func": normalize_args})
 def cloud_commands_group():
@@ -99,73 +98,54 @@
     help="Schedule the deployment on given date",
 )
 @click.option(
     "--deployment_id",
     type=str,
     help="Update an existing deployment, retaining its URL",
 )
-@click.option(
-    "-b",
-    "--deploy_best",
-    "autopick_machine_by_best_sla",
-    type=click.Choice(list(Sla), case_sensitive=False),
-    help="Let Autumn8 pick the server type automatically for the deployment",
-)
 @options.use_cloud_provider_picker(
     # prompt disabled, as only A8F works atm
     optional=True,
     default_value=CloudServiceProvider.AUTUMN8,
 )
 def deploy(
     organization_id: int,
     model_id: int,
     should_schedule: bool,
     schedule_on: Optional[str],
     deployment_id: Optional[str],
     machine_type: Optional[str],
     environment: CliEnvironment,
     cloud_provider: CloudServiceProvider,
-    autopick_machine_by_best_sla: Optional[Sla],
     quiet,
 ):
     """Deploy a model from AutoDL onto cloud."""
 
-    if machine_type is None and autopick_machine_by_best_sla is None:
+    if machine_type is None:
         machine_type = questionary.text(
             message="Machine type (ie. c5.2xlarge)"
         ).unsafe_ask()
+    if machine_type is None:
+        raise RuntimeError("Machine type was not picked, aborting...")
 
     schedule_on = validate_and_ask_about_schedule(should_schedule, schedule_on)
 
     logger.info(
         "Launching a new deployment with %s...",
-        machine_type or f"best {autopick_machine_by_best_sla}",
+        machine_type,
+    )
+    deployments = cloud_api.deploy(
+        organization_id,
+        environment,
+        machine_type=machine_type,
+        service_provider=cloud_provider,
+        schedule_on=schedule_on,
+        deployment_id=deployment_id,
+        model_id=model_id,
     )
-    if machine_type is not None:
-        deployments = cloud_api.deploy(
-            organization_id,
-            environment,
-            machine_type=machine_type,
-            service_provider=cloud_provider,
-            schedule_on=schedule_on,
-            deployment_id=deployment_id,
-            model_id=model_id,
-        )
-    else:
-        assert autopick_machine_by_best_sla is not None
-
-        deployments = cloud_api.deploy_by_best_sla(
-            organization_id,
-            environment,
-            best_sla=autopick_machine_by_best_sla,
-            service_provider=cloud_provider,
-            schedule_on=schedule_on,
-            deployment_id=deployment_id,
-            model_id=model_id,
-        )
 
     click.echo(json.dumps(deployments, indent=4))
 
 
 @cloud_commands_group.command()
 @options.use_environment
 @options.use_organization_id
@@ -288,15 +268,15 @@
         str
     ] = DEFAULT_DOCKER_CONTAINER_REGISTRY,
     container_http_request_path: str = "",
     custom_headers: List[str] = [],
     # disabled, cause these are not working properly right now on a8f
     # docker_environment: Optional[Dict[str, str]] = None,
     # docker_entrypoint: Optional[str] = None,
-    input: Union[Dict[str, str], List[str], str, None] = None,
+    input: Optional[str] = None,
 ):
     """
     Run an inference on a given Docker image by creating
     a temporary container and calling an HTTP request against it
     """
     machine_type: str = (
         questionary.text(message="Machine type (ie. c5.2xlarge)").unsafe_ask()
@@ -345,16 +325,16 @@
             url=url,
             json={
                 "container_image_name": docker_image_name,
                 "container_registry": docker_container_registry,
                 "container_port": docker_port,
                 "http_request_input": input,
                 "http_request_path": container_http_request_path,
+                "http_request_headers": custom_headers_parsed,
             },
-            headers=custom_headers_parsed,
             timeout=None,
         )
 
         logger.info("Container responded with:")
         click.echo(response.text)
         response.raise_for_status()
```

### Comparing `autumn8-1.0.5rc9/autumn8/cli/commands/models.py` & `autumn8-1.1.0rc1/autumn8/cli/commands/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     announce_model_upload_response,
     normalize_args,
 )
 from autumn8.cli.validation import validate_input_dims_json, validate_input_file
 from autumn8.common.config.settings import supported_quants
 from autumn8.exceptions import UserActionRequiredException
 from autumn8.lib import api, api_creds, logging
-from autumn8.lib import service as autodl
+from autumn8.lib import service as autodl_service
+from autumn8.types.router import NewModelInfo
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
 
 logger = logging.getLogger(__name__)
 
 
@@ -307,15 +308,15 @@
         click.echo(f"{json.dumps(model_config, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
 
-    model_upload_response = autodl.upload_model(
+    model_upload_response = autodl_service.upload_model(
         environment,
         organization_id,
         model_config,
         model_filepath_or_url=model_filepath_or_url,
         input_file_path=input_file,
         max_upload_workers=max_upload_workers,
     )
@@ -326,14 +327,45 @@
 class SupportedModel(str, enum.Enum):
     GPTJ = "gptj"
 
 
 supported_models_by_human_readable_label = {"GPT-J 6B": SupportedModel.GPTJ}
 
 
+def dir_contains_file(dir_filepath: str, filename: str):
+    return any(
+        member_fname == filename for member_fname in os.listdir(dir_filepath)
+    )
+
+
+def sanity_check_if_folder_contains_checkpoint_files(dir_filepath: str):
+    errors: List[str] = []
+    if not any(
+        fname.startswith("pytorch_model") and fname.endswith(".bin")
+        for fname in os.listdir(dir_filepath)
+    ):
+        errors.append("there are no pytorch_model*.bin weight files")
+
+    # if not dir_contains_file(dir_filepath, "generation_config.json"):
+    #     errors.append("the generation_config.json file is missing")
+
+    if not dir_contains_file(dir_filepath, "config.json"):
+        errors.append("the config.json file is missing")
+
+    # if not dir_contains_file(dir_filepath, "pytorch_model.bin.index.json"):
+    #     errors.append("the pytorch_model.bin.index.json file is missing")
+
+    if not len(errors) == 0:
+        error_details_message = ",\n".join(errors)
+
+        raise click.ClickException(
+            f"{dir_filepath} is not a valid checkpoint dir:\n{error_details_message}"
+        )
+
+
 @model_commands_group.command()
 @options.use_environment
 @click.argument("checkpoint_filepath_or_url")
 @common_upload_args
 @click.option(
     "-m",
     "--model_type",
@@ -388,36 +420,39 @@
         input_dims=input_dims,
         input_file=input_file,
         inferred_model_name=inferred_model_name,
         inferred_quantization=inferred_quantization,
         inferred_input_dims=inferred_input_dims,
         should_skip_inputs=should_skip_inputs,
     )
-    model_config = {
-        "name": model_name,
-        "framework": framework,
-        "quantization": quantization,
-        "inputs": input_dims,
-        "group_id": group_id,
-        "model_type": model_type,
-    }
+    model_config = NewModelInfo(
+        name=model_name,
+        framework=framework,
+        quantization=quantization,
+        inputs=input_dims,
+        group_id=group_id,
+        model_file_type=model_type,
+    )
 
     if not auto_confirm:
         logger.info("")
         logger.info("The details for your model are as follows:")
-        click.echo(f"{json.dumps(model_config, indent=4)}")
+        click.echo(f"{json.dumps(model_config.dict(), indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
 
     if os.path.isdir(os.path.abspath(checkpoint_filepath_or_url)):
         # TODO: add zip progress bar
         time_start = time.time()
+        sanity_check_if_folder_contains_checkpoint_files(
+            checkpoint_filepath_or_url
+        )
         logger.info("Zipping the model checkpoint folder, please wait...")
         checkpoint_filepath_or_url = zip_checkpoint_dir(
             os.path.abspath(checkpoint_filepath_or_url), model_name
         )
         checkpoint_filepath_or_url = os.path.abspath(checkpoint_filepath_or_url)
 
         logger.info("Zipping finished in %s seconds", time.time() - time_start)
@@ -427,21 +462,20 @@
     logger.warning(
         "If the upload isn't utilizing the whole network bandwidth, "
         + "please drop the upload and try again with "
         + "the --max_upload_workers flag set to a higher value "
         + "(currently =%s).",
         max_upload_workers,
     )
-    model_upload_response = autodl.upload_model(
+    model_upload_response = autodl_service.upload_model(
         environment,
         organization_id,
         model_config,
         model_filepath_or_url=checkpoint_filepath_or_url,
         input_file_path=input_file,
-        model_type=model_type,
         max_upload_workers=max_upload_workers,
     )
 
     announce_model_upload_response(model_upload_response)
 
 
 @model_commands_group.command()
```

### Comparing `autumn8-1.0.5rc9/autumn8/cli/examples.py` & `autumn8-1.1.0rc1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/interactive.py` & `autumn8-1.1.0rc1/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/main.py` & `autumn8-1.1.0rc1/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/options.py` & `autumn8-1.1.0rc1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/pending_uploads.py` & `autumn8-1.1.0rc1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/cli/validation.py` & `autumn8-1.1.0rc1/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/common/config/cloud_info.py` & `autumn8-1.1.0rc1/autumn8/common/config/cloud_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 # https://github.com/banzaicloud/cloudinfo
 
 import os
 from dataclasses import dataclass
 from http import HTTPStatus
 from typing import Dict, Literal, Optional, Union
 
+import libenv
 import requests
 from fastapi import HTTPException
 
 from autumn8.common.config.settings import CloudServiceProvider
 
 CPU_ARCHITECTURE = Literal["x86_64", "arm64"]
 
+SERVICE_PROVIDER_NAME_TRANSLATION_DICT = {
+    "alibaba": "alibaba",
+    "amazon": "amazon",
+    "azure": "azure",
+    "digitalocean": "digitalocean",
+    "google cloud platform": "google",
+    "oracle": "oracle",
+}
+
 
 @dataclass
 class InstanceDescription:
     label: str
     family: str
     instance_description_link: str
     hw: str
@@ -37,50 +47,55 @@
     aws_govcloud: Union[bool, str] = False
 
 
 def map_autodl_service_provider_to_cloudinfo_provider(
     autodl_service_provider: str,
 ) -> str:
     # based off of https://github.com/banzaicloud/cloudinfo/tree/master/internal/cloudinfo/providers
-    translation_dict = {
-        "Alibaba": "alibaba",
-        "Amazon": "amazon",
-        "Azure": "azure",
-        "DigitalOcean": "digitalocean",
-        "Google Cloud Platform": "google",
-        "Oracle": "oracle",
-    }
-    if autodl_service_provider not in translation_dict:
+    if (
+        autodl_service_provider.lower()
+        not in SERVICE_PROVIDER_NAME_TRANSLATION_DICT
+    ):
         raise ValueError(
             f"Unsupported service provider {autodl_service_provider}"
         )
 
-    return translation_dict[autodl_service_provider]
+    return SERVICE_PROVIDER_NAME_TRANSLATION_DICT[
+        autodl_service_provider.lower()
+    ]
 
 
 class CloudInfoService:
     _cloud_products_info = None
 
     def __init__(
-        self, provider, region, fetch_data_from_cloud_info: bool = True
+        self,
+        provider: str,
+        region: str,
+        fetch_data_from_cloud_info: bool = True,
     ) -> None:
         self.cloudinfo_service_enabled = fetch_data_from_cloud_info
+        if (
+            provider.lower()
+            not in SERVICE_PROVIDER_NAME_TRANSLATION_DICT.keys()
+        ):
+            raise RuntimeError("Invalid provider")
         self.provider = provider
         self.region = region
 
     @property
     def cloud_products_info(self):
         """Get cloud products info and cache it for further reuse"""
 
         if not self.cloudinfo_service_enabled:
             return None
 
         if self._cloud_products_info is None:
             service_type = "compute"
-            cloudinfo_api_path = os.environ["CLOUDINFO_API_PATH"]
+            cloudinfo_api_path = libenv.CLOUDINFO_API_PATH
             provider = map_autodl_service_provider_to_cloudinfo_provider(
                 self.provider
             )
 
             url = f"{cloudinfo_api_path}/providers/{provider}/services/{service_type}/regions/{self.region}/products"
 
             response = requests.get(
```

### Comparing `autumn8-1.0.5rc9/autumn8/common/config/settings.py` & `autumn8-1.1.0rc1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/common/config/supported_instances.py` & `autumn8-1.1.0rc1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/common/types.py` & `autumn8-1.1.0rc1/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/env/__init__.py` & `autumn8-1.1.0rc1/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/examples/mnist.py` & `autumn8-1.1.0rc1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/examples/model.py` & `autumn8-1.1.0rc1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/examples/sbert-alpha.py` & `autumn8-1.1.0rc1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.1.0rc1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/__init__.py` & `autumn8-1.1.0rc1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/api/cloud.py` & `autumn8-1.1.0rc1/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/api/lab.py` & `autumn8-1.1.0rc1/autumn8/lib/api/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.lib import logging
 from autumn8.lib.api_creds import retrieve_api_creds
 from autumn8.lib.http import require_ok_response, url_with_params
+from autumn8.types.router import NewModelInfo
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 APP_NAME = "autumn8"
 APP_AUTHOR = "autumn8"
 
 logger = logging.getLogger(__name__)
@@ -89,23 +90,23 @@
     require_ok_response(response)
     return response.json()
 
 
 def post_model(
     environment: CliEnvironment,
     organization_id: int,
-    model_config: Dict[str, Any],
+    model_config: NewModelInfo,
 ):
     autodl_host = environment.value.app_host
     api_route = f"{autodl_host}/api/lab/model"
     logger.info("Submitting model to %s", api_route)
     response = requests.post(
         url_with_params(api_route, {"organization_id": organization_id}),
         headers={"Content-Type": "application/json"},
-        data=json.dumps(model_config),
+        data=json.dumps(model_config.dict()),
         auth=HTTPBasicAuth(*retrieve_api_creds()),
     )
 
     require_ok_response(response)
     return response.json()
```

### Comparing `autumn8-1.0.5rc9/autumn8/lib/api/user.py` & `autumn8-1.1.0rc1/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/api_creds.py` & `autumn8-1.1.0rc1/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/asyncio.py` & `autumn8-1.1.0rc1/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/http.py` & `autumn8-1.1.0rc1/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/logging.py` & `autumn8-1.1.0rc1/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/logging.yaml` & `autumn8-1.1.0rc1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/package_resolver.py` & `autumn8-1.1.0rc1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/autumn8/lib/service.py` & `autumn8-1.1.0rc1/autumn8/lib/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import uuid
 from typing import Any, Dict, Optional
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.lib import api, logging
+from autumn8.types.router import NewModelInfo
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 logger = logging.getLogger(__name__)
 
 
 def resume_upload_model(upload_task):
@@ -22,31 +23,30 @@
     except s3.meta.client.exceptions.NoSuchUpload:
         pending_uploads.abort_and_forget_upload(upload_task["run_id"])
 
 
 def upload_model(
     environment: CliEnvironment,
     organization_id: int,
-    model_config: Dict[str, Any],
+    model_config: NewModelInfo,
     model_filepath_or_url: str,
     input_file_path: Optional[str],
     max_upload_workers: int = DEFAULT_MAX_UPLOAD_WORKERS,
     model_file_upload_id: Optional[str] = None,
     input_file_upload_id: Optional[str] = None,
     run_id: Optional[str] = None,
-    **kwargs,
 ):
     if run_id is None:  # used for resuming upload
         run_id = str(uuid.uuid4())
 
     function_args = locals()
 
     time_start = time.time()
     logger.info("Uploading the model files...")
-    model_config["s3_file_url"] = api.lab.post_model_file(
+    model_config.s3_file_url = api.lab.post_model_file(
         organization_id=organization_id,
         environment=environment,
         filepath_or_url=model_filepath_or_url,
         file_type="model",
         resume_args=function_args,
         id_key="model_file_upload_id",
         upload_id=model_file_upload_id,
@@ -54,15 +54,15 @@
     )
     logger.debug("Model uploaded in %.03f seconds", time.time() - time_start)
 
     # TODO: support uploading inputs via links
     if input_file_path != None and len(input_file_path) > 0:
         time_start = time.time()
         logger.info("Uploading the input files...")
-        model_config["s3_input_file_url"] = api.lab.post_model_file(
+        model_config.s3_input_file_url = api.lab.post_model_file(
             organization_id=organization_id,
             environment=environment,
             filepath_or_url=input_file_path,
             file_type="input",
             resume_args=function_args,
             id_key="input_file_upload_id",
             upload_id=input_file_upload_id,
```

### Comparing `autumn8-1.0.5rc9/autumn8.egg-info/PKG-INFO` & `autumn8-1.1.0rc1/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc9
+Version: 1.1.0rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc9/autumn8.egg-info/SOURCES.txt` & `autumn8-1.1.0rc1/autumn8.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 pyproject.toml
 setup.py
 autumn8/__init__.py
 autumn8/exceptions.py
+autumn8/i18n.py
+autumn8/libenv.py
 autumn8.egg-info/PKG-INFO
 autumn8.egg-info/SOURCES.txt
 autumn8.egg-info/dependency_links.txt
 autumn8.egg-info/entry_points.txt
 autumn8.egg-info/requires.txt
 autumn8.egg-info/top_level.txt
 autumn8/cli/__init__.py
@@ -48,9 +50,10 @@
 autumn8/lib/package_resolver.py
 autumn8/lib/service.py
 autumn8/lib/api/__init__.py
 autumn8/lib/api/cloud.py
 autumn8/lib/api/lab.py
 autumn8/lib/api/user.py
 autumn8/types/deployment.py
+autumn8/types/router.py
 tests/test_io_bottleneck_detection.py
 tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc9/pyproject.toml` & `autumn8-1.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/tests/test_io_bottleneck_detection.py` & `autumn8-1.1.0rc1/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc9/tests/test_settings.py` & `autumn8-1.1.0rc1/tests/test_settings.py`

 * *Files identical despite different names*

