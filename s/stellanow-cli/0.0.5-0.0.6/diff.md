# Comparing `tmp/stellanow_cli-0.0.5.tar.gz` & `tmp/stellanow_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.5.tar", last modified: Fri Jun 16 12:37:39 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.6.tar", last modified: Mon Jun 19 16:48:07 2023, max compression
```

## Comparing `stellanow_cli-0.0.5.tar` & `stellanow_cli-0.0.6.tar`

### file list

```diff
@@ -1,71 +1,81 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.496592 stellanow_cli-0.0.5/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       81 2023-06-16 12:36:11.000000 stellanow_cli-0.0.5/MANIFEST.in
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 12:37:39.495745 stellanow_cli-0.0.5/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     9422 2023-06-16 09:24:43.000000 stellanow_cli-0.0.5/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7653 2023-06-16 09:24:43.000000 stellanow_cli-0.0.5/README.public
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-16 12:37:39.496749 stellanow_cli-0.0.5/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      933 2023-06-16 09:19:11.000000 stellanow_cli-0.0.5/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:38.953419 stellanow_cli-0.0.5/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.5/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.178194 stellanow_cli-0.0.5/stellanow_cli/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/_version.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1377 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3377 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/command_config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      937 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1343 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1025 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/__pycache__/validate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-16 12:30:29.000000 stellanow_cli-0.0.5/stellanow_cli/_version.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.200683 stellanow_cli-0.0.5/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.5/stellanow_cli/api/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.207458 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      663 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6002 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.5/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.5/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.273458 stellanow_cli-0.0.5/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.304415 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      629 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3880 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/csharp_code_generator.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.335203 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/.footer.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/.header.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      488 2023-06-15 09:32:04.000000 stellanow_cli-0.0.5/stellanow_cli/code_generators/templates/csharp.template
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.5/stellanow_cli/command_config.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.384714 stellanow_cli-0.0.5/stellanow_cli/commands/
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.403414 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2933 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2687 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3473 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:54:02.000000 stellanow_cli-0.0.5/stellanow_cli/commands/_init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3819 2023-06-15 20:54:02.000000 stellanow_cli-0.0.5/stellanow_cli/commands/configure.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1224 2023-06-15 20:53:53.000000 stellanow_cli-0.0.5/stellanow_cli/commands/events.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3013 2023-06-15 20:53:46.000000 stellanow_cli-0.0.5/stellanow_cli/commands/generate.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     4091 2023-06-15 20:53:23.000000 stellanow_cli-0.0.5/stellanow_cli/commands/plan.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.468931 stellanow_cli-0.0.5/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.5/stellanow_cli/config/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.488002 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/int.cpython-310.pyc
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.5/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.5/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.5/stellanow_cli/config/int.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.5/stellanow_cli/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.5/stellanow_cli/utils.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.5/stellanow_cli/validate.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.112902 stellanow_cli-0.0.5/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     7813 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2290 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-16 12:37:38.000000 stellanow_cli-0.0.5/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-16 12:37:39.493685 stellanow_cli-0.0.5/tests/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.5/tests/test_command_configure.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.802685 stellanow_cli-0.0.6/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-19 16:41:18.000000 stellanow_cli-0.0.6/MANIFEST.in
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7877 2023-06-19 16:48:07.802070 stellanow_cli-0.0.6/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      225 2023-06-19 16:39:22.000000 stellanow_cli-0.0.6/Pipfile
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)    10615 2023-06-18 17:42:46.000000 stellanow_cli-0.0.6/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7703 2023-06-19 16:47:39.000000 stellanow_cli-0.0.6/README.public
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-19 16:48:07.802740 stellanow_cli-0.0.6/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1517 2023-06-19 16:43:28.000000 stellanow_cli-0.0.6/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.485457 stellanow_cli-0.0.6/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 16:37:56.000000 stellanow_cli-0.0.6/stellanow_cli/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.541154 stellanow_cli-0.0.6/stellanow_cli/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      510 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      245 2023-06-17 12:38:37.000000 stellanow_cli-0.0.6/stellanow_cli/__pycache__/_run.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      200 2023-06-19 15:36:11.000000 stellanow_cli-0.0.6/stellanow_cli/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1333 2023-06-17 12:36:38.000000 stellanow_cli-0.0.6/stellanow_cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       82 2023-06-17 12:37:59.000000 stellanow_cli-0.0.6/stellanow_cli/_run.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-19 16:47:53.000000 stellanow_cli-0.0.6/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.563998 stellanow_cli-0.0.6/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      446 2023-06-19 15:08:44.000000 stellanow_cli-0.0.6/stellanow_cli/api/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.577955 stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-19 15:36:10.000000 stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1505 2023-06-17 11:42:52.000000 stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5438 2023-06-19 16:30:05.000000 stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      769 2023-06-17 11:30:12.000000 stellanow_cli-0.0.6/stellanow_cli/api/datatypes.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6177 2023-06-19 15:46:34.000000 stellanow_cli-0.0.6/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1291 2023-06-17 12:31:26.000000 stellanow_cli-0.0.6/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.634557 stellanow_cli-0.0.6/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      455 2023-06-18 17:14:47.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.644713 stellanow_cli-0.0.6/stellanow_cli/code_generators/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      672 2023-06-18 17:15:34.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1813 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     5040 2023-06-19 15:36:11.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4519 2023-06-19 15:35:26.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/csharp_code_generator.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.649553 stellanow_cli-0.0.6/stellanow_cli/code_generators/templates/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-10 10:14:46.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/templates/.footer.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      186 2023-06-10 10:54:41.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/templates/.header.template
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      534 2023-06-18 12:11:51.000000 stellanow_cli-0.0.6/stellanow_cli/code_generators/templates/csharp.template
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.689739 stellanow_cli-0.0.6/stellanow_cli/commands/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.723096 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3765 2023-06-19 15:36:11.000000 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2918 2023-06-17 12:42:45.000000 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1358 2023-06-17 12:36:38.000000 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/events.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4215 2023-06-19 16:30:05.000000 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3725 2023-06-19 16:30:05.000000 stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      323 2023-06-19 15:19:46.000000 stellanow_cli-0.0.6/stellanow_cli/commands/_init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4161 2023-06-19 15:35:49.000000 stellanow_cli-0.0.6/stellanow_cli/commands/command_config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3796 2023-06-17 12:42:05.000000 stellanow_cli-0.0.6/stellanow_cli/commands/configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1223 2023-06-17 12:31:26.000000 stellanow_cli-0.0.6/stellanow_cli/commands/events.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4292 2023-06-19 16:27:00.000000 stellanow_cli-0.0.6/stellanow_cli/commands/generate.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     4400 2023-06-19 16:27:00.000000 stellanow_cli-0.0.6/stellanow_cli/commands/plan.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.759468 stellanow_cli-0.0.6/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.6/stellanow_cli/config/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.766208 stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      938 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1426 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      855 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/dev.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      851 2023-06-15 21:06:36.000000 stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/int.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.6/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.6/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.6/stellanow_cli/config/int.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.779251 stellanow_cli-0.0.6/stellanow_cli/utils/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       88 2023-06-19 15:36:07.000000 stellanow_cli-0.0.6/stellanow_cli/utils/__init__.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.784477 stellanow_cli-0.0.6/stellanow_cli/utils/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      310 2023-06-19 15:36:10.000000 stellanow_cli-0.0.6/stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      926 2023-06-19 15:34:53.000000 stellanow_cli-0.0.6/stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1859 2023-06-17 12:36:38.000000 stellanow_cli-0.0.6/stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      864 2023-06-19 15:06:03.000000 stellanow_cli-0.0.6/stellanow_cli/utils/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1159 2023-06-17 11:25:53.000000 stellanow_cli-0.0.6/stellanow_cli/utils/utils.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.528263 stellanow_cli-0.0.6/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7877 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2637 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-19 16:48:07.000000 stellanow_cli-0.0.6/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.794498 stellanow_cli-0.0.6/tests/
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-19 16:48:07.798932 stellanow_cli-0.0.6/tests/__pycache__/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1837 2023-06-18 17:07:08.000000 stellanow_cli-0.0.6/tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.6/tests/test_command_configure.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     2222 2023-06-18 17:07:07.000000 stellanow_cli-0.0.6/tests/test_generate_class_handles_all_valueTypes.py
```

### Comparing `stellanow_cli-0.0.5/PKG-INFO` & `stellanow_cli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stellanow_cli
-Version: 0.0.5
-Summary: A comprehensive Python package for data analysis and visualization.
+Version: 0.0.6
+Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
 Requires-Python: >=3.10
 
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
@@ -61,15 +61,15 @@
 
 Command usage:
 
     stellanow configure --profile myProfile
 
 Command options:
 
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
 This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
 The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
 
@@ -128,13 +128,20 @@
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 * **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
+Release Notes
+-------------
+
+Version: TODO
+
+TODO
+
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
 The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.5/README.md` & `stellanow_cli-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 
 Here is how to use the command:
 
     stellanow configure --profile YOUR_PROFILE_NAME
 
 If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
+### Internal Environment Selection
+As an internal development feature, all commands in the StellaNow CLI tool - including the **'configure'** command - come equipped with a hidden option, **'--env'**. This feature is specifically designed for our internal developers to easily designate the target API environment during their operations.
+
+The **'--env'** option accepts one of two arguments: **'dev'** or **'int'**. These arguments enable developers to switch between the Development and Integration environments, offering a high degree of control over their interactions with the StellaNow services.
+
+In the case of the **'configure'** command, the **'--env'** option goes a step further - the selected environment ('dev' or 'int') gets saved in the configuration file under the associated profile. This ensures the persistence of the chosen API environment across multiple sessions, relieving developers from the need to specify it each time.
+
+As a hidden feature, **'--env'** does not appear when using the **'--help'** command. This maintains the simplicity of the help output for general users while providing a powerful, flexible tool for our developers to streamline their workflows.
+
 ### Environment Variables
 The stellanow CLI can also read the following environment variables:
 
 * **`STELLANOW_ACCESS_KEY`**: Your access key.
 * **`STELLANOW_ACCESS_TOKEN`**: Your access token.
```

### Comparing `stellanow_cli-0.0.5/README.public` & `stellanow_cli-0.0.6/stellanow_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: stellanow-cli
+Version: 0.0.6
+Summary: Command-line interface for the StellaNow SDK code generation and comparison tool.
+Requires-Python: >=3.10
+
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
@@ -55,15 +61,15 @@
 
 Command usage:
 
     stellanow configure --profile myProfile
 
 Command options:
 
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
 This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
 The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
 
@@ -122,13 +128,20 @@
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 * **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
+Release Notes
+-------------
+
+Version: TODO
+
+TODO
+
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/__pycache__/cli.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/__pycache__/cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 21:06:20 2023 UTC, .py size: 1354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,84 @@
-00000000: 6f0d 0d0a 0000 0000 4c7d 8b64 4a05 0000  o.......L}.dJ...
+00000000: 6f0d 0d0a 0000 0000 9ea7 8d64 0b05 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6403 6404 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6403 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6403 6406 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6403 6408 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6501 6a0e 6409 640a 8d01  m.Z...e.j.d.d...
 00000090: 6501 6a0f 650d 640b 640c 8d02 6501 6a10  e.j.e.d.d...e.j.
 000000a0: 640d 640e 8400 8301 8301 8301 5a11 6511  d.d.........Z.e.
 000000b0: a012 6505 a101 0100 6511 a012 6507 a101  ..e.....e...e...
 000000c0: 0100 6511 a012 6509 a101 0100 6511 a012  ..e...e.....e...
