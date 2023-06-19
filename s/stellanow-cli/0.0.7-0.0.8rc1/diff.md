# Comparing `tmp/stellanow_cli-0.0.7.tar.gz` & `tmp/stellanow_cli-0.0.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.7.tar", last modified: Mon Jun 19 16:56:16 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.8rc1.tar", last modified: Mon Jun 19 17:15:25 2023, max compression
```

## Comparing `stellanow_cli-0.0.7.tar` & `stellanow_cli-0.0.8rc1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.214619 stellanow_cli-0.0.7/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-19 16:41:18.000000 stellanow_cli-0.0.7/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7900 2023-06-19 16:56:16.214224 stellanow_cli-0.0.7/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-19 16:39:22.000000 stellanow_cli-0.0.7/Pipfile
--rw-r--r--   0 tom-kandziora   (501) staff       (20)    10615 2023-06-18 17:42:46.000000 stellanow_cli-0.0.7/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7726 2023-06-19 16:55:32.000000 stellanow_cli-0.0.7/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-19 16:56:16.214680 stellanow_cli-0.0.7/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1517 2023-06-19 16:43:28.000000 stellanow_cli-0.0.7/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.165568 stellanow_cli-0.0.7/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 16:37:56.000000 stellanow_cli-0.0.7/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.181374 stellanow_cli-0.0.7/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      245 2023-06-17 12:38:37.000000 stellanow_cli-0.0.7/stellanow_cli/__pycache__/_run.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-19 15:36:11.000000 stellanow_cli-0.0.7/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1333 2023-06-17 12:36:38.000000 stellanow_cli-0.0.7/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       82 2023-06-17 12:37:59.000000 stellanow_cli-0.0.7/stellanow_cli/_run.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-19 16:56:12.000000 stellanow_cli-0.0.7/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.183280 stellanow_cli-0.0.7/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      446 2023-06-19 15:08:44.000000 stellanow_cli-0.0.7/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.185194 stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-19 15:36:10.000000 stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1505 2023-06-17 11:42:52.000000 stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5438 2023-06-19 16:30:05.000000 stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      769 2023-06-17 11:30:12.000000 stellanow_cli-0.0.7/stellanow_cli/api/datatypes.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6177 2023-06-19 15:46:34.000000 stellanow_cli-0.0.7/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1291 2023-06-17 12:31:26.000000 stellanow_cli-0.0.7/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.187129 stellanow_cli-0.0.7/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      455 2023-06-18 17:14:47.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.189272 stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      672 2023-06-18 17:15:34.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5040 2023-06-19 15:36:11.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4519 2023-06-19 15:35:26.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.191635 stellanow_cli-0.0.7/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.7/stellanow_cli/code_generators/templates/csharp.template
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.195880 stellanow_cli-0.0.7/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.199445 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3765 2023-06-19 15:36:11.000000 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2918 2023-06-17 12:42:45.000000 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-17 12:36:38.000000 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4215 2023-06-19 16:30:05.000000 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3725 2023-06-19 16:30:05.000000 stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 15:19:46.000000 stellanow_cli-0.0.7/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4161 2023-06-19 15:35:49.000000 stellanow_cli-0.0.7/stellanow_cli/commands/command_config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3796 2023-06-17 12:42:05.000000 stellanow_cli-0.0.7/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1223 2023-06-17 12:31:26.000000 stellanow_cli-0.0.7/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4292 2023-06-19 16:27:00.000000 stellanow_cli-0.0.7/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4400 2023-06-19 16:27:00.000000 stellanow_cli-0.0.7/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.202890 stellanow_cli-0.0.7/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.7/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.206501 stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.7/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.7/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.7/stellanow_cli/config/int.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.209130 stellanow_cli-0.0.7/stellanow_cli/utils/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-19 15:36:07.000000 stellanow_cli-0.0.7/stellanow_cli/utils/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.211472 stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-19 15:36:10.000000 stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      926 2023-06-19 15:34:53.000000 stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1859 2023-06-17 12:36:38.000000 stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      864 2023-06-19 15:06:03.000000 stellanow_cli-0.0.7/stellanow_cli/utils/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1159 2023-06-17 11:25:53.000000 stellanow_cli-0.0.7/stellanow_cli/utils/utils.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.179084 stellanow_cli-0.0.7/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7900 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2637 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-19 16:56:16.000000 stellanow_cli-0.0.7/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.212918 stellanow_cli-0.0.7/tests/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:56:16.213602 stellanow_cli-0.0.7/tests/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.7/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.7/tests/test_command_configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2222 2023-06-18 17:07:07.000000 stellanow_cli-0.0.7/tests/test_generate_class_handles_all_valueTypes.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.860833 stellanow_cli-0.0.8rc1/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-19 16:41:18.000000 stellanow_cli-0.0.8rc1/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8070 2023-06-19 17:15:25.860472 stellanow_cli-0.0.8rc1/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-19 16:39:22.000000 stellanow_cli-0.0.8rc1/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10615 2023-06-18 17:42:46.000000 stellanow_cli-0.0.8rc1/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7893 2023-06-19 17:15:08.000000 stellanow_cli-0.0.8rc1/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-19 17:15:25.860898 stellanow_cli-0.0.8rc1/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1517 2023-06-19 16:43:28.000000 stellanow_cli-0.0.8rc1/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.755762 stellanow_cli-0.0.8rc1/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 16:37:56.000000 stellanow_cli-0.0.8rc1/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.817940 stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      245 2023-06-17 12:38:37.000000 stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1333 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       82 2023-06-17 12:37:59.000000 stellanow_cli-0.0.8rc1/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       26 2023-06-19 17:15:20.000000 stellanow_cli-0.0.8rc1/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.820476 stellanow_cli-0.0.8rc1/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      446 2023-06-19 15:08:44.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.823187 stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1505 2023-06-17 11:42:52.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5438 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      769 2023-06-17 11:30:12.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6177 2023-06-19 15:46:34.000000 stellanow_cli-0.0.8rc1/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1291 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc1/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.825465 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      455 2023-06-18 17:14:47.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.828881 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      672 2023-06-18 17:15:34.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5040 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4519 2023-06-19 15:35:26.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.831261 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.844114 stellanow_cli-0.0.8rc1/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.847839 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3765 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2918 2023-06-17 12:42:45.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4215 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3725 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 15:19:46.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4161 2023-06-19 15:35:49.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3796 2023-06-17 12:42:05.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1223 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4292 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4400 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc1/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.850459 stellanow_cli-0.0.8rc1/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.853256 stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.8rc1/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.855599 stellanow_cli-0.0.8rc1/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-19 15:36:07.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.857700 stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      926 2023-06-19 15:34:53.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1859 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      864 2023-06-19 15:06:03.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1159 2023-06-17 11:25:53.000000 stellanow_cli-0.0.8rc1/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.798678 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8070 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2637 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-19 17:15:25.000000 stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.859195 stellanow_cli-0.0.8rc1/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 17:15:25.859848 stellanow_cli-0.0.8rc1/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.8rc1/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.8rc1/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2222 2023-06-18 17:07:07.000000 stellanow_cli-0.0.8rc1/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.7/PKG-INFO` & `stellanow_cli-0.0.8rc1/README.public`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,73 @@
-Metadata-Version: 2.1
-Name: stellanow_cli
-Version: 0.0.7
-Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
-Requires-Python: >=3.10
-
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
 
 To install the StellaNow CLI tool, run the following command:
 
+.. code-block:: bash
+
     pip install stellanow-cli
 
+
 The tool is hosted on PYPI and can be installed via pip.
 
 Usage
 -----
 
-After installation, you can use the 'stellanow' command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
+After installation, you can use the ``stellanow`` command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
 
 **Configure**
 
-You can use the 'configure' command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
+You can use the ``configure`` command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
 
 Here is how to use the command:
 
+.. code-block:: bash
+
     stellanow configure --profile YOUR_PROFILE_NAME
 
-If no profile is specified, the configurations will be stored under the 'DEFAULT' profile. Profile names are case-sensitive.
+
+If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile. Profile names are case-sensitive.
 
 **Environment Variables**
 
 The stellanow CLI can also read the following environment variables:
 
-    STELLANOW_ACCESS_KEY: Your access key.
-    STELLANOW_ACCESS_TOKEN: Your access token.
+.. code-block:: bash
+
+    STELLANOW_ACCESS_KEY: <Your access key>
+    STELLANOW_ACCESS_TOKEN: <Your access token>
+
 
 **Credentials Precedence Order**
 
 In StellaNow CLI, there is a specific order of precedence for the way credentials and other settings are obtained. This means if a setting is provided in more than one place, the setting from the source with the highest precedence will be used. The order of precedence is:
 
+.. code-block:: bash
+
     Environment Variables -> Command Line Options -> Configuration File
 
+
 * **Environment Variables**: These have the highest precedence. If a setting is provided as an environment variable, it will override any value provided as a command line option or in the configuration file.
 * **Command Line Options**: These have the second-highest precedence. If a setting is provided as a command line option, it will override any value provided in the configuration file.
 * **Configuration File**: This has the lowest precedence. Settings in the configuration file will be used if no value for the same setting is provided as an environment variable or as a command line option.
 
 * This order of precedence provides flexibility, allowing you to set default values in the configuration file but override them for specific operations with command line options or environment variables.
 
 Commands
 --------
 
-**'configure'**
+**`configure`**
 
-The **'configure'** command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
+The ``configure`` command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
@@ -78,44 +84,53 @@
 
 **'events'**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow events
 
+
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
 **'plan'**
 
 The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow plan --input_dir .
 
+
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
 * **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
 
 **'generate'**
 
 The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
+
 This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
 
 Command options:
 
 * **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
 * **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
 * **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
@@ -143,8 +158,8 @@
 TODO
 
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.7/README.md` & `stellanow_cli-0.0.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/README.public` & `stellanow_cli-0.0.8rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,79 @@
+Metadata-Version: 2.1
+Name: stellanow_cli
+Version: 0.0.8rc1
+Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
+Requires-Python: >=3.10
+
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
 
 To install the StellaNow CLI tool, run the following command:
 
+.. code-block:: bash
+
     pip install stellanow-cli
 
+
 The tool is hosted on PYPI and can be installed via pip.
 
 Usage
 -----
 
-After installation, you can use the 'stellanow' command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
+After installation, you can use the ``stellanow`` command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
 
 **Configure**
 
-You can use the 'configure' command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
+You can use the ``configure`` command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
 
 Here is how to use the command:
 
+.. code-block:: bash
+
     stellanow configure --profile YOUR_PROFILE_NAME
 
-If no profile is specified, the configurations will be stored under the 'DEFAULT' profile. Profile names are case-sensitive.
+
+If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile. Profile names are case-sensitive.
 
 **Environment Variables**
 
 The stellanow CLI can also read the following environment variables:
 
-    STELLANOW_ACCESS_KEY: Your access key.
-    STELLANOW_ACCESS_TOKEN: Your access token.
+.. code-block:: bash
+
+    STELLANOW_ACCESS_KEY: <Your access key>
+    STELLANOW_ACCESS_TOKEN: <Your access token>
+
 
 **Credentials Precedence Order**
 
 In StellaNow CLI, there is a specific order of precedence for the way credentials and other settings are obtained. This means if a setting is provided in more than one place, the setting from the source with the highest precedence will be used. The order of precedence is:
 
+.. code-block:: bash
+
     Environment Variables -> Command Line Options -> Configuration File
 
+
 * **Environment Variables**: These have the highest precedence. If a setting is provided as an environment variable, it will override any value provided as a command line option or in the configuration file.
 * **Command Line Options**: These have the second-highest precedence. If a setting is provided as a command line option, it will override any value provided in the configuration file.
 * **Configuration File**: This has the lowest precedence. Settings in the configuration file will be used if no value for the same setting is provided as an environment variable or as a command line option.
 
 * This order of precedence provides flexibility, allowing you to set default values in the configuration file but override them for specific operations with command line options or environment variables.
 
 Commands
 --------
 
-**'configure'**
+**`configure`**
 
-The **'configure'** command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
+The ``configure`` command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
@@ -72,44 +90,53 @@
 
 **'events'**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow events
 
+
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
 **'plan'**
 
 The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow plan --input_dir .
 
+
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
 * **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
 
 **'generate'**
 
 The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
+
 This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
 
 Command options:
 
 * **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
 * **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
 * **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
@@ -137,8 +164,8 @@
 TODO
 
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.7/setup.py` & `stellanow_cli-0.0.8rc1/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/api/datatypes.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/api/datatypes.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/cli.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/code_generators/templates/csharp.template` & `stellanow_cli-0.0.8rc1/stellanow_cli/code_generators/templates/csharp.template`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/command_config.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/generate.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/commands/plan.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/config/__pycache__/int.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/config/config.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/utils/logger.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli/utils/utils.py` & `stellanow_cli-0.0.8rc1/stellanow_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.7
+Version: 0.0.8rc1
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
 
 To install the StellaNow CLI tool, run the following command:
 
