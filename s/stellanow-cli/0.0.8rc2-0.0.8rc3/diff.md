# Comparing `tmp/stellanow_cli-0.0.8rc2.tar.gz` & `tmp/stellanow_cli-0.0.8rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.8rc2.tar", last modified: Mon Jun 19 19:28:16 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.8rc3.tar", last modified: Mon Jun 19 19:49:34 2023, max compression
```

## Comparing `stellanow_cli-0.0.8rc2.tar` & `stellanow_cli-0.0.8rc3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.696197 stellanow_cli-0.0.8rc2/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-19 16:41:18.000000 stellanow_cli-0.0.8rc2/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8069 2023-06-19 19:28:16.695829 stellanow_cli-0.0.8rc2/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-19 16:39:22.000000 stellanow_cli-0.0.8rc2/Pipfile
--rw-r--r--   0 tom-kandziora   (501) staff       (20)    10615 2023-06-18 17:42:46.000000 stellanow_cli-0.0.8rc2/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7892 2023-06-19 19:27:48.000000 stellanow_cli-0.0.8rc2/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-19 19:28:16.696253 stellanow_cli-0.0.8rc2/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1517 2023-06-19 16:43:28.000000 stellanow_cli-0.0.8rc2/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.627819 stellanow_cli-0.0.8rc2/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 16:37:56.000000 stellanow_cli-0.0.8rc2/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.651314 stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      245 2023-06-17 12:38:37.000000 stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/_run.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1333 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       82 2023-06-17 12:37:59.000000 stellanow_cli-0.0.8rc2/stellanow_cli/_run.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       26 2023-06-19 19:28:14.000000 stellanow_cli-0.0.8rc2/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.654274 stellanow_cli-0.0.8rc2/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      446 2023-06-19 15:08:44.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.657060 stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1505 2023-06-17 11:42:52.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5438 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      769 2023-06-17 11:30:12.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/datatypes.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6177 2023-06-19 15:46:34.000000 stellanow_cli-0.0.8rc2/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1291 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc2/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.659499 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      455 2023-06-18 17:14:47.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.662123 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      672 2023-06-18 17:15:34.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     5040 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4519 2023-06-19 15:35:26.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.664388 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/templates/csharp.template
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.676645 stellanow_cli-0.0.8rc2/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.681408 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3765 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2918 2023-06-17 12:42:45.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4215 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3725 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 15:19:46.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4161 2023-06-19 15:35:49.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/command_config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3796 2023-06-17 12:42:05.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1223 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4292 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4400 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc2/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.684616 stellanow_cli-0.0.8rc2/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.687784 stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.8rc2/stellanow_cli/config/int.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.690756 stellanow_cli-0.0.8rc2/stellanow_cli/utils/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-19 15:36:07.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.692888 stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      926 2023-06-19 15:34:53.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1859 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      864 2023-06-19 15:06:03.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1159 2023-06-17 11:25:53.000000 stellanow_cli-0.0.8rc2/stellanow_cli/utils/utils.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.648153 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     8069 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2637 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-19 19:28:16.000000 stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.694497 stellanow_cli-0.0.8rc2/tests/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:28:16.695211 stellanow_cli-0.0.8rc2/tests/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.8rc2/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.8rc2/tests/test_command_configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2222 2023-06-18 17:07:07.000000 stellanow_cli-0.0.8rc2/tests/test_generate_class_handles_all_valueTypes.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.493235 stellanow_cli-0.0.8rc3/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-19 16:41:18.000000 stellanow_cli-0.0.8rc3/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8060 2023-06-19 19:49:34.492901 stellanow_cli-0.0.8rc3/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-19 16:39:22.000000 stellanow_cli-0.0.8rc3/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10615 2023-06-18 17:42:46.000000 stellanow_cli-0.0.8rc3/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7883 2023-06-19 19:49:15.000000 stellanow_cli-0.0.8rc3/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-19 19:49:34.493286 stellanow_cli-0.0.8rc3/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1517 2023-06-19 16:43:28.000000 stellanow_cli-0.0.8rc3/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.419630 stellanow_cli-0.0.8rc3/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 16:37:56.000000 stellanow_cli-0.0.8rc3/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.451646 stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      245 2023-06-17 12:38:37.000000 stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1333 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       82 2023-06-17 12:37:59.000000 stellanow_cli-0.0.8rc3/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       26 2023-06-19 19:49:20.000000 stellanow_cli-0.0.8rc3/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.454415 stellanow_cli-0.0.8rc3/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      446 2023-06-19 15:08:44.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.456975 stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1505 2023-06-17 11:42:52.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5438 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      769 2023-06-17 11:30:12.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6177 2023-06-19 15:46:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1291 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc3/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.460822 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      455 2023-06-18 17:14:47.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.464062 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      672 2023-06-18 17:15:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5040 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4519 2023-06-19 15:35:26.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.467150 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.474975 stellanow_cli-0.0.8rc3/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.479009 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3765 2023-06-19 15:36:11.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2918 2023-06-17 12:42:45.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4215 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3725 2023-06-19 16:30:05.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 15:19:46.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4161 2023-06-19 15:35:49.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3796 2023-06-17 12:42:05.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1223 2023-06-17 12:31:26.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4292 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4400 2023-06-19 16:27:00.000000 stellanow_cli-0.0.8rc3/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.482373 stellanow_cli-0.0.8rc3/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.485588 stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.8rc3/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.487685 stellanow_cli-0.0.8rc3/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-19 15:36:07.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.489744 stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-19 15:36:10.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      926 2023-06-19 15:34:53.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1859 2023-06-17 12:36:38.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      864 2023-06-19 15:06:03.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1159 2023-06-17 11:25:53.000000 stellanow_cli-0.0.8rc3/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.441731 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     8060 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2637 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-19 19:49:34.000000 stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.491275 stellanow_cli-0.0.8rc3/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 19:49:34.492180 stellanow_cli-0.0.8rc3/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.8rc3/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.8rc3/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2222 2023-06-18 17:07:07.000000 stellanow_cli-0.0.8rc3/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.8rc2/PKG-INFO` & `stellanow_cli-0.0.8rc3/README.public`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: stellanow_cli
-Version: 0.0.8rc2
-Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
-Requires-Python: >=3.10
-
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
@@ -76,84 +70,85 @@
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
 
 Command options:
 
-* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
 
-This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
+This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is ``myProfile``. If you do not specify a profile, the command will default to the ``DEFAULT`` profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
-The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
+The command then writes these configurations to a file named ``config.ini`` in the ``.stellanow`` directory of your home folder. If this directory or file does not exist, they will be created.
 
-**'events'**
+**`events`**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
+
 .. code-block:: bash
 
     stellanow events
 
 
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
-**'plan'**
+**`plan`**
 
-The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
+The ``plan`` command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow plan --input_dir .
 
 
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
-* **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
+* ``--input_dir (-i)``: The directory to read generated classes from. Defaults to the current directory.
 
-**'generate'**
+**`generate`**
 
-The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
+The ``generate`` command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
 
-This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
+This will generate C# classes for events ``Event1`` and ``Event2``, placing them in the current directory. The generated classes will be in the namespace ``MyApp.Messages``. If a file for an event already exists, it will be overwritten due to the ``--force`` flag.
 
 Command options:
 
-* **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
-* **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
-* **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
-* **'--events (-e)'**: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
-* **'--language (-l)'**: The programming language for the generated classes. Can be 'csharp'. Defaults to 'csharp'.
+* ``--namespace (-n)``: The namespace for the generated classes. Defaults to an empty string.
+* ``--destination (-d)``: The directory to save the generated classes. Defaults to the current directory.
+* ``--force (-f)``: A flag indicating whether to overwrite existing files. Defaults to false.
+* ``--events (-e)``: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
+* ``--language (-l)``: The programming language for the generated classes. Can be ``csharp``. Defaults to ``csharp``.
 
 **Common Command Options**
 
-* **'--access_key'**: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
-* **'--access_token'**: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
-* **'--organization_id'**: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
-* **'--project_id'**: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
-* **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
+* ``--access_key``: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
+* ``--access_token``: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
+* ``--organization_id``: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
+* ``--project_id``: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
+* ``--verbose (-v)``: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
 Release Notes
 -------------
@@ -163,8 +158,8 @@
 TODO
 
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.8rc2/README.md` & `stellanow_cli-0.0.8rc3/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/README.public` & `stellanow_cli-0.0.8rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: stellanow_cli
+Version: 0.0.8rc3
+Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
+Requires-Python: >=3.10
+
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
@@ -70,84 +76,85 @@
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
 
 Command options:
 
-* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
 
-This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
+This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is ``myProfile``. If you do not specify a profile, the command will default to the ``DEFAULT`` profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
-The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
+The command then writes these configurations to a file named ``config.ini`` in the ``.stellanow`` directory of your home folder. If this directory or file does not exist, they will be created.
 
-**'events'**
+**`events`**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
+
 .. code-block:: bash
 
     stellanow events
 
 
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
-**'plan'**
+**`plan`**
 
-The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
+The ``plan`` command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow plan --input_dir .
 
 
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
-* **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
+* ``--input_dir (-i)``: The directory to read generated classes from. Defaults to the current directory.
 
-**'generate'**
+**`generate`**
 
-The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
+The ``generate`` command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
 
-This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
+This will generate C# classes for events ``Event1`` and ``Event2``, placing them in the current directory. The generated classes will be in the namespace ``MyApp.Messages``. If a file for an event already exists, it will be overwritten due to the ``--force`` flag.
 
 Command options:
 
-* **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
-* **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
-* **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
-* **'--events (-e)'**: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
-* **'--language (-l)'**: The programming language for the generated classes. Can be 'csharp'. Defaults to 'csharp'.
+* ``--namespace (-n)``: The namespace for the generated classes. Defaults to an empty string.
+* ``--destination (-d)``: The directory to save the generated classes. Defaults to the current directory.
+* ``--force (-f)``: A flag indicating whether to overwrite existing files. Defaults to false.
+* ``--events (-e)``: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
+* ``--language (-l)``: The programming language for the generated classes. Can be ``csharp``. Defaults to ``csharp``.
 
 **Common Command Options**
 
-* **'--access_key'**: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
-* **'--access_token'**: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
-* **'--organization_id'**: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
-* **'--project_id'**: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
-* **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
+* ``--access_key``: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
+* ``--access_token``: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
+* ``--organization_id``: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
+* ``--project_id``: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
+* ``--verbose (-v)``: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
 Release Notes
 -------------
@@ -157,8 +164,8 @@
 TODO
 
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.8rc2/setup.py` & `stellanow_cli-0.0.8rc3/setup.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/api/datatypes.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/api/datatypes.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/api/stellanow_api.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/cli.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/cli.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/code_generators/templates/csharp.template` & `stellanow_cli-0.0.8rc3/stellanow_cli/code_generators/templates/csharp.template`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/command_config.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/command_config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/generate.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/commands/plan.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/config/__pycache__/int.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/config/config.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/utils/logger.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/utils/logger.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli/utils/utils.py` & `stellanow_cli-0.0.8rc3/stellanow_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellanow-cli
-Version: 0.0.8rc2
+Version: 0.0.8rc3
 Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