-000000d0: 650b a101 0100 6513 640f 6b02 725d 6511  e.....e.d.k.r]e.
-000000e0: 8300 0100 6402 5300 6402 5300 2910 613c  ....d.S.d.S.).a<
-000000f0: 0100 000a 436f 7079 7269 6768 7420 2843  ....Copyright (C
-00000100: 2920 3230 3232 2d32 3032 3320 5374 656c  ) 2022-2023 Stel
-00000110: 6c61 2054 6563 686e 6f6c 6f67 6965 7320  la Technologies 
-00000120: 2855 4b29 204c 696d 6974 6564 2e0a 0a54  (UK) Limited...T
-00000130: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
-00000140: 7468 6520 7072 6f70 7269 6574 6172 7920  the proprietary 
-00000150: 696e 666f 726d 6174 696f 6e20 6f66 2053  information of S
-00000160: 7465 6c6c 6120 5465 6368 6e6f 6c6f 6769  tella Technologi
-00000170: 6573 2028 554b 2920 4c69 6d69 7465 642e  es (UK) Limited.
-00000180: 0a55 7365 2c20 7265 7072 6f64 7563 7469  .Use, reproducti
-00000190: 6f6e 2c20 6f72 2072 6564 6973 7472 6962  on, or redistrib
-000001a0: 7574 696f 6e20 6f66 2074 6869 7320 736f  ution of this so
-000001b0: 6674 7761 7265 2069 7320 7374 7269 6374  ftware is strict
-000001c0: 6c79 2070 726f 6869 6269 7465 6420 7769  ly prohibited wi
-000001d0: 7468 6f75 740a 7468 6520 6578 7072 6573  thout.the expres
-000001e0: 7320 7772 6974 7465 6e20 7065 726d 6973  s written permis
-000001f0: 7369 6f6e 206f 6620 5374 656c 6c61 2054  sion of Stella T
-00000200: 6563 686e 6f6c 6f67 6965 7320 2855 4b29  echnologies (UK)
-00000210: 204c 696d 6974 6564 2e0a 416c 6c20 7269   Limited..All ri
-00000220: 6768 7473 2072 6573 6572 7665 642e 0ae9  ghts reserved...
-00000230: 0000 0000 4ee9 0100 0000 2901 da0d 636f  ....N.....)...co
-00000240: 6e66 6967 7572 655f 636d 6429 01da 0c67  nfigure_cmd)...g
-00000250: 656e 6572 6174 655f 636d 6429 01da 0870  enerate_cmd)...p
-00000260: 6c61 6e5f 636d 6429 01da 0a65 7665 6e74  lan_cmd)...event
-00000270: 735f 636d 6429 01da 0b5f 5f76 6572 7369  s_cmd)...__versi
-00000280: 6f6e 5f5f 5429 01da 0563 6861 696e 7a0b  on__T)...chainz.
-00000290: 2528 7665 7273 696f 6e29 7329 02da 0776  %(version)s)...v
-000002a0: 6572 7369 6f6e da07 6d65 7373 6167 6563  ersion..messagec
-000002b0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000002c0: 0700 0000 4300 0000 7334 0000 0074 00a0  ....C...s4...t..
-000002d0: 01a1 007d 0174 026a 03a0 0464 01a1 017d  ...}.t.j...d...}
-000002e0: 027c 01a0 0574 026a 03a0 067c 0264 0264  .|...t.j...|.d.d
-000002f0: 03a1 03a1 0101 007c 017c 005f 0764 0453  .......|.|._.d.S
-00000300: 0029 057a 5143 6f6d 6d61 6e64 2d6c 696e  .).zQCommand-lin
-00000310: 6520 696e 7465 7266 6163 6520 666f 7220  e interface for 
-00000320: 7468 6520 5374 656c 6c61 4e6f 7720 5344  the StellaNow SD
-00000330: 4b20 636f 6465 2067 656e 6572 6174 696f  K code generatio
-00000340: 6e20 616e 6420 636f 6d70 6172 6973 6f6e  n and comparison
-00000350: 2074 6f6f 6c2e fa01 7e7a 0a2e 7374 656c   tool...~z..stel
-00000360: 6c61 6e6f 777a 0a63 6f6e 6669 672e 696e  lanowz.config.in
-00000370: 694e 2908 da0c 636f 6e66 6967 7061 7273  iN)...configpars
-00000380: 6572 5a0c 436f 6e66 6967 5061 7273 6572  erZ.ConfigParser
-00000390: da02 6f73 da04 7061 7468 da0a 6578 7061  ..os..path..expa
-000003a0: 6e64 7573 6572 da04 7265 6164 da04 6a6f  nduser..read..jo
-000003b0: 696e da03 6f62 6a29 03da 0363 7478 5a06  in..obj)...ctxZ.
-000003c0: 636f 6e66 6967 da04 686f 6d65 a900 7215  config..home..r.
-000003d0: 0000 00fa 512f 5573 6572 732f 746f 6d2d  ....Q/Users/tom-
-000003e0: 6b61 6e64 7a69 6f72 612f 4465 764c 6f63  kandziora/DevLoc
-000003f0: 616c 2f73 7465 6c6c 612f 7374 656c 6c61  al/stella/stella
-00000400: 2d6e 6f77 2f53 7465 6c6c 614e 6f77 434c  -now/StellaNowCL
-00000410: 492f 7374 656c 6c61 6e6f 775f 636c 692f  I/stellanow_cli/
-00000420: 636c 692e 7079 da03 636c 6917 0000 0073  cli.py..cli....s
-00000430: 0800 0000 0806 0c03 1603 0a03 7217 0000  ............r...
-00000440: 00da 085f 5f6d 6169 6e5f 5f29 14da 075f  ...__main__)..._
-00000450: 5f64 6f63 5f5f 5a05 636c 6963 6b72 0c00  _doc__Z.clickr..
-00000460: 0000 720d 0000 005a 1263 6f6d 6d61 6e64  ..r....Z.command
-00000470: 732e 636f 6e66 6967 7572 6572 0300 0000  s.configurer....
-00000480: 5a11 636f 6d6d 616e 6473 2e67 656e 6572  Z.commands.gener
-00000490: 6174 6572 0400 0000 5a0d 636f 6d6d 616e  ater....Z.comman
-000004a0: 6473 2e70 6c61 6e72 0500 0000 5a0f 636f  ds.planr....Z.co
-000004b0: 6d6d 616e 6473 2e65 7665 6e74 7372 0600  mmands.eventsr..
-000004c0: 0000 5a08 5f76 6572 7369 6f6e 7207 0000  ..Z._versionr...
-000004d0: 00da 0567 726f 7570 5a0e 7665 7273 696f  ...groupZ.versio
-000004e0: 6e5f 6f70 7469 6f6e 5a0c 7061 7373 5f63  n_optionZ.pass_c
-000004f0: 6f6e 7465 7874 7217 0000 005a 0b61 6464  ontextr....Z.add
-00000500: 5f63 6f6d 6d61 6e64 da08 5f5f 6e61 6d65  _command..__name
-00000510: 5f5f 7215 0000 0072 1500 0000 7215 0000  __r....r....r...
-00000520: 0072 1600 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000530: 0100 0000 7328 0000 0004 0208 0908 0108  ....s(..........
-00000540: 010c 020c 010c 010c 010c 010a 030c 0104  ................
-00000550: 010e 010a 0f0a 010a 010a 0108 030a 0104  ................
-00000560: ff                                       .
+000000d0: 650b a101 0100 6402 5300 290f 613c 0100  e.....d.S.).a<..
+000000e0: 000a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
+000000f0: 3230 3232 2d32 3032 3320 5374 656c 6c61  2022-2023 Stella
+00000100: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
+00000110: 4b29 204c 696d 6974 6564 2e0a 0a54 6869  K) Limited...Thi
+00000120: 7320 736f 6674 7761 7265 2069 7320 7468  s software is th
+00000130: 6520 7072 6f70 7269 6574 6172 7920 696e  e proprietary in
+00000140: 666f 726d 6174 696f 6e20 6f66 2053 7465  formation of Ste
+00000150: 6c6c 6120 5465 6368 6e6f 6c6f 6769 6573  lla Technologies
+00000160: 2028 554b 2920 4c69 6d69 7465 642e 0a55   (UK) Limited..U
+00000170: 7365 2c20 7265 7072 6f64 7563 7469 6f6e  se, reproduction
+00000180: 2c20 6f72 2072 6564 6973 7472 6962 7574  , or redistribut
+00000190: 696f 6e20 6f66 2074 6869 7320 736f 6674  ion of this soft
+000001a0: 7761 7265 2069 7320 7374 7269 6374 6c79  ware is strictly
+000001b0: 2070 726f 6869 6269 7465 6420 7769 7468   prohibited with
+000001c0: 6f75 740a 7468 6520 6578 7072 6573 7320  out.the express 
+000001d0: 7772 6974 7465 6e20 7065 726d 6973 7369  written permissi
+000001e0: 6f6e 206f 6620 5374 656c 6c61 2054 6563  on of Stella Tec
+000001f0: 686e 6f6c 6f67 6965 7320 2855 4b29 204c  hnologies (UK) L
+00000200: 696d 6974 6564 2e0a 416c 6c20 7269 6768  imited..All righ
+00000210: 7473 2072 6573 6572 7665 642e 0ae9 0000  ts reserved.....
+00000220: 0000 4ee9 0100 0000 2901 da0d 636f 6e66  ..N.....)...conf
+00000230: 6967 7572 655f 636d 6429 01da 0c67 656e  igure_cmd)...gen
+00000240: 6572 6174 655f 636d 6429 01da 0870 6c61  erate_cmd)...pla
+00000250: 6e5f 636d 6429 01da 0a65 7665 6e74 735f  n_cmd)...events_
+00000260: 636d 6429 01da 0b5f 5f76 6572 7369 6f6e  cmd)...__version
+00000270: 5f5f 5429 01da 0563 6861 696e 7a0b 2528  __T)...chainz.%(
+00000280: 7665 7273 696f 6e29 7329 02da 0776 6572  version)s)...ver
+00000290: 7369 6f6e da07 6d65 7373 6167 6563 0100  sion..messagec..
+000002a0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+000002b0: 0000 4300 0000 7334 0000 0074 00a0 01a1  ..C...s4...t....
+000002c0: 007d 0174 026a 03a0 0464 01a1 017d 027c  .}.t.j...d...}.|
+000002d0: 01a0 0574 026a 03a0 067c 0264 0264 03a1  ...t.j...|.d.d..
+000002e0: 03a1 0101 007c 017c 005f 0764 0453 0029  .....|.|._.d.S.)
+000002f0: 057a 5143 6f6d 6d61 6e64 2d6c 696e 6520  .zQCommand-line 
+00000300: 696e 7465 7266 6163 6520 666f 7220 7468  interface for th
+00000310: 6520 5374 656c 6c61 4e6f 7720 5344 4b20  e StellaNow SDK 
+00000320: 636f 6465 2067 656e 6572 6174 696f 6e20  code generation 
+00000330: 616e 6420 636f 6d70 6172 6973 6f6e 2074  and comparison t
+00000340: 6f6f 6c2e fa01 7e7a 0a2e 7374 656c 6c61  ool...~z..stella
+00000350: 6e6f 777a 0a63 6f6e 6669 672e 696e 694e  nowz.config.iniN
+00000360: 2908 da0c 636f 6e66 6967 7061 7273 6572  )...configparser
+00000370: 5a0c 436f 6e66 6967 5061 7273 6572 da02  Z.ConfigParser..
+00000380: 6f73 da04 7061 7468 da0a 6578 7061 6e64  os..path..expand
+00000390: 7573 6572 da04 7265 6164 da04 6a6f 696e  user..read..join
+000003a0: da03 6f62 6a29 03da 0363 7478 5a06 636f  ..obj)...ctxZ.co
+000003b0: 6e66 6967 da04 686f 6d65 a900 7215 0000  nfig..home..r...
+000003c0: 00fa 512f 5573 6572 732f 746f 6d2d 6b61  ..Q/Users/tom-ka
+000003d0: 6e64 7a69 6f72 612f 4465 764c 6f63 616c  ndziora/DevLocal
+000003e0: 2f73 7465 6c6c 612f 7374 656c 6c61 2d6e  /stella/stella-n
+000003f0: 6f77 2f53 7465 6c6c 614e 6f77 434c 492f  ow/StellaNowCLI/
+00000400: 7374 656c 6c61 6e6f 775f 636c 692f 636c  stellanow_cli/cl
+00000410: 692e 7079 da03 636c 6915 0000 0073 0800  i.py..cli....s..
+00000420: 0000 0806 0c03 1603 0a03 7217 0000 0029  ..........r....)
+00000430: 13da 075f 5f64 6f63 5f5f 5a05 636c 6963  ...__doc__Z.clic
+00000440: 6b72 0c00 0000 720d 0000 005a 1263 6f6d  kr....r....Z.com
+00000450: 6d61 6e64 732e 636f 6e66 6967 7572 6572  mands.configurer
+00000460: 0300 0000 5a11 636f 6d6d 616e 6473 2e67  ....Z.commands.g
+00000470: 656e 6572 6174 6572 0400 0000 5a0d 636f  enerater....Z.co
+00000480: 6d6d 616e 6473 2e70 6c61 6e72 0500 0000  mmands.planr....
+00000490: 5a0f 636f 6d6d 616e 6473 2e65 7665 6e74  Z.commands.event
+000004a0: 7372 0600 0000 5a08 5f76 6572 7369 6f6e  sr....Z._version
+000004b0: 7207 0000 00da 0567 726f 7570 5a0e 7665  r......groupZ.ve
+000004c0: 7273 696f 6e5f 6f70 7469 6f6e 5a0c 7061  rsion_optionZ.pa
+000004d0: 7373 5f63 6f6e 7465 7874 7217 0000 005a  ss_contextr....Z
+000004e0: 0b61 6464 5f63 6f6d 6d61 6e64 7215 0000  .add_commandr...
+000004f0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000500: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
+00000510: 0000 0004 0008 0908 0108 010c 020c 010c  ................
+00000520: 010c 010c 010a 030c 0104 010e 010a 0f0a  ................
+00000530: 010a 010e 01                             .....
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/__pycache__/command_config.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:52:20 2023 UTC, .py size: 3856 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,212 +1,236 @@
-00000000: 6f0d 0d0a 0000 0000 047a 8b64 100f 0000  o........z.d....
+00000000: 6f0d 0d0a 0000 0000 d575 9064 4110 0000  o........u.dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
+00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6402 6c03 5a03 6403 6404 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6403 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 6d06 5a06 0100 6403 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
-00000070: 0100 6403 6407 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
-00000080: 6408 6c0c 6d0d 5a0d 0100 6409 640a 8400  d.l.m.Z...d.d...
-00000090: 5a0e 640b 640c 8400 5a0f 6402 5300 290d  Z.d.d...Z.d.S.).
-000000a0: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
-000000b0: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
-000000c0: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-000000d0: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-000000e0: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
-000000f0: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
-00000100: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
-00000110: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
-00000120: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
-00000130: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
-00000140: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
-00000150: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
-00000160: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
-00000170: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
-00000180: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
-00000190: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
-000001a0: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
-000001b0: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
-000001c0: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
-000001d0: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-000001e0: 0ae9 0000 0000 4ee9 0100 0000 2901 da09  ......N.....)...
-000001f0: 5374 656c 6c61 4150 4929 02da 0c73 6574  StellaAPI)...set
-00000200: 7570 5f6c 6f67 6765 72da 066c 6f67 6765  up_logger..logge
-00000210: 7229 01da 0e73 6e61 6b65 5f74 6f5f 6361  r)...snake_to_ca
-00000220: 6d65 6c29 01da 0943 6f6e 6669 6744 6576  mel)...ConfigDev
-00000230: 2901 da09 436f 6e66 6967 496e 7463 0100  )...ConfigIntc..
-00000240: 0000 0000 0000 0000 0000 0300 0000 0c00  ................
-00000250: 0000 4300 0000 737c 0000 0074 006a 0164  ..C...s|...t.j.d
-00000260: 0164 0264 038d 0274 006a 0164 0464 0564  .d.d...t.j.d.d.d
-00000270: 0664 078d 0374 006a 0164 0864 0964 038d  .d...t.j.d.d.d..
-00000280: 0274 006a 0164 0a64 0b64 038d 0274 006a  .t.j.d.d.d...t.j
-00000290: 0164 0c64 0d64 0e64 0f8d 0374 006a 0164  .d.d.d.d...t.j.d
-000002a0: 1064 0564 1164 128d 0374 006a 0164 1364  .d.d.d...t.j.d.d
-000002b0: 1464 0564 1564 168d 0467 077d 0174 027c  .d.d.d...g.}.t.|
-000002c0: 0183 0144 005d 067d 027c 027c 0083 017d  ...D.].}.|.|...}
-000002d0: 0071 357c 0053 0029 177a 400a 2020 2020  .q5|.S.).z@.    
-000002e0: 436f 6d6d 6f6e 2043 4c49 206f 7074 696f  Common CLI optio
-000002f0: 6e73 2074 6f20 6265 2075 7365 6420 6163  ns to be used ac
-00000300: 726f 7373 206d 756c 7469 706c 6520 636f  ross multiple co
-00000310: 6d6d 616e 6473 0a20 2020 207a 0c2d 2d61  mmands.    z.--a
-00000320: 6363 6573 735f 6b65 797a 7854 6865 2061  ccess_keyzxThe a
-00000330: 6363 6573 7320 6b65 7920 6372 6564 656e  ccess key creden
-00000340: 7469 616c 2066 6f72 2061 6363 6573 7369  tial for accessi
-00000350: 6e67 2074 6865 2053 7465 6c6c 614e 6f77  ng the StellaNow
-00000360: 2041 5049 2e20 5468 6973 2073 686f 756c   API. This shoul
-00000370: 6420 6265 2074 6865 2073 616d 6520 6173  d be the same as
-00000380: 2079 6f75 7220 5374 656c 6c61 4e6f 7720   your StellaNow 
-00000390: 6163 636f 756e 7420 6163 6365 7373 206b  account access k
-000003a0: 6579 2e29 01da 0468 656c 707a 0e2d 2d61  ey.)...helpz.--a
-000003b0: 6363 6573 735f 746f 6b65 6e54 7a7c 5468  ccess_tokenTz|Th
-000003c0: 6520 6163 6365 7373 2074 6f6b 656e 2063  e access token c
-000003d0: 7265 6465 6e74 6961 6c20 666f 7220 6163  redential for ac
-000003e0: 6365 7373 696e 6720 7468 6520 5374 656c  cessing the Stel
-000003f0: 6c61 4e6f 7720 4150 492e 2054 6869 7320  laNow API. This 
-00000400: 7368 6f75 6c64 2062 6520 7468 6520 7361  should be the sa
-00000410: 6d65 2061 7320 796f 7572 2053 7465 6c6c  me as your Stell
-00000420: 614e 6f77 2061 6363 6f75 6e74 2061 6363  aNow account acc
-00000430: 6573 7320 746f 6b65 6e2e 2902 da0a 6869  ess token.)...hi
-00000440: 6465 5f69 6e70 7574 7209 0000 007a 112d  de_inputr....z.-
-00000450: 2d6f 7267 616e 697a 6174 696f 6e5f 6964  -organization_id
-00000460: 7a8c 5468 6520 756e 6971 7565 2069 6465  z.The unique ide
-00000470: 6e74 6966 6965 7220 2855 5549 4429 206f  ntifier (UUID) o
-00000480: 6620 7468 6520 6f72 6761 6e69 7a61 7469  f the organizati
-00000490: 6f6e 2069 6e20 5374 656c 6c61 4e6f 772e  on in StellaNow.
-000004a0: 2054 6869 7320 6973 2075 7365 6420 746f   This is used to
-000004b0: 2073 636f 7065 2074 6865 206f 7065 7261   scope the opera
-000004c0: 7469 6f6e 7320 7769 7468 696e 2074 6865  tions within the
-000004d0: 2067 6976 656e 206f 7267 616e 697a 6174   given organizat
-000004e0: 696f 6e27 7320 636f 6e74 6578 742e 7a0c  ion's context.z.
-000004f0: 2d2d 7072 6f6a 6563 745f 6964 7a82 5468  --project_idz.Th
-00000500: 6520 756e 6971 7565 2069 6465 6e74 6966  e unique identif
-00000510: 6965 7220 2855 5549 4429 206f 6620 7468  ier (UUID) of th
-00000520: 6520 7072 6f6a 6563 7420 696e 2053 7465  e project in Ste
-00000530: 6c6c 614e 6f77 2e20 5468 6973 2069 7320  llaNow. This is 
-00000540: 7573 6564 2074 6f20 7363 6f70 6520 7468  used to scope th
-00000550: 6520 6f70 6572 6174 696f 6e73 2077 6974  e operations wit
-00000560: 6869 6e20 7468 6520 6769 7665 6e20 7072  hin the given pr
-00000570: 6f6a 6563 7427 7320 636f 6e74 6578 742e  oject's context.
-00000580: 7a09 2d2d 7072 6f66 696c 65da 0744 4546  z.--profile..DEF
-00000590: 4155 4c54 7a9b 5468 6520 7072 6f66 696c  AULTz.The profil
-000005a0: 6520 6e61 6d65 2066 6f72 2073 746f 7269  e name for stori
-000005b0: 6e67 2061 2070 6172 7469 6375 6c61 7220  ng a particular 
-000005c0: 7365 7420 6f66 2063 6f6e 6669 6775 7261  set of configura
-000005d0: 7469 6f6e 732e 2049 6620 6e6f 2070 726f  tions. If no pro
-000005e0: 6669 6c65 2069 7320 7370 6563 6966 6965  file is specifie
-000005f0: 642c 2074 6865 2063 6f6e 6669 6775 7261  d, the configura
-00000600: 7469 6f6e 7320 7769 6c6c 2062 6520 7374  tions will be st
-00000610: 6f72 6564 2075 6e64 6572 2074 6865 2027  ored under the '
-00000620: 4445 4641 554c 5427 2070 726f 6669 6c65  DEFAULT' profile
-00000630: 2e29 02da 0764 6566 6175 6c74 7209 0000  .)...defaultr...
-00000640: 007a 052d 2d65 6e76 da00 2902 da06 6869  .z.--env..)...hi
-00000650: 6464 656e 7209 0000 007a 092d 2d76 6572  ddenr....z.--ver
-00000660: 626f 7365 7a02 2d76 7a43 456e 6162 6c65  bosez.-vzCEnable
-00000670: 7320 7665 7262 6f73 6520 6d6f 6465 2c20  s verbose mode, 
-00000680: 7768 6963 6820 6f75 7470 7574 7320 6d6f  which outputs mo
-00000690: 7265 2064 6574 6169 6c65 6420 6c6f 6767  re detailed logg
-000006a0: 696e 6720 6d65 7373 6167 6573 2e29 02da  ing messages.)..
-000006b0: 0769 735f 666c 6167 7209 0000 0029 03da  .is_flagr....)..
-000006c0: 0563 6c69 636b da06 6f70 7469 6f6e da08  .click..option..
-000006d0: 7265 7665 7273 6564 2903 da01 66da 0a64  reversed)...f..d
-000006e0: 6563 6f72 6174 6f72 73da 0964 6563 6f72  ecorators..decor
-000006f0: 6174 6f72 a900 7216 0000 00fa 5c2f 5573  ator..r.....\/Us
-00000700: 6572 732f 746f 6d2d 6b61 6e64 7a69 6f72  ers/tom-kandzior
-00000710: 612f 4465 764c 6f63 616c 2f73 7465 6c6c  a/DevLocal/stell
-00000720: 612f 7374 656c 6c61 2d6e 6f77 2f53 7465  a/stella-now/Ste
-00000730: 6c6c 614e 6f77 434c 492f 7374 656c 6c61  llaNowCLI/stella
-00000740: 6e6f 775f 636c 692f 636f 6d6d 616e 645f  now_cli/command_
-00000750: 636f 6e66 6967 2e70 79da 0d63 6f6d 6d6f  config.py..commo
-00000760: 6e5f 6f70 7469 6f6e 1500 0000 732a 0000  n_option....s*..
-00000770: 0006 0502 0104 ff08 0302 0104 ff06 0302  ................
-00000780: 0104 ff06 0302 0104 ff08 0302 0104 ff0e  ................
-00000790: 0310 0104 ef0c 150a 0104 0172 1800 0000  ...........r....
-000007a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000007b0: 0004 0000 0003 0000 0073 1a00 0000 7400  .........s....t.
-000007c0: a001 8800 a101 8700 6601 6401 6402 8408  ........f.d.d...
-000007d0: 8301 7d01 7c01 5300 2903 4e63 0000 0000  ..}.|.S.).Nc....
-000007e0: 0000 0000 0000 0000 0800 0000 0800 0000  ................
-000007f0: 1f00 0000 7336 0100 0074 00a0 01a1 007d  ....s6...t.....}
-00000800: 027c 01a0 0264 0164 02a1 027d 0374 03a0  .|...d.d...}.t..
-00000810: 0464 03a1 0174 03a0 0464 04a1 0164 059c  .d...t...d...d..
-00000820: 027d 0464 0644 005d 287d 057c 057c 0476  .}.d.D.](}.|.|.v
-00000830: 0072 2a7c 047c 0519 0064 0075 0172 2a7c  .r*|.|...d.u.r*|
-00000840: 047c 0519 007c 017c 053c 0071 177c 057c  .|...|.|.<.q.|.|
-00000850: 0176 0173 347c 017c 0519 0064 0075 0072  .v.s4|.|...d.u.r
-00000860: 3f7c 026a 056a 027c 037c 0564 0064 078d  ?|.j.j.|.|.d.d..
-00000870: 037c 017c 053c 0071 177c 0164 0819 0064  .|.|.<.q.|.d...d
-00000880: 0075 0072 4a64 097c 0164 083c 0074 067c  .u.rJd.|.d.<.t.|
-00000890: 01a0 0264 0aa1 0183 0101 0074 0764 0b64  ...d.......t.d.d
-000008a0: 0c84 007c 01a0 08a1 0044 0083 0183 0172  ...|.....D.....r
-000008b0: 6674 09a0 0a64 0da1 0101 007c 02a0 0b64  ft...d.....|...d
-000008c0: 0ea1 0101 0064 0f74 0c7c 01a0 0264 08a1  .....d.t.|...d..
-000008d0: 0183 019b 009d 027d 0674 0d83 00a0 027c  .......}.t.....|
-000008e0: 06a1 0170 7774 0e7d 0774 0f7c 0783 007c  ...pwt.}.t.|...|
-000008f0: 01a0 0264 10a1 017c 01a0 0264 11a1 017c  ...d...|...d...|
-00000900: 01a0 0264 12a1 017c 01a0 0264 13a1 0183  ...d...|...d....
-00000910: 057c 0164 143c 007c 026a 1088 0067 017c  .|.d.<.|.j...g.|
-00000920: 00a2 0152 0069 007c 01a4 018e 0153 0029  ...R.i.|.....S.)
-00000930: 154e da07 7072 6f66 696c 6572 0b00 0000  .N..profiler....
-00000940: 5a14 5354 454c 4c41 4e4f 575f 4143 4345  Z.STELLANOW_ACCE
-00000950: 5353 5f4b 4559 5a16 5354 454c 4c41 4e4f  SS_KEYZ.STELLANO
-00000960: 575f 4143 4345 5353 5f54 4f4b 454e 2902  W_ACCESS_TOKEN).
-00000970: da0a 6163 6365 7373 5f6b 6579 da0c 6163  ..access_key..ac
-00000980: 6365 7373 5f74 6f6b 656e 2906 721a 0000  cess_token).r...
-00000990: 0072 1b00 0000 da0f 6f72 6761 6e69 7a61  .r......organiza
-000009a0: 7469 6f6e 5f69 64da 0a70 726f 6a65 6374  tion_id..project
-000009b0: 5f69 6472 1900 0000 da03 656e 7629 01da  _idr......env)..
-000009c0: 0866 616c 6c62 6163 6b72 1e00 0000 5a03  .fallbackr....Z.
-000009d0: 4e69 6cda 0776 6572 626f 7365 6301 0000  Nil..verbosec...
-000009e0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000009f0: 0073 0000 0073 1800 0000 8100 7c00 5d07  .s...s......|.].
-00000a00: 7d01 7c01 6400 7500 5600 0100 7102 6400  }.|.d.u.V...q.d.
-00000a10: 5300 2901 4e72 1600 0000 2902 da02 2e30  S.).Nr....)....0
-00000a20: da05 7661 6c75 6572 1600 0000 7216 0000  ..valuer....r...
-00000a30: 0072 1700 0000 da09 3c67 656e 6578 7072  .r......<genexpr
-00000a40: 3e4d 0000 0073 0400 0000 0280 1600 7a2f  >M...s........z/
-00000a50: 6c6f 6164 5f63 6f6e 6669 672e 3c6c 6f63  load_config.<loc
-00000a60: 616c 733e 2e77 7261 7070 6572 2e3c 6c6f  als>.wrapper.<lo
-00000a70: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
-00000a80: 5141 6c6c 2072 6571 7569 7265 6420 6f70  QAll required op
-00000a90: 7469 6f6e 7320 6172 6520 6e6f 7420 7365  tions are not se
-00000aa0: 742e 2050 6c65 6173 6520 7573 6520 7468  t. Please use th
-00000ab0: 6520 2263 6f6e 6669 6775 7265 2220 636f  e "configure" co
-00000ac0: 6d6d 616e 6420 746f 2073 6574 2074 6865  mmand to set the
-00000ad0: 6d2e 7202 0000 00da 0643 6f6e 6669 6772  m.r......Configr
-00000ae0: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00000af0: 0000 00da 0a73 7465 6c6c 615f 6170 6929  .....stella_api)
-00000b00: 1172 1000 0000 da13 6765 745f 6375 7272  .r......get_curr
-00000b10: 656e 745f 636f 6e74 6578 74da 0367 6574  ent_context..get
-00000b20: da02 6f73 da06 6765 7465 6e76 da03 6f62  ..os..getenv..ob
-00000b30: 6a72 0400 0000 da03 616e 79da 0676 616c  jr......any..val
-00000b40: 7565 7372 0500 0000 da05 6572 726f 72da  uesr......error.
-00000b50: 0465 7869 7472 0600 0000 da07 676c 6f62  .exitr......glob
-00000b60: 616c 7372 0800 0000 7203 0000 00da 0669  alsr....r......i
-00000b70: 6e76 6f6b 6529 08da 0461 7267 73da 066b  nvoke)...args..k
-00000b80: 7761 7267 73da 0363 7478 7219 0000 005a  wargs..ctxr....Z
-00000b90: 0865 6e76 5f76 6172 73da 036b 6579 5a15  .env_vars..keyZ.
-00000ba0: 656e 765f 636f 6e66 6967 5f63 6c61 7373  env_config_class
-00000bb0: 5f6e 616d 655a 1065 6e76 5f63 6f6e 6669  _nameZ.env_confi
-00000bc0: 675f 636c 6173 73a9 0172 1300 0000 7216  g_class..r....r.
-00000bd0: 0000 0072 1700 0000 da07 7772 6170 7065  ...r......wrappe
-00000be0: 7234 0000 0073 3600 0000 0802 0c02 0803  r4...s6.........
-00000bf0: 0801 06fe 0805 1402 0e01 1402 1601 0280  ................
-00000c00: 0c02 0801 0e02 1603 0a01 0a01 1402 1001  ................
-00000c10: 0203 0401 0801 0801 0801 0801 08fb 1808  ................
-00000c20: 7a1c 6c6f 6164 5f63 6f6e 6669 672e 3c6c  z.load_config.<l
-00000c30: 6f63 616c 733e 2e77 7261 7070 6572 2902  ocals>.wrapper).
-00000c40: da09 6675 6e63 746f 6f6c 73da 0577 7261  ..functools..wra
-00000c50: 7073 2902 7213 0000 0072 3600 0000 7216  ps).r....r6...r.
-00000c60: 0000 0072 3500 0000 7217 0000 00da 0b6c  ...r5...r......l
-00000c70: 6f61 645f 636f 6e66 6967 3300 0000 7306  oad_config3...s.
-00000c80: 0000 0008 010e 0104 2a72 3900 0000 2910  ........*r9...).
-00000c90: da07 5f5f 646f 635f 5f72 1000 0000 7237  ..__doc__r....r7
-00000ca0: 0000 0072 2800 0000 5a03 6170 6972 0300  ...r(...Z.apir..
-00000cb0: 0000 7205 0000 0072 0400 0000 da05 7574  ..r....r......ut
-00000cc0: 696c 7372 0600 0000 5a0a 636f 6e66 6967  ilsr....Z.config
-00000cd0: 2e64 6576 7207 0000 005a 0a63 6f6e 6669  .devr....Z.confi
-00000ce0: 672e 696e 7472 0800 0000 7218 0000 0072  g.intr....r....r
-00000cf0: 3900 0000 7216 0000 0072 1600 0000 7216  9...r....r....r.
-00000d00: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000d10: 653e 0100 0000 7316 0000 0004 0008 0908  e>....s.........
-00000d20: 0108 010c 0210 010c 010c 010c 0108 030c  ................
-00000d30: 1e                                       .
+00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 5a04 6401 6402 6c05 5a05 6403 6404 6c06  Z.d.d.l.Z.d.d.l.
+00000060: 6d07 5a07 0100 6403 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000070: 0100 6403 6406 6c0a 6d0b 5a0b 0100 6403  ..d.d.l.m.Z...d.
+00000080: 6407 6c0c 6d0d 5a0d 0100 6403 6408 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6504 a010 6511 a101 5a12  m.Z...e...e...Z.
+000000a0: 6409 640a 8400 5a13 640b 640c 8400 5a14  d.d...Z.d.d...Z.
+000000b0: 6402 5300 290d 613c 0100 000a 436f 7079  d.S.).a<....Copy
+000000c0: 7269 6768 7420 2843 2920 3230 3232 2d32  right (C) 2022-2
+000000d0: 3032 3320 5374 656c 6c61 2054 6563 686e  023 Stella Techn
+000000e0: 6f6c 6f67 6965 7320 2855 4b29 204c 696d  ologies (UK) Lim
+000000f0: 6974 6564 2e0a 0a54 6869 7320 736f 6674  ited...This soft
+00000100: 7761 7265 2069 7320 7468 6520 7072 6f70  ware is the prop
+00000110: 7269 6574 6172 7920 696e 666f 726d 6174  rietary informat
+00000120: 696f 6e20 6f66 2053 7465 6c6c 6120 5465  ion of Stella Te
+00000130: 6368 6e6f 6c6f 6769 6573 2028 554b 2920  chnologies (UK) 
+00000140: 4c69 6d69 7465 642e 0a55 7365 2c20 7265  Limited..Use, re
+00000150: 7072 6f64 7563 7469 6f6e 2c20 6f72 2072  production, or r
+00000160: 6564 6973 7472 6962 7574 696f 6e20 6f66  edistribution of
+00000170: 2074 6869 7320 736f 6674 7761 7265 2069   this software i
+00000180: 7320 7374 7269 6374 6c79 2070 726f 6869  s strictly prohi
+00000190: 6269 7465 6420 7769 7468 6f75 740a 7468  bited without.th
+000001a0: 6520 6578 7072 6573 7320 7772 6974 7465  e express writte
+000001b0: 6e20 7065 726d 6973 7369 6f6e 206f 6620  n permission of 
+000001c0: 5374 656c 6c61 2054 6563 686e 6f6c 6f67  Stella Technolog
+000001d0: 6965 7320 2855 4b29 204c 696d 6974 6564  ies (UK) Limited
+000001e0: 2e0a 416c 6c20 7269 6768 7473 2072 6573  ..All rights res
+000001f0: 6572 7665 642e 0ae9 0000 0000 4ee9 0200  erved.......N...
+00000200: 0000 2901 da09 5374 656c 6c61 4150 4929  ..)...StellaAPI)
+00000210: 01da 0943 6f6e 6669 6749 6e74 2901 da03  ...ConfigInt)...
+00000220: 456e 7629 01da 0c73 6574 7570 5f6c 6f67  Env)...setup_log
+00000230: 6765 7229 01da 0e73 6e61 6b65 5f74 6f5f  ger)...snake_to_
+00000240: 6361 6d65 6c63 0100 0000 0000 0000 0000  camelc..........
+00000250: 0000 0300 0000 0c00 0000 4300 0000 7392  ..........C...s.
+00000260: 0000 0074 006a 0164 0164 0264 038d 0274  ...t.j.d.d.d...t
+00000270: 006a 0164 0464 0564 0664 078d 0374 006a  .j.d.d.d.d...t.j
+00000280: 0164 0864 0964 038d 0274 006a 0164 0a64  .d.d.d...t.j.d.d
+00000290: 0b64 038d 0274 006a 0164 0c64 0d64 0e64  .d...t.j.d.d.d.d
+000002a0: 0f8d 0374 006a 0164 1064 0574 006a 0264  ...t.j.d.d.t.j.d
+000002b0: 1164 1284 0074 0344 0083 0164 1364 148d  .d...t.D...d.d..
+000002c0: 0264 1564 168d 0474 006a 0164 1764 1864  .d.d...t.j.d.d.d
+000002d0: 0564 1964 1a8d 0467 077d 0174 047c 0183  .d.d...g.}.t.|..
+000002e0: 0144 005d 067d 027c 027c 0083 017d 0071  .D.].}.|.|...}.q
+000002f0: 407c 0053 0029 1b7a 400a 2020 2020 436f  @|.S.).z@.    Co
+00000300: 6d6d 6f6e 2043 4c49 206f 7074 696f 6e73  mmon CLI options
+00000310: 2074 6f20 6265 2075 7365 6420 6163 726f   to be used acro
+00000320: 7373 206d 756c 7469 706c 6520 636f 6d6d  ss multiple comm
+00000330: 616e 6473 0a20 2020 207a 0c2d 2d61 6363  ands.    z.--acc
+00000340: 6573 735f 6b65 797a 7854 6865 2061 6363  ess_keyzxThe acc
+00000350: 6573 7320 6b65 7920 6372 6564 656e 7469  ess key credenti
+00000360: 616c 2066 6f72 2061 6363 6573 7369 6e67  al for accessing
+00000370: 2074 6865 2053 7465 6c6c 614e 6f77 2041   the StellaNow A
+00000380: 5049 2e20 5468 6973 2073 686f 756c 6420  PI. This should 
+00000390: 6265 2074 6865 2073 616d 6520 6173 2079  be the same as y
+000003a0: 6f75 7220 5374 656c 6c61 4e6f 7720 6163  our StellaNow ac
+000003b0: 636f 756e 7420 6163 6365 7373 206b 6579  count access key
+000003c0: 2e29 01da 0468 656c 707a 0e2d 2d61 6363  .)...helpz.--acc
+000003d0: 6573 735f 746f 6b65 6e54 7a7c 5468 6520  ess_tokenTz|The 
+000003e0: 6163 6365 7373 2074 6f6b 656e 2063 7265  access token cre
+000003f0: 6465 6e74 6961 6c20 666f 7220 6163 6365  dential for acce
+00000400: 7373 696e 6720 7468 6520 5374 656c 6c61  ssing the Stella
+00000410: 4e6f 7720 4150 492e 2054 6869 7320 7368  Now API. This sh
+00000420: 6f75 6c64 2062 6520 7468 6520 7361 6d65  ould be the same
+00000430: 2061 7320 796f 7572 2053 7465 6c6c 614e   as your StellaN
+00000440: 6f77 2061 6363 6f75 6e74 2061 6363 6573  ow account acces
+00000450: 7320 746f 6b65 6e2e 2902 da0a 6869 6465  s token.)...hide
+00000460: 5f69 6e70 7574 7208 0000 007a 112d 2d6f  _inputr....z.--o
+00000470: 7267 616e 697a 6174 696f 6e5f 6964 7a8c  rganization_idz.
+00000480: 5468 6520 756e 6971 7565 2069 6465 6e74  The unique ident
+00000490: 6966 6965 7220 2855 5549 4429 206f 6620  ifier (UUID) of 
+000004a0: 7468 6520 6f72 6761 6e69 7a61 7469 6f6e  the organization
+000004b0: 2069 6e20 5374 656c 6c61 4e6f 772e 2054   in StellaNow. T
+000004c0: 6869 7320 6973 2075 7365 6420 746f 2073  his is used to s
+000004d0: 636f 7065 2074 6865 206f 7065 7261 7469  cope the operati
+000004e0: 6f6e 7320 7769 7468 696e 2074 6865 2067  ons within the g
+000004f0: 6976 656e 206f 7267 616e 697a 6174 696f  iven organizatio
+00000500: 6e27 7320 636f 6e74 6578 742e 7a0c 2d2d  n's context.z.--
+00000510: 7072 6f6a 6563 745f 6964 7a82 5468 6520  project_idz.The 
+00000520: 756e 6971 7565 2069 6465 6e74 6966 6965  unique identifie
+00000530: 7220 2855 5549 4429 206f 6620 7468 6520  r (UUID) of the 
+00000540: 7072 6f6a 6563 7420 696e 2053 7465 6c6c  project in Stell
+00000550: 614e 6f77 2e20 5468 6973 2069 7320 7573  aNow. This is us
+00000560: 6564 2074 6f20 7363 6f70 6520 7468 6520  ed to scope the 
+00000570: 6f70 6572 6174 696f 6e73 2077 6974 6869  operations withi
+00000580: 6e20 7468 6520 6769 7665 6e20 7072 6f6a  n the given proj
+00000590: 6563 7427 7320 636f 6e74 6578 742e 7a09  ect's context.z.
+000005a0: 2d2d 7072 6f66 696c 65da 0744 4546 4155  --profile..DEFAU
+000005b0: 4c54 7a9b 5468 6520 7072 6f66 696c 6520  LTz.The profile 
+000005c0: 6e61 6d65 2066 6f72 2073 746f 7269 6e67  name for storing
+000005d0: 2061 2070 6172 7469 6375 6c61 7220 7365   a particular se
+000005e0: 7420 6f66 2063 6f6e 6669 6775 7261 7469  t of configurati
+000005f0: 6f6e 732e 2049 6620 6e6f 2070 726f 6669  ons. If no profi
+00000600: 6c65 2069 7320 7370 6563 6966 6965 642c  le is specified,
+00000610: 2074 6865 2063 6f6e 6669 6775 7261 7469   the configurati
+00000620: 6f6e 7320 7769 6c6c 2062 6520 7374 6f72  ons will be stor
+00000630: 6564 2075 6e64 6572 2074 6865 2027 4445  ed under the 'DE
+00000640: 4641 554c 5427 2070 726f 6669 6c65 2e29  FAULT' profile.)
+00000650: 02da 0764 6566 6175 6c74 7208 0000 007a  ...defaultr....z
+00000660: 052d 2d65 6e76 6301 0000 0000 0000 0000  .--envc.........
+00000670: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000680: 1200 0000 6700 7c00 5d05 7d01 7c01 6a00  ....g.|.].}.|.j.
+00000690: 9102 7102 5300 a900 2901 da05 7661 6c75  ..q.S...)...valu
+000006a0: 6529 02da 022e 30da 0165 720c 0000 0072  e)....0..er....r
+000006b0: 0c00 0000 fa65 2f55 7365 7273 2f74 6f6d  .....e/Users/tom
+000006c0: 2d6b 616e 647a 696f 7261 2f44 6576 4c6f  -kandziora/DevLo
+000006d0: 6361 6c2f 7374 656c 6c61 2f73 7465 6c6c  cal/stella/stell
+000006e0: 612d 6e6f 772f 5374 656c 6c61 4e6f 7743  a-now/StellaNowC
+000006f0: 4c49 2f73 7465 6c6c 616e 6f77 5f63 6c69  LI/stellanow_cli
+00000700: 2f63 6f6d 6d61 6e64 732f 636f 6d6d 616e  /commands/comman
+00000710: 645f 636f 6e66 6967 2e70 79da 0a3c 6c69  d_config.py..<li
+00000720: 7374 636f 6d70 3e2e 0000 0073 0200 0000  stcomp>....s....
+00000730: 1200 7a21 636f 6d6d 6f6e 5f6f 7074 696f  ..z!common_optio
+00000740: 6e2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  n.<locals>.<list
+00000750: 636f 6d70 3e46 2901 da0e 6361 7365 5f73  comp>F)...case_s
+00000760: 656e 7369 7469 7665 da00 2903 da06 6869  ensitive..)...hi
+00000770: 6464 656e da04 7479 7065 7208 0000 007a  dden..typer....z
+00000780: 092d 2d76 6572 626f 7365 7a02 2d76 7a43  .--verbosez.-vzC
+00000790: 456e 6162 6c65 7320 7665 7262 6f73 6520  Enables verbose 
+000007a0: 6d6f 6465 2c20 7768 6963 6820 6f75 7470  mode, which outp
+000007b0: 7574 7320 6d6f 7265 2064 6574 6169 6c65  uts more detaile
+000007c0: 6420 6c6f 6767 696e 6720 6d65 7373 6167  d logging messag
+000007d0: 6573 2e29 02da 0769 735f 666c 6167 7208  es.)...is_flagr.
+000007e0: 0000 0029 05da 0563 6c69 636b da06 6f70  ...)...click..op
+000007f0: 7469 6f6e da06 4368 6f69 6365 7205 0000  tion..Choicer...
+00000800: 00da 0872 6576 6572 7365 6429 03da 0166  ...reversed)...f
+00000810: da0a 6465 636f 7261 746f 7273 da09 6465  ..decorators..de
+00000820: 636f 7261 746f 7272 0c00 0000 720c 0000  coratorr....r...
+00000830: 0072 1000 0000 da0d 636f 6d6d 6f6e 5f6f  .r......common_o
+00000840: 7074 696f 6e1a 0000 0073 2a00 0000 0605  ption....s*.....
+00000850: 0201 04ff 0803 0201 04ff 0603 0201 04ff  ................
+00000860: 0603 0201 04ff 0803 0201 04ff 2403 1001  ............$...
+00000870: 04ef 0c15 0a01 0401 721e 0000 0063 0100  ........r....c..
+00000880: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000890: 0000 0300 0000 731a 0000 0074 00a0 0188  ......s....t....
+000008a0: 00a1 0187 0066 0164 0164 0284 0883 017d  .....f.d.d.....}
+000008b0: 017c 0153 0029 034e 6300 0000 0000 0000  .|.S.).Nc.......
+000008c0: 0000 0000 0008 0000 0008 0000 001f 0000  ................
+000008d0: 0073 5e01 0000 7400 a001 a100 7d02 7c01  .s^...t.....}.|.
+000008e0: a002 6401 6402 a102 7d03 7403 a004 6403  ..d.d...}.t...d.
+000008f0: a101 7403 a004 6404 a101 6405 9c02 7d04  ..t...d...d...}.
+00000900: 6406 4400 5d28 7d05 7c05 7c04 7600 722a  d.D.](}.|.|.v.r*
+00000910: 7c04 7c05 1900 6400 7501 722a 7c04 7c05  |.|...d.u.r*|.|.
+00000920: 1900 7c01 7c05 3c00 7117 7c05 7c01 7601  ..|.|.<.q.|.|.v.
+00000930: 7334 7c01 7c05 1900 6400 7500 723f 7c02  s4|.|...d.u.r?|.
+00000940: 6a05 6a02 7c03 7c05 6400 6407 8d03 7c01  j.j.|.|.d.d...|.
+00000950: 7c05 3c00 7117 7c01 6408 1900 6400 7500  |.<.q.|.d...d.u.
+00000960: 724a 6409 7c01 6408 3c00 7406 7c01 a002  rJd.|.d.<.t.|...
+00000970: 640a a101 8301 0100 7407 640b 640c 8400  d.......t.d.d...
+00000980: 7c01 a008 a100 4400 8301 8301 7266 7409  |.....D.....rft.
+00000990: a00a 640d a101 0100 7c02 a00b 640e a101  ..d.....|...d...
+000009a0: 0100 640f 740c 7c01 a002 6408 a101 8301  ..d.t.|...d.....
+000009b0: 9b00 9d02 7d06 7a10 740d 740e a00f 6410  ....}.z.t.t...d.
+000009c0: 7c01 a002 6408 a101 9b00 9d02 a101 7c06  |...d.........|.
+000009d0: 8302 7d07 5700 6e0b 0400 7410 798b 0100  ..}.W.n...t.y...
+000009e0: 0100 0100 7411 7d07 5900 6e01 7700 7412  ....t.}.Y.n.w.t.
+000009f0: 7c07 8300 7c01 a002 6411 a101 7c01 a002  |...|...d...|...
+00000a00: 6412 a101 7c01 a002 6413 a101 7c01 a002  d...|...d...|...
+00000a10: 6414 a101 8305 7c01 6415 3c00 7c02 6a13  d.....|.d.<.|.j.
+00000a20: 8800 6701 7c00 a201 5200 6900 7c01 a401  ..g.|...R.i.|...
+00000a30: 8e01 5300 2916 4eda 0770 726f 6669 6c65  ..S.).N..profile
+00000a40: 720a 0000 005a 1453 5445 4c4c 414e 4f57  r....Z.STELLANOW
+00000a50: 5f41 4343 4553 535f 4b45 595a 1653 5445  _ACCESS_KEYZ.STE
+00000a60: 4c4c 414e 4f57 5f41 4343 4553 535f 544f  LLANOW_ACCESS_TO
+00000a70: 4b45 4e29 02da 0a61 6363 6573 735f 6b65  KEN)...access_ke
+00000a80: 79da 0c61 6363 6573 735f 746f 6b65 6e29  y..access_token)
+00000a90: 0672 2000 0000 7221 0000 00da 0f6f 7267  .r ...r!.....org
+00000aa0: 616e 697a 6174 696f 6e5f 6964 da0a 7072  anization_id..pr
+00000ab0: 6f6a 6563 745f 6964 721f 0000 00da 0365  oject_idr......e
+00000ac0: 6e76 2901 da08 6661 6c6c 6261 636b 7224  nv)...fallbackr$
+00000ad0: 0000 005a 034e 696c da07 7665 7262 6f73  ...Z.Nil..verbos
+00000ae0: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
+00000af0: 0000 0300 0000 7300 0000 7318 0000 0081  ......s...s.....
+00000b00: 007c 005d 077d 017c 0164 0075 0056 0001  .|.].}.|.d.u.V..
+00000b10: 0071 0264 0053 0029 014e 720c 0000 0029  .q.d.S.).Nr....)
+00000b20: 0272 0e00 0000 720d 0000 0072 0c00 0000  .r....r....r....
+00000b30: 720c 0000 0072 1000 0000 da09 3c67 656e  r....r......<gen
+00000b40: 6578 7072 3e52 0000 0073 0400 0000 0280  expr>R...s......
+00000b50: 1600 7a2f 6c6f 6164 5f63 6f6e 6669 672e  ..z/load_config.
+00000b60: 3c6c 6f63 616c 733e 2e77 7261 7070 6572  <locals>.wrapper
+00000b70: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000b80: 7072 3e7a 5141 6c6c 2072 6571 7569 7265  pr>zQAll require
+00000b90: 6420 6f70 7469 6f6e 7320 6172 6520 6e6f  d options are no
+00000ba0: 7420 7365 742e 2050 6c65 6173 6520 7573  t set. Please us
+00000bb0: 6520 7468 6520 2263 6f6e 6669 6775 7265  e the "configure
+00000bc0: 2220 636f 6d6d 616e 6420 746f 2073 6574  " command to set
+00000bd0: 2074 6865 6d2e e901 0000 00da 0643 6f6e   them........Con
+00000be0: 6669 677a 1573 7465 6c6c 616e 6f77 5f63  figz.stellanow_c
+00000bf0: 6c69 2e63 6f6e 6669 672e 7220 0000 0072  li.config.r ...r
+00000c00: 2100 0000 7222 0000 0072 2300 0000 da0a  !...r"...r#.....
+00000c10: 7374 656c 6c61 5f61 7069 2914 7217 0000  stella_api).r...
+00000c20: 00da 1367 6574 5f63 7572 7265 6e74 5f63  ...get_current_c
+00000c30: 6f6e 7465 7874 da03 6765 74da 026f 73da  ontext..get..os.
+00000c40: 0667 6574 656e 76da 036f 626a 7206 0000  .getenv..objr...
+00000c50: 00da 0361 6e79 da06 7661 6c75 6573 da06  ...any..values..
+00000c60: 6c6f 6767 6572 da05 6572 726f 72da 0465  logger..error..e
+00000c70: 7869 7472 0700 0000 da07 6765 7461 7474  xitr......getatt
+00000c80: 72da 0969 6d70 6f72 746c 6962 da0d 696d  r..importlib..im
+00000c90: 706f 7274 5f6d 6f64 756c 65da 0b49 6d70  port_module..Imp
+00000ca0: 6f72 7445 7272 6f72 7204 0000 0072 0300  ortErrorr....r..
+00000cb0: 0000 da06 696e 766f 6b65 2908 da04 6172  ....invoke)...ar
+00000cc0: 6773 da06 6b77 6172 6773 da03 6374 7872  gs..kwargs..ctxr
+00000cd0: 1f00 0000 5a08 656e 765f 7661 7273 da03  ....Z.env_vars..
+00000ce0: 6b65 795a 1565 6e76 5f63 6f6e 6669 675f  keyZ.env_config_
+00000cf0: 636c 6173 735f 6e61 6d65 5a10 656e 765f  class_nameZ.env_
+00000d00: 636f 6e66 6967 5f63 6c61 7373 a901 721b  config_class..r.
+00000d10: 0000 0072 0c00 0000 7210 0000 00da 0777  ...r....r......w
+00000d20: 7261 7070 6572 3900 0000 7342 0000 0008  rapper9...sB....
+00000d30: 020c 0208 0308 0106 fe08 0514 020e 0114  ................
+00000d40: 0216 0102 800c 0208 010e 0216 030a 010a  ................
+00000d50: 0114 0202 0116 0102 0108 ff0c 0208 0102  ................
+00000d60: ff02 0404 0108 0108 0108 0108 0108 fb18  ................
+00000d70: 087a 1c6c 6f61 645f 636f 6e66 6967 2e3c  .z.load_config.<
+00000d80: 6c6f 6361 6c73 3e2e 7772 6170 7065 7229  locals>.wrapper)
+00000d90: 02da 0966 756e 6374 6f6f 6c73 da05 7772  ...functools..wr
+00000da0: 6170 7329 0272 1b00 0000 723f 0000 0072  aps).r....r?...r
+00000db0: 0c00 0000 723e 0000 0072 1000 0000 da0b  ....r>...r......
+00000dc0: 6c6f 6164 5f63 6f6e 6669 6738 0000 0073  load_config8...s
+00000dd0: 0600 0000 0801 0e01 042e 7242 0000 0029  ..........rB...)
+00000de0: 15da 075f 5f64 6f63 5f5f 7236 0000 0072  ...__doc__r6...r
+00000df0: 1700 0000 7240 0000 00da 076c 6f67 6769  ....r@.....loggi
+00000e00: 6e67 722d 0000 00da 0361 7069 7203 0000  ngr-.....apir...
+00000e10: 005a 0a63 6f6e 6669 672e 696e 7472 0400  .Z.config.intr..
+00000e20: 0000 da06 636f 6e66 6967 7205 0000 005a  ....configr....Z
+00000e30: 0c75 7469 6c73 2e6c 6f67 6765 7272 0600  .utils.loggerr..
+00000e40: 0000 da05 7574 696c 7372 0700 0000 da09  ....utilsr......
+00000e50: 6765 744c 6f67 6765 72da 085f 5f6e 616d  getLogger..__nam
+00000e60: 655f 5f72 3200 0000 721e 0000 0072 4200  e__r2...r....rB.
+00000e70: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000e80: 0072 1000 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000e90: 0100 0000 731c 0000 0004 0008 0908 0108  ....s...........
+00000ea0: 0108 0108 010c 020c 010c 010c 010c 010a  ................
+00000eb0: 0308 030c 1e                             .....
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/__pycache__/logger.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:52:13 2023 UTC, .py size: 879 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-00000000: 6f0d 0d0a 0000 0000 fd79 8b64 6f03 0000  o........y.do...
+00000000: 6f0d 0d0a 0000 0000 327a 8b64 fd01 0000  o.......2z.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
-00000030: 5a00 6401 6402 6c01 5a01 6501 a002 6403  Z.d.d.l.Z.e...d.
-00000040: a101 5a03 6404 6504 6602 6405 6406 8404  ..Z.d.e.f.d.d...
-00000050: 5a05 6402 5300 2907 613c 0100 000a 436f  Z.d.S.).a<....Co
-00000060: 7079 7269 6768 7420 2843 2920 3230 3232  pyright (C) 2022
-00000070: 2d32 3032 3320 5374 656c 6c61 2054 6563  -2023 Stella Tec
-00000080: 686e 6f6c 6f67 6965 7320 2855 4b29 204c  hnologies (UK) L
-00000090: 696d 6974 6564 2e0a 0a54 6869 7320 736f  imited...This so
-000000a0: 6674 7761 7265 2069 7320 7468 6520 7072  ftware is the pr
-000000b0: 6f70 7269 6574 6172 7920 696e 666f 726d  oprietary inform
-000000c0: 6174 696f 6e20 6f66 2053 7465 6c6c 6120  ation of Stella 
-000000d0: 5465 6368 6e6f 6c6f 6769 6573 2028 554b  Technologies (UK
-000000e0: 2920 4c69 6d69 7465 642e 0a55 7365 2c20  ) Limited..Use, 
-000000f0: 7265 7072 6f64 7563 7469 6f6e 2c20 6f72  reproduction, or
-00000100: 2072 6564 6973 7472 6962 7574 696f 6e20   redistribution 
-00000110: 6f66 2074 6869 7320 736f 6674 7761 7265  of this software
-00000120: 2069 7320 7374 7269 6374 6c79 2070 726f   is strictly pro
-00000130: 6869 6269 7465 6420 7769 7468 6f75 740a  hibited without.
-00000140: 7468 6520 6578 7072 6573 7320 7772 6974  the express writ
-00000150: 7465 6e20 7065 726d 6973 7369 6f6e 206f  ten permission o
-00000160: 6620 5374 656c 6c61 2054 6563 686e 6f6c  f Stella Technol
-00000170: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
-00000180: 6564 2e0a 416c 6c20 7269 6768 7473 2072  ed..All rights r
-00000190: 6573 6572 7665 642e 0ae9 0000 0000 4e5a  eserved.......NZ
-000001a0: 0d73 7465 6c6c 616e 6f77 5f63 6c69 da07  .stellanow_cli..
-000001b0: 7665 7262 6f73 6563 0100 0000 0000 0000  verbosec........
-000001c0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
-000001d0: 7354 0000 007c 0072 0974 00a0 0174 026a  sT...|.r.t...t.j
-000001e0: 03a1 0101 006e 0674 00a0 0174 026a 04a1  .....n.t...t.j..
-000001f0: 0101 0074 02a0 05a1 007d 017c 01a0 0174  ...t.....}.|...t
-00000200: 026a 06a1 0101 0074 02a0 0764 01a1 017d  .j.....t...d...}
-00000210: 027c 01a0 087c 02a1 0101 0074 00a0 097c  .|...|.....t...|
-00000220: 01a1 0101 0064 0053 0029 024e 7a1b 2528  .....d.S.).Nz.%(
-00000230: 6c65 7665 6c6e 616d 6529 7320 2d20 2528  levelname)s - %(
-00000240: 6d65 7373 6167 6529 7329 0ada 066c 6f67  message)s)...log
-00000250: 6765 725a 0873 6574 4c65 7665 6cda 076c  gerZ.setLevel..l
-00000260: 6f67 6769 6e67 da04 494e 464f 5a07 5741  ogging..INFOZ.WA
-00000270: 524e 494e 475a 0d53 7472 6561 6d48 616e  RNINGZ.StreamHan
-00000280: 646c 6572 da05 4445 4255 47da 0946 6f72  dler..DEBUG..For
-00000290: 6d61 7474 6572 5a0c 7365 7446 6f72 6d61  matterZ.setForma
-000002a0: 7474 6572 5a0a 6164 6448 616e 646c 6572  tterZ.addHandler
-000002b0: 2903 7202 0000 00da 0263 68da 0966 6f72  ).r......ch..for
-000002c0: 6d61 7474 6572 a900 720a 0000 00fa 542f  matter..r.....T/
-000002d0: 5573 6572 732f 746f 6d2d 6b61 6e64 7a69  Users/tom-kandzi
-000002e0: 6f72 612f 4465 764c 6f63 616c 2f73 7465  ora/DevLocal/ste
-000002f0: 6c6c 612f 7374 656c 6c61 2d6e 6f77 2f53  lla/stella-now/S
-00000300: 7465 6c6c 614e 6f77 434c 492f 7374 656c  tellaNowCLI/stel
-00000310: 6c61 6e6f 775f 636c 692f 6c6f 6767 6572  lanow_cli/logger
-00000320: 2e70 79da 0c73 6574 7570 5f6c 6f67 6765  .py..setup_logge
-00000330: 7210 0000 0073 1000 0000 0401 0e01 0c02  r....s..........
-00000340: 0803 0c01 0a03 0a01 0e03 720c 0000 0029  ..........r....)
-00000350: 06da 075f 5f64 6f63 5f5f 7204 0000 005a  ...__doc__r....Z
-00000360: 0967 6574 4c6f 6767 6572 7203 0000 00da  .getLoggerr.....
-00000370: 0462 6f6f 6c72 0c00 0000 720a 0000 0072  .boolr....r....r
-00000380: 0a00 0000 720a 0000 0072 0b00 0000 da08  ....r....r......
-00000390: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-000003a0: 0004 0008 090a 0312 03                   .........
+00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
+00000040: 6404 6c03 6d04 5a04 0100 4700 6405 6406  d.l.m.Z...G.d.d.
+00000050: 8400 6406 6502 8303 5a05 6407 5300 2908  ..d.e...Z.d.S.).
+00000060: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
+00000070: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
+00000080: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
+00000090: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
+000000a0: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
+000000b0: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
+000000c0: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
+000000d0: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
+000000e0: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
+000000f0: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
+00000100: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
+00000110: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
+00000120: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
+00000130: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
+00000140: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
+00000150: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
+00000160: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
+00000170: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
+00000180: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
+00000190: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
+000001a0: 0ae9 0000 0000 2901 da04 456e 756d e901  ......)...Enum..
+000001b0: 0000 0029 01da 0643 6f6e 6669 6763 0000  ...)...Configc..
+000001c0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+000001d0: 0000 4000 0000 7320 0000 0065 005a 0164  ..@...s ...e.Z.d
+000001e0: 005a 0264 015a 0364 025a 0465 0564 0364  .Z.d.Z.d.Z.e.d.d
+000001f0: 0484 0083 015a 0664 0553 0029 06da 0345  .....Z.d.S.)...E
+00000200: 6e76 da03 696e 74da 0364 6576 6301 0000  nv..int..devc...
+00000210: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000220: 0043 0000 0073 0a00 0000 7c00 7400 6a01  .C...s....|.t.j.
+00000230: 7600 5300 2901 4e29 0272 0500 0000 da0b  v.S.).N).r......
+00000240: 5f5f 6d65 6d62 6572 735f 5f29 01da 0576  __members__)...v
+00000250: 616c 7565 a900 720a 0000 00fa 5d2f 5573  alue..r.....]/Us
+00000260: 6572 732f 746f 6d2d 6b61 6e64 7a69 6f72  ers/tom-kandzior
+00000270: 612f 4465 764c 6f63 616c 2f73 7465 6c6c  a/DevLocal/stell
+00000280: 612f 7374 656c 6c61 2d6e 6f77 2f53 7465  a/stella-now/Ste
+00000290: 6c6c 614e 6f77 434c 492f 7374 656c 6c61  llaNowCLI/stella
+000002a0: 6e6f 775f 636c 692f 636f 6e66 6967 2f5f  now_cli/config/_
+000002b0: 5f69 6e69 745f 5f2e 7079 da08 6973 5f76  _init__.py..is_v
+000002c0: 616c 6964 1300 0000 7302 0000 000a 027a  alid....s......z
+000002d0: 0c45 6e76 2e69 735f 7661 6c69 644e 2907  .Env.is_validN).
+000002e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000002f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000300: 6d65 5f5f da03 494e 545a 0344 4556 da0c  me__..INTZ.DEV..
+00000310: 7374 6174 6963 6d65 7468 6f64 720c 0000  staticmethodr...
+00000320: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
+00000330: 720b 0000 0072 0500 0000 0f00 0000 730a  r....r........s.
+00000340: 0000 0008 0004 0104 0102 020e 0172 0500  .............r..
+00000350: 0000 4e29 06da 075f 5f64 6f63 5f5f da04  ..N)...__doc__..
+00000360: 656e 756d 7202 0000 00da 0663 6f6e 6669  enumr......confi
+00000370: 6772 0400 0000 7205 0000 0072 0a00 0000  gr....r....r....
+00000380: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
+00000390: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
+000003a0: 0000 0400 0c09 0c02 1403                 ..........
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:54:39 2023 UTC, .py size: 422 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-00000000: 6f0d 0d0a 0000 0000 8f7a 8b64 a601 0000  o........z.d....
+00000000: 6f0d 0d0a 0000 0000 7c6f 9064 be01 0000  o.......|o.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6403  m.Z.m.Z.m.Z...d.
-00000050: 5300 2904 613c 0100 000a 436f 7079 7269  S.).a<....Copyri
-00000060: 6768 7420 2843 2920 3230 3232 2d32 3032  ght (C) 2022-202
-00000070: 3320 5374 656c 6c61 2054 6563 686e 6f6c  3 Stella Technol
-00000080: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
-00000090: 6564 2e0a 0a54 6869 7320 736f 6674 7761  ed...This softwa
-000000a0: 7265 2069 7320 7468 6520 7072 6f70 7269  re is the propri
-000000b0: 6574 6172 7920 696e 666f 726d 6174 696f  etary informatio
-000000c0: 6e20 6f66 2053 7465 6c6c 6120 5465 6368  n of Stella Tech
-000000d0: 6e6f 6c6f 6769 6573 2028 554b 2920 4c69  nologies (UK) Li
-000000e0: 6d69 7465 642e 0a55 7365 2c20 7265 7072  mited..Use, repr
-000000f0: 6f64 7563 7469 6f6e 2c20 6f72 2072 6564  oduction, or red
-00000100: 6973 7472 6962 7574 696f 6e20 6f66 2074  istribution of t
-00000110: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
-00000120: 7374 7269 6374 6c79 2070 726f 6869 6269  strictly prohibi
-00000130: 7465 6420 7769 7468 6f75 740a 7468 6520  ted without.the 
-00000140: 6578 7072 6573 7320 7772 6974 7465 6e20  express written 
-00000150: 7065 726d 6973 7369 6f6e 206f 6620 5374  permission of St
-00000160: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-00000170: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-00000180: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
-00000190: 7665 642e 0ae9 0100 0000 2905 da09 5374  ved.......)...St
-000001a0: 656c 6c61 4150 49da 0b53 7465 6c6c 6145  ellaAPI..StellaE
-000001b0: 7665 6e74 da0b 5374 656c 6c61 4669 656c  vent..StellaFiel
-000001c0: 64da 0c53 7465 6c6c 6145 6e74 6974 79da  d..StellaEntity.
-000001d0: 1353 7465 6c6c 6145 7665 6e74 4465 7461  .StellaEventDeta
-000001e0: 696c 6564 4e29 07da 075f 5f64 6f63 5f5f  iledN)...__doc__
-000001f0: 5a0d 7374 656c 6c61 6e6f 775f 6170 6972  Z.stellanow_apir
-00000200: 0200 0000 7203 0000 0072 0400 0000 7205  ....r....r....r.
-00000210: 0000 0072 0600 0000 a900 7208 0000 0072  ...r......r....r
-00000220: 0800 0000 fa5a 2f55 7365 7273 2f74 6f6d  .....Z/Users/tom
-00000230: 2d6b 616e 647a 696f 7261 2f44 6576 4c6f  -kandziora/DevLo
-00000240: 6361 6c2f 7374 656c 6c61 2f73 7465 6c6c  cal/stella/stell
-00000250: 612d 6e6f 772f 5374 656c 6c61 4e6f 7743  a-now/StellaNowC
-00000260: 4c49 2f73 7465 6c6c 616e 6f77 5f63 6c69  LI/stellanow_cli
-00000270: 2f61 7069 2f5f 5f69 6e69 745f 5f2e 7079  /api/__init__.py
-00000280: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000290: 0000 0004 0020 09                        ..... .
+00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
+00000050: 6d07 5a07 0100 6404 5300 2905 613c 0100  m.Z...d.S.).a<..
+00000060: 000a 436f 7079 7269 6768 7420 2843 2920  ..Copyright (C) 
+00000070: 3230 3232 2d32 3032 3320 5374 656c 6c61  2022-2023 Stella
+00000080: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
+00000090: 4b29 204c 696d 6974 6564 2e0a 0a54 6869  K) Limited...Thi
+000000a0: 7320 736f 6674 7761 7265 2069 7320 7468  s software is th
+000000b0: 6520 7072 6f70 7269 6574 6172 7920 696e  e proprietary in
+000000c0: 666f 726d 6174 696f 6e20 6f66 2053 7465  formation of Ste
+000000d0: 6c6c 6120 5465 6368 6e6f 6c6f 6769 6573  lla Technologies
+000000e0: 2028 554b 2920 4c69 6d69 7465 642e 0a55   (UK) Limited..U
+000000f0: 7365 2c20 7265 7072 6f64 7563 7469 6f6e  se, reproduction
+00000100: 2c20 6f72 2072 6564 6973 7472 6962 7574  , or redistribut
+00000110: 696f 6e20 6f66 2074 6869 7320 736f 6674  ion of this soft
+00000120: 7761 7265 2069 7320 7374 7269 6374 6c79  ware is strictly
+00000130: 2070 726f 6869 6269 7465 6420 7769 7468   prohibited with
+00000140: 6f75 740a 7468 6520 6578 7072 6573 7320  out.the express 
+00000150: 7772 6974 7465 6e20 7065 726d 6973 7369  written permissi
+00000160: 6f6e 206f 6620 5374 656c 6c61 2054 6563  on of Stella Tec
+00000170: 686e 6f6c 6f67 6965 7320 2855 4b29 204c  hnologies (UK) L
+00000180: 696d 6974 6564 2e0a 416c 6c20 7269 6768  imited..All righ
+00000190: 7473 2072 6573 6572 7665 642e 0ae9 0100  ts reserved.....
+000001a0: 0000 2901 da09 5374 656c 6c61 4150 4929  ..)...StellaAPI)
+000001b0: 04da 0b53 7465 6c6c 6145 7665 6e74 da0c  ...StellaEvent..
+000001c0: 5374 656c 6c61 456e 7469 7479 da0b 5374  StellaEntity..St
+000001d0: 656c 6c61 4669 656c 64da 1353 7465 6c6c  ellaField..Stell
+000001e0: 6145 7665 6e74 4465 7461 696c 6564 4e29  aEventDetailedN)
+000001f0: 08da 075f 5f64 6f63 5f5f 5a0d 7374 656c  ...__doc__Z.stel
+00000200: 6c61 6e6f 775f 6170 6972 0200 0000 5a09  lanow_apir....Z.
+00000210: 6461 7461 7479 7065 7372 0300 0000 7204  datatypesr....r.
+00000220: 0000 0072 0500 0000 7206 0000 00a9 0072  ...r....r......r
+00000230: 0800 0000 7208 0000 00fa 5a2f 5573 6572  ....r.....Z/User
+00000240: 732f 746f 6d2d 6b61 6e64 7a69 6f72 612f  s/tom-kandziora/
+00000250: 4465 764c 6f63 616c 2f73 7465 6c6c 612f  DevLocal/stella/
+00000260: 7374 656c 6c61 2d6e 6f77 2f53 7465 6c6c  stella-now/Stell
+00000270: 614e 6f77 434c 492f 7374 656c 6c61 6e6f  aNowCLI/stellano
+00000280: 775f 636c 692f 6170 692f 5f5f 696e 6974  w_cli/api/__init
+00000290: 5f5f 2e70 79da 083c 6d6f 6475 6c65 3e01  __.py..<module>.
+000002a0: 0000 0073 0600 0000 0400 0c09 1c01       ...s..........
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:54:33 2023 UTC, .py size: 6483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,376 +1,340 @@
-00000000: 6f0d 0d0a 0000 0000 897a 8b64 5319 0000  o........z.dS...
+00000000: 6f0d 0d0a 0000 0000 5a78 9064 2118 0000  o.......Zx.d!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
-00000060: 6d08 5a08 6d09 5a09 0100 6406 6407 6c0a  m.Z.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6406 6408 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6504 4700 6409 640a 8400 640a 8302  ..e.G.d.d...d...
-00000090: 8301 5a0d 6504 4700 640b 640c 8400 640c  ..Z.e.G.d.d...d.
-000000a0: 8302 8301 5a0e 6504 4700 640d 640e 8400  ....Z.e.G.d.d...
-000000b0: 640e 8302 8301 5a0f 6504 4700 640f 6410  d.....Z.e.G.d.d.
-000000c0: 8400 6410 650f 8303 8301 5a10 4700 6411  ..d.e.....Z.G.d.
-000000d0: 6412 8400 6412 6511 8303 5a12 4700 6413  d...d.e...Z.G.d.
-000000e0: 6414 8400 6414 8302 5a13 6402 5300 2915  d...d...Z.d.S.).
-000000f0: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
-00000100: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
-00000110: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-00000120: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-00000130: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
-00000140: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
-00000150: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
-00000160: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
-00000170: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
-00000180: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
-00000190: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
-000001a0: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
-000001b0: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
-000001c0: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
-000001d0: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
-000001e0: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
-000001f0: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
-00000200: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
-00000210: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
-00000220: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-00000230: 0ae9 0000 0000 4e29 01da 0964 6174 6163  ......N)...datac
-00000240: 6c61 7373 2901 da07 6d61 7873 697a 6529  lass)...maxsize)
-00000250: 02da 0947 656e 6572 6174 6f72 da04 4c69  ...Generator..Li
-00000260: 7374 e902 0000 0029 01da 066c 6f67 6765  st.....)...logge
-00000270: 7229 01da 0643 6f6e 6669 6763 0000 0000  r)...Configc....
-00000280: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000290: 4000 0000 731e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000002a0: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-000002b0: 023c 0064 0353 0029 04da 0c53 7465 6c6c  .<.d.S.)...Stell
-000002c0: 6145 6e74 6974 79da 0269 64da 046e 616d  aEntity..id..nam
-000002d0: 654e a905 da08 5f5f 6e61 6d65 5f5f da0a  eN....__name__..
-000002e0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000002f0: 616c 6e61 6d65 5f5f da03 7374 72da 0f5f  alname__..str.._
-00000300: 5f61 6e6e 6f74 6174 696f 6e73 5f5f a900  _annotations__..
-00000310: 7212 0000 0072 1200 0000 fa5f 2f55 7365  r....r....._/Use
-00000320: 7273 2f74 6f6d 2d6b 616e 647a 696f 7261  rs/tom-kandziora
-00000330: 2f44 6576 4c6f 6361 6c2f 7374 656c 6c61  /DevLocal/stella
-00000340: 2f73 7465 6c6c 612d 6e6f 772f 5374 656c  /stella-now/Stel
-00000350: 6c61 4e6f 7743 4c49 2f73 7465 6c6c 616e  laNowCLI/stellan
-00000360: 6f77 5f63 6c69 2f61 7069 2f73 7465 6c6c  ow_cli/api/stell
-00000370: 616e 6f77 5f61 7069 2e70 7972 0900 0000  anow_api.pyr....
-00000380: 1500 0000 7306 0000 000a 0008 020c 0172  ....s..........r
-00000390: 0900 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000003a0: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
-000003b0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-000003c0: 6401 3c00 6503 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
-000003d0: 6403 3c00 6404 5300 2905 da0b 5374 656c  d.<.d.S.)...Stel
-000003e0: 6c61 4669 656c 6472 0a00 0000 720b 0000  laFieldr....r...
-000003f0: 005a 0976 616c 7565 5479 7065 4e72 0c00  .Z.valueTypeNr..
-00000400: 0000 7212 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00000410: 0072 1300 0000 7214 0000 001b 0000 0073  .r....r........s
-00000420: 0800 0000 0a00 0802 0801 0c01 7214 0000  ............r...
-00000430: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000440: 0000 0300 0000 4000 0000 7336 0000 0065  ......@...s6...e
-00000450: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
-00000460: 0065 0365 0464 023c 0065 0565 0464 033c  .e.e.d.<.e.e.d.<
-00000470: 0065 0365 0464 043c 0065 0365 0464 053c  .e.e.d.<.e.e.d.<
-00000480: 0064 0653 0029 07da 0b53 7465 6c6c 6145  .d.S.)...StellaE
-00000490: 7665 6e74 720a 0000 0072 0b00 0000 da08  ventr....r......
-000004a0: 6973 4163 7469 7665 da09 6372 6561 7465  isActive..create
-000004b0: 6441 74da 0975 7064 6174 6564 4174 4e29  dAt..updatedAtN)
-000004c0: 0672 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000004d0: 7210 0000 0072 1100 0000 da04 626f 6f6c  r....r......bool
-000004e0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000004f0: 1300 0000 7215 0000 0022 0000 0073 0c00  ....r...."...s..
-00000500: 0000 0a00 0802 0801 0801 0801 0c01 7215  ..............r.
-00000510: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000520: 0000 0000 0300 0000 4000 0000 732e 0000  ........@...s...
-00000530: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
-00000540: 013c 0065 0565 0619 0065 0464 023c 0065  .<.e.e...e.d.<.e
-00000550: 0565 0719 0065 0464 033c 0064 0453 0029  .e...e.d.<.d.S.)
-00000560: 05da 1353 7465 6c6c 6145 7665 6e74 4465  ...StellaEventDe
-00000570: 7461 696c 6564 da0b 6465 7363 7269 7074  tailed..descript
-00000580: 696f 6eda 0666 6965 6c64 73da 0865 6e74  ion..fields..ent
-00000590: 6974 6965 734e 2908 720d 0000 0072 0e00  itiesN).r....r..
-000005a0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-000005b0: 0072 0500 0000 7214 0000 0072 0900 0000  .r....r....r....
-000005c0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000005d0: 1300 0000 721a 0000 002b 0000 0073 0800  ....r....+...s..
-000005e0: 0000 0a00 0802 0c01 1001 721a 0000 0063  ..........r....c
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0300 0000 0000 0000 7328 0000 0065 005a  ........s(...e.Z
-00000610: 0164 005a 0264 015a 0387 0066 0164 0264  .d.Z.d.Z...f.d.d
-00000620: 0384 085a 0464 0464 0584 005a 0587 0004  ...Z.d.d...Z....
-00000630: 005a 0653 0029 06da 0e53 7465 6c6c 6141  .Z.S.)...StellaA
-00000640: 5049 4572 726f 727a 2e45 7863 6570 7469  PIErrorz.Excepti
-00000650: 6f6e 2072 6169 7365 6420 666f 7220 6572  on raised for er
-00000660: 726f 7273 2069 6e20 7468 6520 5374 656c  rors in the Stel
-00000670: 6c61 2041 5049 2e63 0300 0000 0000 0000  la API.c........
-00000680: 0000 0000 0300 0000 0300 0000 0300 0000  ................
-00000690: 731e 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
-000006a0: 0174 0283 00a0 037c 006a 00a1 0101 0064  .t.....|.j.....d
-000006b0: 0053 00a9 014e 2904 da07 6d65 7373 6167  .S...N)...messag
-000006c0: 65da 0665 7272 6f72 73da 0573 7570 6572  e..errors..super
-000006d0: da08 5f5f 696e 6974 5f5f 2903 da04 7365  ..__init__)...se
-000006e0: 6c66 7220 0000 0072 2100 0000 a901 da09  lfr ...r!.......
-000006f0: 5f5f 636c 6173 735f 5f72 1200 0000 7213  __class__r....r.
-00000700: 0000 0072 2300 0000 3500 0000 7306 0000  ...r#...5...s...
-00000710: 0006 0106 0112 017a 1753 7465 6c6c 6141  .......z.StellaA
-00000720: 5049 4572 726f 722e 5f5f 696e 6974 5f5f  PIError.__init__
-00000730: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000740: 0003 0000 0043 0000 0073 1200 0000 7c00  .....C...s....|.
-00000750: 6a00 9b00 6401 7c00 6a01 9b00 9d03 5300  j...d.|.j.....S.
-00000760: 2902 4efa 0120 2902 7220 0000 0072 2100  ).N.. ).r ...r!.
-00000770: 0000 2901 7224 0000 0072 1200 0000 7212  ..).r$...r....r.
-00000780: 0000 0072 1300 0000 da07 5f5f 7374 725f  ...r......__str_
-00000790: 5f3a 0000 0073 0200 0000 1201 7a16 5374  _:...s......z.St
-000007a0: 656c 6c61 4150 4945 7272 6f72 2e5f 5f73  ellaAPIError.__s
-000007b0: 7472 5f5f 2907 720d 0000 0072 0e00 0000  tr__).r....r....
-000007c0: 720f 0000 00da 075f 5f64 6f63 5f5f 7223  r......__doc__r#
-000007d0: 0000 0072 2800 0000 da0d 5f5f 636c 6173  ...r(.....__clas
-000007e0: 7363 656c 6c5f 5f72 1200 0000 7212 0000  scell__r....r...
-000007f0: 0072 2500 0000 7213 0000 0072 1e00 0000  .r%...r....r....
-00000800: 3200 0000 7308 0000 0008 0004 010c 0210  2...s...........
-00000810: 0572 1e00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000820: 0000 0000 0000 000a 0000 0040 0000 0073  ...........@...s
-00000830: 6c00 0000 6500 5a01 6400 5a02 6401 6503  l...e.Z.d.Z.d.e.
-00000840: 6402 6504 6403 6504 6404 6504 6405 6504  d.e.d.e.d.e.d.e.
-00000850: 660a 6406 6407 8404 5a05 6408 6409 8400  f.d.d...Z.d.d...
-00000860: 5a06 640a 640b 8400 5a07 640c 640d 8400  Z.d.d...Z.d.d...
-00000870: 5a08 640e 6509 650a 640f 640f 6603 1900  Z.d.e.e.d.d.f...
-00000880: 6602 6410 6411 8404 5a0b 6412 6504 640e  f.d.d...Z.d.e.d.
-00000890: 650c 6604 6413 6414 8404 5a0d 640f 5300  e.f.d.d...Z.d.S.
-000008a0: 2915 da09 5374 656c 6c61 4150 49da 0a65  )...StellaAPI..e
-000008b0: 6e76 5f63 6f6e 6669 67da 0a61 6363 6573  nv_config..acces
-000008c0: 735f 6b65 79da 0c61 6363 6573 735f 746f  s_key..access_to
-000008d0: 6b65 6eda 0f6f 7267 616e 697a 6174 696f  ken..organizatio
-000008e0: 6e5f 6964 da0a 7072 6f6a 6563 745f 6964  n_id..project_id
-000008f0: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
-00000900: 0002 0000 0043 0000 0073 3600 0000 7c01  .....C...s6...|.
-00000910: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
-00000920: 7c04 7c00 5f03 7c05 7c00 5f04 6400 7c00  |.|._.|.|._.d.|.
-00000930: 5f05 6400 7c00 5f06 7c00 a007 a100 0100  _.d.|._.|.......
-00000940: 6400 5300 721f 0000 0029 0872 2c00 0000  d.S.r....).r,...
-00000950: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00000960: 3000 0000 da0a 6175 7468 5f74 6f6b 656e  0.....auth_token
-00000970: da0d 7265 6672 6573 685f 746f 6b65 6eda  ..refresh_token.
-00000980: 0c61 7574 6865 6e74 6963 6174 6529 0672  .authenticate).r
-00000990: 2400 0000 722c 0000 0072 2d00 0000 722e  $...r,...r-...r.
-000009a0: 0000 0072 2f00 0000 7230 0000 0072 1200  ...r/...r0...r..
-000009b0: 0000 7212 0000 0072 1300 0000 7223 0000  ..r....r....r#..
-000009c0: 003f 0000 0073 1000 0000 0601 0602 0601  .?...s..........
-000009d0: 0601 0601 0601 0601 0c02 7a12 5374 656c  ..........z.Stel
-000009e0: 6c61 4150 492e 5f5f 696e 6974 5f5f 6302  laAPI.__init__c.
-000009f0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
-00000a00: 0000 0043 0000 0073 cc00 0000 7a09 7c01  ...C...s....z.|.
-00000a10: a000 a100 a001 6401 a101 7d02 5700 6e0c  ......d...}.W.n.
-00000a20: 0400 7400 6a02 7915 0100 0100 0100 6400  ..t.j.y.......d.
-00000a30: 7d02 5900 6e01 7700 7c01 6a03 0400 6402  }.Y.n.w.|.j...d.
-00000a40: 6b02 724d 0100 7404 7c02 7405 8302 7227  k.rM..t.|.t...r'
-00000a50: 7c02 a001 6403 a101 6e01 7c02 7d03 7c03  |...d...n.|.}.|.
-00000a60: 4400 5d1f 7d04 7c04 a001 6404 a101 0400  D.].}.|...d.....
-00000a70: 6405 6b02 723d 0100 7c00 a006 a100 0100  d.k.r=..|.......
-00000a80: 0100 6400 5300 6406 6b02 7245 7407 6407  ..d.S.d.k.rEt.d.
-00000a90: 7c02 8302 8201 0900 7407 6408 7c02 8302  |.......t.d.|...
-00000aa0: 8201 6400 5300 0400 6409 6b02 7257 0100  ..d.S...d.k.rW..
-00000ab0: 7407 640a 7c02 8302 8201 640b 6b02 725f  t.d.|.....d.k.r_
-00000ac0: 7407 640c 7c02 8302 8201 0900 7c01 a008  t.d.|.......|...
-00000ad0: a100 0100 6400 5300 290d 4eda 0764 6574  ....d.S.).N..det
-00000ae0: 6169 6c73 6991 0100 0072 2100 0000 5a09  ailsi....r!...Z.
-00000af0: 6572 726f 7243 6f64 655a 1169 6e61 6374  errorCodeZ.inact
-00000b00: 6976 6541 7574 6854 6f6b 656e 5a17 7772  iveAuthTokenZ.wr
-00000b10: 6f6e 6755 7365 726e 616d 654f 7250 6173  ongUsernameOrPas
-00000b20: 7377 6f72 647a 3755 6e61 7574 686f 7269  swordz7Unauthori
-00000b30: 7a65 643a 2050 726f 7669 6465 6420 7573  zed: Provided us
-00000b40: 6572 6e61 6d65 206f 7220 7061 7373 776f  ername or passwo
-00000b50: 7264 2069 7320 696e 7661 6c69 642e 5a0c  rd is invalid.Z.
-00000b60: 556e 6175 7468 6f72 697a 6564 6993 0100  Unauthorizedi...
-00000b70: 007a 4b46 6f72 6269 6464 656e 3a20 4163  .zKForbidden: Ac
-00000b80: 6365 7373 2074 6f20 7468 6520 4150 4920  cess to the API 
-00000b90: 6973 2072 6573 7472 6963 7465 6420 6f6e  is restricted on
-00000ba0: 6c79 2074 6f20 7768 6974 656c 6973 7465  ly to whiteliste
-00000bb0: 6420 636f 6e6e 6563 7469 6f6e 732e 6994  d connections.i.
-00000bc0: 0100 007a 094e 6f74 2046 6f75 6e64 2909  ...z.Not Found).
-00000bd0: da04 6a73 6f6e da03 6765 745a 0f4a 534f  ..json..getZ.JSO
-00000be0: 4e44 6563 6f64 6545 7272 6f72 5a0b 7374  NDecodeErrorZ.st
-00000bf0: 6174 7573 5f63 6f64 65da 0a69 7369 6e73  atus_code..isins
-00000c00: 7461 6e63 65da 0464 6963 74da 0c61 7574  tance..dict..aut
-00000c10: 685f 7265 6672 6573 6872 1e00 0000 5a10  h_refreshr....Z.
-00000c20: 7261 6973 655f 666f 725f 7374 6174 7573  raise_for_status
-00000c30: 2905 7224 0000 00da 0872 6573 706f 6e73  ).r$.....respons
-00000c40: 6572 3400 0000 7221 0000 00da 0565 7272  er4...r!.....err
-00000c50: 6f72 7212 0000 0072 1200 0000 7213 0000  orr....r....r...
-00000c60: 00da 105f 6861 6e64 6c65 5f72 6573 706f  ..._handle_respo
-00000c70: 6e73 654b 0000 0073 3600 0000 0201 1201  nseK...s6.......
-00000c80: 0e01 0801 02ff 0403 0a01 1802 0802 0801  ................
-00000c90: 0a01 0801 0601 0601 0a01 0201 0a01 04f8  ................
-00000ca0: 0a09 0201 0201 0201 04fe 0604 0a01 0201  ................
-00000cb0: 0c01 7a1a 5374 656c 6c61 4150 492e 5f68  ..z.StellaAPI._h
-00000cc0: 616e 646c 655f 7265 7370 6f6e 7365 6301  andle_responsec.
-00000cd0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-00000ce0: 0000 0043 0000 0073 9800 0000 7400 a001  ...C...s....t...
-00000cf0: 6401 a101 0100 7c00 6a02 6400 7501 720f  d.....|.j.d.u.r.
-00000d00: 7c00 a003 a100 0100 6e36 7c00 6a04 7c00  |.......n6|.j.|.
-00000d10: 6a05 7c00 6a05 7c00 6a06 6402 6403 9c05  j.|.j.|.j.d.d...
-00000d20: 7d01 6400 7c00 5f07 6400 7c00 5f02 7408  }.d.|._.d.|._.t.
-00000d30: 6a09 7c00 6a0a 6a0b 7c01 6404 8d02 7d02  j.|.j.j.|.d...}.
-00000d40: 7c00 a00c 7c02 a101 0100 7c02 a00d a100  |...|.....|.....
-00000d50: a00e 6405 a101 a00e 6406 a101 7c00 5f07  ..d.....d...|._.
-00000d60: 7c02 a00d a100 a00e 6405 a101 a00e 6407  |.......d.....d.
-00000d70: a101 7c00 5f02 7400 a001 6408 a101 0100  ..|._.t...d.....
-00000d80: 6400 5300 2909 4e7a 1e41 7574 6865 6e74  d.S.).Nz.Authent
-00000d90: 6963 6174 696e 6720 746f 2074 6865 2041  icating to the A
-00000da0: 5049 202e 2e2e 205a 0a62 6163 6b6f 6666  PI ... Z.backoff
-00000db0: 6963 6529 055a 0872 6561 6c6d 5f69 64da  ice).Z.realm_id.
-00000dc0: 0875 7365 726e 616d 65da 0565 6d61 696c  .username..email
-00000dd0: da08 7061 7373 776f 7264 5a09 636c 6965  ..passwordZ.clie
-00000de0: 6e74 5f69 64a9 0172 3500 0000 7234 0000  nt_id..r5...r4..
-00000df0: 0072 2e00 0000 7232 0000 007a 1941 7574  .r....r2...z.Aut
-00000e00: 6865 6e74 6963 6174 696f 6e20 5375 6363  hentication Succ
-00000e10: 6573 7366 756c 290f 7207 0000 00da 0469  essful).r......i
-00000e20: 6e66 6f72 3200 0000 7239 0000 0072 2f00  nfor2...r9...r/.
-00000e30: 0000 722d 0000 0072 2e00 0000 7231 0000  ..r-...r....r1..
-00000e40: 00da 0872 6571 7565 7374 73da 0470 6f73  ...requests..pos
-00000e50: 7472 2c00 0000 da08 6175 7468 5f75 726c  tr,.....auth_url
-00000e60: 723c 0000 0072 3500 0000 7236 0000 00a9  r<...r5...r6....
-00000e70: 0372 2400 0000 da04 626f 6479 723a 0000  .r$.....bodyr:..
-00000e80: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000e90: 7233 0000 0069 0000 0073 2000 0000 0a01  r3...i...s .....
-00000ea0: 0a02 0a01 0403 0401 0401 0401 0201 06fb  ................
-00000eb0: 0608 0601 1202 0a01 1602 1601 0e02 7a16  ..............z.
-00000ec0: 5374 656c 6c61 4150 492e 6175 7468 656e  StellaAPI.authen
-00000ed0: 7469 6361 7465 6301 0000 0000 0000 0000  ticatec.........
-00000ee0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000ef0: 8c00 0000 7c00 6a00 6400 7500 720b 7c00  ....|.j.d.u.r.|.
-00000f00: a001 a100 0100 6400 5300 7402 a003 6401  ......d.S.t...d.
-00000f10: a101 0100 6402 7c00 6a00 6901 7d01 6400  ....d.|.j.i.}.d.
-00000f20: 7c00 5f04 6400 7c00 5f00 7405 6a06 7c00  |._.d.|._.t.j.|.
-00000f30: 6a07 6a08 7c01 6403 8d02 7d02 7c00 a009  j.j.|.d...}.|...
-00000f40: 7c02 a101 0100 7c02 a00a a100 a00b 6404  |.....|.......d.
-00000f50: a101 a00b 6405 a101 7c00 5f04 7c02 a00a  ....d...|._.|...
-00000f60: a100 a00b 6404 a101 a00b 6402 a101 7c00  ....d.....d...|.
-00000f70: 5f00 7402 a003 6406 a101 0100 6400 5300  _.t...d.....d.S.
-00000f80: 2907 4e7a 1841 5049 2054 6f6b 656e 2052  ).Nz.API Token R
-00000f90: 6566 7265 7368 696e 6720 2e2e 2e72 3200  efreshing ...r2.
-00000fa0: 0000 7240 0000 0072 3400 0000 722e 0000  ..r@...r4...r...
-00000fb0: 007a 1c41 5049 2054 6f6b 656e 2052 6566  .z.API Token Ref
-00000fc0: 7265 7368 2053 7563 6365 7373 6675 6c29  resh Successful)
-00000fd0: 0c72 3200 0000 7233 0000 0072 0700 0000  .r2...r3...r....
-00000fe0: 7241 0000 0072 3100 0000 7242 0000 0072  rA...r1...rB...r
-00000ff0: 4300 0000 722c 0000 00da 1061 7574 685f  C...r,.....auth_
-00001000: 7265 6672 6573 685f 7572 6c72 3c00 0000  refresh_urlr<...
-00001010: 7235 0000 0072 3600 0000 7245 0000 0072  r5...r6...rE...r
-00001020: 1200 0000 7212 0000 0072 1300 0000 7239  ....r....r....r9
-00001030: 0000 0082 0000 0073 1600 0000 0a01 0c01  .......s........
-00001040: 0a02 0a02 0602 0601 1202 0a01 1602 1601  ................
-00001050: 0e02 7a16 5374 656c 6c61 4150 492e 6175  ..z.StellaAPI.au
-00001060: 7468 5f72 6566 7265 7368 da06 7265 7475  th_refresh..retu
-00001070: 726e 4e63 0100 0000 0000 0000 0000 0000  rnNc............
-00001080: 0800 0000 0900 0000 6300 0000 73e4 0000  ........c...s...
-00001090: 0081 0064 017d 0174 007d 027c 017c 026b  ...d.}.t.}.|.|.k
-000010a0: 0072 707c 006a 016a 026a 037c 006a 0464  .rp|.j.j.j.|.j.d
-000010b0: 028d 0164 037c 019b 0064 049d 0317 007d  ...d.|...d.....}
-000010c0: 0364 0564 067c 006a 059b 009d 0269 017d  .d.d.|.j.....i.}
-000010d0: 0474 066a 077c 037c 0464 078d 027d 057c  .t.j.|.|.d...}.|
-000010e0: 00a0 087c 05a1 0101 007c 05a0 09a1 00a0  ...|.....|......
-000010f0: 0764 0869 00a1 02a0 0764 0967 00a1 027d  .d.i.....d.g...}
-00001100: 067c 05a0 09a1 00a0 0764 0869 00a1 02a0  .|.......d.i....
-00001110: 0764 0a64 0ba1 027d 027c 0673 4864 0053  .d.d...}.|.sHd.S
-00001120: 007c 0644 005d 1b7d 0774 0a7c 07a0 0764  .|.D.].}.t.|...d
-00001130: 0ca1 017c 07a0 0764 0da1 017c 07a0 0764  ...|...d...|...d
-00001140: 0ea1 017c 07a0 0764 0fa1 017c 07a0 0764  ...|...d...|...d
-00001150: 10a1 0164 118d 0556 0001 0071 4a7c 0164  ...d...V...qJ|.d
-00001160: 0137 007d 017c 017c 026b 0073 0964 0053  .7.}.|.|.k.s.d.S
-00001170: 0064 0053 0029 124e e901 0000 0029 01da  .d.S.).N.....)..
-00001180: 0970 726f 6a65 6374 4964 7a0c 3f70 6167  .projectIdz.?pag
-00001190: 654e 756d 6265 723d 7a0e 2670 6167 6553  eNumber=z.&pageS
-000011a0: 697a 653d 3130 3030 da0d 4175 7468 6f72  ize=1000..Author
-000011b0: 697a 6174 696f 6efa 0742 6561 7265 7220  ization..Bearer 
-000011c0: a901 da07 6865 6164 6572 7372 3400 0000  ....headersr4...
-000011d0: da07 7265 7375 6c74 735a 0d6e 756d 6265  ..resultsZ.numbe
-000011e0: 724f 6650 6167 6573 7201 0000 0072 0a00  rOfPagesr....r..
-000011f0: 0000 720b 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001200: 0072 1800 0000 2905 720a 0000 0072 0b00  .r....).r....r..
-00001210: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001220: 0029 0b72 0300 0000 722c 0000 00da 0a65  .).r....r,.....e
-00001230: 7665 6e74 735f 7572 6cda 0666 6f72 6d61  vents_url..forma
-00001240: 7472 3000 0000 7231 0000 0072 4200 0000  tr0...r1...rB...
-00001250: 7236 0000 0072 3c00 0000 7235 0000 0072  r6...r<...r5...r
-00001260: 1500 0000 2908 7224 0000 005a 0b70 6167  ....).r$...Z.pag
-00001270: 655f 6e75 6d62 6572 5a0f 6e75 6d62 6572  e_numberZ.number
-00001280: 5f6f 665f 7061 6765 73da 0375 726c 724e  _of_pages..urlrN
-00001290: 0000 0072 3a00 0000 da06 6576 656e 7473  ...r:.....events
-000012a0: da05 6576 656e 7472 1200 0000 7212 0000  ..eventr....r...
-000012b0: 0072 1300 0000 da0a 6765 745f 6576 656e  .r......get_even
-000012c0: 7473 9500 0000 732c 0000 0002 8004 0104  ts....s,........
-000012d0: 0108 011e 0110 010e 020a 0118 0218 0104  ................
-000012e0: 0104 0108 0202 0108 0108 0108 0108 0108  ................
-000012f0: 010a fb08 0810 eb7a 1453 7465 6c6c 6141  .......z.StellaA
-00001300: 5049 2e67 6574 5f65 7665 6e74 73da 0865  PI.get_events..e
-00001310: 7665 6e74 5f69 6463 0200 0000 0000 0000  vent_idc........
-00001320: 0000 0000 0800 0000 0a00 0000 4300 0000  ............C...
-00001330: 73b4 0000 007c 006a 006a 016a 027c 006a  s....|.j.j.j.|.j
-00001340: 037c 0164 018d 027d 0264 0264 037c 006a  .|.d...}.d.d.|.j
-00001350: 049b 009d 0269 017d 0374 056a 067c 027c  .....i.}.t.j.|.|
-00001360: 0364 048d 027d 047c 00a0 077c 04a1 0101  .d...}.|...|....
-00001370: 007c 04a0 08a1 00a0 0664 0569 00a1 027d  .|.......d.i...}
-00001380: 0564 0664 0784 007c 05a0 0664 0867 00a1  .d.d...|...d.g..
-00001390: 0244 0083 017d 0664 0964 0784 007c 05a0  .D...}.d.d...|..
-000013a0: 0664 0a67 00a1 0244 0083 017d 0774 097c  .d.g...D...}.t.|
-000013b0: 05a0 0664 0ba1 017c 05a0 0664 0ca1 017c  ...d...|...d...|
-000013c0: 05a0 0664 0da1 017c 05a0 0664 0ea1 017c  ...d...|...d...|
-000013d0: 05a0 0664 0fa1 017c 05a0 0664 10a1 017c  ...d...|...d...|
-000013e0: 077c 0664 118d 0853 0029 124e 2902 724a  .|.d...S.).N).rJ
-000013f0: 0000 005a 0765 7665 6e74 4964 724b 0000  ...Z.eventIdrK..
-00001400: 0072 4c00 0000 724d 0000 0072 3400 0000  .rL...rM...r4...
-00001410: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001420: 0006 0000 0053 0000 00f3 1a00 0000 6700  .....S........g.
-00001430: 7c00 5d09 7d01 7400 6400 6900 7c01 a401  |.].}.t.d.i.|...
-00001440: 8e01 9102 7102 5300 a901 7212 0000 0029  ....q.S...r....)
-00001450: 0172 0900 0000 2902 da02 2e30 5a06 656e  .r....)....0Z.en
-00001460: 7469 7479 7212 0000 0072 1200 0000 7213  tityr....r....r.
-00001470: 0000 00da 0a3c 6c69 7374 636f 6d70 3eb9  .....<listcomp>.
-00001480: 0000 00f3 0200 0000 1a00 7a2f 5374 656c  ..........z/Stel
-00001490: 6c61 4150 492e 6765 745f 6576 656e 745f  laAPI.get_event_
-000014a0: 6465 7461 696c 732e 3c6c 6f63 616c 733e  details.<locals>
-000014b0: 2e3c 6c69 7374 636f 6d70 3e72 1d00 0000  .<listcomp>r....
-000014c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000014d0: 0006 0000 0053 0000 0072 5700 0000 7258  .....S...rW...rX
-000014e0: 0000 0029 0172 1400 0000 2902 7259 0000  ...).r....).rY..
-000014f0: 00da 0566 6965 6c64 7212 0000 0072 1200  ...fieldr....r..
-00001500: 0000 7213 0000 0072 5a00 0000 bc00 0000  ..r....rZ.......
-00001510: 725b 0000 0072 1c00 0000 720a 0000 0072  r[...r....r....r
-00001520: 0b00 0000 721b 0000 0072 1600 0000 7217  ....r....r....r.
-00001530: 0000 0072 1800 0000 2908 720a 0000 0072  ...r....).r....r
-00001540: 0b00 0000 721b 0000 0072 1600 0000 7217  ....r....r....r.
-00001550: 0000 0072 1800 0000 721c 0000 0072 1d00  ...r....r....r..
-00001560: 0000 290a 722c 0000 00da 0965 7665 6e74  ..).r,.....event
-00001570: 5f75 726c 7251 0000 0072 3000 0000 7231  _urlrQ...r0...r1
-00001580: 0000 0072 4200 0000 7236 0000 0072 3c00  ...rB...r6...r<.
-00001590: 0000 7235 0000 0072 1a00 0000 2908 7224  ..r5...r....).r$
-000015a0: 0000 0072 5600 0000 7252 0000 0072 4e00  ...rV...rR...rN.
-000015b0: 0000 723a 0000 0072 3400 0000 721d 0000  ..r:...r4...r...
-000015c0: 0072 1c00 0000 7212 0000 0072 1200 0000  .r....r....r....
-000015d0: 7213 0000 00da 1167 6574 5f65 7665 6e74  r......get_event
-000015e0: 5f64 6574 6169 6c73 af00 0000 7322 0000  _details....s"..
-000015f0: 0014 0110 010e 020a 0110 0216 0316 0302  ................
-00001600: 0308 0108 0108 0108 0108 0108 0102 0102  ................
-00001610: 0106 f87a 1b53 7465 6c6c 6141 5049 2e67  ...z.StellaAPI.g
-00001620: 6574 5f65 7665 6e74 5f64 6574 6169 6c73  et_event_details
-00001630: 290e 720d 0000 0072 0e00 0000 720f 0000  ).r....r....r...
-00001640: 0072 0800 0000 7210 0000 0072 2300 0000  .r....r....r#...
-00001650: 723c 0000 0072 3300 0000 7239 0000 0072  r<...r3...r9...r
-00001660: 0400 0000 7215 0000 0072 5500 0000 721a  ....r....rU...r.
-00001670: 0000 0072 5e00 0000 7212 0000 0072 1200  ...r^...r....r..
-00001680: 0000 7212 0000 0072 1300 0000 722b 0000  ..r....r....r+..
-00001690: 003e 0000 0073 0e00 0000 0800 1e01 080c  .>...s..........
-000016a0: 081e 0819 1813 161a 722b 0000 0029 1472  ........r+...).r
-000016b0: 2900 0000 7235 0000 0072 4200 0000 da0b  )...r5...rB.....
-000016c0: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
-000016d0: da03 7379 7372 0300 0000 da06 7479 7069  ..sysr......typi
-000016e0: 6e67 7204 0000 0072 0500 0000 7207 0000  ngr....r....r...
-000016f0: 00da 0663 6f6e 6669 6772 0800 0000 7209  ...configr....r.
-00001700: 0000 0072 1400 0000 7215 0000 0072 1a00  ...r....r....r..
-00001710: 0000 da09 4578 6365 7074 696f 6e72 1e00  ....Exceptionr..
-00001720: 0000 722b 0000 0072 1200 0000 7212 0000  ..r+...r....r...
-00001730: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
-00001740: 6475 6c65 3e01 0000 0073 2400 0000 0400  dule>....s$.....
-00001750: 0809 0801 0c02 0c01 1001 0c02 0c01 0203  ................
-00001760: 1001 0205 1001 0206 1001 0208 1201 1006  ................
-00001770: 120c                                     ..
+00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
+00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
+00000060: 6405 6c07 6d08 5a08 0100 6406 6407 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
+00000080: 0100 6503 a00e 650f a101 5a10 4700 6408  ..e...e...Z.G.d.
+00000090: 6409 8400 6409 6511 8303 5a12 4700 640a  d...d.e...Z.G.d.
+000000a0: 640b 8400 640b 8302 5a13 6402 5300 290c  d...d...Z.d.S.).
+000000b0: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
+000000c0: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
+000000d0: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
+000000e0: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
+000000f0: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
+00000100: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
+00000110: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
+00000120: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
+00000130: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
+00000140: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
+00000150: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
+00000160: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
+00000170: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
+00000180: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
+00000190: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
+000001a0: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
+000001b0: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
+000001c0: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
+000001d0: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
+000001e0: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
+000001f0: 0ae9 0000 0000 4e29 01da 0947 656e 6572  ......N)...Gener
+00000200: 6174 6f72 e902 0000 0029 01da 0643 6f6e  ator.....)...Con
+00000210: 6669 67e9 0100 0000 2904 da0c 5374 656c  fig.....)...Stel
+00000220: 6c61 456e 7469 7479 da0b 5374 656c 6c61  laEntity..Stella
+00000230: 4669 656c 64da 0b53 7465 6c6c 6145 7665  Field..StellaEve
+00000240: 6e74 da13 5374 656c 6c61 4576 656e 7444  nt..StellaEventD
+00000250: 6574 6169 6c65 6463 0000 0000 0000 0000  etailedc........
+00000260: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000270: 7328 0000 0065 005a 0164 005a 0264 015a  s(...e.Z.d.Z.d.Z
+00000280: 0387 0066 0164 0264 0384 085a 0464 0464  ...f.d.d...Z.d.d
+00000290: 0584 005a 0587 0004 005a 0653 0029 06da  ...Z.....Z.S.)..
+000002a0: 0e53 7465 6c6c 6141 5049 4572 726f 727a  .StellaAPIErrorz
+000002b0: 2e45 7863 6570 7469 6f6e 2072 6169 7365  .Exception raise
+000002c0: 6420 666f 7220 6572 726f 7273 2069 6e20  d for errors in 
+000002d0: 7468 6520 5374 656c 6c61 2041 5049 2e63  the Stella API.c
+000002e0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000002f0: 0300 0000 0300 0000 731e 0000 007c 017c  ........s....|.|
+00000300: 005f 007c 027c 005f 0174 0283 00a0 037c  ._.|.|._.t.....|
+00000310: 006a 00a1 0101 0064 0053 00a9 014e 2904  .j.....d.S...N).
+00000320: da07 6d65 7373 6167 65da 0665 7272 6f72  ..message..error
+00000330: 73da 0573 7570 6572 da08 5f5f 696e 6974  s..super..__init
+00000340: 5f5f 2903 da04 7365 6c66 720c 0000 0072  __)...selfr....r
+00000350: 0d00 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000360: 5fa9 00fa 5f2f 5573 6572 732f 746f 6d2d  _..._/Users/tom-
+00000370: 6b61 6e64 7a69 6f72 612f 4465 764c 6f63  kandziora/DevLoc
+00000380: 616c 2f73 7465 6c6c 612f 7374 656c 6c61  al/stella/stella
+00000390: 2d6e 6f77 2f53 7465 6c6c 614e 6f77 434c  -now/StellaNowCL
+000003a0: 492f 7374 656c 6c61 6e6f 775f 636c 692f  I/stellanow_cli/
+000003b0: 6170 692f 7374 656c 6c61 6e6f 775f 6170  api/stellanow_ap
+000003c0: 692e 7079 720f 0000 001b 0000 0073 0600  i.pyr........s..
+000003d0: 0000 0601 0601 1201 7a17 5374 656c 6c61  ........z.Stella
+000003e0: 4150 4945 7272 6f72 2e5f 5f69 6e69 745f  APIError.__init_
+000003f0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000400: 0000 0300 0000 4300 0000 7312 0000 007c  ......C...s....|
+00000410: 006a 009b 0064 017c 006a 019b 009d 0353  .j...d.|.j.....S
+00000420: 0029 024e fa01 2029 0272 0c00 0000 720d  .).N.. ).r....r.
+00000430: 0000 0029 0172 1000 0000 7213 0000 0072  ...).r....r....r
+00000440: 1300 0000 7214 0000 00da 075f 5f73 7472  ....r......__str
+00000450: 5f5f 2000 0000 7302 0000 0012 017a 1653  __ ...s......z.S
+00000460: 7465 6c6c 6141 5049 4572 726f 722e 5f5f  tellaAPIError.__
+00000470: 7374 725f 5f29 07da 085f 5f6e 616d 655f  str__)...__name_
+00000480: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000490: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+000004a0: 6f63 5f5f 720f 0000 0072 1600 0000 da0d  oc__r....r......
+000004b0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1300  __classcell__r..
+000004c0: 0000 7213 0000 0072 1100 0000 7214 0000  ..r....r....r...
+000004d0: 0072 0a00 0000 1800 0000 7308 0000 0008  .r........s.....
+000004e0: 0004 010c 0210 0572 0a00 0000 6300 0000  .......r....c...
+000004f0: 0000 0000 0000 0000 0000 0000 000a 0000  ................
+00000500: 0040 0000 0073 6c00 0000 6500 5a01 6400  .@...sl...e.Z.d.
+00000510: 5a02 6401 6503 6402 6504 6403 6504 6404  Z.d.e.d.e.d.e.d.
+00000520: 6504 6405 6504 660a 6406 6407 8404 5a05  e.d.e.f.d.d...Z.
+00000530: 6408 6409 8400 5a06 640a 640b 8400 5a07  d.d...Z.d.d...Z.
+00000540: 640c 640d 8400 5a08 640e 6509 650a 640f  d.d...Z.d.e.e.d.
+00000550: 640f 6603 1900 6602 6410 6411 8404 5a0b  d.f...f.d.d...Z.
+00000560: 6412 6504 640e 650c 6604 6413 6414 8404  d.e.d.e.f.d.d...
+00000570: 5a0d 640f 5300 2915 da09 5374 656c 6c61  Z.d.S.)...Stella
+00000580: 4150 49da 0a65 6e76 5f63 6f6e 6669 67da  API..env_config.
+00000590: 0a61 6363 6573 735f 6b65 79da 0c61 6363  .access_key..acc
+000005a0: 6573 735f 746f 6b65 6eda 0f6f 7267 616e  ess_token..organ
+000005b0: 697a 6174 696f 6e5f 6964 da0a 7072 6f6a  ization_id..proj
+000005c0: 6563 745f 6964 6306 0000 0000 0000 0000  ect_idc.........
+000005d0: 0000 0006 0000 0002 0000 0043 0000 0073  ...........C...s
+000005e0: 3600 0000 7c01 7c00 5f00 7c02 7c00 5f01  6...|.|._.|.|._.
+000005f0: 7c03 7c00 5f02 7c04 7c00 5f03 7c05 7c00  |.|._.|.|._.|.|.
+00000600: 5f04 6400 7c00 5f05 6400 7c00 5f06 7c00  _.d.|._.d.|._.|.
+00000610: a007 a100 0100 6400 5300 720b 0000 0029  ......d.S.r....)
+00000620: 0872 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00000630: 7220 0000 0072 2100 0000 da0a 6175 7468  r ...r!.....auth
+00000640: 5f74 6f6b 656e da0d 7265 6672 6573 685f  _token..refresh_
+00000650: 746f 6b65 6eda 0c61 7574 6865 6e74 6963  token..authentic
+00000660: 6174 6529 0672 1000 0000 721d 0000 0072  ate).r....r....r
+00000670: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+00000680: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000690: 0000 720f 0000 0025 0000 0073 1000 0000  ..r....%...s....
+000006a0: 0601 0602 0601 0601 0601 0601 0601 0c02  ................
+000006b0: 7a12 5374 656c 6c61 4150 492e 5f5f 696e  z.StellaAPI.__in
+000006c0: 6974 5f5f 6302 0000 0000 0000 0000 0000  it__c...........
+000006d0: 0005 0000 0008 0000 0043 0000 0073 d000  .........C...s..
+000006e0: 0000 7a0b 7c01 a000 a100 a001 6401 7402  ..z.|.......d.t.
+000006f0: 8300 a102 7d02 5700 6e0d 0400 7400 6a03  ....}.W.n...t.j.
+00000700: 7918 0100 0100 0100 7402 8300 7d02 5900  y.......t...}.Y.
+00000710: 6e01 7700 7c01 6a04 0400 6402 6b02 724f  n.w.|.j...d.k.rO
+00000720: 0100 7c02 a001 6403 7405 8300 a102 7d03  ..|...d.t.....}.
+00000730: 7c03 4400 5d1f 7d04 7c04 a001 6404 a101  |.D.].}.|...d...
+00000740: 0400 6405 6b02 723b 0100 7c00 a006 a100  ..d.k.r;..|.....
+00000750: 0100 0100 6400 5300 6406 6b02 7243 7407  ....d.S.d.k.rCt.
+00000760: 6407 7c02 8302 8201 0900 7407 6408 7c02  d.|.......t.d.|.
+00000770: 8302 8201 7c01 a008 a100 0100 6400 5300  ....|.......d.S.
+00000780: 0400 6409 6b02 7259 0100 7407 640a 7c02  ..d.k.rY..t.d.|.
+00000790: 8302 8201 640b 6b02 7261 7407 640c 7c02  ....d.k.rat.d.|.
+000007a0: 8302 8201 0900 7c01 a008 a100 0100 6400  ......|.......d.
+000007b0: 5300 290d 4eda 0764 6574 6169 6c73 6991  S.).N..detailsi.
+000007c0: 0100 0072 0d00 0000 5a09 6572 726f 7243  ...r....Z.errorC
+000007d0: 6f64 655a 1169 6e61 6374 6976 6541 7574  odeZ.inactiveAut
+000007e0: 6854 6f6b 656e 5a17 7772 6f6e 6755 7365  hTokenZ.wrongUse
+000007f0: 726e 616d 654f 7250 6173 7377 6f72 647a  rnameOrPasswordz
+00000800: 3755 6e61 7574 686f 7269 7a65 643a 2050  7Unauthorized: P
+00000810: 726f 7669 6465 6420 7573 6572 6e61 6d65  rovided username
+00000820: 206f 7220 7061 7373 776f 7264 2069 7320   or password is 
+00000830: 696e 7661 6c69 642e 5a0c 556e 6175 7468  invalid.Z.Unauth
+00000840: 6f72 697a 6564 6993 0100 007a 4b46 6f72  orizedi....zKFor
+00000850: 6269 6464 656e 3a20 4163 6365 7373 2074  bidden: Access t
+00000860: 6f20 7468 6520 4150 4920 6973 2072 6573  o the API is res
+00000870: 7472 6963 7465 6420 6f6e 6c79 2074 6f20  tricted only to 
+00000880: 7768 6974 656c 6973 7465 6420 636f 6e6e  whitelisted conn
+00000890: 6563 7469 6f6e 732e 6994 0100 007a 094e  ections.i....z.N
+000008a0: 6f74 2046 6f75 6e64 2909 da04 6a73 6f6e  ot Found)...json
+000008b0: da03 6765 74da 0464 6963 74da 0f4a 534f  ..get..dict..JSO
+000008c0: 4e44 6563 6f64 6545 7272 6f72 5a0b 7374  NDecodeErrorZ.st
+000008d0: 6174 7573 5f63 6f64 65da 046c 6973 74da  atus_code..list.
+000008e0: 0c61 7574 685f 7265 6672 6573 6872 0a00  .auth_refreshr..
+000008f0: 0000 5a10 7261 6973 655f 666f 725f 7374  ..Z.raise_for_st
+00000900: 6174 7573 2905 7210 0000 00da 0872 6573  atus).r......res
+00000910: 706f 6e73 6572 2500 0000 720d 0000 00da  ponser%...r.....
+00000920: 0565 7272 6f72 7213 0000 0072 1300 0000  .errorr....r....
+00000930: 7214 0000 00da 105f 6861 6e64 6c65 5f72  r......_handle_r
+00000940: 6573 706f 6e73 6531 0000 0073 3600 0000  esponse1...s6...
+00000950: 0201 1601 0e01 0a01 02ff 0403 0a01 0e01  ................
+00000960: 0802 0801 0a01 0801 0601 0601 0a01 0201  ................
+00000970: 0a01 0c02 0a01 0201 0201 0201 04fe 0604  ................
+00000980: 0a01 0201 0c01 7a1a 5374 656c 6c61 4150  ......z.StellaAP
+00000990: 492e 5f68 616e 646c 655f 7265 7370 6f6e  I._handle_respon
+000009a0: 7365 6301 0000 0000 0000 0000 0000 0003  sec.............
+000009b0: 0000 0006 0000 0043 0000 0073 a000 0000  .......C...s....
+000009c0: 7400 a001 6401 a101 0100 7c00 6a02 6400  t...d.....|.j.d.
+000009d0: 7501 720f 7c00 a003 a100 0100 6e3a 7c00  u.r.|.......n:|.
+000009e0: 6a04 7c00 6a05 7c00 6a05 7c00 6a06 6402  j.|.j.|.j.|.j.d.
+000009f0: 6403 9c05 7d01 6400 7c00 5f07 6400 7c00  d...}.d.|._.d.|.
+00000a00: 5f02 7408 6a09 7c00 6a0a 6a0b 7c01 6404  _.t.j.|.j.j.|.d.
+00000a10: 8d02 7d02 7c00 a00c 7c02 a101 0100 7c02  ..}.|...|.....|.
+00000a20: a00d a100 a00e 6405 740f 8300 a102 a00e  ......d.t.......
+00000a30: 6406 a101 7c00 5f07 7c02 a00d a100 a00e  d...|._.|.......
+00000a40: 6405 740f 8300 a102 a00e 6407 a101 7c00  d.t.......d...|.
+00000a50: 5f02 7400 a001 6408 a101 0100 6400 5300  _.t...d.....d.S.
+00000a60: 2909 4e7a 1e41 7574 6865 6e74 6963 6174  ).Nz.Authenticat
+00000a70: 696e 6720 746f 2074 6865 2041 5049 202e  ing to the API .
+00000a80: 2e2e 205a 0a62 6163 6b6f 6666 6963 6529  .. Z.backoffice)
+00000a90: 055a 0872 6561 6c6d 5f69 64da 0875 7365  .Z.realm_id..use
+00000aa0: 726e 616d 65da 0565 6d61 696c da08 7061  rname..email..pa
+00000ab0: 7373 776f 7264 5a09 636c 6965 6e74 5f69  sswordZ.client_i
+00000ac0: 64a9 0172 2600 0000 7225 0000 0072 1f00  d..r&...r%...r..
+00000ad0: 0000 7223 0000 007a 1941 7574 6865 6e74  ..r#...z.Authent
+00000ae0: 6963 6174 696f 6e20 5375 6363 6573 7366  ication Successf
+00000af0: 756c 2910 da06 6c6f 6767 6572 da04 696e  ul)...logger..in
+00000b00: 666f 7223 0000 0072 2b00 0000 7220 0000  for#...r+...r ..
+00000b10: 0072 1e00 0000 721f 0000 0072 2200 0000  .r....r....r"...
+00000b20: da08 7265 7175 6573 7473 da04 706f 7374  ..requests..post
+00000b30: 721d 0000 00da 0861 7574 685f 7572 6c72  r......auth_urlr
+00000b40: 2e00 0000 7226 0000 0072 2700 0000 7228  ....r&...r'...r(
+00000b50: 0000 00a9 0372 1000 0000 da04 626f 6479  .....r......body
+00000b60: 722c 0000 0072 1300 0000 7213 0000 0072  r,...r....r....r
+00000b70: 1400 0000 7224 0000 0050 0000 0073 2000  ....r$...P...s .
+00000b80: 0000 0a01 0a02 0a01 0403 0401 0401 0401  ................
+00000b90: 0201 06fb 0608 0601 1202 0a01 1a02 1a01  ................
+00000ba0: 0e02 7a16 5374 656c 6c61 4150 492e 6175  ..z.StellaAPI.au
+00000bb0: 7468 656e 7469 6361 7465 6301 0000 0000  thenticatec.....
+00000bc0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000bd0: 0000 0073 9400 0000 7c00 6a00 6400 7500  ...s....|.j.d.u.
+00000be0: 720b 7c00 a001 a100 0100 6400 5300 7402  r.|.......d.S.t.
+00000bf0: a003 6401 a101 0100 6402 7c00 6a00 6901  ..d.....d.|.j.i.
+00000c00: 7d01 6400 7c00 5f04 6400 7c00 5f00 7405  }.d.|._.d.|._.t.
+00000c10: 6a06 7c00 6a07 6a08 7c01 6403 8d02 7d02  j.|.j.j.|.d...}.
+00000c20: 7c00 a009 7c02 a101 0100 7c02 a00a a100  |...|.....|.....
+00000c30: a00b 6404 740c 8300 a102 a00b 6405 a101  ..d.t.......d...
+00000c40: 7c00 5f04 7c02 a00a a100 a00b 6404 740c  |._.|.......d.t.
+00000c50: 8300 a102 a00b 6402 a101 7c00 5f00 7402  ......d...|._.t.
+00000c60: a003 6406 a101 0100 6400 5300 2907 4e7a  ..d.....d.S.).Nz
+00000c70: 1841 5049 2054 6f6b 656e 2052 6566 7265  .API Token Refre
+00000c80: 7368 696e 6720 2e2e 2e72 2300 0000 7232  shing ...r#...r2
+00000c90: 0000 0072 2500 0000 721f 0000 007a 1c41  ...r%...r....z.A
+00000ca0: 5049 2054 6f6b 656e 2052 6566 7265 7368  PI Token Refresh
+00000cb0: 2053 7563 6365 7373 6675 6c29 0d72 2300   Successful).r#.
+00000cc0: 0000 7224 0000 0072 3300 0000 7234 0000  ..r$...r3...r4..
+00000cd0: 0072 2200 0000 7235 0000 0072 3600 0000  .r"...r5...r6...
+00000ce0: 721d 0000 00da 1061 7574 685f 7265 6672  r......auth_refr
+00000cf0: 6573 685f 7572 6c72 2e00 0000 7226 0000  esh_urlr....r&..
+00000d00: 0072 2700 0000 7228 0000 0072 3800 0000  .r'...r(...r8...
+00000d10: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000d20: 2b00 0000 6900 0000 7316 0000 000a 010c  +...i...s.......
+00000d30: 010a 020a 0206 0206 0112 020a 011a 021a  ................
+00000d40: 010e 027a 1653 7465 6c6c 6141 5049 2e61  ...z.StellaAPI.a
+00000d50: 7574 685f 7265 6672 6573 68da 0672 6574  uth_refresh..ret
+00000d60: 7572 6e4e 6301 0000 0000 0000 0000 0000  urnNc...........
+00000d70: 0007 0000 0007 0000 0063 0000 0073 b200  .........c...s..
+00000d80: 0000 8100 6401 7d01 7400 a001 6402 6402  ....d.}.t...d.d.
+00000d90: a102 4400 5d4d 7d02 7c00 6a02 6a03 6a04  ..D.]M}.|.j.j.j.
+00000da0: 7c00 6a05 6403 8d01 6404 7c02 9b00 6405  |.j.d...d.|...d.
+00000db0: 7c01 9b00 6406 9d05 1700 7d03 6407 6408  |...d.....}.d.d.
+00000dc0: 7c00 6a06 9b00 9d02 6901 7d04 7407 6a08  |.j.....i.}.t.j.
+00000dd0: 7c03 7c04 6409 8d02 7d05 7c00 a009 7c05  |.|.d...}.|...|.
+00000de0: a101 0100 7c05 a00a a100 a008 640a 740b  ....|.......d.t.
+00000df0: 8300 a102 a008 640b 6700 a102 7d06 7c06  ......d.g...}.|.
+00000e00: 7343 0100 6400 5300 640c 640d 8400 7c06  sC..d.S.d.d...|.
+00000e10: 4400 8301 4500 6400 4800 0100 740c 7c06  D...E.d.H...t.|.
+00000e20: 8301 7c01 6b00 7256 0100 6400 5300 7109  ..|.k.rV..d.S.q.
+00000e30: 6400 5300 290e 4e69 e803 0000 7205 0000  d.S.).Ni....r...
+00000e40: 0029 01da 0970 726f 6a65 6374 4964 7a0c  .)...projectIdz.
+00000e50: 3f70 6167 654e 756d 6265 723d 7a0a 2670  ?pageNumber=z.&p
+00000e60: 6167 6553 697a 653d 7a17 2666 696c 7465  ageSize=z.&filte
+00000e70: 723d 496e 636c 7564 6549 6e61 6374 6976  r=IncludeInactiv
+00000e80: 65da 0d41 7574 686f 7269 7a61 7469 6f6e  e..Authorization
+00000e90: fa07 4265 6172 6572 20a9 01da 0768 6561  ..Bearer ....hea
+00000ea0: 6465 7273 7225 0000 00da 0772 6573 756c  dersr%.....resul
+00000eb0: 7473 6301 0000 0000 0000 0000 0000 0002  tsc.............
+00000ec0: 0000 0009 0000 0073 0000 0073 4000 0000  .......s...s@...
+00000ed0: 8100 7c00 5d1b 7d01 7400 7c01 a001 6400  ..|.].}.t.|...d.
+00000ee0: a101 7c01 a001 6401 a101 7c01 a001 6402  ..|...d...|...d.
+00000ef0: a101 7c01 a001 6403 a101 7c01 a001 6404  ..|...d...|...d.
+00000f00: a101 6405 8d05 5600 0100 7102 6406 5300  ..d...V...q.d.S.
+00000f10: 2907 da02 6964 da04 6e61 6d65 da08 6973  )...id..name..is
+00000f20: 4163 7469 7665 da09 6372 6561 7465 6441  Active..createdA
+00000f30: 74da 0975 7064 6174 6564 4174 2905 7242  t..updatedAt).rB
+00000f40: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
+00000f50: 0000 7246 0000 004e 2902 7208 0000 0072  ..rF...N).r....r
+00000f60: 2700 0000 2902 da02 2e30 da05 6576 656e  '...)....0..even
+00000f70: 7472 1300 0000 7213 0000 0072 1400 0000  tr....r....r....
+00000f80: da09 3c67 656e 6578 7072 3e8a 0000 0073  ..<genexpr>....s
+00000f90: 1600 0000 0280 0400 0207 02fa 0801 0801  ................
+00000fa0: 0801 0801 0801 04fb 0aff 7a27 5374 656c  ..........z'Stel
+00000fb0: 6c61 4150 492e 6765 745f 6576 656e 7473  laAPI.get_events
+00000fc0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000fd0: 7072 3e29 0dda 0969 7465 7274 6f6f 6c73  pr>)...itertools
+00000fe0: da05 636f 756e 7472 1d00 0000 da0a 6576  ..countr......ev
+00000ff0: 656e 7473 5f75 726c da06 666f 726d 6174  ents_url..format
+00001000: 7221 0000 0072 2200 0000 7235 0000 0072  r!...r"...r5...r
+00001010: 2700 0000 722e 0000 0072 2600 0000 7228  '...r....r&...r(
+00001020: 0000 00da 036c 656e 2907 7210 0000 005a  .....len).r....Z
+00001030: 0970 6167 655f 7369 7a65 5a0b 7061 6765  .page_sizeZ.page
+00001040: 5f6e 756d 6265 72da 0375 726c 7240 0000  _number..urlr@..
+00001050: 0072 2c00 0000 da06 6576 656e 7473 7213  .r,.....eventsr.
+00001060: 0000 0072 1300 0000 7214 0000 00da 0a67  ...r....r......g
+00001070: 6574 5f65 7665 6e74 737c 0000 0073 2600  et_events|...s&.
+00001080: 0000 0280 0401 1001 1001 1001 04ff 1002  ................
+00001090: 0e02 0a01 1a02 0401 0601 0602 0207 0cf9  ................
+000010a0: 0c0a 0601 02ff 04ea 7a14 5374 656c 6c61  ........z.Stella
+000010b0: 4150 492e 6765 745f 6576 656e 7473 da08  API.get_events..
+000010c0: 6576 656e 745f 6964 6302 0000 0000 0000  event_idc.......
+000010d0: 0000 0000 0008 0000 000a 0000 0043 0000  .............C..
+000010e0: 0073 ba00 0000 7c00 6a00 6a01 6a02 7c00  .s....|.j.j.j.|.
+000010f0: 6a03 7c01 6401 8d02 7d02 6402 6403 7c00  j.|.d...}.d.d.|.
+00001100: 6a04 9b00 9d02 6901 7d03 7405 6a06 7c02  j.....i.}.t.j.|.
+00001110: 7c03 6404 8d02 7d04 7c00 a007 7c04 a101  |.d...}.|...|...
+00001120: 0100 7c04 a008 a100 a006 6405 7409 8300  ..|.......d.t...
+00001130: a102 7d05 6406 6407 8400 7c05 a006 6408  ..}.d.d...|...d.
+00001140: 740a 8300 a102 4400 8301 7d06 6409 6407  t.....D...}.d.d.
+00001150: 8400 7c05 a006 640a 740a 8300 a102 4400  ..|...d.t.....D.
+00001160: 8301 7d07 740b 7c05 a006 640b a101 7c05  ..}.t.|...d...|.
+00001170: a006 640c a101 7c05 a006 640d a101 7c05  ..d...|...d...|.
+00001180: a006 640e a101 7c05 a006 640f a101 7c05  ..d...|...d...|.
+00001190: a006 6410 a101 7c07 7c06 6411 8d08 5300  ..d...|.|.d...S.
+000011a0: 2912 4e29 0272 3c00 0000 5a07 6576 656e  ).N).r<...Z.even
+000011b0: 7449 6472 3d00 0000 723e 0000 0072 3f00  tIdr=...r>...r?.
+000011c0: 0000 7225 0000 0063 0100 0000 0000 0000  ..r%...c........
+000011d0: 0000 0000 0200 0000 0600 0000 5300 0000  ............S...
+000011e0: f31a 0000 0067 007c 005d 097d 0174 0064  .....g.|.].}.t.d
+000011f0: 0069 007c 01a4 018e 0191 0271 0253 00a9  .i.|.......q.S..
+00001200: 0172 1300 0000 2901 7206 0000 0029 0272  .r....).r....).r
+00001210: 4700 0000 da06 656e 7469 7479 7213 0000  G.....entityr...
+00001220: 0072 1300 0000 7214 0000 00da 0a3c 6c69  .r....r......<li
+00001230: 7374 636f 6d70 3ea1 0000 00f3 0200 0000  stcomp>.........
+00001240: 1a00 7a2f 5374 656c 6c61 4150 492e 6765  ..z/StellaAPI.ge
+00001250: 745f 6576 656e 745f 6465 7461 696c 732e  t_event_details.
+00001260: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001270: 6d70 3eda 0865 6e74 6974 6965 7363 0100  mp>..entitiesc..
+00001280: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00001290: 0000 5300 0000 7253 0000 0072 5400 0000  ..S...rS...rT...
+000012a0: 2901 7207 0000 0029 0272 4700 0000 da05  ).r....).rG.....
+000012b0: 6669 656c 6472 1300 0000 7213 0000 0072  fieldr....r....r
+000012c0: 1400 0000 7256 0000 00a4 0000 0072 5700  ....rV.......rW.
+000012d0: 0000 da06 6669 656c 6473 7242 0000 0072  ....fieldsrB...r
+000012e0: 4300 0000 da0b 6465 7363 7269 7074 696f  C.....descriptio
+000012f0: 6e72 4400 0000 7245 0000 0072 4600 0000  nrD...rE...rF...
+00001300: 2908 7242 0000 0072 4300 0000 725b 0000  ).rB...rC...r[..
+00001310: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
+00001320: 725a 0000 0072 5800 0000 290c 721d 0000  rZ...rX...).r...
+00001330: 00da 0965 7665 6e74 5f75 726c 724d 0000  ...event_urlrM..
+00001340: 0072 2100 0000 7222 0000 0072 3500 0000  .r!...r"...r5...
+00001350: 7227 0000 0072 2e00 0000 7226 0000 0072  r'...r....r&...r
+00001360: 2800 0000 722a 0000 0072 0900 0000 2908  (...r*...r....).
+00001370: 7210 0000 0072 5200 0000 724f 0000 0072  r....rR...rO...r
+00001380: 4000 0000 722c 0000 0072 2500 0000 7258  @...r,...r%...rX
+00001390: 0000 0072 5a00 0000 7213 0000 0072 1300  ...rZ...r....r..
+000013a0: 0000 7214 0000 00da 1167 6574 5f65 7665  ..r......get_eve
+000013b0: 6e74 5f64 6574 6169 6c73 9700 0000 7322  nt_details....s"
+000013c0: 0000 0014 0110 010e 020a 0112 0218 0318  ................
+000013d0: 0302 0308 0108 0108 0108 0108 0108 0102  ................
+000013e0: 0102 0106 f87a 1b53 7465 6c6c 6141 5049  .....z.StellaAPI
+000013f0: 2e67 6574 5f65 7665 6e74 5f64 6574 6169  .get_event_detai
+00001400: 6c73 290e 7217 0000 0072 1800 0000 7219  ls).r....r....r.
+00001410: 0000 0072 0400 0000 da03 7374 7272 0f00  ...r......strr..
+00001420: 0000 722e 0000 0072 2400 0000 722b 0000  ..r....r$...r+..
+00001430: 0072 0200 0000 7208 0000 0072 5100 0000  .r....r....rQ...
+00001440: 7209 0000 0072 5d00 0000 7213 0000 0072  r....r]...r....r
+00001450: 1300 0000 7213 0000 0072 1400 0000 721c  ....r....r....r.
+00001460: 0000 0024 0000 0073 0e00 0000 0800 1e01  ...$...s........
+00001470: 080c 081f 0819 1813 161b 721c 0000 0029  ..........r....)
+00001480: 1472 1a00 0000 724a 0000 0072 2600 0000  .r....rJ...r&...
+00001490: da07 6c6f 6767 696e 6772 3500 0000 da06  ..loggingr5.....
+000014a0: 7479 7069 6e67 7202 0000 00da 0663 6f6e  typingr......con
+000014b0: 6669 6772 0400 0000 da09 6461 7461 7479  figr......dataty
+000014c0: 7065 7372 0600 0000 7207 0000 0072 0800  pesr....r....r..
+000014d0: 0000 7209 0000 00da 0967 6574 4c6f 6767  ..r......getLogg
+000014e0: 6572 7217 0000 0072 3300 0000 da09 4578  err....r3.....Ex
+000014f0: 6365 7074 696f 6e72 0a00 0000 721c 0000  ceptionr....r...
+00001500: 0072 1300 0000 7213 0000 0072 1300 0000  .r....r....r....
+00001510: 7214 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001520: 0000 0073 1600 0000 0400 0809 0801 0801  ...s............
+00001530: 0801 0c02 0c02 1801 0a03 1003 120c       ..............
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.6/stellanow_cli/api/stellanow_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,52 +3,26 @@
 
 This software is the proprietary information of Stella Technologies (UK) Limited.
 Use, reproduction, or redistribution of this software is strictly prohibited without
 the express written permission of Stella Technologies (UK) Limited.
 All rights reserved.
 """
 
+import itertools
 import json
+import logging
 import requests
 
-from dataclasses import dataclass
-from sys import maxsize
-from typing import Generator, List
+from typing import Generator
 
-from ..logger import logger
 from ..config import Config
+from .datatypes import StellaEntity, StellaField, StellaEvent, StellaEventDetailed
 
 
-@dataclass
-class StellaEntity:
-    id: str
-    name: str
-
-
-@dataclass
-class StellaField:
-    id: str
-    name: str
-    valueType: str
-
-
-@dataclass
-class StellaEvent:
-    id: str
-    name: str
-    isActive: bool
-    createdAt: str
-    updatedAt: str
-
-
-@dataclass
-class StellaEventDetailed(StellaEvent):
-    description: str
-    fields: List[StellaField]
-    entities: List[StellaEntity]
+logger = logging.getLogger(__name__)
 
 
 class StellaAPIError(Exception):
     """Exception raised for errors in the Stella API."""
 
     def __init__(self, message, errors):
         self.message = message
@@ -70,32 +44,33 @@
         self.auth_token = None
         self.refresh_token = None
 
         self.authenticate()
 
     def _handle_response(self, response):
         try:
-            details = response.json().get("details")
+            details = response.json().get("details", dict())
         except json.JSONDecodeError:
-            details = None
+            details = dict()
 
         match response.status_code:
             case 401:
-                # Normalize to always have a list of errors
-                errors = details.get("errors") if isinstance(details, dict) else details
+                errors = details.get("errors", list())
 
                 for error in errors:
                     match error.get("errorCode"):
                         case "inactiveAuthToken":
                             self.auth_refresh()
                             return
                         case "wrongUsernameOrPassword":
                             raise StellaAPIError('Unauthorized: Provided username or password is invalid.', details)
                         case _:
                             raise StellaAPIError('Unauthorized', details)
+                else:
+                    response.raise_for_status()
             case 403:
                 raise StellaAPIError(
                     "Forbidden: Access to the API is restricted only to whitelisted connections.",
                     details
                 )
             case 404:
                 raise StellaAPIError('Not Found', details)
@@ -118,16 +93,16 @@
 
             self.auth_token = None
             self.refresh_token = None
 
             response = requests.post(self.env_config.auth_url, json=body)
             self._handle_response(response)
 
-            self.auth_token = response.json().get("details").get("access_token")
-            self.refresh_token = response.json().get("details").get("refresh_token")
+            self.auth_token = response.json().get("details", dict()).get("access_token")
+            self.refresh_token = response.json().get("details", dict()).get("refresh_token")
 
         logger.info("Authentication Successful")
 
     def auth_refresh(self):
         if self.refresh_token is None:
             self.authenticate()
         else:
@@ -137,59 +112,60 @@
 
             self.auth_token = None
             self.refresh_token = None
 
             response = requests.post(self.env_config.auth_refresh_url, json=body)
             self._handle_response(response)
 
-            self.auth_token = response.json().get("details").get("access_token")
-            self.refresh_token = response.json().get("details").get("refresh_token")
+            self.auth_token = response.json().get("details", dict()).get("access_token")
+            self.refresh_token = response.json().get("details", dict()).get("refresh_token")
 
             logger.info("API Token Refresh Successful")
 
     def get_events(self) -> Generator[StellaEvent, None, None]:
-        page_number = 1
-        number_of_pages = maxsize
-        while page_number < number_of_pages:
-            url = self.env_config.events_url.format(projectId=self.project_id) + f"?pageNumber={page_number}&pageSize=1000"
+        page_size = 1000
+        for page_number in itertools.count(1, 1):
+            url = self.env_config.events_url.format(projectId=self.project_id) + \
+                  f"?pageNumber={page_number}&pageSize={page_size}&filter=IncludeInactive"
             headers = {"Authorization": f"Bearer {self.auth_token}"}
 
             response = requests.get(url, headers=headers)
             self._handle_response(response)
 
-            events = response.json().get("details", {}).get("results", [])
-            number_of_pages = response.json().get("details", {}).get("numberOfPages", 0)
+            events = response.json().get("details", dict()).get("results", [])
             if not events:
                 break
 
-            for event in events:
-                yield StellaEvent(
+            yield from (
+                StellaEvent(
                     id=event.get('id'),
                     name=event.get('name'),
                     isActive=event.get('isActive'),
                     createdAt=event.get('createdAt'),
                     updatedAt=event.get('updatedAt')
-                )
+                ) for event in events
+            )
 
-            page_number += 1
+            if len(events) < page_size:
+                break
 
     def get_event_details(self, event_id: str) -> StellaEventDetailed:
         url = self.env_config.event_url.format(projectId=self.project_id, eventId=event_id)
         headers = {"Authorization": f"Bearer {self.auth_token}"}
 
         response = requests.get(url, headers=headers)
         self._handle_response(response)
 
-        details = response.json().get("details", {})
+        details = response.json().get("details", dict())
 
         # create StellaEntity objects from the 'entities' list
-        entities = [StellaEntity(**entity) for entity in details.get('entities', [])]
+        entities = [StellaEntity(**entity) for entity in details.get('entities', list())]
 
         # create StellaField objects from the 'fields' list
-        fields = [StellaField(**field) for field in details.get('fields', [])]
+        fields = [StellaField(**field) for field in details.get('fields', list())]
 
         # create and return StellaEventDetailed object
         return StellaEventDetailed(
             id=details.get('id'),
             name=details.get('name'),
             description=details.get('description'),
             isActive=details.get('isActive'),
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/cli.py` & `stellanow_cli-0.0.6/stellanow_cli/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-
 """
 Copyright (C) 2022-2023 Stella Technologies (UK) Limited.
 
 This software is the proprietary information of Stella Technologies (UK) Limited.
 Use, reproduction, or redistribution of this software is strictly prohibited without
 the express written permission of Stella Technologies (UK) Limited.
 All rights reserved.