+.. code-block:: bash
+
     pip install stellanow-cli
 
+
 The tool is hosted on PYPI and can be installed via pip.
 
 Usage
 -----
 
-After installation, you can use the 'stellanow' command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
+After installation, you can use the ``stellanow`` command in your terminal to interact with StellaNow services. Here is how to use some of the available commands:
 
 **Configure**
 
-You can use the 'configure' command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
+You can use the ``configure`` command to setup the necessary credentials and configurations for a specific profile. The profile will store a particular set of configurations.
 
 Here is how to use the command:
 
+.. code-block:: bash
+
     stellanow configure --profile YOUR_PROFILE_NAME
 
-If no profile is specified, the configurations will be stored under the 'DEFAULT' profile. Profile names are case-sensitive.
+
+If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile. Profile names are case-sensitive.
 
 **Environment Variables**
 
 The stellanow CLI can also read the following environment variables:
 
-    STELLANOW_ACCESS_KEY: Your access key.
-    STELLANOW_ACCESS_TOKEN: Your access token.
+.. code-block:: bash
+
+    STELLANOW_ACCESS_KEY: <Your access key>
+    STELLANOW_ACCESS_TOKEN: <Your access token>
+
 
 **Credentials Precedence Order**
 
 In StellaNow CLI, there is a specific order of precedence for the way credentials and other settings are obtained. This means if a setting is provided in more than one place, the setting from the source with the highest precedence will be used. The order of precedence is:
 