@@ -76,84 +76,85 @@
 .. code-block:: bash
 
     stellanow configure --profile myProfile
 
 
 Command options:
 
-* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
 
-This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
+This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is ``myProfile``. If you do not specify a profile, the command will default to the ``DEFAULT`` profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
-The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
+The command then writes these configurations to a file named ``config.ini`` in the ``.stellanow`` directory of your home folder. If this directory or file does not exist, they will be created.
 
-**'events'**
+**`events`**
 
 The **'events'** command fetches the latest event specifications from the API and outputs a list of the events into the terminal prompt.
 
 Command usage:
+
 .. code-block:: bash
 
     stellanow events
 
 
 This will print a table of all available events with their metadata (EventID, Event Name, Is Active, Created At, Updated At).
 
 Command options:
 
 * No options required.
 
-**'plan'**
+**`plan`**
 
-The **'plan'** command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
+The ``plan`` command compares currently generated classes with the specifications fetched from the API and provides a summary of changes.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow plan --input_dir .
 
 
 This will scan all the auto-generated files in the current directory and compare them with the latest specifications from the API.
 
 Command options:
 
-* **'--input_dir (-i)'**: The directory to read generated classes from. Defaults to the current directory.
+* ``--input_dir (-i)``: The directory to read generated classes from. Defaults to the current directory.
 