@@ -38,11 +36,7 @@
     ctx.obj = config
 
 
 cli.add_command(configure_cmd)
 cli.add_command(generate_cmd)
 cli.add_command(plan_cmd)
 cli.add_command(events_cmd)
-
-
-if __name__ == '__main__':
-    cli()
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.5/stellanow_cli/code_generators/code_generator.py` & `stellanow_cli-0.0.6/stellanow_cli/code_generators/code_generator.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.5/stellanow_cli/command_config.py` & `stellanow_cli-0.0.6/stellanow_cli/commands/command_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 
 This software is the proprietary information of Stella Technologies (UK) Limited.
 Use, reproduction, or redistribution of this software is strictly prohibited without
 the express written permission of Stella Technologies (UK) Limited.
 All rights reserved.
 """
 
+import importlib
 import click
 import functools
+import logging
 import os
 
-from .api import StellaAPI
-from .logger import setup_logger, logger
-from .utils import snake_to_camel
-from .config.dev import ConfigDev
-from .config.int import ConfigInt
+from ..api import StellaAPI
+from ..config.int import ConfigInt
+from ..config import Env
+from ..utils.logger import setup_logger
+from ..utils import snake_to_camel
+
+
+logger = logging.getLogger(__name__)
 
 
 def common_option(f):
     """
     Common CLI options to be used across multiple commands
     """
     decorators = [
@@ -34,15 +39,15 @@
                           "This is used to scope the operations within the given organization's context."),
         click.option('--project_id',
                      help="The unique identifier (UUID) of the project in StellaNow. "
                           "This is used to scope the operations within the given project's context."),
         click.option('--profile', default='DEFAULT',
                      help="The profile name for storing a particular set of configurations. "
                           "If no profile is specified, the configurations will be stored under the 'DEFAULT' profile."),
-        click.option('--env', hidden=True, help=""),
+        click.option('--env', hidden=True, type=click.Choice([e.value for e in Env], case_sensitive=False), help=""),
         click.option('--verbose', '-v', is_flag=True, help="Enables verbose mode, which outputs more detailed logging "
                                                            "messages.")
     ]
 
     for decorator in reversed(decorators):
         f = decorator(f)
     return f
@@ -75,15 +80,19 @@
 
         # Check if all required options are present
         if any(value is None for value in kwargs.values()):
             logger.error('All required options are not set. Please use the "configure" command to set them.')
             ctx.exit(1)
 
         env_config_class_name = f"Config{snake_to_camel(kwargs.get('env'))}"
-        env_config_class = globals().get(env_config_class_name) or ConfigInt
+        try:
+            env_config_class = getattr(importlib.import_module(f"stellanow_cli.config.{kwargs.get('env')}"),
+                                       env_config_class_name)
+        except ImportError:
+            env_config_class = ConfigInt
 
         # Create StellaAPI instance and pass it as a named argument
         kwargs['stella_api'] = StellaAPI(
             env_config_class(),
             kwargs.get('access_key'),
             kwargs.get('access_token'),
             kwargs.get('organization_id'),
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/configure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:54:02 2023 UTC, .py size: 3819 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,184 +1,183 @@
-00000000: 6f0d 0d0a 0000 0000 6a7a 8b64 eb0e 0000  o.......jz.d....
+00000000: 6f0d 0d0a 0000 0000 1daa 8d64 d40e 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6403 6404 6c05 6d06 5a06 0100 6403  Z.d.d.l.m.Z...d.
-00000060: 6405 6c07 6d07 5a07 0100 6403 6406 6c08  d.l.m.Z...d.d.l.
-00000070: 6d09 5a09 0100 6501 6a0a 6407 6408 8d01  m.Z...e.j.d.d...
-00000080: 6501 6a0b 6409 640a 640b 640c 640d 8d04  e.j.d.d.d.d.d...
-00000090: 6501 6a0b 640e 640f 6501 6a0c 6410 6411  e.j.d.d.e.j.d.d.
-000000a0: 8400 6509 4400 8301 640b 6412 8d02 6413  ..e.D...d.d...d.
-000000b0: 8d03 6501 6a0d 6414 6407 8400 8301 8301  ..e.j.d.d.......
-000000c0: 8301 8301 5a0e 650e 5a0f 6402 5300 2915  ....Z.e.Z.d.S.).
-000000d0: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
-000000e0: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
-000000f0: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-00000100: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-00000110: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
-00000120: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
-00000130: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
-00000140: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
-00000150: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
-00000160: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
-00000170: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
-00000180: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
-00000190: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
-000001a0: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
-000001b0: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
-000001c0: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
-000001d0: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
-000001e0: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
-000001f0: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
-00000200: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-00000210: 0ae9 0000 0000 4ee9 0200 0000 2901 da0d  ......N.....)...
+00000050: 5a04 6403 6404 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
+00000060: 0100 6403 6405 6c08 6d09 5a09 0100 6501  ..d.d.l.m.Z...e.
+00000070: 6a0a 6406 6407 8d01 6501 6a0b 6408 6409  j.d.d...e.j.d.d.
+00000080: 640a 640b 640c 8d04 6501 6a0b 640d 640e  d.d.d...e.j.d.d.
+00000090: 6501 6a0c 640f 6410 8400 6509 4400 8301  e.j.d.d...e.D...
+000000a0: 640a 6411 8d02 6412 8d03 6501 6a0d 6413  d.d...d...e.j.d.
+000000b0: 6406 8400 8301 8301 8301 8301 5a0e 650e  d...........Z.e.
+000000c0: 5a0f 6402 5300 2914 613c 0100 000a 436f  Z.d.S.).a<....Co
+000000d0: 7079 7269 6768 7420 2843 2920 3230 3232  pyright (C) 2022
+000000e0: 2d32 3032 3320 5374 656c 6c61 2054 6563  -2023 Stella Tec
+000000f0: 686e 6f6c 6f67 6965 7320 2855 4b29 204c  hnologies (UK) L
+00000100: 696d 6974 6564 2e0a 0a54 6869 7320 736f  imited...This so
+00000110: 6674 7761 7265 2069 7320 7468 6520 7072  ftware is the pr
+00000120: 6f70 7269 6574 6172 7920 696e 666f 726d  oprietary inform
+00000130: 6174 696f 6e20 6f66 2053 7465 6c6c 6120  ation of Stella 
+00000140: 5465 6368 6e6f 6c6f 6769 6573 2028 554b  Technologies (UK
+00000150: 2920 4c69 6d69 7465 642e 0a55 7365 2c20  ) Limited..Use, 
+00000160: 7265 7072 6f64 7563 7469 6f6e 2c20 6f72  reproduction, or
+00000170: 2072 6564 6973 7472 6962 7574 696f 6e20   redistribution 
+00000180: 6f66 2074 6869 7320 736f 6674 7761 7265  of this software
+00000190: 2069 7320 7374 7269 6374 6c79 2070 726f   is strictly pro
+000001a0: 6869 6269 7465 6420 7769 7468 6f75 740a  hibited without.
+000001b0: 7468 6520 6578 7072 6573 7320 7772 6974  the express writ
+000001c0: 7465 6e20 7065 726d 6973 7369 6f6e 206f  ten permission o
+000001d0: 6620 5374 656c 6c61 2054 6563 686e 6f6c  f Stella Technol
+000001e0: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
+000001f0: 6564 2e0a 416c 6c20 7269 6768 7473 2072  ed..All rights r
+00000200: 6573 6572 7665 642e 0ae9 0000 0000 4ee9  eserved.......N.
+00000210: 0200 0000 2902 da06 6c6f 6767 6572 da0d  ....)...logger..
 00000220: 6973 5f76 616c 6964 5f75 7569 6429 01da  is_valid_uuid)..
-00000230: 066c 6f67 6765 7229 01da 0345 6e76 da09  .logger)...Env..
-00000240: 636f 6e66 6967 7572 6529 01da 046e 616d  configure)...nam
-00000250: 657a 092d 2d70 726f 6669 6c65 da07 4445  ez.--profile..DE
-00000260: 4641 554c 5446 7a9b 5468 6520 7072 6f66  FAULTFz.The prof
-00000270: 696c 6520 6e61 6d65 2066 6f72 2073 746f  ile name for sto
-00000280: 7269 6e67 2061 2070 6172 7469 6375 6c61  ring a particula
-00000290: 7220 7365 7420 6f66 2063 6f6e 6669 6775  r set of configu
-000002a0: 7261 7469 6f6e 732e 2049 6620 6e6f 2070  rations. If no p
-000002b0: 726f 6669 6c65 2069 7320 7370 6563 6966  rofile is specif
-000002c0: 6965 642c 2074 6865 2063 6f6e 6669 6775  ied, the configu
-000002d0: 7261 7469 6f6e 7320 7769 6c6c 2062 6520  rations will be 
-000002e0: 7374 6f72 6564 2075 6e64 6572 2074 6865  stored under the
-000002f0: 2027 4445 4641 554c 5427 2070 726f 6669   'DEFAULT' profi
-00000300: 6c65 2e29 03da 0764 6566 6175 6c74 da06  le.)...default..
-00000310: 7072 6f6d 7074 da04 6865 6c70 7a05 2d2d  prompt..helpz.--
-00000320: 656e 7654 6301 0000 0000 0000 0000 0000  envTc...........
-00000330: 0002 0000 0003 0000 0043 0000 0073 1200  .........C...s..
-00000340: 0000 6700 7c00 5d05 7d01 7c01 6a00 9102  ..g.|.].}.|.j...
-00000350: 7102 5300 a900 2901 da05 7661 6c75 6529  q.S...)...value)
-00000360: 02da 022e 30da 0165 720c 0000 0072 0c00  ....0..er....r..
-00000370: 0000 fa60 2f55 7365 7273 2f74 6f6d 2d6b  ...`/Users/tom-k
-00000380: 616e 647a 696f 7261 2f44 6576 4c6f 6361  andziora/DevLoca
-00000390: 6c2f 7374 656c 6c61 2f73 7465 6c6c 612d  l/stella/stella-
-000003a0: 6e6f 772f 5374 656c 6c61 4e6f 7743 4c49  now/StellaNowCLI
-000003b0: 2f73 7465 6c6c 616e 6f77 5f63 6c69 2f63  /stellanow_cli/c
-000003c0: 6f6d 6d61 6e64 732f 636f 6e66 6967 7572  ommands/configur
-000003d0: 652e 7079 da0a 3c6c 6973 7463 6f6d 703e  e.py..<listcomp>
-000003e0: 1800 0000 7302 0000 0012 0072 1100 0000  ....s......r....
-000003f0: 2901 da0e 6361 7365 5f73 656e 7369 7469  )...case_sensiti
-00000400: 7665 2902 da06 6869 6464 656e da04 7479  ve)...hidden..ty
-00000410: 7065 6303 0000 0000 0000 0000 0000 000d  pec.............
-00000420: 0000 0008 0000 0043 0000 0073 ce01 0000  .......C...s....
-00000430: 7400 6401 7c01 9b00 9d02 8301 0100 7c00  t.d.|.........|.
-00000440: 6a01 7d03 7c03 6a02 7c01 6402 6403 6404  j.}.|.j.|.d.d.d.
-00000450: 8d03 7d04 7c03 6a02 7c01 6405 6403 6404  ..}.|.j.|.d.d.d.
-00000460: 8d03 7d05 7c03 6a02 7c01 6406 6403 6404  ..}.|.j.|.d.d.d.
-00000470: 8d03 7d06 7c03 6a02 7c01 6407 6403 6404  ..}.|.j.|.d.d.d.
-00000480: 8d03 7d07 6408 7d08 6409 7d09 0900 7403  ..}.d.}.d.}...t.
-00000490: 6a04 640b 7c04 640c 8d02 7d04 7405 a006  j.d.|.d...}.t...
-000004a0: 7c08 7c04 a102 7342 7405 a006 7c09 7c04  |.|...sBt...|.|.
-000004b0: a102 7243 6e06 7407 a008 640d a101 0100  ..rCn.t...d.....
-000004c0: 712f 0900 7403 6a04 640e 640a 7c05 640f  q/..t.j.d.d.|.d.
-000004d0: 6410 8d04 7d05 7405 a006 6411 7c05 a102  d...}.t...d.|...
-000004e0: 725a 6e06 7407 a008 6412 a101 0100 714a  rZn.t...d.....qJ
-000004f0: 0900 7403 6a04 6413 7c06 640c 8d02 7d06  ..t.j.d.|.d...}.
-00000500: 7409 7c06 8301 726d 6e06 7407 a008 6414  t.|...rmn.t...d.
-00000510: a101 0100 7161 0900 7403 6a04 6415 7c07  ....qa..t.j.d.|.
-00000520: 640c 8d02 7d07 7409 7c07 8301 7280 6e06  d...}.t.|...r.n.
-00000530: 7407 a008 6414 a101 0100 7174 740a 6a0b  t...d.....qtt.j.
-00000540: a00c 6416 a101 7d0a 740a 6a0d 740a 6a0b  ..d...}.t.j.t.j.
-00000550: a00e 7c0a 6417 a102 640a 6418 8d02 0100  ..|.d...d.d.....
-00000560: 740f a010 a100 7d03 740a 6a0b a00e 7c0a  t.....}.t.j...|.
-00000570: 6417 6419 a103 7d0b 740a 6a0b a011 7c0b  d.d...}.t.j...|.
-00000580: a101 72af 7c03 a012 7c0b a101 0100 7c04  ..r.|...|.....|.
-00000590: 7c05 7c06 7c07 641a 9c04 7c03 7c01 3c00  |.|.|.d...|.|.<.
-000005a0: 7c02 6403 7501 72c2 7c02 7c03 7c01 1900  |.d.u.r.|.|.|...
-000005b0: 641b 3c00 7413 7c0b 641c 8302 8f0d 7d0c  d.<.t.|.d.....}.
-000005c0: 7c03 a014 7c0c a101 0100 5700 6403 0400  |...|.....W.d...
-000005d0: 0400 8303 0100 6e08 3100 73d7 7701 0100  ......n.1.s.w...
-000005e0: 0100 0100 5900 0100 7407 a008 641d 7c01  ....Y...t...d.|.
-000005f0: 9b00 641e 9d03 a101 0100 6403 5300 291f  ..d.......d.S.).
-00000600: 7a80 5365 7473 2075 7020 7468 6520 6e65  z.Sets up the ne
-00000610: 6365 7373 6172 7920 6372 6564 656e 7469  cessary credenti
-00000620: 616c 7320 616e 6420 636f 6e66 6967 7572  als and configur
-00000630: 6174 696f 6e73 2066 6f72 2061 2073 7065  ations for a spe
-00000640: 6369 6669 6320 7072 6f66 696c 6520 6f72  cific profile or
-00000650: 2066 6f72 2074 6865 2044 4546 4155 4c54   for the DEFAULT
-00000660: 2070 726f 6669 6c65 2069 6620 6e6f 6e65   profile if none
-00000670: 0a20 2020 2069 7320 7370 6563 6966 6965  .    is specifie
-00000680: 642e 7a23 5072 6f76 6964 6520 636f 6e66  d.z#Provide conf
-00000690: 6967 7572 6174 696f 6e20 666f 7220 7072  iguration for pr
-000006a0: 6f66 696c 653a 20da 0a61 6363 6573 735f  ofile: ..access_
-000006b0: 6b65 794e 2901 da08 6661 6c6c 6261 636b  keyN)...fallback
-000006c0: da0c 6163 6365 7373 5f74 6f6b 656e da0f  ..access_token..
-000006d0: 6f72 6761 6e69 7a61 7469 6f6e 5f69 64da  organization_id.
-000006e0: 0a70 726f 6a65 6374 5f69 647a 335c 625b  .project_idz3\b[
-000006f0: 412d 5a61 2d7a 302d 392e 5f25 2b2d 5d2b  A-Za-z0-9._%+-]+
-00000700: 405b 412d 5a61 2d7a 302d 392e 2d5d 2b5c  @[A-Za-z0-9.-]+\
-00000710: 2e5b 412d 5a7c 612d 7a5d 7b32 2c7d 5c62  .[A-Z|a-z]{2,}\b
-00000720: 7a10 5e5b 612d 7a41 2d5a 302d 395f 2d5d  z.^[a-zA-Z0-9_-]
-00000730: 2b24 547a 0a41 6363 6573 7320 4b65 7929  +$Tz.Access Key)
-00000740: 0172 0900 0000 7a8b 496e 7661 6c69 6420  .r....z.Invalid 
-00000750: 6163 6365 7373 206b 6579 2066 6f72 6d61  access key forma
-00000760: 742e 2049 7420 7368 6f75 6c64 2062 6520  t. It should be 
-00000770: 6120 7661 6c69 6420 656d 6169 6c20 6164  a valid email ad
-00000780: 6472 6573 7320 6f72 2061 2073 7472 696e  dress or a strin
-00000790: 6720 636f 6e74 6169 6e69 6e67 206f 6e6c  g containing onl
-000007a0: 7920 616c 7068 616e 756d 6572 6963 2063  y alphanumeric c
-000007b0: 6861 7261 6374 6572 732c 2064 6173 6865  haracters, dashe
-000007c0: 732c 2061 6e64 2075 6e64 6572 7363 6f72  s, and underscor
-000007d0: 6573 2e7a 0c41 6363 6573 7320 546f 6b65  es.z.Access Toke
-000007e0: 6e46 2903 da0a 6869 6465 5f69 6e70 7574  nF)...hide_input
-000007f0: 7209 0000 00da 0c73 686f 775f 6465 6661  r......show_defa
-00000800: 756c 747a 0a5e 5c53 7b38 2c36 347d 247a  ultz.^\S{8,64}$z
-00000810: 5949 6e76 616c 6964 2061 6363 6573 7320  YInvalid access 
-00000820: 746f 6b65 6e20 666f 726d 6174 2e20 4974  token format. It
-00000830: 2073 686f 756c 6420 636f 6e74 6169 6e20   should contain 
-00000840: 6e6f 2077 6869 7465 7370 6163 6520 616e  no whitespace an
-00000850: 6420 6265 2038 2d36 3420 6368 6172 6163  d be 8-64 charac
-00000860: 7465 7273 206c 6f6e 672e 7a0f 4f72 6761  ters long.z.Orga
-00000870: 6e69 7a61 7469 6f6e 2049 447a 3349 6e76  nization IDz3Inv
-00000880: 616c 6964 206f 7267 616e 697a 6174 696f  alid organizatio
-00000890: 6e20 4944 2e20 4974 2073 686f 756c 6420  n ID. It should 
-000008a0: 6265 2061 2076 616c 6964 2055 5549 442e  be a valid UUID.
-000008b0: 7a0a 5072 6f6a 6563 7420 4944 fa01 7e7a  z.Project ID..~z
-000008c0: 0a2e 7374 656c 6c61 6e6f 7729 01da 0865  ..stellanow)...e
-000008d0: 7869 7374 5f6f 6b7a 0a63 6f6e 6669 672e  xist_okz.config.
-000008e0: 696e 6929 0472 1500 0000 7217 0000 0072  ini).r....r....r
-000008f0: 1800 0000 7219 0000 00da 0365 6e76 da01  ....r......env..
-00000900: 777a 1b43 6f6e 6669 6775 7261 7469 6f6e  wz.Configuration
-00000910: 2066 6f72 2070 726f 6669 6c65 2027 7a14   for profile 'z.
-00000920: 2720 7361 7665 6420 7375 6363 6573 7366  ' saved successf
-00000930: 756c 6c79 2915 da05 7072 696e 74da 036f  ully)...print..o
-00000940: 626a da03 6765 74da 0563 6c69 636b 720a  bj..get..clickr.
-00000950: 0000 00da 0272 65da 056d 6174 6368 7204  .....re..matchr.
-00000960: 0000 00da 0565 7272 6f72 7203 0000 00da  .....errorr.....
-00000970: 026f 73da 0470 6174 68da 0a65 7870 616e  .os..path..expan
-00000980: 6475 7365 72da 086d 616b 6564 6972 73da  duser..makedirs.
-00000990: 046a 6f69 6eda 0c63 6f6e 6669 6770 6172  .join..configpar
-000009a0: 7365 72da 0c43 6f6e 6669 6750 6172 7365  ser..ConfigParse
-000009b0: 72da 0665 7869 7374 73da 0472 6561 64da  r..exists..read.
-000009c0: 046f 7065 6eda 0577 7269 7465 290d da03  .open..write)...
-000009d0: 6374 785a 0770 726f 6669 6c65 721e 0000  ctxZ.profiler...
-000009e0: 00da 0663 6f6e 6669 6772 1500 0000 7217  ...configr....r.
-000009f0: 0000 0072 1800 0000 7219 0000 005a 0b65  ...r....r....Z.e
-00000a00: 6d61 696c 5f72 6567 6578 5a0c 7374 7269  mail_regexZ.stri
-00000a10: 6e67 5f72 6567 6578 da04 686f 6d65 5a0b  ng_regex..homeZ.
-00000a20: 636f 6e66 6967 5f66 696c 655a 0a63 6f6e  config_fileZ.con
-00000a30: 6669 6766 696c 6572 0c00 0000 720c 0000  figfiler....r...
-00000a40: 0072 1000 0000 7206 0000 0014 0000 0073  .r....r........s
-00000a50: 6200 0000 0e0a 0602 1002 1001 1001 1001  b...............
-00000a60: 0402 0401 0201 0e01 1801 0201 0a02 02fb  ................
-00000a70: 0208 1201 0c01 0201 0a02 02fb 0207 0e01  ................
-00000a80: 0801 0201 0a02 02fb 0207 0e01 0801 0201  ................
-00000a90: 0a02 02fb 0c08 1803 0803 1003 0c01 0a01  ................
-00000aa0: 0204 0201 0201 0201 0afc 0808 0c01 0c03  ................
-00000ab0: 0c01 1cff 1603 2910 da07 5f5f 646f 635f  ......)...__doc_
-00000ac0: 5f72 2300 0000 722c 0000 0072 2700 0000  _r#...r,...r'...
-00000ad0: 7224 0000 00da 0876 616c 6964 6174 6572  r$.....validater
-00000ae0: 0300 0000 7204 0000 0072 3300 0000 7205  ....r....r3...r.
-00000af0: 0000 00da 0763 6f6d 6d61 6e64 da06 6f70  .....command..op
-00000b00: 7469 6f6e da06 4368 6f69 6365 da0c 7061  tion..Choice..pa
-00000b10: 7373 5f63 6f6e 7465 7874 7206 0000 00da  ss_contextr.....
-00000b20: 0d63 6f6e 6669 6775 7265 5f63 6d64 720c  .configure_cmdr.
-00000b30: 0000 0072 0c00 0000 720c 0000 0072 1000  ...r....r....r..
-00000b40: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000b50: 7320 0000 0004 0008 0908 0108 0108 010c  s ..............
-00000b60: 020c 010c 010a 030a 0102 0104 ff22 0304  ............."..
-00000b70: 0110 0108 4d                             ....M
+00000230: 0345 6e76 da09 636f 6e66 6967 7572 6529  .Env..configure)
+00000240: 01da 046e 616d 657a 092d 2d70 726f 6669  ...namez.--profi
+00000250: 6c65 da07 4445 4641 554c 5446 7a9b 5468  le..DEFAULTFz.Th
+00000260: 6520 7072 6f66 696c 6520 6e61 6d65 2066  e profile name f
+00000270: 6f72 2073 746f 7269 6e67 2061 2070 6172  or storing a par
+00000280: 7469 6375 6c61 7220 7365 7420 6f66 2063  ticular set of c
+00000290: 6f6e 6669 6775 7261 7469 6f6e 732e 2049  onfigurations. I
+000002a0: 6620 6e6f 2070 726f 6669 6c65 2069 7320  f no profile is 
+000002b0: 7370 6563 6966 6965 642c 2074 6865 2063  specified, the c
+000002c0: 6f6e 6669 6775 7261 7469 6f6e 7320 7769  onfigurations wi
+000002d0: 6c6c 2062 6520 7374 6f72 6564 2075 6e64  ll be stored und
+000002e0: 6572 2074 6865 2027 4445 4641 554c 5427  er the 'DEFAULT'
+000002f0: 2070 726f 6669 6c65 2e29 03da 0764 6566   profile.)...def
+00000300: 6175 6c74 da06 7072 6f6d 7074 da04 6865  ault..prompt..he
+00000310: 6c70 7a05 2d2d 656e 7654 6301 0000 0000  lpz.--envTc.....
+00000320: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000330: 0000 0073 1200 0000 6700 7c00 5d05 7d01  ...s....g.|.].}.
+00000340: 7c01 6a00 9102 7102 5300 a900 2901 da05  |.j...q.S...)...
+00000350: 7661 6c75 6529 02da 022e 30da 0165 720c  value)....0..er.
+00000360: 0000 0072 0c00 0000 fa60 2f55 7365 7273  ...r.....`/Users
+00000370: 2f74 6f6d 2d6b 616e 647a 696f 7261 2f44  /tom-kandziora/D
+00000380: 6576 4c6f 6361 6c2f 7374 656c 6c61 2f73  evLocal/stella/s
+00000390: 7465 6c6c 612d 6e6f 772f 5374 656c 6c61  tella-now/Stella
+000003a0: 4e6f 7743 4c49 2f73 7465 6c6c 616e 6f77  NowCLI/stellanow
+000003b0: 5f63 6c69 2f63 6f6d 6d61 6e64 732f 636f  _cli/commands/co
+000003c0: 6e66 6967 7572 652e 7079 da0a 3c6c 6973  nfigure.py..<lis
+000003d0: 7463 6f6d 703e 1700 0000 7302 0000 0012  tcomp>....s.....
+000003e0: 0072 1100 0000 2901 da0e 6361 7365 5f73  .r....)...case_s
+000003f0: 656e 7369 7469 7665 2902 da06 6869 6464  ensitive)...hidd
+00000400: 656e da04 7479 7065 6303 0000 0000 0000  en..typec.......
+00000410: 0000 0000 000d 0000 0008 0000 0043 0000  .............C..
+00000420: 0073 ce01 0000 7400 6401 7c01 9b00 9d02  .s....t.d.|.....
+00000430: 8301 0100 7c00 6a01 7d03 7c03 6a02 7c01  ....|.j.}.|.j.|.
+00000440: 6402 6403 6404 8d03 7d04 7c03 6a02 7c01  d.d.d...}.|.j.|.
+00000450: 6405 6403 6404 8d03 7d05 7c03 6a02 7c01  d.d.d...}.|.j.|.
+00000460: 6406 6403 6404 8d03 7d06 7c03 6a02 7c01  d.d.d...}.|.j.|.
+00000470: 6407 6403 6404 8d03 7d07 6408 7d08 6409  d.d.d...}.d.}.d.
+00000480: 7d09 0900 7403 6a04 640b 7c04 640c 8d02  }...t.j.d.|.d...
+00000490: 7d04 7405 a006 7c08 7c04 a102 7342 7405  }.t...|.|...sBt.
+000004a0: a006 7c09 7c04 a102 7243 6e06 7407 a008  ..|.|...rCn.t...
+000004b0: 640d a101 0100 712f 0900 7403 6a04 640e  d.....q/..t.j.d.
+000004c0: 640a 7c05 640f 6410 8d04 7d05 7405 a006  d.|.d.d...}.t...
+000004d0: 6411 7c05 a102 725a 6e06 7407 a008 6412  d.|...rZn.t...d.
+000004e0: a101 0100 714a 0900 7403 6a04 6413 7c06  ....qJ..t.j.d.|.
+000004f0: 640c 8d02 7d06 7409 7c06 8301 726d 6e06  d...}.t.|...rmn.
+00000500: 7407 a008 6414 a101 0100 7161 0900 7403  t...d.....qa..t.
+00000510: 6a04 6415 7c07 640c 8d02 7d07 7409 7c07  j.d.|.d...}.t.|.
+00000520: 8301 7280 6e06 7407 a008 6414 a101 0100  ..r.n.t...d.....
+00000530: 7174 740a 6a0b a00c 6416 a101 7d0a 740a  qtt.j...d...}.t.
+00000540: 6a0d 740a 6a0b a00e 7c0a 6417 a102 640a  j.t.j...|.d...d.
+00000550: 6418 8d02 0100 740f a010 a100 7d03 740a  d.....t.....}.t.
+00000560: 6a0b a00e 7c0a 6417 6419 a103 7d0b 740a  j...|.d.d...}.t.
+00000570: 6a0b a011 7c0b a101 72af 7c03 a012 7c0b  j...|...r.|...|.
+00000580: a101 0100 7c04 7c05 7c06 7c07 641a 9c04  ....|.|.|.|.d...
+00000590: 7c03 7c01 3c00 7c02 6403 7501 72c2 7c02  |.|.<.|.d.u.r.|.
+000005a0: 7c03 7c01 1900 641b 3c00 7413 7c0b 641c  |.|...d.<.t.|.d.
+000005b0: 8302 8f0d 7d0c 7c03 a014 7c0c a101 0100  ....}.|...|.....
+000005c0: 5700 6403 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+000005d0: 73d7 7701 0100 0100 0100 5900 0100 7407  s.w.......Y...t.
+000005e0: a008 641d 7c01 9b00 641e 9d03 a101 0100  ..d.|...d.......
+000005f0: 6403 5300 291f 7a80 5365 7473 2075 7020  d.S.).z.Sets up 
+00000600: 7468 6520 6e65 6365 7373 6172 7920 6372  the necessary cr
+00000610: 6564 656e 7469 616c 7320 616e 6420 636f  edentials and co
+00000620: 6e66 6967 7572 6174 696f 6e73 2066 6f72  nfigurations for
+00000630: 2061 2073 7065 6369 6669 6320 7072 6f66   a specific prof
+00000640: 696c 6520 6f72 2066 6f72 2074 6865 2044  ile or for the D
+00000650: 4546 4155 4c54 2070 726f 6669 6c65 2069  EFAULT profile i
+00000660: 6620 6e6f 6e65 0a20 2020 2069 7320 7370  f none.    is sp
+00000670: 6563 6966 6965 642e 7a23 5072 6f76 6964  ecified.z#Provid
+00000680: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00000690: 666f 7220 7072 6f66 696c 653a 20da 0a61  for profile: ..a
+000006a0: 6363 6573 735f 6b65 794e 2901 da08 6661  ccess_keyN)...fa
+000006b0: 6c6c 6261 636b da0c 6163 6365 7373 5f74  llback..access_t
+000006c0: 6f6b 656e da0f 6f72 6761 6e69 7a61 7469  oken..organizati
+000006d0: 6f6e 5f69 64da 0a70 726f 6a65 6374 5f69  on_id..project_i
+000006e0: 647a 335c 625b 412d 5a61 2d7a 302d 392e  dz3\b[A-Za-z0-9.
+000006f0: 5f25 2b2d 5d2b 405b 412d 5a61 2d7a 302d  _%+-]+@[A-Za-z0-
+00000700: 392e 2d5d 2b5c 2e5b 412d 5a7c 612d 7a5d  9.-]+\.[A-Z|a-z]
+00000710: 7b32 2c7d 5c62 7a10 5e5b 612d 7a41 2d5a  {2,}\bz.^[a-zA-Z
+00000720: 302d 395f 2d5d 2b24 547a 0a41 6363 6573  0-9_-]+$Tz.Acces
+00000730: 7320 4b65 7929 0172 0900 0000 7a8b 496e  s Key).r....z.In
+00000740: 7661 6c69 6420 6163 6365 7373 206b 6579  valid access key
+00000750: 2066 6f72 6d61 742e 2049 7420 7368 6f75   format. It shou
+00000760: 6c64 2062 6520 6120 7661 6c69 6420 656d  ld be a valid em
+00000770: 6169 6c20 6164 6472 6573 7320 6f72 2061  ail address or a
+00000780: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
+00000790: 6e67 206f 6e6c 7920 616c 7068 616e 756d  ng only alphanum
+000007a0: 6572 6963 2063 6861 7261 6374 6572 732c  eric characters,
+000007b0: 2064 6173 6865 732c 2061 6e64 2075 6e64   dashes, and und
+000007c0: 6572 7363 6f72 6573 2e7a 0c41 6363 6573  erscores.z.Acces
+000007d0: 7320 546f 6b65 6e46 2903 da0a 6869 6465  s TokenF)...hide
+000007e0: 5f69 6e70 7574 7209 0000 00da 0c73 686f  _inputr......sho
+000007f0: 775f 6465 6661 756c 747a 0a5e 5c53 7b38  w_defaultz.^\S{8
+00000800: 2c36 347d 247a 5949 6e76 616c 6964 2061  ,64}$zYInvalid a
+00000810: 6363 6573 7320 746f 6b65 6e20 666f 726d  ccess token form
+00000820: 6174 2e20 4974 2073 686f 756c 6420 636f  at. It should co
+00000830: 6e74 6169 6e20 6e6f 2077 6869 7465 7370  ntain no whitesp
+00000840: 6163 6520 616e 6420 6265 2038 2d36 3420  ace and be 8-64 
+00000850: 6368 6172 6163 7465 7273 206c 6f6e 672e  characters long.
+00000860: 7a0f 4f72 6761 6e69 7a61 7469 6f6e 2049  z.Organization I
+00000870: 447a 3349 6e76 616c 6964 206f 7267 616e  Dz3Invalid organ
+00000880: 697a 6174 696f 6e20 4944 2e20 4974 2073  ization ID. It s
+00000890: 686f 756c 6420 6265 2061 2076 616c 6964  hould be a valid
+000008a0: 2055 5549 442e 7a0a 5072 6f6a 6563 7420   UUID.z.Project 
+000008b0: 4944 fa01 7e7a 0a2e 7374 656c 6c61 6e6f  ID..~z..stellano
+000008c0: 7729 01da 0865 7869 7374 5f6f 6b7a 0a63  w)...exist_okz.c
+000008d0: 6f6e 6669 672e 696e 6929 0472 1500 0000  onfig.ini).r....
+000008e0: 7217 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000008f0: 0365 6e76 da01 777a 1b43 6f6e 6669 6775  .env..wz.Configu
+00000900: 7261 7469 6f6e 2066 6f72 2070 726f 6669  ration for profi
+00000910: 6c65 2027 7a14 2720 7361 7665 6420 7375  le 'z.' saved su
+00000920: 6363 6573 7366 756c 6c79 2915 da05 7072  ccessfully)...pr
+00000930: 696e 74da 036f 626a da03 6765 74da 0563  int..obj..get..c
+00000940: 6c69 636b 720a 0000 00da 0272 65da 056d  lickr......re..m
+00000950: 6174 6368 7203 0000 00da 0565 7272 6f72  atchr......error
+00000960: 7204 0000 00da 026f 73da 0470 6174 68da  r......os..path.
+00000970: 0a65 7870 616e 6475 7365 72da 086d 616b  .expanduser..mak
+00000980: 6564 6972 73da 046a 6f69 6eda 0c63 6f6e  edirs..join..con
+00000990: 6669 6770 6172 7365 72da 0c43 6f6e 6669  figparser..Confi
+000009a0: 6750 6172 7365 72da 0665 7869 7374 73da  gParser..exists.
+000009b0: 0472 6561 64da 046f 7065 6eda 0577 7269  .read..open..wri
+000009c0: 7465 290d da03 6374 785a 0770 726f 6669  te)...ctxZ.profi
+000009d0: 6c65 721e 0000 00da 0663 6f6e 6669 6772  ler......configr
+000009e0: 1500 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+000009f0: 0000 005a 0b65 6d61 696c 5f72 6567 6578  ...Z.email_regex
+00000a00: 5a0c 7374 7269 6e67 5f72 6567 6578 da04  Z.string_regex..
+00000a10: 686f 6d65 5a0b 636f 6e66 6967 5f66 696c  homeZ.config_fil
+00000a20: 655a 0a63 6f6e 6669 6766 696c 6572 0c00  eZ.configfiler..
+00000a30: 0000 720c 0000 0072 1000 0000 7206 0000  ..r....r....r...
+00000a40: 0013 0000 0073 6200 0000 0e0a 0602 1002  .....sb.........
+00000a50: 1001 1001 1001 0402 0401 0201 0e01 1801  ................
+00000a60: 0201 0a02 02fb 0208 1201 0c01 0201 0a02  ................
+00000a70: 02fb 0207 0e01 0801 0201 0a02 02fb 0207  ................
+00000a80: 0e01 0801 0201 0a02 02fb 0c08 1803 0803  ................
+00000a90: 1003 0c01 0a01 0204 0201 0201 0201 0afc  ................
+00000aa0: 0808 0c01 0c03 0c01 1cff 1603 2910 da07  ............)...
+00000ab0: 5f5f 646f 635f 5f72 2300 0000 722c 0000  __doc__r#...r,..
+00000ac0: 0072 2700 0000 7224 0000 00da 0575 7469  .r'...r$.....uti
+00000ad0: 6c73 7203 0000 0072 0400 0000 7233 0000  lsr....r....r3..
+00000ae0: 0072 0500 0000 da07 636f 6d6d 616e 64da  .r......command.
+00000af0: 066f 7074 696f 6eda 0643 686f 6963 65da  .option..Choice.
+00000b00: 0c70 6173 735f 636f 6e74 6578 7472 0600  .pass_contextr..
+00000b10: 0000 da0d 636f 6e66 6967 7572 655f 636d  ....configure_cm
+00000b20: 6472 0c00 0000 720c 0000 0072 0c00 0000  dr....r....r....
+00000b30: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000b40: 0000 0073 1e00 0000 0400 0809 0801 0801  ...s............
+00000b50: 0801 1002 0c01 0a03 0a01 0201 04ff 2203  ..............".
+00000b60: 0401 1001 084d                           .....M
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/events.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/events.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:53:53 2023 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 617a 8b64 c804 0000  o.......az.d....
+00000000: 6f0d 0d0a 0000 0000 9ea7 8d64 c704 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6501 6a07 6406 6407 8d01  m.Z...e.j.d.d...
 00000060: 6505 6506 6501 6a08 6408 6406 8400 8301  e.e.e.j.d.d.....
 00000070: 8301 8301 8301 5a09 6509 5a0a 6402 5300  ......Z.e.Z.d.S.
@@ -23,15 +23,15 @@
 00000160: 6420 7769 7468 6f75 740a 7468 6520 6578  d without.the ex
 00000170: 7072 6573 7320 7772 6974 7465 6e20 7065  press written pe
 00000180: 726d 6973 7369 6f6e 206f 6620 5374 656c  rmission of Stel
 00000190: 6c61 2054 6563 686e 6f6c 6f67 6965 7320  la Technologies 
 000001a0: 2855 4b29 204c 696d 6974 6564 2e0a 416c  (UK) Limited..Al
 000001b0: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
 000001c0: 642e 0ae9 0000 0000 4e29 01da 0b50 7265  d.......N)...Pre
-000001d0: 7474 7954 6162 6c65 e902 0000 0029 02da  ttyTable.....)..
+000001d0: 7474 7954 6162 6c65 e901 0000 0029 02da  ttyTable.....)..
 000001e0: 0d63 6f6d 6d6f 6e5f 6f70 7469 6f6e da0b  .common_option..
 000001f0: 6c6f 6164 5f63 6f6e 6669 67da 0665 7665  load_config..eve
 00000200: 6e74 7329 01da 046e 616d 6563 0400 0000  nts)...namec....
 00000210: 0000 0000 0000 0000 0800 0000 0800 0000  ................
 00000220: 4b00 0000 7380 0000 0074 0064 017c 029b  K...s....t.d.|..
 00000230: 0064 027c 039b 0064 039d 0583 0101 007c  .d.|...d.......|
 00000240: 01a0 01a1 007d 0574 0267 0064 04a2 0183  .....}.t.g.d....
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/commands/__pycache__/plan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:53:23 2023 UTC, .py size: 4091 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,218 +1,233 @@
-00000000: 6f0d 0d0a 0000 0000 437a 8b64 fb0f 0000  o.......Cz.d....
+00000000: 6f0d 0d0a 0000 0000 d481 9064 3011 0000  o..........d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6401 6403 6c05 6d06 5a06 0100 6401  Z.d.d.l.m.Z...d.
-00000060: 6404 6c07 6d08 5a08 0100 6405 6406 6c09  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 6d0b 5a0b 0100 6405 6407 6c0c  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 0100 6405 6408 6c0e 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000090: 0100 4700 6409 640a 8400 640a 8302 5a0f  ..G.d.d...d...Z.
-000000a0: 640b 6508 650f 1900 640c 6402 6604 640d  d.e.e...d.d.f.d.
-000000b0: 640e 8404 5a10 6504 6a11 640f 6410 8d01  d...Z.e.j.d.d...
-000000c0: 650a 650b 6504 6a12 6411 6412 6413 6414  e.e.e.j.d.d.d.d.
-000000d0: 6415 8d04 6504 6a13 6416 640f 8400 8301  d...e.j.d.d.....
-000000e0: 8301 8301 8301 8301 5a14 6514 5a15 6402  ........Z.e.Z.d.
-000000f0: 5300 2917 613c 0100 000a 436f 7079 7269  S.).a<....Copyri
-00000100: 6768 7420 2843 2920 3230 3232 2d32 3032  ght (C) 2022-202
-00000110: 3320 5374 656c 6c61 2054 6563 686e 6f6c  3 Stella Technol
-00000120: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
-00000130: 6564 2e0a 0a54 6869 7320 736f 6674 7761  ed...This softwa
-00000140: 7265 2069 7320 7468 6520 7072 6f70 7269  re is the propri
-00000150: 6574 6172 7920 696e 666f 726d 6174 696f  etary informatio
-00000160: 6e20 6f66 2053 7465 6c6c 6120 5465 6368  n of Stella Tech
-00000170: 6e6f 6c6f 6769 6573 2028 554b 2920 4c69  nologies (UK) Li
-00000180: 6d69 7465 642e 0a55 7365 2c20 7265 7072  mited..Use, repr
-00000190: 6f64 7563 7469 6f6e 2c20 6f72 2072 6564  oduction, or red
-000001a0: 6973 7472 6962 7574 696f 6e20 6f66 2074  istribution of t
-000001b0: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
-000001c0: 7374 7269 6374 6c79 2070 726f 6869 6269  strictly prohibi
-000001d0: 7465 6420 7769 7468 6f75 740a 7468 6520  ted without.the 
-000001e0: 6578 7072 6573 7320 7772 6974 7465 6e20  express written 
-000001f0: 7065 726d 6973 7369 6f6e 206f 6620 5374  permission of St
-00000200: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-00000210: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-00000220: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
-00000230: 7665 642e 0ae9 0000 0000 4e29 01da 0b50  ved.......N)...P
-00000240: 7265 7474 7954 6162 6c65 2901 da04 4c69  rettyTable)...Li
-00000250: 7374 e902 0000 0029 02da 0d63 6f6d 6d6f  st.....)...commo
-00000260: 6e5f 6f70 7469 6f6e da0b 6c6f 6164 5f63  n_option..load_c
-00000270: 6f6e 6669 6729 01da 1343 7368 6172 7043  onfig)...CsharpC
-00000280: 6f64 6547 656e 6572 6174 6f72 2901 da06  odeGenerator)...
-00000290: 6c6f 6767 6572 6300 0000 0000 0000 0000  loggerc.........
-000002a0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-000002b0: 2600 0000 6500 5a01 6400 5a02 6401 6503  &...e.Z.d.Z.d.e.
-000002c0: 6402 6503 6604 6403 6404 8404 5a04 6405  d.e.f.d.d...Z.d.
-000002d0: 6406 8400 5a05 6407 5300 2908 da0b 536b  d...Z.d.S.)...Sk
-000002e0: 6970 7065 6446 696c 65da 0866 696c 656e  ippedFile..filen
-000002f0: 616d 65da 0672 6561 736f 6e63 0300 0000  ame..reasonc....
-00000300: 0000 0000 0000 0000 0300 0000 0200 0000  ................
-00000310: 4300 0000 7310 0000 007c 017c 005f 007c  C...s....|.|._.|
-00000320: 027c 005f 0164 0053 00a9 014e 2902 720a  .|._.d.S...N).r.
-00000330: 0000 0072 0b00 0000 2903 da04 7365 6c66  ...r....)...self
-00000340: 720a 0000 0072 0b00 0000 a900 720e 0000  r....r......r...
-00000350: 00fa 5b2f 5573 6572 732f 746f 6d2d 6b61  ..[/Users/tom-ka
-00000360: 6e64 7a69 6f72 612f 4465 764c 6f63 616c  ndziora/DevLocal
-00000370: 2f73 7465 6c6c 612f 7374 656c 6c61 2d6e  /stella/stella-n
-00000380: 6f77 2f53 7465 6c6c 614e 6f77 434c 492f  ow/StellaNowCLI/
-00000390: 7374 656c 6c61 6e6f 775f 636c 692f 636f  stellanow_cli/co
-000003a0: 6d6d 616e 6473 2f70 6c61 6e2e 7079 da08  mmands/plan.py..
-000003b0: 5f5f 696e 6974 5f5f 1800 0000 7304 0000  __init__....s...
-000003c0: 0006 010a 017a 1453 6b69 7070 6564 4669  .....z.SkippedFi
-000003d0: 6c65 2e5f 5f69 6e69 745f 5f63 0100 0000  le.__init__c....
-000003e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000003f0: 4300 0000 7310 0000 0074 007c 006a 017c  C...s....t.|.j.|
-00000400: 006a 0267 0283 0153 0072 0c00 0000 2903  .j.g...S.r....).
-00000410: da04 6974 6572 720a 0000 0072 0b00 0000  ..iterr....r....
-00000420: 2901 720d 0000 0072 0e00 0000 720e 0000  ).r....r....r...
-00000430: 0072 0f00 0000 da08 5f5f 6974 6572 5f5f  .r......__iter__
-00000440: 1c00 0000 7302 0000 0010 017a 1453 6b69  ....s......z.Ski
-00000450: 7070 6564 4669 6c65 2e5f 5f69 7465 725f  ppedFile.__iter_
-00000460: 5f4e 2906 da08 5f5f 6e61 6d65 5f5f da0a  _N)...__name__..
-00000470: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000480: 616c 6e61 6d65 5f5f da03 7374 7272 1000  alname__..strr..
-00000490: 0000 7212 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-000004a0: 0072 0e00 0000 720f 0000 0072 0900 0000  .r....r....r....
-000004b0: 1700 0000 7306 0000 0008 0012 010c 0472  ....s..........r
-000004c0: 0900 0000 da0d 736b 6970 7065 645f 6669  ......skipped_fi
-000004d0: 6c65 73da 0672 6574 7572 6e63 0100 0000  les..returnc....
-000004e0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-000004f0: 4300 0000 7344 0000 007c 0072 2074 0064  C...sD...|.r t.d
-00000500: 0183 0101 0074 0164 0264 0367 0283 017d  .....t.d.d.g...}
-00000510: 017c 0044 005d 0b7d 027c 01a0 027c 026a  .|.D.].}.|...|.j
-00000520: 037c 026a 0467 02a1 0101 0071 0e74 007c  .|.j.g.....q.t.|
-00000530: 0183 0101 0064 0053 0064 0053 0029 044e  .....d.S.d.S.).N
-00000540: 7a50 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  zP.=============
-00000550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000560: 3d0a 2020 2020 2020 2020 2053 554d 4d41  =.         SUMMA
-00000570: 5259 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  RY.=============
-00000580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000590: 3d0a da04 4669 6c65 7a18 5265 6173 6f6e  =...Filez.Reason
-000005a0: 2066 6f72 206e 6f74 2063 6f6d 7061 7269   for not compari
-000005b0: 6e67 2905 da05 7072 696e 7472 0200 0000  ng)...printr....
-000005c0: 5a07 6164 645f 726f 7772 0a00 0000 720b  Z.add_rowr....r.
-000005d0: 0000 0029 0372 1700 0000 da05 7461 626c  ...).r......tabl
-000005e0: 655a 0c73 6b69 7070 6564 5f66 696c 6572  eZ.skipped_filer
-000005f0: 0e00 0000 720e 0000 0072 0f00 0000 da0d  ....r....r......
-00000600: 7072 696e 745f 7375 6d6d 6172 7920 0000  print_summary ..
-00000610: 0073 0e00 0000 0401 0801 0c02 0803 1401  .s..............
-00000620: 0c02 04f7 721c 0000 00da 0470 6c61 6e29  ....r......plan)
-00000630: 01da 046e 616d 657a 0b2d 2d69 6e70 7574  ...namez.--input
-00000640: 5f64 6972 7a02 2d69 da01 2e7a 2d54 6865  _dirz.-i...z-The
-00000650: 2064 6972 6563 746f 7279 2074 6f20 7265   directory to re
-00000660: 6164 2067 656e 6572 6174 6564 2063 6c61  ad generated cla
-00000670: 7373 6573 2066 726f 6d2e 2902 da07 6465  sses from.)...de
-00000680: 6661 756c 74da 0468 656c 7063 0300 0000  fault..helpc....
-00000690: 0000 0000 0000 0000 1200 0000 0b00 0000  ................
-000006a0: 4b00 0000 73be 0100 0074 0064 0183 0101  K...s....t.d....
-000006b0: 0064 0274 0183 0069 017d 0464 037d 0567  .d.t...i.}.d.}.g
-000006c0: 007d 0674 026a 037c 029b 0064 049d 0264  .}.t.j.|...d...d
-000006d0: 0564 068d 0244 005d c17d 0774 046a 05a0  .d...D.].}.t.j..
-000006e0: 067c 07a1 0172 2071 1774 0064 077c 079b  .|...r q.t.d.|..
-000006f0: 009d 0283 0101 0074 046a 05a0 077c 07a1  .......t.j...|..
-00000700: 015c 027d 087d 097c 04a0 087c 09a1 017d  .\.}.}.|...|...}
-00000710: 0a7c 0a72 c474 097c 0764 0883 028f 0c7d  .|.r.t.|.d.....}
-00000720: 0b7c 0ba0 0aa1 007d 0c57 0064 0904 0004  .|.....}.W.d....
-00000730: 0083 0301 006e 0831 0073 4a77 0101 0001  .....n.1.sJw....
-00000740: 0001 0059 0001 007c 057c 0c76 0172 6574  ...Y...|.|.v.ret
-00000750: 0ba0 0c64 0a7c 079b 0064 0b9d 03a1 0101  ...d.|...d......
-00000760: 007c 06a0 0d74 0e7c 0764 0c83 02a1 0101  .|...t.|.d......
-00000770: 0071 1774 0fa0 1064 0d7c 0ca1 027d 0d7c  .q.t...d.|...}.|
-00000780: 0d64 0975 0072 8174 0ba0 0c64 0a7c 079b  .d.u.r.t...d.|..
-00000790: 0064 0e9d 03a1 0101 007c 06a0 0d74 0e7c  .d.......|...t.|
-000007a0: 0764 0f83 02a1 0101 0071 177c 0da0 1164  .d.......q.|...d
-000007b0: 10a1 017d 0e7c 01a0 127c 0ea1 017d 0f7a  ...}.|...|...}.z
-000007c0: 0f74 01a0 137c 0f7c 0ca1 027d 1074 0064  .t...|.|...}.t.d
-000007d0: 11a0 147c 10a1 0183 0101 0057 006e 2104  ...|.......W.n!.
-000007e0: 0074 1579 bb01 007d 1101 007a 1574 0ba0  .t.y...}...z.t..
-000007f0: 0c74 167c 1183 01a1 0101 007c 06a0 0d74  .t.|.......|...t
-00000800: 0e7c 0764 1283 02a1 0101 0057 0059 0064  .|.d.......W.Y.d
-00000810: 097d 117e 1171 1764 097d 117e 1177 0177  .}.~.q.d.}.~.w.w
-00000820: 0074 0064 137c 079b 009d 0283 0101 0071  .t.d.|.........q
-00000830: 1774 0ba0 1764 147c 099b 0064 157c 079b  .t...d.|...d.|..
-00000840: 0064 169d 05a1 0101 007c 06a0 0d74 0e7c  .d.......|...t.|
-00000850: 0764 1783 02a1 0101 0071 1774 187c 0683  .d.......q.t.|..
-00000860: 0101 0064 0953 0029 187a 7843 6f6d 7061  ...d.S.).zxCompa
-00000870: 7265 7320 6375 7272 656e 746c 7920 6765  res currently ge
-00000880: 6e65 7261 7465 6420 636c 6173 7365 7320  nerated classes 
-00000890: 7769 7468 2074 6865 2073 7065 6369 6669  with the specifi
-000008a0: 6361 7469 6f6e 7320 6665 7463 6865 6420  cations fetched 
-000008b0: 6672 6f6d 2074 6865 2041 5049 2061 6e64  from the API and
-000008c0: 2070 726f 7669 6465 7320 6120 7375 6d6d   provides a summ
-000008d0: 6172 7920 6f66 0a20 2020 2063 6861 6e67  ary of.    chang
-000008e0: 6573 2e7a 0b50 6c61 6e6e 696e 672e 2e2e  es.z.Planning...
-000008f0: 7a03 2e63 737a 3954 6869 7320 6669 6c65  z..csz9This file
-00000900: 2069 7320 6175 746f 2d67 656e 6572 6174   is auto-generat
-00000910: 6564 2062 7920 5374 656c 6c61 4e6f 7743  ed by StellaNowC
-00000920: 4c49 2e20 444f 204e 4f54 2045 4449 542e  LI. DO NOT EDIT.
-00000930: 7a03 2f2a 2a54 2901 da09 7265 6375 7273  z./**T)...recurs
-00000940: 6976 657a 353d 3d3d 3d3d 3d3d 3d3d 3d3d  ivez5===========
-00000950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000960: 3d3d 3d0a 0a43 6f6d 7061 7269 736f 6e20  ===..Comparison 
-00000970: 666f 7220 6669 6c65 3a20 da01 724e 7a09  for file: ..rNz.
-00000980: 536b 6970 7069 6e67 207a 2320 6265 6361  Skipping z# beca
-00000990: 7573 6520 6974 2077 6173 206e 6f74 2061  use it was not a
-000009a0: 7574 6f2d 6765 6e65 7261 7465 642e 7a12  uto-generated.z.
-000009b0: 4e6f 7420 4175 746f 2d47 656e 6572 6174  Not Auto-Generat
-000009c0: 6564 7a57 4576 656e 7420 4944 3a20 285b  edzWEvent ID: ([
-000009d0: 302d 3961 2d66 412d 465d 7b38 7d2d 5b30  0-9a-fA-F]{8}-[0
-000009e0: 2d39 612d 6641 2d46 5d7b 347d 2d5b 302d  -9a-fA-F]{4}-[0-
-000009f0: 3961 2d66 412d 465d 7b34 7d2d 5b30 2d39  9a-fA-F]{4}-[0-9
-00000a00: 612d 6641 2d46 5d7b 347d 2d5b 302d 3961  a-fA-F]{4}-[0-9a
-00000a10: 2d66 412d 465d 7b31 327d 297a 1f20 6265  -fA-F]{12})z. be
-00000a20: 6361 7573 6520 6e6f 2045 7665 6e74 2049  cause no Event I
-00000a30: 4420 7761 7320 666f 756e 642e 7a12 4576  D was found.z.Ev
-00000a40: 656e 7420 4944 204e 6f74 2046 6f75 6e64  ent ID Not Found
-00000a50: e901 0000 00da 007a 0673 7472 2865 297a  .......z.str(e)z
-00000a60: 1d4e 6f20 6368 616e 6765 7320 6465 7465  .No changes dete
-00000a70: 6374 6564 2069 6e20 6669 6c65 3a20 7a21  cted in file: z!
-00000a80: 4e6f 2067 656e 6572 6174 6f72 2066 6f75  No generator fou
-00000a90: 6e64 2066 6f72 2066 696c 6520 7479 7065  nd for file type
-00000aa0: 207a 0b2e 2053 6b69 7070 696e 6720 721f   z.. Skipping r.
-00000ab0: 0000 007a 1455 6e73 7570 706f 7274 6564  ...z.Unsupported
-00000ac0: 204c 616e 6775 6167 6529 1972 1a00 0000   Language).r....
-00000ad0: 7207 0000 00da 0467 6c6f 625a 0569 676c  r......globZ.igl
-00000ae0: 6f62 da02 6f73 da04 7061 7468 da05 6973  ob..os..path..is
-00000af0: 6469 72da 0873 706c 6974 6578 74da 0367  dir..splitext..g
-00000b00: 6574 da04 6f70 656e da04 7265 6164 7208  et..open..readr.
-00000b10: 0000 00da 0777 6172 6e69 6e67 da06 6170  .....warning..ap
-00000b20: 7065 6e64 7209 0000 00da 0272 65da 0673  pendr......re..s
-00000b30: 6561 7263 68da 0567 726f 7570 da11 6765  earch..group..ge
-00000b40: 745f 6576 656e 745f 6465 7461 696c 73da  t_event_details.
-00000b50: 0867 6574 5f64 6966 66da 046a 6f69 6eda  .get_diff..join.
-00000b60: 0945 7863 6570 7469 6f6e 7216 0000 00da  .Exceptionr.....
-00000b70: 0565 7272 6f72 721c 0000 0029 12da 0363  .errorr....)...c
-00000b80: 7478 da0a 7374 656c 6c61 5f61 7069 5a09  tx..stella_apiZ.
-00000b90: 696e 7075 745f 6469 72da 066b 7761 7267  input_dir..kwarg
-00000ba0: 73da 0a67 656e 6572 6174 6f72 735a 1661  s..generatorsZ.a
-00000bb0: 7574 6f5f 6765 6e65 7261 7465 645f 636f  uto_generated_co
-00000bc0: 6d6d 656e 7472 1700 0000 720a 0000 00da  mmentr....r.....
-00000bd0: 015f da03 6578 74da 0967 656e 6572 6174  ._..ext..generat
-00000be0: 6f72 da01 66da 0d65 7869 7374 696e 675f  or..f..existing_
-00000bf0: 636f 6465 5a0f 6576 656e 745f 6964 5f73  codeZ.event_id_s
-00000c00: 6561 7263 68da 0865 7665 6e74 5f69 645a  earch..event_idZ
-00000c10: 0c65 7665 6e74 5f64 6574 6169 6cda 0464  .event_detail..d
-00000c20: 6966 66da 0165 720e 0000 0072 0e00 0000  iff..er....r....
-00000c30: 720f 0000 0072 1d00 0000 2d00 0000 7354  r....r....-...sT
-00000c40: 0000 0008 0806 0404 ff04 0504 0218 030c  ................
-00000c50: 0202 010e 0210 010a 0104 020c 010a 011c  ................
-00000c60: ff08 0412 0110 0102 0104 0302 0102 0104  ................
-00000c70: fe08 0412 0110 0102 010a 020a 0302 020c  ................
-00000c80: 0112 020e 010e 0110 010c 0108 8002 fd10  ................
-00000c90: 0518 0312 010c 0229 16da 075f 5f64 6f63  .......)...__doc
-00000ca0: 5f5f 7227 0000 0072 3000 0000 7226 0000  __r'...r0...r&..
-00000cb0: 00da 0563 6c69 636b 5a0b 7072 6574 7479  ...clickZ.pretty
-00000cc0: 7461 626c 6572 0200 0000 da06 7479 7069  tabler......typi
-00000cd0: 6e67 7203 0000 00da 0e63 6f6d 6d61 6e64  ngr......command
-00000ce0: 5f63 6f6e 6669 6772 0500 0000 7206 0000  _configr....r...
-00000cf0: 00da 0f63 6f64 655f 6765 6e65 7261 746f  ...code_generato
-00000d00: 7273 7207 0000 0072 0800 0000 7209 0000  rsr....r....r...
-00000d10: 0072 1c00 0000 da07 636f 6d6d 616e 64da  .r......command.
-00000d20: 066f 7074 696f 6eda 0c70 6173 735f 636f  .option..pass_co
-00000d30: 6e74 6578 7472 1d00 0000 da08 706c 616e  ntextr......plan
-00000d40: 5f63 6d64 720e 0000 0072 0e00 0000 720e  _cmdr....r....r.
-00000d50: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000d60: 653e 0100 0000 7326 0000 0004 0008 0908  e>....s&........
-00000d70: 0108 0108 010c 020c 0110 020c 010c 010e  ................
-00000d80: 0316 090a 0d02 0102 0110 0104 0112 0108  ................
-00000d90: 44                                       D
+00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
+00000060: 6d07 5a07 0100 6401 6404 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
+00000070: 0100 6405 6406 6c0a 6d0b 5a0b 6d0c 5a0c  ..d.d.l.m.Z.m.Z.
+00000080: 0100 6407 6408 6c0d 6d0e 5a0e 0100 6505  ..d.d.l.m.Z...e.
+00000090: a00f 6510 a101 5a11 4700 6409 640a 8400  ..e...Z.G.d.d...
+000000a0: 640a 8302 5a12 640b 6509 6512 1900 640c  d...Z.d.e.e...d.
+000000b0: 6402 6604 640d 640e 8404 5a13 6504 6a14  d.f.d.d...Z.e.j.
+000000c0: 640f 6410 8d01 650b 650c 6504 6a15 6411  d.d...e.e.e.j.d.
+000000d0: 6412 6413 6414 6415 8d04 6504 6a16 6416  d.d.d.d...e.j.d.
+000000e0: 640f 8400 8301 8301 8301 8301 8301 5a17  d.............Z.
+000000f0: 6517 5a18 6402 5300 2917 613c 0100 000a  e.Z.d.S.).a<....
+00000100: 436f 7079 7269 6768 7420 2843 2920 3230  Copyright (C) 20
+00000110: 3232 2d32 3032 3320 5374 656c 6c61 2054  22-2023 Stella T
+00000120: 6563 686e 6f6c 6f67 6965 7320 2855 4b29  echnologies (UK)
+00000130: 204c 696d 6974 6564 2e0a 0a54 6869 7320   Limited...This 
+00000140: 736f 6674 7761 7265 2069 7320 7468 6520  software is the 
+00000150: 7072 6f70 7269 6574 6172 7920 696e 666f  proprietary info
+00000160: 726d 6174 696f 6e20 6f66 2053 7465 6c6c  rmation of Stell
+00000170: 6120 5465 6368 6e6f 6c6f 6769 6573 2028  a Technologies (
+00000180: 554b 2920 4c69 6d69 7465 642e 0a55 7365  UK) Limited..Use
+00000190: 2c20 7265 7072 6f64 7563 7469 6f6e 2c20  , reproduction, 
+000001a0: 6f72 2072 6564 6973 7472 6962 7574 696f  or redistributio
+000001b0: 6e20 6f66 2074 6869 7320 736f 6674 7761  n of this softwa
+000001c0: 7265 2069 7320 7374 7269 6374 6c79 2070  re is strictly p
+000001d0: 726f 6869 6269 7465 6420 7769 7468 6f75  rohibited withou
+000001e0: 740a 7468 6520 6578 7072 6573 7320 7772  t.the express wr
+000001f0: 6974 7465 6e20 7065 726d 6973 7369 6f6e  itten permission
+00000200: 206f 6620 5374 656c 6c61 2054 6563 686e   of Stella Techn
+00000210: 6f6c 6f67 6965 7320 2855 4b29 204c 696d  ologies (UK) Lim
+00000220: 6974 6564 2e0a 416c 6c20 7269 6768 7473  ited..All rights
+00000230: 2072 6573 6572 7665 642e 0ae9 0000 0000   reserved.......
+00000240: 4e29 01da 0b50 7265 7474 7954 6162 6c65  N)...PrettyTable
+00000250: 2901 da04 4c69 7374 e901 0000 0029 02da  )...List.....)..
+00000260: 0d63 6f6d 6d6f 6e5f 6f70 7469 6f6e da0b  .common_option..
+00000270: 6c6f 6164 5f63 6f6e 6669 67e9 0200 0000  load_config.....
+00000280: 2901 da13 4373 6861 7270 436f 6465 4765  )...CsharpCodeGe
+00000290: 6e65 7261 746f 7263 0000 0000 0000 0000  neratorc........
+000002a0: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+000002b0: 7326 0000 0065 005a 0164 005a 0264 0165  s&...e.Z.d.Z.d.e
+000002c0: 0364 0265 0366 0464 0364 0484 045a 0464  .d.e.f.d.d...Z.d
+000002d0: 0564 0684 005a 0564 0753 0029 08da 0b53  .d...Z.d.S.)...S
+000002e0: 6b69 7070 6564 4669 6c65 da08 6669 6c65  kippedFile..file
+000002f0: 6e61 6d65 da06 7265 6173 6f6e 6303 0000  name..reasonc...
+00000300: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00000310: 0043 0000 0073 1000 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000320: 7c02 7c00 5f01 6400 5300 a901 4e29 0272  |.|._.d.S...N).r
+00000330: 0a00 0000 720b 0000 0029 03da 0473 656c  ....r....)...sel
+00000340: 6672 0a00 0000 720b 0000 00a9 0072 0e00  fr....r......r..
+00000350: 0000 fa5b 2f55 7365 7273 2f74 6f6d 2d6b  ...[/Users/tom-k
+00000360: 616e 647a 696f 7261 2f44 6576 4c6f 6361  andziora/DevLoca
+00000370: 6c2f 7374 656c 6c61 2f73 7465 6c6c 612d  l/stella/stella-
+00000380: 6e6f 772f 5374 656c 6c61 4e6f 7743 4c49  now/StellaNowCLI
+00000390: 2f73 7465 6c6c 616e 6f77 5f63 6c69 2f63  /stellanow_cli/c
+000003a0: 6f6d 6d61 6e64 732f 706c 616e 2e70 79da  ommands/plan.py.
+000003b0: 085f 5f69 6e69 745f 5f1b 0000 0073 0400  .__init__....s..
+000003c0: 0000 0601 0a01 7a14 536b 6970 7065 6446  ......z.SkippedF
+000003d0: 696c 652e 5f5f 696e 6974 5f5f 6301 0000  ile.__init__c...
+000003e0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000003f0: 0043 0000 0073 1000 0000 7400 7c00 6a01  .C...s....t.|.j.
+00000400: 7c00 6a02 6702 8301 5300 720c 0000 0029  |.j.g...S.r....)
+00000410: 03da 0469 7465 7272 0a00 0000 720b 0000  ...iterr....r...
+00000420: 0029 0172 0d00 0000 720e 0000 0072 0e00  .).r....r....r..
+00000430: 0000 720f 0000 00da 085f 5f69 7465 725f  ..r......__iter_
+00000440: 5f1f 0000 0073 0200 0000 1001 7a14 536b  _....s......z.Sk
+00000450: 6970 7065 6446 696c 652e 5f5f 6974 6572  ippedFile.__iter
+00000460: 5f5f 4e29 06da 085f 5f6e 616d 655f 5fda  __N)...__name__.
+00000470: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000480: 7561 6c6e 616d 655f 5fda 0373 7472 7210  ualname__..strr.
+00000490: 0000 0072 1200 0000 720e 0000 0072 0e00  ...r....r....r..
+000004a0: 0000 720e 0000 0072 0f00 0000 7209 0000  ..r....r....r...
+000004b0: 001a 0000 0073 0600 0000 0800 1201 0c04  .....s..........
+000004c0: 7209 0000 00da 0d73 6b69 7070 6564 5f66  r......skipped_f
+000004d0: 696c 6573 da06 7265 7475 726e 6301 0000  iles..returnc...
+000004e0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+000004f0: 0043 0000 0073 5c00 0000 7c00 722c 7400  .C...s\...|.r,t.
+00000500: 6401 8301 0100 7401 6402 6403 6702 8301  d.....t.d.d.g...
+00000510: 7d01 7c00 4400 5d0b 7d02 7c01 a002 7c02  }.|.D.].}.|...|.
+00000520: 6a03 7c02 6a04 6702 a101 0100 710e 7400  j.|.j.g.....q.t.
+00000530: 7c01 8301 0100 7400 6404 8301 0100 7400  |.....t.d.....t.
+00000540: 6405 8301 0100 7400 6406 8301 0100 6400  d.....t.d.....d.
+00000550: 5300 6400 5300 2907 4e7a 500a 3d3d 3d3d  S.d.S.).NzP.====
+00000560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000570: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020  ==========.     
+00000580: 2020 2020 5355 4d4d 4152 590a 3d3d 3d3d      SUMMARY.====
+00000590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000005a0: 3d3d 3d3d 3d3d 3d3d 3d3d 0ada 0446 696c  ==========...Fil
+000005b0: 657a 1852 6561 736f 6e20 666f 7220 6e6f  ez.Reason for no
+000005c0: 7420 636f 6d70 6172 696e 677a 1f0a 536b  t comparingz..Sk
+000005d0: 6970 7065 6420 5265 6173 6f6e 202d 2045  ipped Reason - E
+000005e0: 7870 6c61 6e61 7469 6f6e 3a0a 7a4c 2d20  xplanation:.zL- 
+000005f0: 4e6f 7420 4175 746f 2d47 656e 6572 6174  Not Auto-Generat
+00000600: 6564 202d 2049 7420 6c6f 6f6b 7320 6c69  ed - It looks li
+00000610: 6b65 2074 6865 2066 696c 6520 7761 7320  ke the file was 
+00000620: 6e6f 7420 6765 6e65 7261 7465 6420 6279  not generated by
+00000630: 2074 6869 7320 434c 492e 7a4c 2d20 4576   this CLI.zL- Ev
+00000640: 656e 7420 4944 204e 6f74 2046 6f75 6e64  ent ID Not Found
+00000650: 202d 2054 6865 2049 4420 6f66 2074 6865   - The ID of the
+00000660: 2065 7665 6e74 2069 7320 6d69 7373 696e   event is missin
+00000670: 6720 696e 2074 6865 2068 6561 6465 7220  g in the header 
+00000680: 636f 6d6d 656e 742e 2905 da05 7072 696e  comment.)...prin
+00000690: 7472 0200 0000 da07 6164 645f 726f 7772  tr......add_rowr
+000006a0: 0a00 0000 720b 0000 0029 0372 1700 0000  ....r....).r....
+000006b0: da05 7461 626c 65da 0c73 6b69 7070 6564  ..table..skipped
+000006c0: 5f66 696c 6572 0e00 0000 720e 0000 0072  _filer....r....r
+000006d0: 0f00 0000 da0d 7072 696e 745f 7375 6d6d  ......print_summ
+000006e0: 6172 7923 0000 0073 1400 0000 0401 0801  ary#...s........
+000006f0: 0c02 0803 1401 0802 0802 0801 0c01 04f3  ................
+00000700: 721e 0000 00da 0470 6c61 6e29 01da 046e  r......plan)...n
+00000710: 616d 657a 0b2d 2d69 6e70 7574 5f64 6972  amez.--input_dir
+00000720: 7a02 2d69 da01 2e7a 2d54 6865 2064 6972  z.-i...z-The dir
+00000730: 6563 746f 7279 2074 6f20 7265 6164 2067  ectory to read g
+00000740: 656e 6572 6174 6564 2063 6c61 7373 6573  enerated classes
+00000750: 2066 726f 6d2e 2902 da07 6465 6661 756c   from.)...defaul
+00000760: 74da 0468 656c 7063 0300 0000 0000 0000  t..helpc........
+00000770: 0000 0000 1200 0000 0b00 0000 4b00 0000  ............K...
+00000780: 73c0 0100 0074 0064 0183 0101 0064 0274  s....t.d.....d.t
+00000790: 0183 0069 017d 0464 037d 0567 007d 0674  ...i.}.d.}.g.}.t
+000007a0: 026a 037c 029b 0064 049d 0264 0564 068d  .j.|...d...d.d..
+000007b0: 0244 005d c27d 0774 046a 05a0 067c 07a1  .D.].}.t.j...|..
+000007c0: 0172 2071 1774 0064 077c 079b 009d 0283  .r q.t.d.|......
+000007d0: 0101 0074 046a 05a0 077c 07a1 015c 027d  ...t.j...|...\.}
+000007e0: 087d 097c 04a0 087c 09a1 017d 0a7c 0a72  .}.|...|...}.|.r
+000007f0: c574 097c 0764 0883 028f 0c7d 0b7c 0ba0  .t.|.d.....}.|..
+00000800: 0aa1 007d 0c57 0064 0904 0004 0083 0301  ...}.W.d........
+00000810: 006e 0831 0073 4a77 0101 0001 0001 0059  .n.1.sJw.......Y
+00000820: 0001 007c 057c 0c76 0172 6574 0ba0 0c64  ...|.|.v.ret...d
+00000830: 0a7c 079b 0064 0b9d 03a1 0101 007c 06a0  .|...d.......|..
+00000840: 0d74 0e7c 0764 0c83 02a1 0101 0071 1774  .t.|.d.......q.t
+00000850: 0fa0 1064 0d7c 0ca1 027d 0d7c 0d64 0975  ...d.|...}.|.d.u
+00000860: 0072 8174 0ba0 0c64 0a7c 079b 0064 0e9d  .r.t...d.|...d..
+00000870: 03a1 0101 007c 06a0 0d74 0e7c 0764 0f83  .....|...t.|.d..
+00000880: 02a1 0101 0071 177c 0da0 1164 10a1 017d  .....q.|...d...}
+00000890: 0e7c 01a0 127c 0ea1 017d 0f7a 1374 1374  .|...|...}.z.t.t
+000008a0: 01a0 147c 0f7c 0ca1 0283 017d 107c 1072  ...|.|.....}.|.r
+000008b0: 9d74 0064 11a0 157c 10a1 0183 0101 0057  .t.d...|.......W
+000008c0: 006e 2104 0074 1679 bf01 007d 1101 007a  .n!..t.y...}...z
+000008d0: 1574 0ba0 0c74 177c 1183 01a1 0101 007c  .t...t.|.......|
+000008e0: 06a0 0d74 0e7c 0764 1283 02a1 0101 0057  ...t.|.d.......W
+000008f0: 0059 0064 097d 117e 1171 1764 097d 117e  .Y.d.}.~.q.d.}.~
+00000900: 1177 0177 0074 0064 1383 0101 0071 1774  .w.w.t.d.....q.t
+00000910: 0ba0 1864 147c 099b 0064 157c 079b 0064  ...d.|...d.|...d
+00000920: 169d 05a1 0101 007c 06a0 0d74 0e7c 0764  .......|...t.|.d
+00000930: 1783 02a1 0101 0071 1774 197c 0683 0101  .......q.t.|....
+00000940: 0064 0953 0029 187a 7843 6f6d 7061 7265  .d.S.).zxCompare
+00000950: 7320 6375 7272 656e 746c 7920 6765 6e65  s currently gene
+00000960: 7261 7465 6420 636c 6173 7365 7320 7769  rated classes wi
+00000970: 7468 2074 6865 2073 7065 6369 6669 6361  th the specifica
+00000980: 7469 6f6e 7320 6665 7463 6865 6420 6672  tions fetched fr
+00000990: 6f6d 2074 6865 2041 5049 2061 6e64 2070  om the API and p
+000009a0: 726f 7669 6465 7320 6120 7375 6d6d 6172  rovides a summar
+000009b0: 7920 6f66 0a20 2020 2063 6861 6e67 6573  y of.    changes
+000009c0: 2e7a 0b50 6c61 6e6e 696e 672e 2e2e 7a03  .z.Planning...z.
+000009d0: 2e63 737a 3954 6869 7320 6669 6c65 2069  .csz9This file i
+000009e0: 7320 6175 746f 2d67 656e 6572 6174 6564  s auto-generated
+000009f0: 2062 7920 5374 656c 6c61 4e6f 7743 4c49   by StellaNowCLI
+00000a00: 2e20 444f 204e 4f54 2045 4449 542e 7a03  . DO NOT EDIT.z.
+00000a10: 2f2a 2a54 2901 da09 7265 6375 7273 6976  /**T)...recursiv
+00000a20: 657a 343d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ez4=============
+00000a30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a40: 3d0a 436f 6d70 6172 6973 6f6e 2066 6f72  =.Comparison for
+00000a50: 2066 696c 653a 20da 0172 4e7a 0953 6b69   file: ..rNz.Ski
+00000a60: 7070 696e 6720 7a23 2062 6563 6175 7365  pping z# because
+00000a70: 2069 7420 7761 7320 6e6f 7420 6175 746f   it was not auto
+00000a80: 2d67 656e 6572 6174 6564 2e7a 124e 6f74  -generated.z.Not
+00000a90: 2041 7574 6f2d 4765 6e65 7261 7465 647a   Auto-Generatedz
+00000aa0: 5745 7665 6e74 2049 443a 2028 5b30 2d39  WEvent ID: ([0-9
+00000ab0: 612d 6641 2d46 5d7b 387d 2d5b 302d 3961  a-fA-F]{8}-[0-9a
+00000ac0: 2d66 412d 465d 7b34 7d2d 5b30 2d39 612d  -fA-F]{4}-[0-9a-
+00000ad0: 6641 2d46 5d7b 347d 2d5b 302d 3961 2d66  fA-F]{4}-[0-9a-f
+00000ae0: 412d 465d 7b34 7d2d 5b30 2d39 612d 6641  A-F]{4}-[0-9a-fA
+00000af0: 2d46 5d7b 3132 7d29 7a1f 2062 6563 6175  -F]{12})z. becau
+00000b00: 7365 206e 6f20 4576 656e 7420 4944 2077  se no Event ID w
+00000b10: 6173 2066 6f75 6e64 2e7a 1245 7665 6e74  as found.z.Event
+00000b20: 2049 4420 4e6f 7420 466f 756e 6472 0400   ID Not Foundr..
+00000b30: 0000 da00 7a06 7374 7228 6529 7a14 4e6f  ....z.str(e)z.No
+00000b40: 2063 6861 6e67 6573 2064 6574 6563 7465   changes detecte
+00000b50: 642e 7a21 4e6f 2067 656e 6572 6174 6f72  d.z!No generator
+00000b60: 2066 6f75 6e64 2066 6f72 2066 696c 6520   found for file 
+00000b70: 7479 7065 207a 0b2e 2053 6b69 7070 696e  type z.. Skippin
+00000b80: 6720 7221 0000 007a 1455 6e73 7570 706f  g r!...z.Unsuppo
+00000b90: 7274 6564 204c 616e 6775 6167 6529 1a72  rted Language).r
+00000ba0: 1a00 0000 7208 0000 00da 0467 6c6f 625a  ....r......globZ
+00000bb0: 0569 676c 6f62 da02 6f73 da04 7061 7468  .iglob..os..path
+00000bc0: da05 6973 6469 72da 0873 706c 6974 6578  ..isdir..splitex
+00000bd0: 74da 0367 6574 da04 6f70 656e da04 7265  t..get..open..re
+00000be0: 6164 da06 6c6f 6767 6572 da07 7761 726e  ad..logger..warn
+00000bf0: 696e 67da 0661 7070 656e 6472 0900 0000  ing..appendr....
+00000c00: da02 7265 da06 7365 6172 6368 da05 6772  ..re..search..gr
+00000c10: 6f75 70da 1167 6574 5f65 7665 6e74 5f64  oup..get_event_d
+00000c20: 6574 6169 6c73 da04 6c69 7374 5a08 6765  etails..listZ.ge
+00000c30: 745f 6469 6666 da04 6a6f 696e da09 4578  t_diff..join..Ex
+00000c40: 6365 7074 696f 6e72 1600 0000 da05 6572  ceptionr......er
+00000c50: 726f 7272 1e00 0000 2912 da03 6374 78da  rorr....)...ctx.
+00000c60: 0a73 7465 6c6c 615f 6170 695a 0969 6e70  .stella_apiZ.inp
+00000c70: 7574 5f64 6972 da06 6b77 6172 6773 da0a  ut_dir..kwargs..
+00000c80: 6765 6e65 7261 746f 7273 5a16 6175 746f  generatorsZ.auto
+00000c90: 5f67 656e 6572 6174 6564 5f63 6f6d 6d65  _generated_comme
+00000ca0: 6e74 7217 0000 0072 0a00 0000 da01 5fda  ntr....r......_.
+00000cb0: 0365 7874 da09 6765 6e65 7261 746f 72da  .ext..generator.
+00000cc0: 0166 5a0d 6578 6973 7469 6e67 5f63 6f64  .fZ.existing_cod
+00000cd0: 655a 0f65 7665 6e74 5f69 645f 7365 6172  eZ.event_id_sear
+00000ce0: 6368 da08 6576 656e 745f 6964 5a0c 6576  ch..event_idZ.ev
+00000cf0: 656e 745f 6465 7461 696c 5a04 6469 6666  ent_detailZ.diff
+00000d00: da01 6572 0e00 0000 720e 0000 0072 0f00  ..er....r....r..
+00000d10: 0000 721f 0000 0034 0000 0073 5800 0000  ..r....4...sX...
+00000d20: 0808 0604 04ff 0405 0402 1803 0c02 0201  ................
+00000d30: 0e02 1001 0a01 0402 0c01 0a01 1cff 0804  ................
+00000d40: 1201 1001 0201 0403 0201 0201 04fe 0804  ................
+00000d50: 1201 1001 0201 0a02 0a03 0202 1001 0401  ................
+00000d60: 0e01 0480 0e01 0e01 1001 0c01 0880 02fd  ................
+00000d70: 0a05 1803 1201 0c02 2919 da07 5f5f 646f  ........)...__do
+00000d80: 635f 5f72 2800 0000 7232 0000 0072 2700  c__r(...r2...r'.
+00000d90: 0000 da05 636c 6963 6bda 076c 6f67 6769  ....click..loggi
+00000da0: 6e67 da0b 7072 6574 7479 7461 626c 6572  ng..prettytabler
+00000db0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000dc0: 00da 0e63 6f6d 6d61 6e64 5f63 6f6e 6669  ...command_confi
+00000dd0: 6772 0500 0000 7206 0000 005a 0f63 6f64  gr....r....Z.cod
+00000de0: 655f 6765 6e65 7261 746f 7273 7208 0000  e_generatorsr...
+00000df0: 00da 0967 6574 4c6f 6767 6572 7213 0000  ...getLoggerr...
+00000e00: 0072 2f00 0000 7209 0000 0072 1e00 0000  .r/...r....r....
+00000e10: da07 636f 6d6d 616e 64da 066f 7074 696f  ..command..optio
+00000e20: 6eda 0c70 6173 735f 636f 6e74 6578 7472  n..pass_contextr
+00000e30: 1f00 0000 da08 706c 616e 5f63 6d64 720e  ......plan_cmdr.
+00000e40: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000e50: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000e60: 7328 0000 0004 0008 0908 0108 0108 0108  s(..............
+00000e70: 010c 020c 0110 020c 010a 030e 0316 090a  ................
+00000e80: 1102 0102 0110 0104 0112 0108 44         ............D
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/configure.py` & `stellanow_cli-0.0.6/stellanow_cli/commands/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 """
 
 import click
 import configparser
 import os
 import re
 