+.. code-block:: bash
+
     Environment Variables -> Command Line Options -> Configuration File
 
+
 * **Environment Variables**: These have the highest precedence. If a setting is provided as an environment variable, it will override any value provided as a command line option or in the configuration file.
 * **Command Line Options**: These have the second-highest precedence. If a setting is provided as a command line option, it will override any value provided in the configuration file.
 * **Configuration File**: This has the lowest precedence. Settings in the configuration file will be used if no value for the same setting is provided as an environment variable or as a command line option.
 
 * This order of precedence provides flexibility, allowing you to set default values in the configuration file but override them for specific operations with command line options or environment variables.
 
 Commands
 --------
 
-**'configure'**
+**`configure`**
 
-The **'configure'** command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
+The ``configure`` command sets up the necessary credentials and configurations for a specific profile or for the DEFAULT profile if none is specified.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
@@ -78,44 +90,53 @@
 
 **'events'**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow events
 
+
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
 **'plan'**
 
 The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow plan --input_dir .
 
+
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
 * **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
 
 **'generate'**
 
 The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
+.. code-block:: bash
+
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
+
 This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
 
 Command options:
 
 * **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
 * **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
 * **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
```

### Comparing `stellanow_cli-0.0.7/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.8rc1/stellanow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc` & `stellanow_cli-0.0.8rc1/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/tests/test_command_configure.py` & `stellanow_cli-0.0.8rc1/tests/test_command_configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.7/tests/test_generate_class_handles_all_valueTypes.py` & `stellanow_cli-0.0.8rc1/tests/test_generate_class_handles_all_valueTypes.py`

 * *Files identical despite different names*