-**'generate'**
+**`generate`**
 
-The **'generate'** command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
+The ``generate`` command fetches the latest event specifications from the API and generates corresponding class code in the desired programming language.
 
 Command usage:
 
 .. code-block:: bash
 
     stellanow generate --namespace MyApp.Messages --destination . --force --events Event1,Event2 --language csharp
 
 
-This will generate C# classes for events 'Event1' and 'Event2', placing them in the current directory. The generated classes will be in the namespace 'MyApp.Messages'. If a file for an event already exists, it will be overwritten due to the **'--force'** flag.
+This will generate C# classes for events ``Event1`` and ``Event2``, placing them in the current directory. The generated classes will be in the namespace ``MyApp.Messages``. If a file for an event already exists, it will be overwritten due to the ``--force`` flag.
 
 Command options:
 
-* **'--namespace (-n)'**: The namespace for the generated classes. Defaults to an empty string.
-* **'--destination (-d)'**: The directory to save the generated classes. Defaults to the current directory.
-* **'--force (-f)'**: A flag indicating whether to overwrite existing files. Defaults to false.
-* **'--events (-e)'**: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
-* **'--language (-l)'**: The programming language for the generated classes. Can be 'csharp'. Defaults to 'csharp'.
+* ``--namespace (-n)``: The namespace for the generated classes. Defaults to an empty string.
+* ``--destination (-d)``: The directory to save the generated classes. Defaults to the current directory.
+* ``--force (-f)``: A flag indicating whether to overwrite existing files. Defaults to false.
+* ``--events (-e)``: A list of specific events to generate. If this option is not provided, classes for all events will be generated.
+* ``--language (-l)``: The programming language for the generated classes. Can be ``csharp``. Defaults to ``csharp``.
 
 **Common Command Options**
 
-* **'--access_key'**: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
-* **'--access_token'**: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
-* **'--organization_id'**: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
-* **'--project_id'**: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
-* **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
+* ``--access_key``: The access key credential for accessing the StellaNow API. This should be the same as your StellaNow account access key.
+* ``--access_token``: The access token credential for accessing the StellaNow API. This should be the same as your StellaNow account access token.
+* ``--organization_id``: The unique identifier (UUID) of the organization in StellaNow. This is used to scope the operations within the given organization's context.
+* ``--project_id``: The unique identifier (UUID) of the project in StellaNow. This is used to scope the operations within the given project's context.
+* ``--profile``: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the ``DEFAULT`` profile.
+* ``--verbose (-v)``: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
 Release Notes
 -------------
```

### Comparing `stellanow_cli-0.0.8rc2/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.8rc3/stellanow_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc` & `stellanow_cli-0.0.8rc3/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/tests/test_command_configure.py` & `stellanow_cli-0.0.8rc3/tests/test_command_configure.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.8rc2/tests/test_generate_class_handles_all_valueTypes.py` & `stellanow_cli-0.0.8rc3/tests/test_generate_class_handles_all_valueTypes.py`

 * *Files identical despite different names*