-from ..validate import is_valid_uuid
-from ..logger import logger
+from ..utils import logger, is_valid_uuid
 from ..config import Env
 
 
 @click.command(name='configure')
 @click.option('--profile', default='DEFAULT', prompt=False,
               help="The profile name for storing a particular set of configurations. "
                    "If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.")
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/events.py` & `stellanow_cli-0.0.6/stellanow_cli/commands/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 All rights reserved.
 """
 
 import click
 
 from prettytable import PrettyTable
 
-from ..command_config import common_option, load_config
+from .command_config import common_option, load_config
 
 
 @click.command(name='events')
 @common_option
 @load_config
 @click.pass_context
 def events(ctx, stella_api, organization_id, project_id, **kwargs):
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/commands/plan.py` & `stellanow_cli-0.0.6/stellanow_cli/commands/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 All rights reserved.
 """
 
 import os
 import re
 import glob
 import click
+import logging
 
 from prettytable import PrettyTable
 from typing import List
 
-from ..command_config import common_option, load_config
+from .command_config import common_option, load_config
 from ..code_generators import CsharpCodeGenerator
-from ..logger import logger
+
+
+logger = logging.getLogger(__name__)
 
 
 class SkippedFile:
     def __init__(self, filename: str, reason: str):
         self.filename = filename
         self.reason = reason
 
@@ -37,14 +40,18 @@
 
         # Populate the table with data from your SkippedFile instances
         for skipped_file in skipped_files:
             table.add_row([skipped_file.filename, skipped_file.reason])
 
         print(table)
 
+        print("\nSkipped Reason - Explanation:\n")
+        print("- Not Auto-Generated - It looks like the file was not generated by this CLI.")
+        print("- Event ID Not Found - The ID of the event is missing in the header comment.")
+
 
 @click.command(name='plan')
 @common_option
 @load_config
 @click.option('--input_dir', '-i', default='.', help='The directory to read generated classes from.')
 @click.pass_context
 def plan(ctx, stella_api, input_dir, **kwargs):
@@ -64,15 +71,15 @@
 
     # Let's iterate over all the files in the input directory
     for filename in glob.iglob(f'{input_dir}/**', recursive=True):
         # Skip if the filename is a directory
         if os.path.isdir(filename):
             continue
 
-        print(f"==============================\n\nComparison for file: {filename}")
+        print(f"==============================\nComparison for file: {filename}")
         _, ext = os.path.splitext(filename)
         generator = generators.get(ext)
 
         if generator:
             with open(filename, 'r') as f:
                 existing_code = f.read()
 
@@ -94,23 +101,23 @@
 
             event_id = event_id_search.group(1)
 
             # We found a matching code generator, let's generate the code for comparison
             event_detail = stella_api.get_event_details(event_id)
 
             try:
-                diff = CsharpCodeGenerator.get_diff(event_detail, existing_code);
-
-                print(''.join(diff))
-            except Exception as e:
+                diff = list(CsharpCodeGenerator.get_diff(event_detail, existing_code))
+                if diff:
+                    print(''.join(diff))
+            except Exception as e:  # TODO: add specific exception
                 logger.warning(str(e))
                 skipped_files.append(SkippedFile(filename, "str(e)"))
                 continue
 
-            print(f"No changes detected in file: {filename}")
+            print(f"No changes detected.")
 
         else:
             logger.error(f'No generator found for file type {ext}. Skipping {filename}.')
             skipped_files.append(SkippedFile(filename, "Unsupported Language"))
 
     print_summary(skipped_files)
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/__init__.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/dev.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:53:06 2023 UTC, .py size: 509 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-00000000: 6f0d 0d0a 0000 0000 327a 8b64 fd01 0000  o.......2z.d....
+00000000: 6f0d 0d0a 0000 0000 287a 8b64 df01 0000  o.......(z.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
+00000020: 0005 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
-00000040: 6404 6c03 6d04 5a04 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000050: 8400 6406 6502 8303 5a05 6407 5300 2908  ..d.e...Z.d.S.).
-00000060: 613c 0100 000a 436f 7079 7269 6768 7420  a<....Copyright 
-00000070: 2843 2920 3230 3232 2d32 3032 3320 5374  (C) 2022-2023 St
-00000080: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
-00000090: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
-000000a0: 0a54 6869 7320 736f 6674 7761 7265 2069  .This software i
-000000b0: 7320 7468 6520 7072 6f70 7269 6574 6172  s the proprietar
-000000c0: 7920 696e 666f 726d 6174 696f 6e20 6f66  y information of
-000000d0: 2053 7465 6c6c 6120 5465 6368 6e6f 6c6f   Stella Technolo
-000000e0: 6769 6573 2028 554b 2920 4c69 6d69 7465  gies (UK) Limite
-000000f0: 642e 0a55 7365 2c20 7265 7072 6f64 7563  d..Use, reproduc
-00000100: 7469 6f6e 2c20 6f72 2072 6564 6973 7472  tion, or redistr
-00000110: 6962 7574 696f 6e20 6f66 2074 6869 7320  ibution of this 
-00000120: 736f 6674 7761 7265 2069 7320 7374 7269  software is stri
-00000130: 6374 6c79 2070 726f 6869 6269 7465 6420  ctly prohibited 
-00000140: 7769 7468 6f75 740a 7468 6520 6578 7072  without.the expr
-00000150: 6573 7320 7772 6974 7465 6e20 7065 726d  ess written perm
-00000160: 6973 7369 6f6e 206f 6620 5374 656c 6c61  ission of Stella
-00000170: 2054 6563 686e 6f6c 6f67 6965 7320 2855   Technologies (U
-00000180: 4b29 204c 696d 6974 6564 2e0a 416c 6c20  K) Limited..All 
-00000190: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-000001a0: 0ae9 0000 0000 2901 da04 456e 756d e901  ......)...Enum..
-000001b0: 0000 0029 01da 0643 6f6e 6669 6763 0000  ...)...Configc..
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000001d0: 0000 4000 0000 7320 0000 0065 005a 0164  ..@...s ...e.Z.d
-000001e0: 005a 0264 015a 0364 025a 0465 0564 0364  .Z.d.Z.d.Z.e.d.d
-000001f0: 0484 0083 015a 0664 0553 0029 06da 0345  .....Z.d.S.)...E
-00000200: 6e76 da03 696e 74da 0364 6576 6301 0000  nv..int..devc...
-00000210: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000220: 0043 0000 0073 0a00 0000 7c00 7400 6a01  .C...s....|.t.j.
-00000230: 7600 5300 2901 4e29 0272 0500 0000 da0b  v.S.).N).r......
-00000240: 5f5f 6d65 6d62 6572 735f 5f29 01da 0576  __members__)...v
-00000250: 616c 7565 a900 720a 0000 00fa 5d2f 5573  alue..r.....]/Us
-00000260: 6572 732f 746f 6d2d 6b61 6e64 7a69 6f72  ers/tom-kandzior
-00000270: 612f 4465 764c 6f63 616c 2f73 7465 6c6c  a/DevLocal/stell
-00000280: 612f 7374 656c 6c61 2d6e 6f77 2f53 7465  a/stella-now/Ste
-00000290: 6c6c 614e 6f77 434c 492f 7374 656c 6c61  llaNowCLI/stella
-000002a0: 6e6f 775f 636c 692f 636f 6e66 6967 2f5f  now_cli/config/_
-000002b0: 5f69 6e69 745f 5f2e 7079 da08 6973 5f76  _init__.py..is_v
-000002c0: 616c 6964 1300 0000 7302 0000 000a 027a  alid....s......z
-000002d0: 0c45 6e76 2e69 735f 7661 6c69 644e 2907  .Env.is_validN).
-000002e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-000002f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000300: 6d65 5f5f da03 494e 545a 0344 4556 da0c  me__..INTZ.DEV..
-00000310: 7374 6174 6963 6d65 7468 6f64 720c 0000  staticmethodr...
-00000320: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00000330: 720b 0000 0072 0500 0000 0f00 0000 730a  r....r........s.
-00000340: 0000 0008 0004 0104 0102 020e 0172 0500  .............r..
-00000350: 0000 4e29 06da 075f 5f64 6f63 5f5f da04  ..N)...__doc__..
-00000360: 656e 756d 7202 0000 00da 0663 6f6e 6669  enumr......confi
-00000370: 6772 0400 0000 7205 0000 0072 0a00 0000  gr....r....r....
-00000380: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000390: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-000003a0: 0000 0400 0c09 0c02 1403                 ..........
+00000040: 6404 6c03 6d04 5a04 0100 6502 4700 6405  d.l.m.Z...e.G.d.
+00000050: 6406 8400 6406 6504 8303 8301 5a05 6407  d...d.e.....Z.d.
+00000060: 5300 2908 613c 0100 000a 436f 7079 7269  S.).a<....Copyri
+00000070: 6768 7420 2843 2920 3230 3232 2d32 3032  ght (C) 2022-202
+00000080: 3320 5374 656c 6c61 2054 6563 686e 6f6c  3 Stella Technol
+00000090: 6f67 6965 7320 2855 4b29 204c 696d 6974  ogies (UK) Limit
+000000a0: 6564 2e0a 0a54 6869 7320 736f 6674 7761  ed...This softwa
+000000b0: 7265 2069 7320 7468 6520 7072 6f70 7269  re is the propri
+000000c0: 6574 6172 7920 696e 666f 726d 6174 696f  etary informatio
+000000d0: 6e20 6f66 2053 7465 6c6c 6120 5465 6368  n of Stella Tech
+000000e0: 6e6f 6c6f 6769 6573 2028 554b 2920 4c69  nologies (UK) Li
+000000f0: 6d69 7465 642e 0a55 7365 2c20 7265 7072  mited..Use, repr
+00000100: 6f64 7563 7469 6f6e 2c20 6f72 2072 6564  oduction, or red
+00000110: 6973 7472 6962 7574 696f 6e20 6f66 2074  istribution of t
+00000120: 6869 7320 736f 6674 7761 7265 2069 7320  his software is 
+00000130: 7374 7269 6374 6c79 2070 726f 6869 6269  strictly prohibi
+00000140: 7465 6420 7769 7468 6f75 740a 7468 6520  ted without.the 
+00000150: 6578 7072 6573 7320 7772 6974 7465 6e20  express written 
+00000160: 7065 726d 6973 7369 6f6e 206f 6620 5374  permission of St
+00000170: 656c 6c61 2054 6563 686e 6f6c 6f67 6965  ella Technologie
+00000180: 7320 2855 4b29 204c 696d 6974 6564 2e0a  s (UK) Limited..
+00000190: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
+000001a0: 7665 642e 0ae9 0000 0000 2901 da09 6461  ved.......)...da
+000001b0: 7461 636c 6173 73e9 0100 0000 2901 da06  taclass.....)...
+000001c0: 436f 6e66 6967 6300 0000 0000 0000 0000  Configc.........
+000001d0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000001e0: 1a00 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
+000001f0: 5a03 6504 6505 6402 3c00 6403 5300 2904  Z.e.e.d.<.d.S.).
+00000200: da09 436f 6e66 6967 4465 767a 2068 7474  ..ConfigDevz htt
+00000210: 7073 3a2f 2f61 7069 2e64 6576 2d61 7773  ps://api.dev-aws
+00000220: 2e73 7465 6c6c 612e 636c 6f75 64da 0862  .stella.cloud..b
+00000230: 6173 655f 7572 6c4e 2906 da08 5f5f 6e61  ase_urlN)...__na
+00000240: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000250: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
+00000260: 0000 00da 0373 7472 da0f 5f5f 616e 6e6f  .....str..__anno
+00000270: 7461 7469 6f6e 735f 5fa9 0072 0c00 0000  tations__..r....
+00000280: 720c 0000 00fa 582f 5573 6572 732f 746f  r.....X/Users/to
+00000290: 6d2d 6b61 6e64 7a69 6f72 612f 4465 764c  m-kandziora/DevL
+000002a0: 6f63 616c 2f73 7465 6c6c 612f 7374 656c  ocal/stella/stel
+000002b0: 6c61 2d6e 6f77 2f53 7465 6c6c 614e 6f77  la-now/StellaNow
+000002c0: 434c 492f 7374 656c 6c61 6e6f 775f 636c  CLI/stellanow_cl
+000002d0: 692f 636f 6e66 6967 2f64 6576 2e70 7972  i/config/dev.pyr
+000002e0: 0500 0000 0f00 0000 7304 0000 000a 0010  ........s.......
+000002f0: 0272 0500 0000 4e29 06da 075f 5f64 6f63  .r....N)...__doc
+00000300: 5f5f da0b 6461 7461 636c 6173 7365 7372  __..dataclassesr
+00000310: 0200 0000 da06 636f 6e66 6967 7204 0000  ......configr...
+00000320: 0072 0500 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000330: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+00000340: 756c 653e 0100 0000 730a 0000 0004 000c  ule>....s.......
+00000350: 090c 0202 0316 01                        .......
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/config.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.5/stellanow_cli/config/__pycache__/dev.cpython-310.pyc` & `stellanow_cli-0.0.6/stellanow_cli/config/__pycache__/int.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 20:52:56 2023 UTC, .py size: 479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 287a 8b64 df01 0000  o.......(z.d....
+00000000: 6f0d 0d0a 0000 0000 237a 8b64 db01 0000  o.......#z.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6404 6c03 6d04 5a04 0100 6502 4700 6405  d.l.m.Z...e.G.d.
 00000050: 6406 8400 6406 6504 8303 8301 5a05 6407  d...d.e.....Z.d.
 00000060: 5300 2908 613c 0100 000a 436f 7079 7269  S.).a<....Copyri
 00000070: 6768 7420 2843 2920 3230 3232 2d32 3032  ght (C) 2022-202
@@ -26,29 +26,29 @@
 00000190: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
 000001a0: 7665 642e 0ae9 0000 0000 2901 da09 6461  ved.......)...da
 000001b0: 7461 636c 6173 73e9 0100 0000 2901 da06  taclass.....)...
 000001c0: 436f 6e66 6967 6300 0000 0000 0000 0000  Configc.........
 000001d0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 000001e0: 1a00 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
 000001f0: 5a03 6504 6505 6402 3c00 6403 5300 2904  Z.e.e.d.<.d.S.).
-00000200: da09 436f 6e66 6967 4465 767a 2068 7474  ..ConfigDevz htt
-00000210: 7073 3a2f 2f61 7069 2e64 6576 2d61 7773  ps://api.dev-aws
-00000220: 2e73 7465 6c6c 612e 636c 6f75 64da 0862  .stella.cloud..b
-00000230: 6173 655f 7572 6c4e 2906 da08 5f5f 6e61  ase_urlN)...__na
-00000240: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000250: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
-00000260: 0000 00da 0373 7472 da0f 5f5f 616e 6e6f  .....str..__anno
-00000270: 7461 7469 6f6e 735f 5fa9 0072 0c00 0000  tations__..r....
-00000280: 720c 0000 00fa 582f 5573 6572 732f 746f  r.....X/Users/to
-00000290: 6d2d 6b61 6e64 7a69 6f72 612f 4465 764c  m-kandziora/DevL
-000002a0: 6f63 616c 2f73 7465 6c6c 612f 7374 656c  ocal/stella/stel
-000002b0: 6c61 2d6e 6f77 2f53 7465 6c6c 614e 6f77  la-now/StellaNow
-000002c0: 434c 492f 7374 656c 6c61 6e6f 775f 636c  CLI/stellanow_cl
-000002d0: 692f 636f 6e66 6967 2f64 6576 2e70 7972  i/config/dev.pyr
-000002e0: 0500 0000 0f00 0000 7304 0000 000a 0010  ........s.......
-000002f0: 0272 0500 0000 4e29 06da 075f 5f64 6f63  .r....N)...__doc
-00000300: 5f5f da0b 6461 7461 636c 6173 7365 7372  __..dataclassesr
-00000310: 0200 0000 da06 636f 6e66 6967 7204 0000  ......configr...
-00000320: 0072 0500 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000330: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
-00000340: 756c 653e 0100 0000 730a 0000 0004 000c  ule>....s.......
-00000350: 090c 0202 0316 01                        .......
+00000200: da09 436f 6e66 6967 496e 747a 1c68 7474  ..ConfigIntz.htt
+00000210: 7073 3a2f 2f61 7069 2e69 6e74 2e73 7465  ps://api.int.ste
+00000220: 6c6c 612e 636c 6f75 64da 0862 6173 655f  lla.cloud..base_
+00000230: 7572 6c4e 2906 da08 5f5f 6e61 6d65 5f5f  urlN)...__name__
+00000240: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000250: 7175 616c 6e61 6d65 5f5f 7206 0000 00da  qualname__r.....
+00000260: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
+00000270: 6f6e 735f 5fa9 0072 0c00 0000 720c 0000  ons__..r....r...
+00000280: 00fa 582f 5573 6572 732f 746f 6d2d 6b61  ..X/Users/tom-ka
+00000290: 6e64 7a69 6f72 612f 4465 764c 6f63 616c  ndziora/DevLocal
+000002a0: 2f73 7465 6c6c 612f 7374 656c 6c61 2d6e  /stella/stella-n
+000002b0: 6f77 2f53 7465 6c6c 614e 6f77 434c 492f  ow/StellaNowCLI/
+000002c0: 7374 656c 6c61 6e6f 775f 636c 692f 636f  stellanow_cli/co
+000002d0: 6e66 6967 2f69 6e74 2e70 7972 0500 0000  nfig/int.pyr....
+000002e0: 0f00 0000 7304 0000 000a 0010 0272 0500  ....s........r..
+000002f0: 0000 4e29 06da 075f 5f64 6f63 5f5f da0b  ..N)...__doc__..
+00000300: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
+00000310: da06 636f 6e66 6967 7204 0000 0072 0500  ..configr....r..
+00000320: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000330: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000340: 0100 0000 730a 0000 0004 000c 090c 0202  ....s...........
+00000350: 0316 01                                  ...
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli/config/config.py` & `stellanow_cli-0.0.6/stellanow_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.5/stellanow_cli/logger.py` & `stellanow_cli-0.0.6/stellanow_cli/utils/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 Use, reproduction, or redistribution of this software is strictly prohibited without
 the express written permission of Stella Technologies (UK) Limited.
 All rights reserved.
 """
 
 import logging
 
-# Setting up the logger
-logger = logging.getLogger('stellanow_cli')
-
 
 def setup_logger(verbose: bool):
+    root_logger = logging.getLogger()
+
     if verbose:
-        logger.setLevel(logging.INFO)
+        root_logger.setLevel(logging.INFO)
     else:
-        logger.setLevel(logging.WARNING)
+        root_logger.setLevel(logging.WARNING)
 
     # Console handler
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)  # Handler level is set to DEBUG
 
     # Create formatter and add it to the handlers
     formatter = logging.Formatter('%(levelname)s - %(message)s')
     ch.setFormatter(formatter)
 
     # Add the handlers to the logger
-    logger.addHandler(ch)
+    root_logger.addHandler(ch)
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli.egg-info/PKG-INFO` & `stellanow_cli-0.0.6/README.public`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: stellanow-cli
-Version: 0.0.5
-Summary: A comprehensive Python package for data analysis and visualization.
-Requires-Python: >=3.10
-
 StellaNow CLI Tool
 ==================
 
 Welcome to the StellaNow CLI tool. This tool automates the process of generating class code from StellaNow event specifications and provides a summary of changes between the generated classes and the specifications fetched from the API. It's recommended to use this tool in conjunction with the StellaNow SDK's to ensure that your application's message classes are up-to-date with the latest specifications.
 
 Installation
 ------------
@@ -61,15 +55,15 @@
 
 Command usage:
 
     stellanow configure --profile myProfile
 
 Command options:
 
-* **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
+* **`--profile`**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 
 This will prompt you for the access key, access token, organization ID, and project ID for the specified profile, which in this case is 'myProfile'. If you do not specify a profile, the command will default to the 'DEFAULT' profile.
 
 The command validates the provided values to ensure they meet the expected formats: the access key should be a valid email address or a string containing only alphanumeric characters, dashes, and underscores; the access token should be a string with no whitespace and a length of 8-64 characters; and both the organization ID and project ID should be valid UUIDs.
 
 The command then writes these configurations to a file named 'config.ini' in the '.stellanow' directory of your home folder. If this directory or file does not exist, they will be created.
 
@@ -128,13 +122,20 @@
 * **'--profile'**: The profile name for storing a particular set of configurations. If no profile is specified, the configurations will be stored under the 'DEFAULT' profile.
 * **'--verbose (-v)'**: Enables verbose mode, which outputs more detailed logging messages.
 
 These options allow for flexible command-line operation, as they let you provide command-specific details without altering your saved profile configurations. If these options are not specified in the command, the values saved in the specified profile (or the DEFAULT profile if none is specified) will be used.
 
 Please note that providing these options at the command line overrides the corresponding saved profile values for the duration of that command execution only. See **Credential Precedence Order** section for details.
 
+Release Notes
+-------------
+
+Version: TODO
+
+TODO
+
 Contact and Licensing
 ---------------------
 
 For further assistance and support, please contact us at **help@stella.systems**
 
-The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
+The StellaNow CLI, its platform, and code are proprietary software. It is licensed under a proprietary license agreement. Unauthorized copying, modification, redistribution, and use in production is prohibited without a proper license agreement. For inquiries about the licensing, please contact us via the above email.
```

### Comparing `stellanow_cli-0.0.5/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.6/stellanow_cli.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 MANIFEST.in
+Pipfile
 README.md
 README.public
 setup.py
 stellanow_cli/__init__.py
+stellanow_cli/_run.py
 stellanow_cli/_version.py
 stellanow_cli/cli.py
-stellanow_cli/command_config.py
-stellanow_cli/logger.py
-stellanow_cli/utils.py
-stellanow_cli/validate.py
 stellanow_cli.egg-info/PKG-INFO
 stellanow_cli.egg-info/SOURCES.txt
 stellanow_cli.egg-info/dependency_links.txt
 stellanow_cli.egg-info/entry_points.txt
 stellanow_cli.egg-info/requires.txt
 stellanow_cli.egg-info/top_level.txt
 stellanow_cli/__pycache__/__init__.cpython-310.pyc
+stellanow_cli/__pycache__/_run.cpython-310.pyc
 stellanow_cli/__pycache__/_version.cpython-310.pyc
 stellanow_cli/__pycache__/cli.cpython-310.pyc
-stellanow_cli/__pycache__/command_config.cpython-310.pyc
-stellanow_cli/__pycache__/logger.cpython-310.pyc
-stellanow_cli/__pycache__/utils.cpython-310.pyc
-stellanow_cli/__pycache__/validate.cpython-310.pyc
 stellanow_cli/api/__init__.py
+stellanow_cli/api/datatypes.py
 stellanow_cli/api/stellanow_api.py
 stellanow_cli/api/__pycache__/__init__.cpython-310.pyc
+stellanow_cli/api/__pycache__/datatypes.cpython-310.pyc
 stellanow_cli/api/__pycache__/stellanow_api.cpython-310.pyc
 stellanow_cli/code_generators/__init__.py
 stellanow_cli/code_generators/code_generator.py
 stellanow_cli/code_generators/csharp_code_generator.py
 stellanow_cli/code_generators/__pycache__/__init__.cpython-310.pyc
 stellanow_cli/code_generators/__pycache__/code_generator.cpython-310.pyc
 stellanow_cli/code_generators/__pycache__/csharp_code_generator.cpython-310.pyc
 stellanow_cli/code_generators/templates/.footer.template
 stellanow_cli/code_generators/templates/.header.template
 stellanow_cli/code_generators/templates/csharp.template
 stellanow_cli/commands/_init__.py
+stellanow_cli/commands/command_config.py
 stellanow_cli/commands/configure.py
 stellanow_cli/commands/events.py
 stellanow_cli/commands/generate.py
 stellanow_cli/commands/plan.py
+stellanow_cli/commands/__pycache__/command_config.cpython-310.pyc
 stellanow_cli/commands/__pycache__/configure.cpython-310.pyc
 stellanow_cli/commands/__pycache__/events.cpython-310.pyc
 stellanow_cli/commands/__pycache__/generate.cpython-310.pyc
 stellanow_cli/commands/__pycache__/plan.cpython-310.pyc
 stellanow_cli/config/__init__.py
 stellanow_cli/config/config.py
 stellanow_cli/config/dev.py
 stellanow_cli/config/int.py
 stellanow_cli/config/__pycache__/__init__.cpython-310.pyc
 stellanow_cli/config/__pycache__/config.cpython-310.pyc
 stellanow_cli/config/__pycache__/dev.cpython-310.pyc
 stellanow_cli/config/__pycache__/int.cpython-310.pyc
-tests/test_command_configure.py
+stellanow_cli/utils/__init__.py
+stellanow_cli/utils/logger.py
+stellanow_cli/utils/utils.py
+stellanow_cli/utils/__pycache__/__init__.cpython-310.pyc
+stellanow_cli/utils/__pycache__/logger.cpython-310.pyc
+stellanow_cli/utils/__pycache__/utils.cpython-310.pyc
+tests/test_command_configure.py
+tests/test_generate_class_handles_all_valueTypes.py
+tests/__pycache__/test_generate_class_handles_all_valueTypes.cpython-310.pyc
```

### Comparing `stellanow_cli-0.0.5/tests/test_command_configure.py` & `stellanow_cli-0.0.6/tests/test_command_configure.py`

 * *Files identical despite different names*

