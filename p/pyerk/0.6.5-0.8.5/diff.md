# Comparing `tmp/pyerk-0.6.5.tar.gz` & `tmp/pyerk-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/workcard/workstickdir/RST/expertise_system/erk/pyerk-core/dist/.tmp-__retdpb/pyerk-0.6.5.tar", last modified: Tue Dec 20 01:53:23 2022, max compression
+gzip compressed data, was "pyerk-0.8.5.tar", last modified: Mon Jun 19 14:26:49 2023, max compression
```

## Comparing `pyerk-0.6.5.tar` & `pyerk-0.8.5.tar`

### file list

```diff
@@ -1,64 +1,79 @@
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.986037 pyerk-0.6.5/
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.954037 pyerk-0.6.5/.circleci/
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1734 2022-12-18 23:21:36.000000 pyerk-0.6.5/.circleci/config.yml
--rw-r--r--   0 ck2       (1000) ck2       (1000)      102 2022-12-18 20:10:59.000000 pyerk-0.6.5/.gitignore
--rw-r--r--   0 ck2       (1000) ck2       (1000)      866 2022-12-18 20:10:59.000000 pyerk-0.6.5/.readthedocs.yml
--rw-r--r--   0 ck2       (1000) ck2       (1000)    34470 2021-03-01 17:49:26.000000 pyerk-0.6.5/LICENSE
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3617 2022-12-20 01:53:23.982037 pyerk-0.6.5/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3110 2022-12-19 19:47:47.000000 pyerk-0.6.5/README.md
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.958037 pyerk-0.6.5/docs/
--rw-r--r--   0 ck2       (1000) ck2       (1000)        6 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/.gitignore
--rw-r--r--   0 ck2       (1000) ck2       (1000)      638 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/Makefile
--rw-r--r--   0 ck2       (1000) ck2       (1000)      430 2022-12-19 19:37:02.000000 pyerk-0.6.5/docs/README.md
--rw-r--r--   0 ck2       (1000) ck2       (1000)      769 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/make.bat
--rw-r--r--   0 ck2       (1000) ck2       (1000)      176 2022-12-19 20:41:48.000000 pyerk-0.6.5/docs/requirements.txt
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.958037 pyerk-0.6.5/docs/source/
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.962037 pyerk-0.6.5/docs/source/_static/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       41 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/source/_static/style.css
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.962037 pyerk-0.6.5/docs/source/_templates/
--rw-r--r--   0 ck2       (1000) ck2       (1000)      156 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/source/_templates/layout.html
--rw-r--r--   0 ck2       (1000) ck2       (1000)     2493 2022-12-19 20:42:29.000000 pyerk-0.6.5/docs/source/conf.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.962037 pyerk-0.6.5/docs/source/devdoc/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       65 2022-12-18 20:10:59.000000 pyerk-0.6.5/docs/source/devdoc/overview.md
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3726 2022-12-19 20:58:00.000000 pyerk-0.6.5/docs/source/index.md
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.966037 pyerk-0.6.5/docs/source/userdoc/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       80 2022-12-19 21:11:12.000000 pyerk-0.6.5/docs/source/userdoc/cli.rst
--rw-r--r--   0 ck2       (1000) ck2       (1000)     4906 2022-12-19 21:06:01.000000 pyerk-0.6.5/docs/source/userdoc/overview.md
--rw-r--r--   0 ck2       (1000) ck2       (1000)      357 2022-12-18 20:17:07.000000 pyerk-0.6.5/pyerkconf-default.toml
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1562 2022-12-18 20:10:59.000000 pyerk-0.6.5/pyproject.toml
--rw-r--r--   0 ck2       (1000) ck2       (1000)      115 2022-12-18 20:31:54.000000 pyerk-0.6.5/requirements.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2022-12-20 01:53:23.986037 pyerk-0.6.5/setup.cfg
--rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2022-12-18 20:10:59.000000 pyerk-0.6.5/setup.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.950037 pyerk-0.6.5/src/
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.978037 pyerk-0.6.5/src/pyerk/
--rw-r--r--   0 ck2       (1000) ck2       (1000)      361 2022-11-19 09:47:30.000000 pyerk-0.6.5/src/pyerk/__init__.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     7972 2022-12-18 20:17:07.000000 pyerk-0.6.5/src/pyerk/auxiliary.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    51160 2022-12-19 19:11:14.000000 pyerk-0.6.5/src/pyerk/builtin_entities.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    63904 2022-12-20 01:06:50.000000 pyerk-0.6.5/src/pyerk/core.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     4423 2022-12-18 20:17:07.000000 pyerk-0.6.5/src/pyerk/erkloader.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3797 2022-11-19 09:47:30.000000 pyerk-0.6.5/src/pyerk/rdfstack.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2022-12-20 01:42:12.000000 pyerk-0.6.5/src/pyerk/release.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     4282 2022-12-18 20:17:07.000000 pyerk-0.6.5/src/pyerk/reportgenerator.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     9692 2022-12-18 20:10:59.000000 pyerk-0.6.5/src/pyerk/ruleengine.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     6843 2022-12-19 21:08:04.000000 pyerk-0.6.5/src/pyerk/script.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1370 2022-12-18 20:17:07.000000 pyerk-0.6.5/src/pyerk/settings.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.982037 pyerk-0.6.5/src/pyerk/templates/
--rw-r--r--   0 ck2       (1000) ck2       (1000)     2466 2022-12-18 20:17:07.000000 pyerk-0.6.5/src/pyerk/templates/report-template.tex
--rw-r--r--   0 ck2       (1000) ck2       (1000)    18788 2022-12-18 20:10:59.000000 pyerk-0.6.5/src/pyerk/visualization.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.978037 pyerk-0.6.5/src/pyerk.egg-info/
--rw-r--r--   0 ck2       (1000) ck2       (1000)     3617 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/PKG-INFO
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1129 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/SOURCES.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/dependency_links.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)       44 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/entry_points.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)      115 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/requires.txt
--rw-r--r--   0 ck2       (1000) ck2       (1000)        6 2022-12-20 01:53:23.000000 pyerk-0.6.5/src/pyerk.egg-info/top_level.txt
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.982037 pyerk-0.6.5/tests/
--rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-03-01 17:49:26.000000 pyerk-0.6.5/tests/__init__.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)    40498 2022-12-19 19:19:50.000000 pyerk-0.6.5/tests/test_core.py
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.982037 pyerk-0.6.5/tests/test_data/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       96 2022-09-05 19:09:39.000000 pyerk-0.6.5/tests/test_data/README.md
-drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2022-12-20 01:53:23.982037 pyerk-0.6.5/tests/test_data/reports/
--rw-r--r--   0 ck2       (1000) ck2       (1000)       65 2022-12-18 20:17:07.000000 pyerk-0.6.5/tests/test_data/reports/.gitignore
--rw-r--r--   0 ck2       (1000) ck2       (1000)     1564 2022-12-18 20:17:07.000000 pyerk-0.6.5/tests/test_data/reports/reportconf.toml
--rw-r--r--   0 ck2       (1000) ck2       (1000)      318 2022-09-14 14:26:01.000000 pyerk-0.6.5/tests/test_data/tmod0_with_errors.py
--rw-r--r--   0 ck2       (1000) ck2       (1000)      220 2022-09-14 14:26:01.000000 pyerk-0.6.5/tests/test_data/tmod1.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:49.018197 pyerk-0.8.5/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.938197 pyerk-0.8.5/.circleci/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1728 2022-12-20 09:47:51.000000 pyerk-0.8.5/.circleci/config.yml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      102 2022-12-18 20:10:59.000000 pyerk-0.8.5/.gitignore
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      866 2022-12-18 20:10:59.000000 pyerk-0.8.5/.readthedocs.yml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    34470 2021-03-01 17:49:26.000000 pyerk-0.8.5/LICENSE
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3617 2023-06-19 14:26:49.018197 pyerk-0.8.5/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3110 2022-12-20 01:54:20.000000 pyerk-0.8.5/README.md
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.942197 pyerk-0.8.5/docs/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        6 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/.gitignore
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      638 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/Makefile
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      430 2022-12-20 01:54:20.000000 pyerk-0.8.5/docs/README.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      769 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/make.bat
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      176 2022-12-20 01:54:20.000000 pyerk-0.8.5/docs/requirements.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.942197 pyerk-0.8.5/docs/source/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.942197 pyerk-0.8.5/docs/source/_static/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       41 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/source/_static/style.css
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.946197 pyerk-0.8.5/docs/source/_templates/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      156 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/source/_templates/layout.html
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     2494 2023-01-03 15:17:01.000000 pyerk-0.8.5/docs/source/conf.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.946197 pyerk-0.8.5/docs/source/devdoc/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       65 2022-12-18 20:10:59.000000 pyerk-0.8.5/docs/source/devdoc/overview.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3726 2022-12-20 01:54:20.000000 pyerk-0.8.5/docs/source/index.md
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.946197 pyerk-0.8.5/docs/source/userdoc/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       80 2022-12-20 01:54:20.000000 pyerk-0.8.5/docs/source/userdoc/cli.rst
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     9093 2023-01-01 22:07:52.000000 pyerk-0.8.5/docs/source/userdoc/overview.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      357 2022-12-18 20:17:07.000000 pyerk-0.8.5/pyerkconf-default.toml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1562 2023-05-25 15:36:34.000000 pyerk-0.8.5/pyproject.toml
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      124 2023-01-22 11:20:49.000000 pyerk-0.8.5/requirements.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2023-06-19 14:26:49.018197 pyerk-0.8.5/setup.cfg
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       38 2022-12-30 14:41:15.000000 pyerk-0.8.5/setup.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.634194 pyerk-0.8.5/src/
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.966197 pyerk-0.8.5/src/pyerk/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      361 2022-11-19 09:47:30.000000 pyerk-0.8.5/src/pyerk/__init__.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    10463 2023-03-26 15:30:02.000000 pyerk-0.8.5/src/pyerk/auxiliary.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    84092 2023-01-25 13:03:36.000000 pyerk-0.8.5/src/pyerk/builtin_entities.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    79830 2023-05-30 19:23:54.000000 pyerk-0.8.5/src/pyerk/core.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     5873 2023-04-04 22:27:54.000000 pyerk-0.8.5/src/pyerk/erkloader.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     2065 2023-01-18 19:59:41.000000 pyerk-0.8.5/src/pyerk/io.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     6854 2023-01-18 19:41:57.000000 pyerk-0.8.5/src/pyerk/rdfstack.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       22 2023-05-31 10:06:30.000000 pyerk-0.8.5/src/pyerk/release.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     4271 2023-01-03 15:17:01.000000 pyerk-0.8.5/src/pyerk/reportgenerator.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    69130 2023-04-04 19:26:27.000000 pyerk-0.8.5/src/pyerk/ruleengine.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     8260 2023-05-25 15:31:58.000000 pyerk-0.8.5/src/pyerk/script.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1636 2023-05-30 22:33:30.000000 pyerk-0.8.5/src/pyerk/settings.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.970197 pyerk-0.8.5/src/pyerk/templates/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     7453 2023-03-26 17:09:07.000000 pyerk-0.8.5/src/pyerk/templates/base.css
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      298 2023-03-26 17:04:47.000000 pyerk-0.8.5/src/pyerk/templates/l1_rule-application-report-stm.html
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     2466 2022-12-18 20:17:07.000000 pyerk-0.8.5/src/pyerk/templates/report-template.tex
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1697 2023-03-26 16:54:26.000000 pyerk-0.8.5/src/pyerk/templates/rule-application-report-page.html
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    18729 2023-01-03 15:17:01.000000 pyerk-0.8.5/src/pyerk/visualization.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.966197 pyerk-0.8.5/src/pyerk.egg-info/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     3617 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/PKG-INFO
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1645 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/SOURCES.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        1 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/dependency_links.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       44 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/entry_points.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      124 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/requires.txt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       17 2023-06-19 14:26:48.000000 pyerk-0.8.5/src/pyerk.egg-info/top_level.txt
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:48.974197 pyerk-0.8.5/tests/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)        0 2021-03-01 17:49:26.000000 pyerk-0.8.5/tests/__init__.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     4163 2023-05-25 15:31:58.000000 pyerk-0.8.5/tests/settings.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    60812 2023-05-25 15:31:58.000000 pyerk-0.8.5/tests/test_core.py
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:49.014197 pyerk-0.8.5/tests/test_data/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       96 2022-09-05 19:09:39.000000 pyerk-0.8.5/tests/test_data/README.md
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      167 2023-05-25 15:31:58.000000 pyerk-0.8.5/tests/test_data/erkpackage.toml
+drwxr-xr-x   0 ck2       (1000) ck2       (1000)        0 2023-06-19 14:26:49.018197 pyerk-0.8.5/tests/test_data/reports/
+-rw-r--r--   0 ck2       (1000) ck2       (1000)       65 2022-12-18 20:17:07.000000 pyerk-0.8.5/tests/test_data/reports/.gitignore
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     1556 2022-12-20 20:30:44.000000 pyerk-0.8.5/tests/test_data/reports/reportconf.toml
+-rw-------   0 ck2       (1000) ck2       (1000)     4447 2023-01-18 18:17:40.000000 pyerk-0.8.5/tests/test_data/test_triples1.nt
+-rw-------   0 ck2       (1000) ck2       (1000)     2921 2023-01-18 21:48:02.000000 pyerk-0.8.5/tests/test_data/test_zebra_triples1.nt
+-rw-------   0 ck2       (1000) ck2       (1000)   194908 2023-01-18 21:57:03.000000 pyerk-0.8.5/tests/test_data/test_zebra_triples2.nt
+-rw-------   0 ck2       (1000) ck2       (1000)   259157 2023-01-22 17:17:34.000000 pyerk-0.8.5/tests/test_data/test_zebra_triples3.nt
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      318 2022-09-14 14:26:01.000000 pyerk-0.8.5/tests/test_data/tmod0_with_errors.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)      220 2022-09-14 14:26:01.000000 pyerk-0.8.5/tests/test_data/tmod1.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     9230 2023-01-04 11:07:20.000000 pyerk-0.8.5/tests/test_data/zebra01.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)     5912 2023-01-22 23:41:13.000000 pyerk-0.8.5/tests/test_data/zebra02.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    15865 2023-01-22 23:50:00.000000 pyerk-0.8.5/tests/test_data/zebra_base_data.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    38072 2023-03-26 14:14:02.000000 pyerk-0.8.5/tests/test_data/zebra_puzzle_rules.py
+-rw-r--r--   0 ck2       (1000) ck2       (1000)    72141 2023-05-25 15:31:58.000000 pyerk-0.8.5/tests/test_rulebased_reasoning.py
```

### Comparing `pyerk-0.6.5/.circleci/config.yml` & `pyerk-0.8.5/.circleci/config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,17 @@
       - run:
           name: Load ERK Modules
           command: |
             echo Cloning erk-data
             cd ..
             mkdir erk-data-for-unittests
             cd erk-data-for-unittests
-            git clone https://github.com/ackrep-org/ocse.git erk-ocse
-            cd erk-ocse
-            git checkout for-unittests
+            git clone https://github.com/ackrep-org/ocse.git ocse
+            cd ocse
+            git checkout ut__pyerk__main
             cd ..
             ls -R
       - run:
           name: Test Core
           command: |
             python -m unittest
```

### Comparing `pyerk-0.6.5/.readthedocs.yml` & `pyerk-0.8.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/LICENSE` & `pyerk-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/PKG-INFO` & `pyerk-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerk
-Version: 0.6.5
+Version: 0.8.5
 Summary: Python based 'Easy Representation of Knowledge' (pyERK)
 Author-email: Carsten Knoll <firstname.lastname@posteo.de>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/ackrep-org/pyerk-core/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyerk-0.6.5/README.md` & `pyerk-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/docs/Makefile` & `pyerk-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/docs/make.bat` & `pyerk-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/docs/source/conf.py` & `pyerk-0.8.5/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 # ones.
 extensions = [
     "sphinx.ext.duration",
     "myst_parser",
     "sphinx.ext.doctest",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
-    'sphinx_rtd_theme',
-    'sphinxarg.ext',
+    "sphinx_rtd_theme",
+    "sphinxarg.ext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -56,26 +56,26 @@
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
 html_theme_options = {
-    'collapse_navigation': True,
-    'sticky_navigation': True,
-    'navigation_depth': 4,
-    'includehidden': True,
-    'titles_only': False
+    "collapse_navigation": True,
+    "sticky_navigation": True,
+    "navigation_depth": 4,
+    "includehidden": True,
+    "titles_only": False,
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 primary_domain = "py"
 
 
-source_suffix = ['.rst', '.md']
-source_parsers = {'.md': 'recommonmark.parser.CommonMarkParser'}
+source_suffix = [".rst", ".md"]
+source_parsers = {".md": "recommonmark.parser.CommonMarkParser"}
 
 # master_doc = 'index'
```

### Comparing `pyerk-0.6.5/docs/source/index.md` & `pyerk-0.8.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/pyproject.toml` & `pyerk-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/src/pyerk/auxiliary.py` & `pyerk-0.8.5/src/pyerk/auxiliary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 import os
 import sys
 import re as regex
 from typing import Iterable, Union, Dict, Any
 from rdflib import Literal
 from colorama import Style, Fore
+from addict import Addict as Container
 from . import settings
 
 """
 Some auxiliary classes and functions for pyerk.
 """
 
 startup_workdir = os.path.abspath(os.getcwd())
 
 
+# the following suffixes for base URIs are used for predicates to RDF-encode qualifiers (statements about statements)
+# strongly inspired by https://en.wikibooks.org/wiki/SPARQL/WIKIDATA_Qualifiers,_References_and_Ranks#Qualifiers
+
+# corresponds to `p` ("http://www.wikidata.org/prop/") -> links to statement nodes
+STATEMENTS_URI_PART = "/STATEMENTS"
+
+# corresponds to `ps` ("http://www.wikidata.org/prop/schema/".") -> links to main object
+PREDICATES_URI_PART = "/PREDICATES"
+
+# corresponds to `pq` ("http://www.wikidata.org/property_qualifier/" ?) -> used for qualifying pred-obj-tuples
+QUALIFIERS_URI_PART = "/QUALIFIERS"
+
+
 class NotYetFinishedError(NotImplementedError):
     pass
 
 
 class OneToOneMapping(object):
     def __init__(self, **kwargs):
         self.a = dict(**kwargs)
         self.b = dict([(v, k) for k, v in kwargs.items()])
 
         # assert 1to1-property
         assert len(self.a) == len(self.b)
 
     def add_pair(self, key_a, key_b):
+
+        if key_a in self.a:
+            msg = f"key_a '{key_a}' does already exist."
+            raise KeyError(msg)
+
+        if key_b in self.b:
+            msg = f"key_b '{key_b}' does already exist."
+            raise KeyError(msg)
+
         self.a[key_a] = key_b
         self.b[key_b] = key_a
 
         # assert 1to1-property
         assert len(self.a) == len(self.b)
 
     def remove_pair(self, key_a=None, key_b=None, strict=True):
@@ -122,26 +145,61 @@
     pass
 
 
 class InvalidShortKeyError(PyERKError):
     pass
 
 
+class InvalidScopeNameError(PyERKError):
+    pass
+
+
+class InvalidScopeTypeError(PyERKError):
+    pass
+
+
 class ModuleAlreadyLoadedError(PyERKError):
     pass
 
 
 class SemanticRuleError(PyERKError):
     pass
 
+class InconsistentEdgeRelations(SemanticRuleError):
+    pass
+
+
+class MissingQualifierError(PyERKError):
+    pass
+
+
+class AmbiguousQualifierError(PyERKError):
+    pass
+
+
+class FunctionalRelationError(PyERKError):
+    pass
+
+
+class RuleTermination(PyERKError):
+    pass
+
+
+class LogicalContradiction(RuleTermination):
+    pass
+
+
+class ReasoningGoalReached(RuleTermination):
+    pass
+
 
 def ensure_valid_short_key(txt: str, strict: bool = True) -> bool:
     conds = [isinstance(txt, str)]
 
-    re_short_key = regex.compile(r"^((Ia?)|(Ra?)|(RE))(\d+)$")
+    re_short_key = regex.compile(r"^((Ia?)|(Ra?)|(S))(\d+)$")
     # produces 5 groups: [{outer-parenthesis}, {inner-p1}, {inner-p2}, {inner-p3}, {last-p}]
     # first (index: 1) and last are the only relevant groups
 
     match = re_short_key.match(txt)
 
     if match is None:
         conds += [False]
@@ -173,14 +231,34 @@
     if not cond and strict:
         msg = f"This seems not to be a valid URI: {txt}. Condition protocoll: {conds}"
         raise InvalidURIError(msg)
 
     return cond
 
 
+def ensure_valid_relation_uri(txt: str, strict=True):
+    conds = [ensure_valid_uri(txt, strict)]
+    conds.append(txt.split("#")[1].startswith("R"))
+
+    cond = all(conds)
+    if not cond and strict:
+        msg = f"This is not a valid relation URI: {txt}. Condition protocoll: {conds}"
+        raise InvalidURIError(msg)
+
+
+def ensure_valid_item_uri(txt: str, strict=True):
+    conds = [ensure_valid_uri(txt, strict)]
+    conds.append(txt.split("#")[1].startswith("I"))
+
+    cond = all(conds)
+    if not cond and strict:
+        msg = f"This is not a valid item URI: {txt}. Condition protocoll: {conds}"
+        raise InvalidURIError(msg)
+
+
 def ensure_valid_prefix(txt: str, strict: bool = True) -> bool:
     """
     To avoid confusion with base_uris prefixes have to meet certain conditions.
 
     :param txt:
     :param strict:
     :return:
@@ -195,14 +273,28 @@
     if not cond and strict:
         msg = f"This seems not to be a valid prefix: {txt}. Condition protocoll: {conds}"
         raise InvalidPrefixError(msg)
 
     return cond
 
 
+def parse_uri(txt: str) -> Container:
+    res = Container(full_uri=txt)
+    res.base_uri, res.short_key = txt.split("#")
+
+    for uri_part in (STATEMENTS_URI_PART, PREDICATES_URI_PART, QUALIFIERS_URI_PART):
+        if res.base_uri.endswith(uri_part):
+            res.sub_ns = uri_part
+            break
+    else:
+        res.sub_ns = None
+
+    return res
+
+
 def ensure_valid_baseuri(txt: str, strict: bool = True) -> bool:
     """
 
     :param txt:
     :param strict:
     :return:
     """
@@ -266,14 +358,23 @@
 
     for key in obsolete_keys:
         dikt.pop(key)
 
     return dikt
 
 
+def uri_set(*args):
+
+    res = []
+    for arg in args:
+        res.append(arg.uri)
+    return set(res)
+
+
+
 def bright(txt):
     return f"{Style.BRIGHT}{txt}{Style.RESET_ALL}"
 
 
 def bblue(txt):
     return f"{Fore.BLUE}{Style.BRIGHT}{txt}{Style.RESET_ALL}"
```

### Comparing `pyerk-0.6.5/src/pyerk/core.py` & `pyerk-0.8.5/src/pyerk/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import sys
 from collections import defaultdict
 from dataclasses import dataclass
 import inspect
 import types
 import abc
 import random
+import functools
+from urllib.parse import quote
 from enum import Enum, unique
 import re as regex
 from addict import Dict as attr_dict
 from typing import Dict, Union, List, Iterable, Optional
 from rdflib import Literal
+import pydantic
 import re
 
 from pyerk import auxiliary as aux
 from pyerk import settings
-from  pyerk.auxiliary import (
+from pyerk.auxiliary import (
     InvalidURIError,
     InvalidPrefixError,
     PyERKError,
     EmptyURIStackError,
     InvalidShortKeyError,
     UnknownPrefixError,
 )
@@ -32,14 +35,16 @@
 if os.environ.get("IPYDEX_AIOE") == "true":
     activate_ips_on_exception()
 
 
 """
     TODO:
 
+    report should link entities to django
+
     model sets as type? and elements as instances?
     manually trigger reload in gui
 
     Caylay-Hamilton-Theorem
     qualifier relations, e.g. for universal quantification
 
     Lyapunov stability theorem
@@ -64,14 +69,58 @@
     <dynamical_system> zu Instanzen der Klasse <mathematical_model>
 
     komplexere Aussagen:
     alle steuerbaren linearen ODE-systeme sind flach
 
 """
 
+allowed_literal_types = (str, bool, float, int, complex)
+
+
+# copied from yamlpyowl project
+def check_type(obj, expected_type, strict=True):
+    """
+    Use the pydantic package to check for (complex) types from the typing module.
+    If type checking passes returns `True`. This allows to use `assert check_type(...)` which allows to omit those
+    type checks (together with other assertions) for performance reasons, e.g. with `python -O ...` .
+    :param obj:             the object to check
+    :param expected_type:   primitive or complex type (like typing.List[dict])
+    :return:                True (or raise an TypeError)
+    """
+
+    class Model(pydantic.BaseModel):
+        data: expected_type
+
+        class Config:
+            # necessary because https://github.com/samuelcolvin/pydantic/issues/182
+            # otherwise check_type raises() an error for types as Dict[str, owl2.Thing]
+            arbitrary_types_allowed = True
+            smart_union=True  # seems to be necessary to respect the ordering of types inside a unioin
+
+    # convert ValidationError to TypeError if the obj does not match the expected type
+    try:
+        mod = Model(data=obj)
+    except pydantic.ValidationError as ve:
+        if not strict:
+            return False
+        msg = (
+            f"Unexpected type. Got: {type(obj)}. Expected: {expected_type}. "
+            f"Further Information:\n {str(ve.errors())}"
+        )
+        raise TypeError(msg)
+
+    if not mod.data == obj:
+        if not strict:
+            return False
+        msg = (
+            f"While type-checking: Unexpected inner structure of parsed model. Expected: {expected_type}"
+        )
+        raise TypeError(msg)
+    return True
+
 
 class Entity(abc.ABC):
     """
     Abstract parent class for both Relations and Items.
 
     Do not forget to call self.__post_init__ at the end of __init__ in subclasses.
     """
@@ -84,28 +133,32 @@
         # this will hold mappings like "R1234": EntityRelation(..., R1234)
         self.relation_dict = {}
         self._method_prototypes = []
         self._namespaces = {}
         self.base_uri = base_uri
         self.uri = None  # will be set in __post_init__
 
+        # simplifies debugging, will be set by _unlink_entity()
+        self._label_after_unlink = None
+        self._unlinked = False
+
     def __call__(self, *args, **kwargs):
-        
+
         custom_call_method = getattr(self, "_custom_call", None)
         if custom_call_method is None:
             msg = f"entity {self} has not defined a _custom_call-method and thus cannot be called"
             raise TypeError(msg)
         else:
             assert callable(custom_call_method)
-            
+
             res = custom_call_method(*args, **kwargs)
-            
+
             if custom_call_post_process := getattr(self, "_custom_call_post_process", None):
                 res = custom_call_post_process(res, *args, **kwargs)
-            
+
             return res
 
     def idoc(self, adhoc_label: str):
         """
         idoc means "inline doc". This function allows to attach a label to entities when using them in code
         because it returns just the Entity-object itself. Thus one can use the following expressions interchageably:
         `I1234` and `I1234.idoc("human readable item name")`
@@ -221,19 +274,19 @@
             for func in parent_class._method_prototypes:
                 self.add_method(func)
 
     def _get_relation_contents(self, rel_uri: str):
 
         aux.ensure_valid_uri(rel_uri)
 
-        relation_edges: List[RelationEdge] = ds.get_relation_edges(self.uri, rel_uri)
+        statements: List[Statement] = ds.get_statements(self.uri, rel_uri)
 
         # for each of the relation edges get a list of the result-objects
         # (this assumes the relation tuple to be a triple (sub, rel, obj))
-        res = [re.relation_tuple[2] for re in relation_edges if re.role is RelationRole.SUBJECT]
+        res = [re.relation_tuple[2] for re in statements if re.role is RelationRole.SUBJECT]
 
         # the following logic decides whether to e.g. return a list of length 1 or the contained entity itself
         # this depends on whether self is a functional relation (->  R22__is_functional)
 
         # if rel_uri == "<bi>R22" -> relation is the R22-entity: we are asking whether self is functional;
         # this must be handled separately to avoid infinite recursion:
         # (note that R22 itself is also a functional relation: only one of {True, False} is meaningful, same holds for
@@ -309,14 +362,21 @@
         :param func:
         :param name:    the name under which the callable object should be accessed
         :return:
         """
         if name is None:
             name = getattr(func, "given_name", func.__name__)
 
+        caller_frame = get_caller_frame(1)
+
+        # TODO: the mod_uri should be taken from the frame where func is defined and not where add_method is called
+        # currently this works because they are usually the same
+        if mod_uri := caller_frame.f_locals.get("__URI__"):
+            func = wrap_function_with_search_uri_context(func, mod_uri)
+
         # ensure that the func object has a `.given_name` attribute
         func.given_name = name
 
         self.__dict__[name] = types.MethodType(func, self)
         self._method_prototypes.append(func)
 
     def _set_relations_from_init_kwargs(self, **kwargs):
@@ -333,55 +393,64 @@
                 # this is unpacked to "scalar relations"
                 for elt in value:
                     self.set_relation(key, elt)
             else:
                 self.set_relation(key, value)
 
     def set_mutliple_relations(
-            self, relation: Union["Relation", str], obj_seq: Union[tuple, list], *args, **kwargs
-    ) -> List["RelationEdge"]:
+        self, relation: Union["Relation", str], obj_seq: Union[tuple, list], *args, **kwargs
+    ) -> List["Statement"]:
         """
-        Convenience function to create multiple RelationEdges at once
+        Convenience function to create multiple Statements at once
         """
         res_list = []
+
+        assert isinstance(obj_seq, (tuple, list))
         for obj in obj_seq:
             res_list.append(self.set_relation(relation, obj, *args, **kwargs))
 
         return res_list
 
     def set_relation(
         self,
         relation: Union["Relation", str],
         obj,
         scope: "Entity" = None,
         proxyitem: Optional["Item"] = None,
         qualifiers: Optional[List["RawQualifier"]] = None,
-    ) -> "RelationEdge":
+        prevent_duplicate=False,
+    ) -> Optional["Statement"]:
         """
         Allows to add a relation after the item was created.
 
         :param relation:    Relation-Entity (or its short_key)
         :param obj:         target (object) of the relation (where self is the subject)
         :param scope:       Entity for the scope in which the relation is defined
-        :param proxyitem:   optional item to which the RelationEdge is associated (e.g. an equation-instance)
+        :param proxyitem:   optional item to which the Statement is associated (e.g. an equation-instance)
         :param qualifiers:  optional list of RawQualifiers (see docstring of this class)
+        :param prevent_duplicate
+                            bool; prevent the creation of a statement which already exists.
         :return:
         """
 
         if isinstance(relation, str):
             if aux.ensure_valid_uri(relation, strict=False):
                 relation = ds.get_entity_by_uri(relation)
             else:
                 # assume we got the short key of the relation
                 relation = ds.get_entity_by_key_str(relation)
 
-        allowed_types = (str, bool, float, int, complex)
+        if prevent_duplicate:
+            existing_objects = self.get_relations(relation.uri, return_obj=True)
+            if obj in existing_objects:
+                return None
+
         if isinstance(relation, Relation):
 
-            if isinstance(obj, (Entity, *allowed_types)) or obj in allowed_types:
+            if isinstance(obj, (Entity, *allowed_literal_types)) or obj in allowed_literal_types:
                 return self._set_relation(relation.uri, obj, scope=scope, qualifiers=qualifiers, proxyitem=proxyitem)
             # Todo: remove obsolete code:
             # elif isinstance(obj, Iterable):
             #     msg = f"Unsupported iterable type ({type(obj)}) of {obj}, while setting relation {relation.short_key}"
             #     raise TypeError(msg)
             # elif isinstance(obj, (Entity, str, bool, float, int, complex)):
             #     # obj is eithter an entity or a literal
@@ -396,15 +465,15 @@
     def _set_relation(
         self,
         rel_uri: str,
         rel_content: object,
         scope: Optional["Entity"] = None,
         qualifiers: Optional[list] = None,
         proxyitem: Optional["Item"] = None,
-    ) -> "RelationEdge":
+    ) -> "Statement":
 
         aux.ensure_valid_uri(rel_uri)
         rel = ds.relations[rel_uri]
 
         # store relation for later usage
         self.relation_dict[rel_uri] = rel
 
@@ -423,175 +492,222 @@
             qualifiers = []
 
         if scope is not None:
             assert scope.R4__is_instance_of == ds.get_entity_by_uri(u("bi__I16__scope"))
             qff_has_defining_scope: QualifierFactory = ds.qff_dict["qff_has_defining_scope"]
             qualifiers.append(qff_has_defining_scope(scope))
 
-        rledg = RelationEdge(
+        stm = Statement(
             relation=rel,
             relation_tuple=(self, rel, rel_content),
             role=RelationRole.SUBJECT,
             corresponding_entity=corresponding_entity,
             corresponding_literal=corresponding_literal,
             scope=scope,
             qualifiers=qualifiers,
             proxyitem=proxyitem,
         )
 
-        ds.set_relation_edge(rledg)
+        ds.set_statement(stm)
 
         if scope is not None:
-            ds.scope_relation_edges[scope.uri].append(rledg)
+            ds.scope_statements[scope.uri].append(stm)
 
         # if the object is not a literal then also store the inverse relation
         if isinstance(rel_content, Entity):
 
-            inv_rledg = RelationEdge(
+            inv_stm = Statement(
                 relation=rel,
                 relation_tuple=(self, rel, rel_content),
                 role=RelationRole.OBJECT,
                 corresponding_entity=self,
                 scope=scope,
-                qualifiers=qualifiers,
+                qualifiers=stm.qualifiers,
                 proxyitem=proxyitem,
             )
 
-            # interconnect the primal RE with the inverse one:
-            rledg.dual_relation_edge = inv_rledg
-            inv_rledg.dual_relation_edge = rledg
+            # interconnect the primal Statement with the inverse one:
+            stm.dual_statement = inv_stm
+            inv_stm.dual_statement = stm
 
-            # ds.set_relation_edge(rel_content.short_key, rel.short_key, inv_rledg)
-            tmp_list = ds.inv_relation_edges[rel_content.uri][rel.uri]
+            # ds.set_statement(rel_content.short_key, rel.short_key, inv_stm)
+            tmp_list = ds.inv_statements[rel_content.uri][rel.uri]
 
             # TODO: maybe check length here for inverse functional
-            tmp_list.append(inv_rledg)
-        return rledg
+            tmp_list.append(inv_stm)
+        return stm
 
     def get_relations(
         self, key_str_or_uri: Optional[str] = None, return_subj: bool = False, return_obj: bool = False
     ) -> Union[Dict[str, list], list]:
         """
-        Return all RelationEdge instance where this item is subject
+        Return all Statement instance where this item is subject
 
         :param key_str_or_uri:      optional; either a verbose key_str (of a builtin entity) or a full uri;
                                     if passed only return the result for this key
         :param return_subj:         default False; if True only return the subject(s) of the relation edges,
-                                    not the whole RE
+                                    not the whole statement
 
         :return:            either the whole dict or just one value (of type list)
         """
 
-        rel_dict = ds.relation_edges[self.uri]
+        if key_str_or_uri is not None and not isinstance(key_str_or_uri, (str)):
+            msg = f"unexpected type for key_str_or_uri: {type(key_str_or_uri)}. Expected a str or None."
+            raise TypeError(msg)
+
+        rel_dict = ds.statements[self.uri]
         return self._return_relations(rel_dict, key_str_or_uri, return_subj, return_obj)
 
     def get_inv_relations(
         self, key_str_or_uri: Optional[str] = None, return_subj: bool = False, return_obj: bool = False
     ) -> Union[Dict[str, list], list]:
         """
-        Return all RelationEdge instance where this item is object
+        Return all Statement instance where this item is object
 
         :param key_str_or_uri:      optional; either a verbose key_str (of a builtin entity) or a full uri;
                                     if passed only return the result for this key
         :param return_subj:         default False; if True only return the subject(s) of the relation edge(s),
-                                    not the whole RE
+                                    not the whole statement
         :param return_obj:          default False; if True only return the object(s) of the relation edge(s),
-                                    not the whole RE
+                                    not the whole statement
 
         :return:            either the whole dict or just one value (of type list)
         """
 
-        inv_rel_dict = ds.inv_relation_edges[self.uri]
+        inv_rel_dict = ds.inv_statements[self.uri]
 
         return self._return_relations(inv_rel_dict, key_str_or_uri, return_subj, return_obj)
 
     @staticmethod
     def _return_relations(
         base_dict,
         key_str_or_uri: str,
         return_subj: bool = False,
         return_obj: bool = False,
     ) -> Union[Dict[str, list], list]:
         """
 
-        :param base_dict:           either ds.relation_edges or ds.inv_relation_edges
+        :param base_dict:           either ds.statements or ds.inv_statements
         :param key_str_or_uri:      optional; either a verbose key_str (of a builtin entity) or a full uri;
                                     if passed only return the result for this key
         :param return_subj:         default False; if True only return the subject(s) of the relation edge(s),
-                                    not the whole RE
+                                    not the whole statement
         :param return_obj:          default False; if True only return the object(s) of the relation edge(s),
-                                    not the whole RE
+                                    not the whole statement
         :return:
         """
         if key_str_or_uri is None:
             return base_dict
 
         # the caller wants only results for this key (e.g. "R4")
         if aux.ensure_valid_uri(key_str_or_uri, strict=False):
             uri = key_str_or_uri
         else:
             # we try to resolve a prefix and use the active module and finally builtins as fallback
             key_str = key_str_or_uri
             pr_key = process_key_str(key_str)
             uri = pr_key.uri
 
-        rledg_res: Union[RelationEdge, List[RelationEdge]] = base_dict.get(uri, [])
+        stm_res: Union[Statement, List[Statement]] = base_dict.get(uri, [])
         if return_subj:
-            # do not return the RelationEdge instance(s) but only the subject(s)
-            if isinstance(rledg_res, list):
-                rledg_res: List[RelationEdge]
-                res = [re.subject for re in rledg_res]
+            # do not return the Statement instance(s) but only the subject(s)
+            if isinstance(stm_res, list):
+                stm_res: List[Statement]
+                res = [re.subject for re in stm_res]
             else:
-                assert isinstance(rledg_res, RelationEdge)
-                res = rledg_res.subject
+                assert isinstance(stm_res, Statement)
+                res = stm_res.subject
         elif return_obj:
-            # do not return the RelationEdge instance(s) but only the object(s)
-            if isinstance(rledg_res, list):
-                rledg_res: List[RelationEdge]
-                res = [re.object for re in rledg_res]
+            # do not return the Statement instance(s) but only the object(s)
+            if isinstance(stm_res, list):
+                stm_res: List[Statement]
+                res = [re.object for re in stm_res]
             else:
-                assert isinstance(rledg_res, RelationEdge)
-                res = rledg_res.object
+                assert isinstance(stm_res, Statement)
+                res = stm_res.object
 
         else:
-            res = rledg_res
+            res = stm_res
         return res
 
+    def overwrite_statement(self, rel_key_str_or_uri: str, new_obj: "Entity", qualifiers=None) -> "Statement":
+        # the caller wants only results for this key (e.g. "R4")
+
+        assert isinstance(rel_key_str_or_uri, str)
+
+        if aux.ensure_valid_uri(rel_key_str_or_uri, strict=False):
+            rel_uri = rel_key_str_or_uri
+        else:
+            # we try to resolve a prefix and use the active module and finally builtins as fallback
+            key_str = rel_key_str_or_uri
+            pr_key = process_key_str(key_str)
+            rel_uri = pr_key.uri
+
+        rel = ds.get_entity_by_uri(rel_uri)
+
+        stm = self.get_relations(rel_uri)
+
+        if isinstance(stm, list):
+            if len(stm) == 0:
+                msg = f"Unexpectedly found empty statement list for entity {self} and relation {rel}"
+                raise aux.PyERKError(msg)
+            if len(stm) > 1:
+                msg = f"Unexpectedly found length-{len(stm)} statement list for entity {self} and relation {rel}"
+                raise aux.PyERKError(msg)
+            stm = stm[0]
+
+        assert isinstance(stm, Statement)
+
+        if stm.qualifiers:
+            raise NotImplementedError("Processing old qualifiers is not yet implemented while overwriting statements")
+
+        stm.unlink()
+        return self.set_relation(rel, new_obj, qualifiers=qualifiers)
+
+
+def wrap_function_with_search_uri_context(func, uri):
+    @functools.wraps(func)
+    def wrapped_func(*args, **kwargs):
+        with search_uri_context(uri=uri):
+            return func(*args, **kwargs)
+
+    return wrapped_func
+
 
 class DataStore:
     """
     Provides objects to store all data that would be global otherwise
     """
 
     def __init__(self):
         self.items = {}
         self.relations = {}
 
         # dict of lists store keys of the entities (not the entities itself, to simplify deletion)
         self.entities_created_in_mod = defaultdict(list)
 
-        self.rledgs_created_in_mod = defaultdict(dict)
+        self.stms_created_in_mod = defaultdict(dict)
 
         # mappings like .a = {"my/mod/uri": "/path/to/mod.py"} and .b = {"/path/to/mod.py": "my/mod/uri"}
         self.mod_path_mapping = aux.OneToOneMapping()
 
         # for every entity uri store a dict that maps relation uris to lists of corresponding relation-edges
-        self.relation_edges = defaultdict(dict)
+        self.statements = defaultdict(dict)
 
         # also do this for the inverse relations (for easy querying)
-        self.inv_relation_edges = defaultdict(lambda: defaultdict(list))
+        self.inv_statements = defaultdict(lambda: defaultdict(list))
 
         # for every scope-item key store the relevant relation-edges
-        self.scope_relation_edges = defaultdict(list)
+        self.scope_statements = defaultdict(list)
 
         # for every relation key store the relevant relation-edges
-        self.relation_relation_edges = defaultdict(list)
+        self.relation_statements = defaultdict(list)
 
-        # store a map {uri: RE-instance} of all relation edges
-        self.relation_edge_uri_map = {}
+        # store a map {uri: Statement-instance} of all relation edges
+        self.statement_uri_map = {}
 
         # this will be set on demand
         self.rdfgraph = None
 
         # dict to store important QualifierFactory instances which are created in builtin_entities but needed in core
         self.qff_dict = {}
 
@@ -613,14 +729,26 @@
 
         # dict like {uri1: <mod1>, ...}
         self.uri_mod_dict = {}
 
         # this list serves to keep track of nested scopes
         self.scope_stack = []
 
+        # store unlinked entities
+        self.unlinked_entities = {}
+
+    def get_item_by_label(self, label) -> Entity:
+        """
+        Search over all item and return the first item which has the provided label.
+        Useful during interactive debugging. Not useful for production!
+        """
+        for uri, itm in self.items.items():
+            if itm.R1 == label:
+                return itm
+
     def get_entity_by_key_str(self, key_str, mod_uri=None) -> Entity:
         """
         :param key_str:     str like I1234 or I1234__some_label
         :param mod_uri:     optional uri of the module; if None the active module is assumed
 
         :return:            corresponding entity
         """
@@ -661,74 +789,112 @@
 
         if strict and res is None:
             msg = f"No entity found for URI {uri}."
             raise aux.UnknownURIError(msg)
 
         return res
 
-    def get_relation_edges(self, entity_uri: str, rel_uri: str) -> List["RelationEdge"]:
+    @staticmethod
+    def _default_subject_filter(entity):
         """
-        self.relation_edges maps an entity_key to an inner_dict.
-        The inner_dict maps an relation_key to a RelationEdge or List[RelationEdge].
+        used to prevent items from scopes showing up inside the results of `get_subjects_for_relation`.
+        """
+        # R20["has defining scope"]>
+        return getattr(entity, "R20") is None
+
+    def get_subjects_for_relation(self, rel_uri: str, filter=None):
+
+        stm_list: List[Statement] = self.relation_statements[rel_uri]
+
+        res = []
+        if isinstance(filter, allowed_literal_types) or isinstance(filter, Entity):
+            cond_func = lambda obj: obj == filter
+        else:
+            cond_func = lambda obj: True
+        for stm in stm_list:
+            if cond_func(stm.object) and self._default_subject_filter(stm.subject):
+                res.append(stm.subject)
+
+        return res
+
+    def get_statements(self, entity_uri: str, rel_uri: str) -> List["Statement"]:
+        """
+        self.statements maps an entity_key to an inner_dict.
+        The inner_dict maps an relation_key to a Statement or List[Statement].
 
         :param entity_uri:
         :param rel_uri:
         :return:
         """
         aux.ensure_valid_uri(rel_uri)
         aux.ensure_valid_uri(entity_uri)
 
         # We return an empty list if the entity has no such relation.
         # TODO: model this as defaultdict?
-        return self.relation_edges[entity_uri].get(rel_uri, list())
+        return self.statements[entity_uri].get(rel_uri, list())
 
-    def set_relation_edge(self, re_object: "RelationEdge") -> None:
+    def set_statement(self, stm: "Statement") -> None:
         """
-        Insert a RelationEdge into the relevant data structures of the DataStorage (self)
+        Insert a Statement into the relevant data structures of the DataStorage (self)
 
         This method does not handle the dual realtion. It must be created and stored separately.
 
-        :param re_object:   RelationEdge instance
+        :param stm:   Statement instance
         :return:
         """
 
-        subj_uri = re_object.relation_tuple[0].uri
-        rel_uri = re_object.relation_tuple[1].uri
+        subj_uri = stm.relation_tuple[0].uri
+        try:
+            subj_label = str(stm.relation_tuple[0].R1)
+        except:
+            subj_label = "<unknown label>"
+
+        rel_uri = stm.relation_tuple[1].uri
         aux.ensure_valid_uri(subj_uri)
         aux.ensure_valid_uri(rel_uri)
 
-        self.relation_relation_edges[rel_uri].append(re_object)
-        self.relation_edge_uri_map[re_object.uri] = re_object
+        self.relation_statements[rel_uri].append(stm)
+        self.statement_uri_map[stm.uri] = stm
 
         relation = self.relations[rel_uri]
 
-        # inner_obj will be either a list of relation_edges or None
+        # stm_list will be either a list of statements or None
         # for some R22-related reason (see below) we cannot use a default dict here,
         # thus we need to do the case distinction manually
-        inner_obj = self.relation_edges[subj_uri].get(rel_uri, None)
+        stm_list = self.statements[subj_uri].get(rel_uri, None)
 
-        if inner_obj is None:
-            self.relation_edges[subj_uri][rel_uri] = [re_object]
+        if stm_list is None or len(stm_list) == 0:
+            self.statements[subj_uri][rel_uri] = [stm]
 
-        elif isinstance(inner_obj, list):
-            # R22__is_functional, this means there can only be one value for this relation and this item
-            if relation.R22:
+        elif isinstance(stm_list, list):
+            exception_flag = stm.get_first_qualifier_obj_with_rel(
+                "R65__allows_alternative_functional_value", tolerate_key_error=True
+            )
+            if relation.R22 and not exception_flag:
+                # R22__is_functional, this means there can only be one value for this relation and this item
                 msg = (
-                    f"for entity/relation-edge {subj_uri} there already exists a RelationEdge for "
-                    f"functional relation with key {rel_uri}. Another one is not allowed."
+                    f"for subject {subj_uri} there already exists a statement for relation {stm.predicate}. "
+                    f"This relation is functional (R22), thus another statement is not allowed."
                 )
-                raise ValueError(msg)
-            elif relation.R32:
-                # TODO: handle multiple laguages here !!qa
-                pass
-            inner_obj.append(re_object)
+                raise aux.FunctionalRelationError(msg)
+            elif relation.R32 and not exception_flag:
+                lang_list = [get_language_of_str_literal(s.object) for s in stm_list]
+                new_lang = get_language_of_str_literal(stm.object)
+                if new_lang in lang_list:
+                    msg = (
+                        f"for subject {subj_uri} ({subj_label}) there already exists statements for relation "
+                        f"{stm.predicate} with the object languages {lang_list}. This relation is functional for "
+                        f"each language (R32). Thus another statement with language `{new_lang}` is not allowed."
+                    )
+                    raise aux.FunctionalRelationError(msg)
+            stm_list.append(stm)
 
         else:
             msg = (
-                f"unexpected type ({type(inner_obj)}) of dict content for entity {subj_uri} and "
+                f"unexpected type ({type(stm_list)}) of dict content for entity {subj_uri} and "
                 f"relation {rel_uri}. Expected list or None"
             )
             raise TypeError(msg)
 
     def get_uri_for_prefix(self, prefix: str) -> str:
         res = self.uri_prefix_mapping.b.get(prefix)
 
@@ -864,35 +1030,38 @@
     :return:
     """
     assert len(l1d) == 1
     return tuple(*l1d.items())
 
 
 # define regular expressions outside of the function (they have to be compiled only once)
-# use https://pythex.org/ with fixture e. g `some_prefix__RE000['test label']` to understand these
-re_prefix_shortkey_suffix = re.compile(r"^((.+?)__)?((Ia?)|(Ra?)|(RE))(\d+)(.*)$")
+# use https://pythex.org/ with fixture e. g `some_prefix__S000['test label']` to understand these
+re_prefix_shortkey_suffix = re.compile(r"^((.+?)__)?((Ia?)|(Ra?)|(S))(\d+)(.*)$")
 re_suffix_underscore = re.compile(r"^__([\w\-]+)$")  # \w means alphanumeric (including `_`);
 re_suffix_square_brackets = re.compile(r"""^\[["'](.+)["']\]""")
 
 
 def process_key_str(
-        key_str: str, check: bool = True, resolve_prefix: bool = True, mod_uri: str = None,
+    key_str: str,
+    check: bool = True,
+    resolve_prefix: bool = True,
+    mod_uri: str = None,
 ) -> ProcessedStmtKey:
     """
     In ERK there are the following kinds of keys:
         - a) short_key like `R1234`
         - b) name-labeled key like `R1234__my_relation` (consisting of a short_key, a delimiter (`__`) and a label)
         - c) prefixed short_key like `bi__R1234`
         - d) prefixed name-labeled key like `bi__R1234__my_relation`
 
         - e) index-labeld key like  `R1234["my relation"]`
         - f) prefixed index-labeld key like  `bi__R1234["my relation"]`
 
     See also: userdoc/overview.html#keys-in-pyerk
-    
+
     Also, the leading character indicates the entity type (EType).
 
     This function expects any of these cases.
     :param key_str:     a string like "R1234__my_relation" or "R1234" or "bi__R1234__my_relation"
     :param check:       boolean flag; determines if the label part should be checked wrt its consistency to
     :param resolve_prefix:
                         boolean flag; determines if
@@ -959,43 +1128,61 @@
 
 
 def _resolve_prefix(pr_key: ProcessedStmtKey, passed_mod_uri: str = None) -> None:
     """
     get uri from prefix or from passed argument or from active module
     """
     active_mod_uri = get_active_mod_uri(strict=False)
+    if _search_uri_stack:
+        search_uri = _search_uri_stack[-1]
+    else:
+        search_uri = None
 
     if pr_key.prefix is None:
-        if active_mod_uri is None:
+        if active_mod_uri is None and search_uri is None:
             if passed_mod_uri:
                 mod_uri = passed_mod_uri
             else:
                 # assume that `builtin_entities` is meant
                 mod_uri = settings.BUILTINS_URI
         else:
             # Situation: create_item(..., R321="some value") within an active module
-            # (no prefix). short_key R321 could refer to active module or to builtin_entities -> search in this order
+            # (no prefix). short_key R321 could refer to
+            # a) the module where the function is defined which performs this call (search_uri)),
+            # b) the active module or c) builtin_entities -> search in this order
 
             # 1. check that passed_mod_uri does not contradict
-            if passed_mod_uri and (passed_mod_uri != active_mod_uri):
+            if passed_mod_uri and (passed_mod_uri not in (active_mod_uri, search_uri)):
                 msg = (
-                    f"encountered inconsistent uris for object with key_str {pr_key.original_key_str}. "
-                    f"from active mod: '{active_mod_uri}' vs explicitly passed: '{passed_mod_uri}'."
+                    f"Encountered inconsistent uris for object with key_str {pr_key.original_key_str}. "
+                    f"Explicitly passed: '{passed_mod_uri}'."
+                    f"expected one of: '{active_mod_uri}' (active mod) or '{search_uri}' (search_uri)."
                 )
                 raise aux.InvalidURIError(msg)
 
-            # 2. check active mod
-            candidate_uri = aux.make_uri(active_mod_uri, pr_key.short_key)
-            res_entity = ds.get_entity_by_uri(candidate_uri, strict=False)
+            # 2a) check search_uri context
+            if search_uri:
 
-            if res_entity is not None:
-                pr_key.uri = candidate_uri
-                return
+                candidate_uri = aux.make_uri(search_uri, pr_key.short_key)
+                res_entity = ds.get_entity_by_uri(candidate_uri, strict=False)
 
-            # try builtin_entities as fallback
+                if res_entity is not None:
+                    pr_key.uri = candidate_uri
+                    return
+
+            # 2b) check active mod
+            if active_mod_uri:
+                candidate_uri = aux.make_uri(active_mod_uri, pr_key.short_key)
+                res_entity = ds.get_entity_by_uri(candidate_uri, strict=False)
+
+                if res_entity is not None:
+                    pr_key.uri = candidate_uri
+                    return
+
+            # 2c) try builtin_entities as fallback
             candidate_uri = aux.make_uri(settings.BUILTINS_URI, pr_key.short_key)
             res_entity = ds.get_entity_by_uri(candidate_uri, strict=False)
 
             if res_entity is not None:
                 pr_key.uri = candidate_uri
                 return
             else:
@@ -1034,21 +1221,21 @@
 
     try:
         entity = ds.get_entity_by_uri(pkey.uri)
     except KeyError:
         # entity does not exist -> no label to compare with
         return
     label_compare_str1 = entity.R1
-    label_compare_str2 = entity.R1.replace(" ", "_")
+    label_compare_str2 = entity.R1.replace(" ", "_").replace("-", "_")
 
     if pkey.label.lower() not in (label_compare_str1.lower(), label_compare_str2.lower()):
         msg = (
-            f'check of label consistency failed for key {pkey.original_key_str}. Expected:  one of '
+            f"check of label consistency failed for key {pkey.original_key_str}. Expected:  one of "
             f'("{label_compare_str1}", "{label_compare_str2}") but got  "{pkey.label}". '
-            'Note: this test is *not* case-sensitive.'
+            "Note: this test is *not* case-sensitive."
         )
         raise ValueError(msg)
 
 
 def u(key_str: str) -> str:
     """
     Convenience function converting "[prefix__]I1234__my_label"  to "[moduri#]I1234".
@@ -1065,28 +1252,35 @@
 
 # noinspection PyShadowingNames
 class Item(Entity):
     def __init__(self, base_uri: str, key_str: str, **kwargs):
         super().__init__(base_uri=base_uri)
 
         res = process_key_str(key_str, check=False, resolve_prefix=False)
-        assert res.etype == EType.ITEM
+        msg = f"invalid entity type deduced from key string: {key_str}: expected {EType.ITEM} but got {res.etype}."
+        assert res.etype == EType.ITEM, msg
 
         self.short_key = res.short_key
         self.uri = aux.make_uri(self.base_uri, self.short_key)
+
+        assert self.uri not in ds.items, f"{self.uri} is already occupied. Cannot create new item."
+
         self._set_relations_from_init_kwargs(**kwargs)
 
         self.__post_init__()
 
     def __repr__(self):
-        try:
-            R1 = getattr(self, "R1", "no label")
-        except ValueError:
-            R1 = "<<ValueError while retrieving R1>>"
-        return f'<Item {self.short_key}["{R1}"]>'
+        if not self._unlinked:
+            try:
+                r1 = getattr(self, "R1", "no label")
+            except ValueError:
+                r1 = "<<ValueError while retrieving R1>>"
+        else:
+            r1 = getattr(self, "_label_after_unlink", "no label")
+        return f'<Item {self.short_key}["{r1}"]>'
 
 
 def get_active_mod_uri(strict: bool = True) -> Union[str, None]:
     try:
         res = _uri_stack[-1]
     except IndexError:
         msg = (
@@ -1151,16 +1345,19 @@
 
         # set label
         self._set_relations_from_init_kwargs(**kwargs)
 
         self.__post_init__()
 
     def __repr__(self):
-        R1 = getattr(self, "R1", "no label")
-        return f'<Relation {self.short_key}["{R1}"]>'
+        if not self._unlinked:
+            r1 = getattr(self, "R1", "no label")
+        else:
+            r1 = getattr(self, "_label_after_unlink", "no label")
+        return f'<Relation {self.short_key}["{r1}"]>'
 
 
 @unique
 class RelationRole(Enum):
     """
     Statement types.
     """
@@ -1231,15 +1428,15 @@
 
     :param prefix:
     :param prefix2:
     :return:
     """
 
     active_mod_uri = get_active_mod_uri()
-    km = ds.uri_keymanager_dict[active_mod_uri]
+    km: KeyManager = ds.uri_keymanager_dict[active_mod_uri]
     num_key = km.pop()
     if prefix is None:
         assert not prefix2
         return num_key
 
     assert prefix in ("I", "R")
 
@@ -1249,16 +1446,16 @@
 
 def repl_spc_by_udsc(txt: str) -> str:
     return txt.replace(" ", "_")
 
 
 class RawQualifier:
     """
-    Precursor to a real Qualifier (which is a RelationEdge) where the subject is yet unspecified
-    (will be the qualified RelationEdge). Instances of this class are produced by QualifierFactory
+    Precursor to a real Qualifier (which is a Statement) where the subject is yet unspecified
+    (will be the qualified Statement). Instances of this class are produced by QualifierFactory
     """
 
     def __init__(self, rel: Relation, obj: Union[Literal, Entity]):
         self.rel = rel
         self.obj = obj
 
     def __repr__(self):
@@ -1297,28 +1494,28 @@
             assert isinstance(registry_name, str) and registry_name not in ds.qff_dict
             ds.qff_dict[registry_name] = self
 
     def __call__(self, obj):
         return RawQualifier(self.relation, obj)
 
 
-class RelationEdge:
+class Statement:
     """
     Models a conrete (instantiated/applied) relation between entities. This is basically a dict.
     """
 
     def __init__(
         self,
         relation: Relation = None,
         relation_tuple: tuple = None,
         role: RelationRole = None,
         corresponding_entity: Entity = None,
         corresponding_literal=None,
         scope=None,
-        qualifiers: Optional[List[RawQualifier]] = None,
+        qualifiers: Optional[Union[List[RawQualifier], List["QualifierStatement"]]] = None,
         proxyitem: Optional[Item] = None,
     ) -> None:
         """
 
         :param relation:
         :param relation_tuple:
         :param role:                    RelationRole.SUBJECT for normal and RelationRole.OBJECT for inverse edges
@@ -1327,173 +1524,188 @@
         :param corresponding_literal:   This is the literal on the "other side" of the relation (depending of `role`) or
         :param scope:                   None in case that other side is an Entity
         :param qualifiers:              list of relation edges, that describe `self` more precisely
                                         (cf. wikidata qualifiers)
         :param proxyitem:               associated item; e.g. a equation-item
         """
 
-        self.short_key = f"RE{pop_uri_based_key()}"
+        # S means "statement" (successor of earlier RE for "relation edge")
+        self.short_key = f"S{pop_uri_based_key()}"
         mod_uri = get_active_mod_uri()
         self.base_uri = mod_uri
         self.uri = f"{aux.make_uri(self.base_uri, self.short_key)}"
         self.relation = relation
         self.rsk = relation.short_key  # to conviniently access this attribute in visualization
         self.relation_tuple = relation_tuple
         self.subject = relation_tuple[0]
         self.predicate = relation_tuple[1]
         self.object = relation_tuple[2]
         self.role = role
         self.scope = scope
         self.corresponding_entity = corresponding_entity
         self.corresponding_literal = corresponding_literal
+        self.dual_statement = None
+        self.unlinked = None
         self.qualifiers = []
         self._process_qualifiers(qualifiers)
-        self.dual_relation_edge = None
-        self.unlinked = None
 
-        ds.rledgs_created_in_mod[mod_uri][self.uri] = self
+        ds.stms_created_in_mod[mod_uri][self.uri] = self
 
-        assert self.uri not in ds.relation_edge_uri_map
-        ds.relation_edge_uri_map[self.uri] = self
+        assert self.uri not in ds.statement_uri_map
+        ds.statement_uri_map[self.uri] = self
 
         # TODO: replace this by qualifier
         self.proxyitem = proxyitem
 
     @property
     def key_str(self):
-        # TODO: the "attribute" `.key_str` for RelationEdge is deprecated; use `.short_key` instead
+        # TODO: the "attribute" `.key_str` for Statement is deprecated; use `.short_key` instead
         return self.short_key
 
     def __repr__(self):
 
         res = f"{self.short_key}{self.relation_tuple}"
         return res
 
-    def _process_qualifiers(self, qlist: List[RawQualifier], scope: Optional["Entity"] = None) -> None:
+    def _process_qualifiers(
+        self, qlist: Union[List[RawQualifier], List["QualifierStatement"]], scope: Optional["Entity"] = None
+    ) -> None:
 
-        if qlist is None:
+        if not qlist:
             # nothing to do
             return
 
+        if isinstance(qlist[0], QualifierStatement):
+            # this is the case when an inverse statement is created
+            self.qualifiers = [*qlist]
+            return
+
         for qf in qlist:
 
             if isinstance(qf.obj, Entity):
                 corresponding_entity = qf.obj
                 corresponding_literal = None
             else:
                 corresponding_entity = None
                 corresponding_literal = repr(qf.obj)
 
-            qf_rledg = RelationEdge(
+            qf_stm = QualifierStatement(
                 relation=qf.rel,
                 relation_tuple=(self, qf.rel, qf.obj),
                 role=RelationRole.SUBJECT,
                 corresponding_entity=corresponding_entity,
                 corresponding_literal=corresponding_literal,
                 scope=scope,
                 qualifiers=None,
                 proxyitem=None,
             )
-            self.qualifiers.append(qf_rledg)
-
-            # save the qualifyer-relation edge (and its inverse) in the appropriate data structures
+            self.qualifiers.append(qf_stm)
 
-            # this is the RelationEdge from the original RE instance to the object (thus role=SUBJECT)
-            ds.set_relation_edge(re_object=qf_rledg)
+            # save the qualifier statement in the appropriate data structures
+            ds.set_statement(stm=qf_stm)
 
-            # we might also need dual edge
             if isinstance(qf.obj, Entity):
-                # add inverse relation
-                dual_rledg = qf_rledg.create_dual()
-                ds.inv_relation_edges[qf.obj.uri][qf.rel.uri].append(dual_rledg)
-
-    def create_dual(self):
-        if self.role == RelationRole.SUBJECT:
-            new_role = RelationRole.OBJECT
-        elif self.role == RelationRole.OBJECT:
-            new_role = RelationRole.SUBJECT
-        else:
-            msg = (
-                f"Unexpected value for `self.role`: {self.role}. Expected either `RelationRole.SUBJECT` or "
-                "`RelationRole.OBJECT`"
-            )
-            raise ValueError(msg)
+                ds.inv_statements[qf.obj.uri][qf.rel.uri].append(qf_stm)
 
-        dual_rledg = RelationEdge(
-            relation=self.relation,
-            relation_tuple=self.relation_tuple,
-            role=new_role,
-            corresponding_entity=self.corresponding_entity,
-            scope=self.scope,
-            qualifiers=self.qualifiers,
-            proxyitem=self.proxyitem,
-        )
+    def is_qualifier(self):
+        # TODO: replace this by isinstance(stm, QualifierStatement)
+        return isinstance(self.subject, Statement)
 
-        # establish interconnection
-        dual_rledg.dual_relation_edge = self
-        self.dual_relation_edge = dual_rledg
+    def get_first_qualifier_obj_with_rel(self, key=None, uri=None, tolerate_key_error=False):
+        assert [key, uri].count(None) == 1, "exactly one of the arguments must be provided, not 0 not 2"
 
-        return dual_rledg
+        if key:
+            try:
+                uri = process_key_str(key).uri
+            except KeyError:
+                if tolerate_key_error:
+                    # this allows to ask for qualifiers before they are created
+                    return None
+                else:
+                    raise
+
+        for qstm in self.qualifiers:
+            if qstm.predicate.uri == uri:
+                return qstm.object
 
-    def is_qualifier(self):
-        return isinstance(self.subject, RelationEdge)
+        return None
 
     def unlink(self, *args) -> None:
         """
-        Remove this RelationEdge instance from all data structures in the global data storage
+        Remove this Statement instance from all data structures in the global data storage
         :return:
         """
 
         if not len(self.relation_tuple) == 3:
             raise NotImplementedError
 
         if self.unlinked:
             return
 
         subj, pred, obj = self.relation_tuple
 
-        if self.is_qualifier():
-            # _xx !! -> uri
-            _ = ds.relation_edges.pop(subj.uri, [])
+        if isinstance(self, QualifierStatement):
+            ds.statements.pop(subj.uri, None)
+
+            assert isinstance(subj, Statement)
+
+            # seems like during unloading of modules the qualifiers might already have been removed
+            # -> do nothing
+            try:
+                subj.qualifiers.remove(self)
+            except ValueError:
+                pass
+            try:
+                subj.dual_statement.qualifiers.remove(self)
+            except (ValueError, AttributeError):
+                # AttributeError means that dual_statement was None
+                pass
 
         if self.role == RelationRole.SUBJECT:
 
-            subj_rel_edges: Dict[str : List[RelationEdge]] = ds.relation_edges[subj.uri]
+            subj_rel_edges: Dict[str : List[Statement]] = ds.statements[subj.uri]
             tolerant_removal(subj_rel_edges.get(pred.uri, []), self)
 
-            # ds.relation_relation_edges: for every relation key stores a list of relevant relation-edges
+            # ds.relation_statements: for every relation key stores a list of relevant relation-edges
             # (check before accessing the *defaultdict* to avoid to create a key just by looking)
-            if pred.uri in ds.relation_relation_edges:
-                tolerant_removal(ds.relation_relation_edges.get(pred.uri, []), self)
+            if pred.uri in ds.relation_statements:
+                tolerant_removal(ds.relation_statements.get(pred.uri, []), self)
 
         elif self.role == RelationRole.OBJECT:
             assert isinstance(obj, Entity)
-            obj_rel_edges: Dict[str : List[RelationEdge]] = ds.inv_relation_edges[obj.uri]
+            obj_rel_edges: Dict[str : List[Statement]] = ds.inv_statements[obj.uri]
             # (check before accessing, see above)
             if pred.uri in obj_rel_edges:
                 tolerant_removal(obj_rel_edges[pred.uri], self)
         else:
             msg = f"Unexpected .role attribute: {self.role}"
             raise ValueError(msg)
 
         # this prevents from infinite recursion
         self.unlinked = True
-        if self.dual_relation_edge is not None:
-            self.dual_relation_edge.unlink()
+        if self.dual_statement is not None:
+            self.dual_statement.unlink()
 
         for qf in self.qualifiers:
-            qf: RelationEdge
+            qf: Statement
             qf.unlink()
 
-        ds.relation_edge_uri_map.pop(self.uri)
+        ds.statement_uri_map.pop(self.uri)
 
         # TODO: remove obsolete key-recycling
         ds.released_keys.append(self.short_key)
 
 
+class QualifierStatement(Statement):
+    def __init__(self, *args, **kwargs):
+        # self.dual_qualifier = None
+        super().__init__(*args, **kwargs)
+        self.short_key = f"Q{self.short_key}"
+
+
 def tolerant_removal(sequence, element):
     """
     call sequence.remove(element) but tolerate KeyError and ValueError
     :param sequence:
     :param element:
     :return:
     """
@@ -1535,15 +1747,17 @@
         if processed_key.etype != EType.RELATION:
             msg = f"unexpected key: {key} during creation of item {rel_key}."
             raise ValueError(msg)
 
         new_kwargs[processed_key.short_key] = value
 
     rel = Relation(mod_uri, rel_key, **new_kwargs)
-    assert rel.uri not in ds.relations
+    if rel.uri in ds.relations:
+        msg = f"URI '{rel.uri}' has already been used."
+        raise aux.InvalidURIError(msg)
     ds.relations[rel.uri] = rel
     ds.entities_created_in_mod[mod_uri].append(rel.uri)
     return rel
 
 
 def create_builtin_item(*args, **kwargs) -> Item:
     with uri_context(uri=settings.BUILTINS_URI):
@@ -1702,45 +1916,59 @@
     """
 
     def __init__(self, *args, **kwargs):
         pass
 
 
 _uri_stack = []
+_search_uri_stack = []
 
 
-class uri_context:
-    """
-    Context manager for creating entities with a given uri
-    """
-
-    def __init__(self, uri: str, prefix: str = None):
+class abstract_uri_context:
+    def __init__(self, uri_stack: list, uri: str, prefix: str = None):
+        self.uri_stack = uri_stack
         self.uri = uri
         self.prefix = prefix
 
     def __enter__(self):
         """
         implicitly called in the head of the with statemet
         :return:
         """
-        _uri_stack.append(self.uri)
+        self.uri_stack.append(self.uri)
 
         if self.prefix:
             ds.uri_prefix_mapping.add_pair(self.uri, self.prefix)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         # this is the place to handle exceptions
 
-        res = _uri_stack.pop()
+        res = self.uri_stack.pop()
         assert res == self.uri
         if self.prefix:
             ds.uri_prefix_mapping.remove_pair(self.uri, self.prefix)
 
 
+class uri_context(abstract_uri_context):
+    """
+    Context manager for creating entities with a given uri
+    """
+    def __init__(self, uri: str, prefix: str = None):
+        super().__init__(_uri_stack, uri, prefix)
+
+
+class search_uri_context(abstract_uri_context):
+    """
+    uri Context manager for searching for entities with a given key
+    """
+    def __init__(self, uri: str, prefix: str = None):
+        super().__init__(_search_uri_stack, uri, prefix)
+
+
 def unload_mod(mod_uri: str, strict=True) -> None:
     """
     Delete all references to entities comming from a module with `mod_id`
 
     :param mod_uri: str; uri of the module, see its __URI__ attribute
     :param strict:  boolean; raise Exception if module seems be not loaded
 
@@ -1749,43 +1977,44 @@
 
     # prepare the list to store the released keys
     ds.released_keys.clear()
 
     # TODO: This might to check dependencies in the future
 
     entity_uris: List[str] = ds.entities_created_in_mod.pop(mod_uri, [])
+    stm_dict = ds.stms_created_in_mod.pop(mod_uri, {})
 
-    if not entity_uris and strict:
-        msg = f"Seems like no entities from {mod_uri} have been loaded. This is unexpected."
+    if strict and (not entity_uris and not stm_dict):
+        msg = f"Seems like neither entities nor statements from {mod_uri} have been loaded. This is unexpected."
         raise KeyError(msg)
 
     for uri in entity_uris:
         _unlink_entity(uri)
-        assert uri not in ds.relation_relation_edges.keys()
+        assert uri not in ds.relation_statements.keys()
 
-    intersection_set = set(entity_uris).intersection(ds.relation_relation_edges.keys())
+    intersection_set = set(entity_uris).intersection(ds.relation_statements.keys())
 
     msg = "Unexpectedly some of the entity keys are still present"
     assert len(intersection_set) == 0, msg
 
-    rledg_dict = ds.rledgs_created_in_mod.pop(mod_uri, {})
-    for uri, rledg in rledg_dict.items():
-        assert isinstance(rledg, RelationEdge)
-        rledg.unlink()
+    for uri, stm in stm_dict.items():
+        stm: Statement
+        assert isinstance(stm, Statement)
+        stm.unlink()
 
     try:
         ds.mod_path_mapping.remove_pair(key_a=mod_uri)
     except KeyError:
         if strict:
             raise
         else:
             pass
 
-    aux.clean_dict(ds.relation_edges)
-    aux.clean_dict(ds.inv_relation_edges)
+    aux.clean_dict(ds.statements)
+    aux.clean_dict(ds.inv_statements)
 
     # TODO: obsolete
     res = list(ds.released_keys)
 
     try:
         ds.uri_keymanager_dict.pop(mod_uri)
     except KeyError:
@@ -1803,76 +2032,174 @@
     if modname := ds.modnames.get(mod_uri):
         sys.modules.pop(modname)
 
     # empty the list again to avoid confusion in future uses
     ds.released_keys.clear()
 
 
-def _unlink_entity(uri: str) -> None:
+def _unlink_entity(uri: str, remove_from_mod=False) -> None:
     """
     Remove the occurrence of this the respective entitiy from all relevant data structures
 
     :param uri:     entity uri
     :return:        None
     """
+    assert isinstance(uri, str)
     aux.ensure_valid_uri(uri)
     entity: Entity = ds.get_entity_by_uri(uri)
+    r1 = getattr(entity, "R1", "<unknown entity>")
+    entity._label_after_unlink = f"!!unlinked: {r1}"
+    entity._unlinked = True
+    ds.unlinked_entities[uri] = entity
+
+    if remove_from_mod:
+        mod_uri = uri.split("#")[0]
+        mod_entities = ds.entities_created_in_mod[mod_uri]
+
+        # TODO: this could be speed up by using a dict instead of a list for mod_entities
+        mod_entities.remove(uri)
+
     res1 = ds.items.pop(uri, None)
     res2 = ds.relations.pop(uri, None)
 
-    if uri == "Ia9108":
-        pass
-        # set_trace()
-
     if res1 is None and res2 is None:
         msg = f"No entity with key {uri} could be found. This is unexpected."
         raise KeyError(msg)
 
     # now delete the relation edges from the data structures
-    re_dict = ds.relation_edges.pop(entity.uri, {})
-    inv_re_dict = ds.inv_relation_edges.pop(entity.uri, {})
+    re_dict = ds.statements.pop(entity.uri, {})
+    inv_re_dict = ds.inv_statements.pop(entity.uri, {})
 
     # in case res1 is a scope-item we delete all corressponding relation edges, otherwise nothing happens
-    scope_rels = ds.scope_relation_edges.pop(uri, [])
+    scope_rels = ds.scope_statements.pop(uri, [])
 
     re_list = list(scope_rels)
 
-    # create a item-list of all RelationEdges instances where `ek` is involved either as subject or object
+    # create a item-list of all Statements instances where `ek` is involved either as subject or object
     re_item_list = list(re_dict.items()) + list(inv_re_dict.items())
 
     for rel_uri, local_re_list in re_item_list:
         # rel_uri: uri of the relation (like "pyerk/foo#R1234")
-        # re_list: list of RelationEdge instances
+        # re_list: list of Statement instances
         re_list.extend(local_re_list)
 
     if isinstance(entity, Relation):
 
-        tmp = ds.relation_relation_edges.pop(uri, [])
+        tmp = ds.relation_statements.pop(uri, [])
         re_list.extend(tmp)
 
-    # now iterate over all RelationEdge instances
-    for re in re_list:
-        re: RelationEdge
-        re.unlink(uri)
+    # now iterate over all Statement instances
+    for stm in re_list:
+        stm: Statement
+        stm.unlink(uri)
 
-    # during unlinking of the RelationEdges the default dicts might have been recreating some keys -> pop again
+    # during unlinking of the Statements the default dicts might have been recreating some keys -> pop again
     # TODO: obsolete because we clean up the defaultdicts anyway
-    ds.relation_edges.pop(entity.uri, None)
-    ds.inv_relation_edges.pop(entity.uri, None)
+    ds.statements.pop(entity.uri, None)
+    ds.inv_statements.pop(entity.uri, None)
 
     ds.released_keys.append(uri)
 
 
+def replace_and_unlink_entity(old_entity: Entity, new_entity: Entity):
+    """
+    Replace all statements where `old_entity` is subject or object with new relations where `new_entity` is sub or obj.
+    For the "subject-case" only process those statements for which `new_entity` does not yet have any relations.
+    Thus do not replace e.g. the R4__is_instance_of statement of `new_entity`.
+
+    Then unlink `old_entity`.
+    """
+
+    res = RuleResult()
+
+    from pyerk import builtin_entities as bi
+
+    # these predicates should not be replaced
+    omit_uris = aux.uri_set(
+        bi.R1["has label"], bi.R2["has description"], bi.R4["is instance of"], bi.R57["is placeholder"]
+    )
+
+    # ensure both entities exist (raise UnknownURIError otherwise):
+    ds.get_entity_by_uri(old_entity.uri)
+    ds.get_entity_by_uri(new_entity.uri)
+
+    stm_dict1 = old_entity.get_inv_relations()  # where it is obj
+    stm_dict2 = old_entity.get_relations()  # where it is subj
+
+    _unlink_entity(old_entity.uri, remove_from_mod=True)
+    res.unlinked_entities.append(old_entity)
+    res.replacements.append((old_entity, new_entity))
+
+    for relation_uri, stm_list in list(stm_dict1.items()) + list(stm_dict2.items()):
+        for stm in stm_list:
+            new_stm = None
+            stm: Statement
+            subject, predicate, obj = stm.relation_tuple
+            if predicate.uri in omit_uris:
+                continue
+            subject: Item
+            qlf = stm.qualifiers
+            if obj == old_entity:
+                # case1: old_entity was object, subject stays the same
+                new_stm = subject.set_relation(predicate, new_entity, qualifiers=qlf, prevent_duplicate=True)
+                res.add_statement(new_stm)
+                continue
+            else:
+                # case2: old_entity was subject, subject must be new_entity
+                assert subject == old_entity
+
+                # prevent the creation of a duplicated statement
+                existing_objs = new_entity.get_relations(predicate.uri, return_obj=True)
+                if not obj in existing_objs:
+
+                    # it is possible that predicate is functional and new_entitiy.predicate has a value
+                    # different from obj. this is OK if one of them is a placeholder
+                    if len(existing_objs) == 1 and predicate.R22__is_functional:
+                        existing_obj = existing_objs[0]
+                        if obj.R57__is_placeholder:
+                            # ignore it -> continue with next statement
+                            continue
+                        elif not existing_obj.R57__is_placeholder and not obj.R57__is_placeholder:
+                            msg = (
+                                f"confilicting statement for functional predicate {predicate} and non-placeholder "
+                                f"objects: {obj} (of old_entity)  and {existing_obj} of new_entity, while replacing"
+                                f"{old_entity} (old) with {new_entity} (new)."
+                            )
+                            raise aux.FunctionalRelationError(msg)
+                        else:
+                            assert existing_obj.R57__is_placeholder and not obj.R57__is_placeholder
+                            # replace the placeholder with the non-placeholder information
+                            chgd_stm = new_entity.overwrite_statement(predicate.uri, obj, qualifiers=qlf)
+                            res.changed_statements.append(chgd_stm)
+                            continue
+                    else:
+                        # no replacement has to be made
+                        new_stm = new_entity.set_relation(predicate, obj, qualifiers=qlf)
+                        res.add_statement(new_stm)
+                        continue
+                else:
+                    assert obj in existing_objs
+                    # no new information available -> continue with next statement
+                    continue
+
+    return res
+
+
 def register_mod(uri: str, keymanager: KeyManager, check_uri=True):
     frame = get_caller_frame(upcount=1)
     path = os.path.abspath(frame.f_globals["__file__"])
     if check_uri:
         assert frame.f_globals.get("__URI__", None) == uri
     if uri != settings.BUILTINS_URI:
         # the builtin module is an exception because it should not be unloaded
+
+        if uri in ds.mod_path_mapping.a:
+            msg = f"URI '{uri}' was already registered by {ds.mod_path_mapping.a[uri]}."
+            raise aux.InvalidURIError(msg)
+
         ds.mod_path_mapping.add_pair(key_a=uri, key_b=path)
 
     # all modules should have their own key manager
     ds.uri_keymanager_dict[uri] = keymanager
 
 
 def start_mod(uri):
@@ -1889,14 +2216,21 @@
 
 
 def end_mod():
     _uri_stack.pop()
     assert len(_uri_stack) == 0
 
 
+def get_language_of_str_literal(obj: Union[str, Literal]):
+    if isinstance(obj, Literal):
+        return obj.language
+
+    return None
+
+
 class LangaguageCode:
     def __init__(self, langtag):
         assert langtag in settings.SUPPORTED_LANGUAGES
 
         self.langtag = langtag
 
     def __rmatmul__(self, arg: str) -> Literal:
@@ -1914,9 +2248,91 @@
         return res
 
 
 en = LangaguageCode("en")
 de = LangaguageCode("de")
 
 
+class RuleResult:
+    def __init__(self):
+        self.new_statements = []
+        self.changed_statements = []
+        self.new_entities = []
+        self.unlinked_entities = []
+        self.partial_results = []
+        self.replacements = []
+        self._rule = None
+        self.apply_time = None
+        self.exception = None
+        self.creator_object = None
+
+        # dict like {rel_uri1: [stm1, stm2, ...]}
+        # maps a relation uri to a list of statements which have this relation as predicate
+        self.rel_map = defaultdict(list)
+
+    def add_statement(self, stm: Statement):
+        if stm is None:
+            return
+        assert stm not in self.new_statements
+        self.new_statements.append(stm)
+        self.rel_map[stm.predicate.uri].append(stm)
+
+    def add_statements(self, stms: List[Statement]):
+        for stm in stms:
+            self.add_statement(stm)
+
+    def add_entity(self, entity: Entity):
+        self.new_entities.append(entity)
+
+    def extend(self, part: "RuleResult"):
+        assert isinstance(part, RuleResult)
+        self.add_statements(part.new_statements)
+        self.new_entities.extend(part.new_entities)
+        self.unlinked_entities.extend(part.unlinked_entities)
+        self.replacements.extend(part.replacements)
+        if part.exception:
+            self.exception = part.exception
+
+    def add_partial(self, part: "RuleResult"):
+        if self.apply_time is None:
+            self.apply_time = 0
+
+        self.apply_time += part.apply_time
+        self.extend(part)
+        self.partial_results.append(part)
+
+    def __repr__(self):
+        if self.apply_time is None:
+            aplt = "? s"
+        else:
+            aplt = f"{round(self.apply_time, 3)} s"
+        res = (
+            f"{type(self).__name__} ({aplt}): new_stms: {len(self.new_statements)}, parts: {len(self.partial_results)}"
+        )
+        return res
+
+    @property
+    def rule(self):
+        """
+        Convenience property for easy access to the corresponding rule
+        """
+        if self._rule is None:
+            if self.partial_results:
+                return self.partial_results[0].rule
+
+        return self._rule
+
+
+def format_entity_html(e: Entity):
+
+    short_txt = f'<span class="entity">{e.R1}</span>'
+    detailed_txt = f'<span class="entity">{e.short_key}["{e.R1}"]</span>'
+
+    return f'<span class="js-toggle" data-short-txt="{quote(short_txt)}" data-detailed-txt="{quote(detailed_txt)}">{short_txt}</span>'
+
+
+def format_literal_html(obj):
+    return f'<span class="literal">{repr(obj)}</span>'
+
+
 def script_main(fpath):
     IPS()
```

### Comparing `pyerk-0.6.5/src/pyerk/reportgenerator.py` & `pyerk-0.8.5/src/pyerk/reportgenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from . import erkloader
 import pyerk as p
 from pyerk.erkloader import preserve_cwd
 
 from . import settings
 
 
-
-
 def generate_report(reportconf_path: str):
 
     rg = ReportGenerator(reportconf_path)
     rg.generate_report()
 
 
 class ReportGenerator:
@@ -41,17 +39,15 @@
         self.authors = None
         self.content = None
         self.reportconf = resolve_entities_in_nested_data(self.reportconf_raw)
         self.resolve_entities()
 
     @staticmethod
     def load_report_conf(reportconf_path: str) -> dict:
-        """
-
-        """
+        """ """
 
         os.chdir(p.aux.startup_workdir)
         try:
             with open(reportconf_path, "rb") as fp:
                 conf = tomllib.load(fp)
         except FileNotFoundError:
             raise
@@ -78,15 +74,15 @@
         self.authors = self.reportconf.get("authors").values()
         self.content = self.reportconf.get("content")
         assert len(self.authors) > 0
         assert len(self.content) > 0
 
     def generate_report(self):
         jin_env = Environment(loader=FileSystemLoader(settings.TEMPLATE_PATH))
-        template_doc = jin_env.get_template('report-template.tex')
+        template_doc = jin_env.get_template("report-template.tex")
 
         # WIP!
         affiliations = []
         af_counter = 1
         for at in self.authors:
 
             af_list = at.get("affiliation", [])
```

### Comparing `pyerk-0.6.5/src/pyerk/script.py` & `pyerk-0.8.5/src/pyerk/script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 """
 Command line interface for erk package
 """
 import os
 import argparse
+from pathlib import Path
+
+try:
+    # this will be part of standard library for python >= 3.11
+    import tomllib
+except ModuleNotFoundError:
+    import tomli as tomllib
+
+
+
+
 from . import core, erkloader, rdfstack
 from . import visualization
 from . import reportgenerator
 from . import auxiliary as aux
 from . import settings
+from . import release
 
 from ipydex import IPS, activate_ips_on_exception
 
 activate_ips_on_exception()
 
 
 def create_parser():
@@ -36,20 +48,28 @@
         type=int,
         metavar="NUMBER_OF_NEW_KEYS",
     )
 
     parser.add_argument(
         "-l",
         "--load-mod",
-        help="load module from path with prefix.",
+        help="load module (.py file) from path with prefix.",
         nargs=2,
         default=None,
         metavar=("MOD_PATH", "PREFIX"),
     )
 
+    parser.add_argument(
+        "-lp",
+        "--load-package",
+        help="load erk package (represented by erkpackage.tomle file)",
+        default=None,
+        metavar=("PACKAGE_TOML_PATH"),
+    )
+
     # background: in earlier versions default erk-module paths were specified wrt the path of the
     # pyerk.core python module (and thus not wrt the current working dir).
     # This flag served to switch to "real" paths (interpreted wrt the current working directory)
     # This behavior is now deprecated
     parser.add_argument(
         "-rwd",
         "--relative-to-workdir",
@@ -82,15 +102,15 @@
         help="create a visualization for the entity",
         metavar="uri",
     )
 
     parser.add_argument(
         "-i",
         "--interactive-session",
-        help="start an interactive session (with the specified module loaded)",
+        help="start an interactive session (with the specified module/package loaded)",
         action="store_true",
     )
 
     parser.add_argument(
         "-dj",
         "--start-django",
         help="start the django server from the current directory",
@@ -100,36 +120,54 @@
     parser.add_argument(
         "-djs",
         "--start-django-shell",
         help="start the django shell from the current directory (mainly useful for development)",
         action="store_true",
     )
 
+    parser.add_argument("--dbg", help="start debug routine", default=None, action="store_true")
+
     parser.add_argument(
-        "--dbg", help="start debug routine", default=None, action="store_true"
+        "--version",
+        help="print the version and exit",
+        action="store_true",
     )
-    
+
     return parser
-    
+
 
 def main():
 
     args = create_parser().parse_args()
 
     if args.dbg:
         debug()
         exit()
 
+    if args.version:
+        print(release.__version__)
+        exit()
+
+    if args.load_mod is not None and args.load_package is not None:
+        print(aux.byellow(
+            "The options to load a module and to load a package are mutually exclusive"
+        ))
+        exit()
+        
     if args.load_mod is not None:
 
         path, prefix = args.load_mod
         loaded_mod = process_mod(path=path, prefix=prefix, relative_to_workdir=True)
+    elif args.load_package is not None:
+        loaded_mod, prefix = process_package(args.load_package)
     else:
         loaded_mod = None
         prefix = None
+        
+
 
     if args.interactive_session:
         interactive_session(loaded_mod, prefix)
         exit()
 
     # typical calls to generate new keys:
     # pyerk --new-keys 30 --load-mod ../knowledge-base/rules/rules1.py rl
@@ -156,62 +194,68 @@
             uri = key
         aux.ensure_valid_uri(uri)
         visualization.visualize_entity(uri, write_tmp_files=True)
     elif args.start_django:
         try:
             import pyerkdjango.core
         except ImportError:
-            print(
-                aux.bred("Error:"), "the module pyerkdjango seems not to be installed."
-            )
+            print(aux.bred("Error:"), "the module pyerkdjango seems not to be installed.")
             # exit(10)
             raise
         pyerkdjango.core.start_django()
     elif args.start_django_shell:
         try:
             import pyerkdjango.core
         except ImportError:
-            print(
-                aux.bred("Error:"), "the module pyerkdjango seems not to be installed."
-            )
+            print(aux.bred("Error:"), "the module pyerkdjango seems not to be installed.")
             # exit(10)
             raise
         pyerkdjango.core.start_django_shell()
     else:
         print("nothing to do, see option `--help` for more info")
 
 
-def process_mod(
-    path: str, prefix: str, relative_to_workdir: bool = False
-) -> erkloader.ModuleType:
+def process_package(pkg_path: str) -> erkloader.ModuleType:
+    
+    
+    if os.path.isdir(pkg_path):
+        pkg_path = os.path.join(pkg_path, "erkpackage.toml")
+    
+    with open(pkg_path, "rb") as fp:
+        erk_conf_dict = tomllib.load(fp)
+    ocse_main_rel_path = erk_conf_dict["main_module"]
+    main_module_prefix = erk_conf_dict["main_module_prefix"]
+    ocse_main_mod_path = Path(pkg_path).parent.joinpath(ocse_main_rel_path).as_posix()
+    
+    mod = erkloader.load_mod_from_path(modpath=ocse_main_mod_path, prefix=main_module_prefix)
+    return mod, main_module_prefix
+
+
+def process_mod(path: str, prefix: str, relative_to_workdir: bool = False) -> erkloader.ModuleType:
 
     if not relative_to_workdir:
         msg = "using mod paths which are not relative to workdir is deprecated since pyerk version 0.6.0"
         raise DeprecationWarning(msg)
 
     smart_relative = None
-    mod1 = erkloader.load_mod_from_path(
-        path, prefix=prefix, smart_relative=smart_relative
-    )
+    mod1 = erkloader.load_mod_from_path(path, prefix=prefix, smart_relative=smart_relative)
 
     # perform sanity check
     # rdfstack.check_all_relation_types()
     return mod1
 
 
 def debug():
     """
     Debug function for development of core and script modules.
     To interactively examine modules (builtin and others) use `--interactive-session`
     """
 
     ERK_ROOT_DIR = aux.get_erk_root_dir()
-    TEST_DATA_PATH = os.path.join(
-        ERK_ROOT_DIR, "erk-data", "ocse", "control_theory1.py"
-    )
+    TEST_DATA_PATH = os.path.join(ERK_ROOT_DIR, "erk-data", "ocse", "control_theory1.py")
     mod1 = erkloader.load_mod_from_path(TEST_DATA_PATH, prefix="ct")  # noqa
     ds = core.ds
     ds.rdfgraph = rdfstack.create_rdf_triples()
     qsrc = rdfstack.get_sparql_example_query2()
     res = ds.rdfgraph.query(qsrc)
     z = aux.apply_func_to_table_cells(rdfstack.convert_from_rdf_to_pyerk, res)  # noqa
     IPS()
```

### Comparing `pyerk-0.6.5/src/pyerk/settings.py` & `pyerk-0.8.5/src/pyerk/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # This is the settings module of pyerk (backend). It is assumed to take precedence over django settings.
 
 import os
 import sys
+import logging
 
 try:
     # this will be part of standard library for python >= 3.11
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
+logger = logging.getLogger("pyerk")
+
 # for now we only support a subset of languages with wich the authors are familiar
 # if you miss a language, please consider contributing
 SUPPORTED_LANGUAGES = ["en", "de"]
 # https://en.wikipedia.org/wiki/IETF_language_tag
 
 
 # TODO: This should be specifyable for every module
@@ -31,21 +34,25 @@
 URI_SEP = "#"
 
 # todo: some time in the future pyerk should become indendent from the OCSE
 # for now it is convenient to have the URI stored here
 OCSE_URI = "erk:/ocse/0.2"
 
 
+# this is relevant to look for pyerk-data to load (specified by a configuration file)
 BASE_DIR = os.getenv("PYERK_BASE_DIR", "")
 if not BASE_DIR:
     BASE_DIR = "./"
 BASE_DIR = os.path.abspath(BASE_DIR)
 
 
-confpath = os.path.join(BASE_DIR, "erkpackage.toml")
-
+confpath = os.getenv("PYERK_CONF_PATH", "")
+if not confpath:
+    confpath = os.path.join(BASE_DIR, "erkpackage.toml")
 
 try:
     with open(confpath, "rb") as fp:
         CONF = tomllib.load(fp)
 except FileNotFoundError:
+    msg = f"file not found: {confpath}"
+    logger.warning(msg)
     CONF = {}
```

### Comparing `pyerk-0.6.5/src/pyerk/templates/report-template.tex` & `pyerk-0.8.5/src/pyerk/templates/report-template.tex`

 * *Files identical despite different names*

### Comparing `pyerk-0.6.5/src/pyerk/visualization.py` & `pyerk-0.8.5/src/pyerk/visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         self.id = f"node_{self.short_key}"  # this serves to recognize the nodes in svg code
         self.url_template = url_template
 
         if isinstance(entity, p.Item):
             self.shape = "circle"
         elif isinstance(entity, p.Relation):
             self.shape = "hexagon"
-        elif isinstance(entity, p.RelationEdge):
+        elif isinstance(entity, p.Statement):
             self.shape = "cds"
         else:
             msg = f"Unexpected entity type: {type(entity)} during creation of EntityNode in visualization."
             raise TypeError(msg)
 
         # TODO: handle different languages here
         self.label = self.smart_label = entity.R1
@@ -345,15 +345,15 @@
     base_node = create_node(entity, url_template)
     G.add_node(base_node, color="#2ca02c")
 
     for rel_key, re_list in list(re_dict.items()) + list(inv_re_dict.items()):
         if rel_key in REL_BLACKLIST:
             continue
 
-        re_list: List[p.RelationEdge]
+        re_list: List[p.Statement]
         for re in re_list:
             assert len(re.relation_tuple) == 3
             subj, pred, obj = re.relation_tuple
 
             edge = Edge(pred, url_template)
             edge.perform_html_wrapping()
             if re.role == p.RelationRole.SUBJECT:
@@ -371,37 +371,37 @@
 def get_color_for_item(item: p.Item) -> str:
     # TODO: add color by base_uri
     if item.short_key == "I14":
         return "red"
     return "black"
 
 
-def get_color_for_rledg(rledg: p.RelationEdge) -> str:
+def get_color_for_stm(stm: p.Statement) -> str:
     cmap = {"R3": mpl_colors[0], "R4": mpl_colors[1]}
 
-    return cmap.get(rledg.rsk, "black")
+    return cmap.get(stm.rsk, "black")
 
 
 def create_complete_graph(
     url_template="",
     limit: Optional[int] = None,
 ) -> nx.DiGraph:
     """
     :param url_template:    template to insert links based on uris
     :param limit:
     :return:
     """
 
     added_items_nodes = {}
-    added_relation_edges = {}
+    added_statements = {}
     G = nx.DiGraph()
 
     i = 0
     relation_dict: dict
-    for item_uri, relation_dict in p.ds.relation_edges.items():
+    for item_uri, relation_dict in p.ds.statements.items():
         item = p.ds.get_entity_by_uri(item_uri)
         if not isinstance(item, p.Item) or item.short_key in ["I000"]:
             continue
         # count only items
         i += 1
         if limit and i == limit:
             break
@@ -410,40 +410,40 @@
             pass
         else:
             node = create_node(item, url_template)
         G.add_node(node, label=item.short_key, color=get_color_for_item(item))
         added_items_nodes[item_uri] = node
 
         # iterate over relation edges
-        for relation_uri, rledg_list in relation_dict.items():
-            rledg: p.RelationEdge
-            for rledg in rledg_list:
-                if rledg.role != p.RelationRole.SUBJECT:
+        for relation_uri, stm_list in relation_dict.items():
+            stm: p.Statement
+            for stm in stm_list:
+                if stm.role != p.RelationRole.SUBJECT:
                     continue
-                if rledg.relation_tuple[1].uri in REL_BLACKLIST:
+                if stm.relation_tuple[1].uri in REL_BLACKLIST:
                     continue
 
-                obj = rledg.relation_tuple[-1]
+                obj = stm.relation_tuple[-1]
                 if isinstance(obj, p.Item):
                     if other_node := added_items_nodes.get(obj.uri):
                         pass
                     else:
                         other_node = create_node(obj, url_template)
                         G.add_node(other_node, label=obj.short_key, color=get_color_for_item(obj))
                         added_items_nodes[obj.uri] = other_node
                 else:
                     # obj is a literal, we omit that for now
                     continue
 
-                # edge_label = f"{rledg.relation_tuple[1].short_key}"
-                edge_label = f"{rledg.relation_tuple[1].short_key}"
-                G.add_edge(node, other_node, label=edge_label, color=get_color_for_rledg(rledg))
+                # edge_label = f"{stm.relation_tuple[1].short_key}"
+                edge_label = f"{stm.relation_tuple[1].short_key}"
+                G.add_edge(node, other_node, label=edge_label, color=get_color_for_stm(stm))
 
-                assert rledg.uri not in added_relation_edges
-                added_relation_edges[rledg.uri] = 1
+                assert stm.uri not in added_statements
+                added_statements[stm.uri] = 1
 
     return G
 
 
 def render_graph_to_dot(G: nx.DiGraph) -> str:
     """
 
@@ -561,15 +561,15 @@
         graph={"rankdir": "BT", "nodesep": 0.2},
         node=lambda u, d: {
             # "shape": "point",
             "shape": "circle",
             "style": "filled",
             "fixedsize": True,
             "color": d.get("color", "black"),
-            "width": .3,
+            "width": 0.3,
             "fontsize": 2,
             "label": d.get("label", "undefined label"),
             "fillcolor": "#45454533",
         },
         edge=lambda u, v, d: {
             "style": "solid",
             "arrowhead": "normal",
```

### Comparing `pyerk-0.6.5/src/pyerk.egg-info/PKG-INFO` & `pyerk-0.8.5/src/pyerk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerk
-Version: 0.6.5
+Version: 0.8.5
 Summary: Python based 'Easy Representation of Knowledge' (pyERK)
 Author-email: Carsten Knoll <firstname.lastname@posteo.de>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/ackrep-org/pyerk-core/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyerk-0.6.5/tests/test_core.py` & `pyerk-0.8.5/tests/test_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,98 +1,45 @@
 import unittest
 import sys
 import os
 from os.path import join as pjoin
+from typing import Dict, List, Union
 
 import rdflib
 
 # noinspection PyUnresolvedReferences
 from ipydex import IPS, activate_ips_on_exception, set_trace  # noqa
 import pyerk as p
 import pyerk.visualization as visualization
+import pyerk.io
+from pyerk.auxiliary import uri_set
 import git
 import pyerk.reportgenerator as rgen
 
-"""
-recommended ways to run the tests from the repo root (where setup.py lives):
 
-# all tests
-nosetests --rednose --nocapture
-python3 -m unititest
+from .settings import (
+    ERK_ROOT_DIR,
+    TEST_DATA_DIR1,
+    TEST_DATA_PARENT_PATH,
+    TEST_DATA_REPO_PATH,
+    TEST_DATA_PATH2,
+    TEST_DATA_PATH_MA,
+    TEST_DATA_PATH3,
+    TEST_DATA_PATH_ZEBRA_BASE_DATA,
+    TEST_DATA_PATH_ZEBRA02,
+    TEST_MOD_NAME,
+    TEST_DATA_REPO_COMMIT_SHA,
+    # TEST_ACKREP_DATA_FOR_UT_PATH,
+    TEST_BASE_URI,
+    WRITE_TMP_FILES,
+    HouskeeperMixin,
+   
+    
+    )
 
-# single class
-
-
-"""
-
-activate_ips_on_exception()
-
-current_dir = os.path.dirname(os.path.abspath(sys.modules.get(__name__).__file__))
-
-ERK_ROOT_DIR = p.aux.get_erk_root_dir()
-
-# path for basic (staged) test data
-TEST_DATA_DIR1 = pjoin(ERK_ROOT_DIR, "pyerk-core", "tests", "test_data")
-
-# path for "realistic" test data
-TEST_DATA_PARENT_PATH = pjoin(ERK_ROOT_DIR, "erk-data-for-unittests")
-TEST_DATA_REPO_PATH = pjoin(TEST_DATA_PARENT_PATH, "erk-ocse")
-TEST_DATA_PATH2 = pjoin(TEST_DATA_REPO_PATH, "control_theory1.py")
-TEST_DATA_PATH3 = pjoin(TEST_DATA_REPO_PATH, "agents1.py")
-TEST_MOD_NAME = "control_theory1"
-
-# useful to get the currently latest sha strings:
-# git log --pretty=oneline | head
-TEST_DATA_REPO_COMMIT_SHA = "b795a5f16ca1e385e03b300f2e9601c6f3c03233"  # (2022-12-01 01:45:51)
-
-# TODO: make this more robust (e.g. search for config file or environment variable)
-# TODO: put link to docs here (directory layout)
-TEST_ACKREP_DATA_FOR_UT_PATH = pjoin(ERK_ROOT_DIR, "..", "ackrep", "ackrep_data_for_unittests")
-
-os.environ["UNITTEST"] = "True"
-
-__URI__ = TEST_BASE_URI = "erk:/local/unittest/"
-
-
-# this serves to print the test-method-name before it is executed (useful for debugging, see setUP below)
-PRINT_TEST_METHODNAMES = True
-
-# some tests might generate files such as `tmp.svg` as a byproduct for debugging. The following flags controls this.
-WRITE_TMP_FILES = False
-
-
-class HouskeeperMixin:
-    """
-    Class to provide common functions for all our TestCase subclasses
-    """
-
-    def setUp(self):
-        self.print_methodnames()
-        self.register_this_module()
-
-    def tearDown(self) -> None:
-        self.unload_all_mods()
-
-    @staticmethod
-    def unload_all_mods():
-        p.unload_mod(TEST_BASE_URI, strict=False)
-
-        # unload all modules which where loaded by a test
-        for mod_id in list(p.ds.mod_path_mapping.a.keys()):
-            p.unload_mod(mod_id)
-
-    @staticmethod
-    def register_this_module():
-        keymanager = p.KeyManager()
-        p.register_mod(TEST_BASE_URI, keymanager)
-
-    def print_methodnames(self):
-        if PRINT_TEST_METHODNAMES:
-            # noinspection PyUnresolvedReferences
-            print("In method", p.aux.bgreen(self._testMethodName))
 
 
 class Test_00_Core(HouskeeperMixin, unittest.TestCase):
     def test_a0__ensure_expected_test_data(self):
         """
         Construct a list of all sha-strings which where commited in the current branch and assert that
         the expected string is among them. This heuristics assumes that it is OK if the data-repo is newer than
@@ -152,36 +99,35 @@
             res = p.process_key_str("some_prefix__I000__double_label_['redundant']", check=False)
 
     def test_b1__uri_contex_manager(self):
         """
         Test defined behavior of errors occur in uri_context
         :return:
         """
-
         self.assertEqual(len(p.core._uri_stack), 0)
         try:
             with p.uri_context(uri=TEST_BASE_URI):
                 raise ValueError
         except ValueError:
             pass
         self.assertEqual(len(p.core._uri_stack), 0)
 
         self.assertEqual(len(p.ds.entities_created_in_mod), 1)
         L1 = len(p.ds.items)
         L2 = len(p.ds.relations)
-        L3 = len(p.ds.relation_edge_uri_map)
+        L3 = len(p.ds.statement_uri_map)
         try:
             _ = p.erkloader.load_mod_from_path(pjoin(TEST_DATA_DIR1, "tmod0_with_errors.py"), prefix="tm0")
         except ValueError:
             pass
         # assert that no enties remain in the data structures
         self.assertEqual(len(p.ds.entities_created_in_mod), 1)
         self.assertEqual(L1, len(p.ds.items))
         self.assertEqual(L2, len(p.ds.relations))
-        self.assertEqual(L3, len(p.ds.relation_edge_uri_map))
+        self.assertEqual(L3, len(p.ds.statement_uri_map))
         self.assertEqual(len(p.core._uri_stack), 0)
 
     def test_key_manager(self):
         p.KeyManager.instance = None
 
         km = p.KeyManager(minval=100, maxval=105)
 
@@ -236,25 +182,25 @@
         self.tearDown()
 
         # after tearing down there should be no i32 instances left
         i32_instance_rels = p.I32["evaluated mapping"].get_inv_relations("R4__is_instance_of")
         self.assertEqual(len(i32_instance_rels), 0)
 
         builtin_entity_uris = set(p.ds.entities_created_in_mod[p.BUILTINS_URI])
-        builtin_rledg_uris = set(p.ds.rledgs_created_in_mod[p.BUILTINS_URI])
+        builtin_stm_uris = set(p.ds.stms_created_in_mod[p.BUILTINS_URI])
         available_item_keys = set(p.ds.items.keys())
         available_relation_keys = set(p.ds.relations.keys())
-        available_relation_edge_keys = set(p.ds.relation_edge_uri_map.keys())
-        available_relation_relation_edge_keys = set(p.ds.relation_relation_edges.keys())
+        available_statement_keys = set(p.ds.statement_uri_map.keys())
+        available_relation_statement_keys = set(p.ds.relation_statements.keys())
 
         diff1 = available_item_keys.difference(builtin_entity_uris)
         diff2 = available_relation_keys.difference(builtin_entity_uris)
 
-        diff3 = available_relation_edge_keys.difference(builtin_rledg_uris)
-        diff4 = available_relation_relation_edge_keys.difference(builtin_entity_uris)
+        diff3 = available_statement_keys.difference(builtin_stm_uris)
+        diff4 = available_relation_statement_keys.difference(builtin_entity_uris)
 
         self.assertEqual(len(diff1), 0)
         self.assertEqual(len(diff2), 0)
         self.assertEqual(len(diff3), 0)
         self.assertEqual(len(diff4), 0)
 
     def test_a03_tear_down(self):
@@ -263,19 +209,19 @@
 
         :return:
         """
 
         # ensure that builtins are loaded
         self.assertGreater(len(p.ds.items), 40)
         self.assertGreater(len(p.ds.relations), 40)
-        self.assertGreater(len(p.ds.relation_edge_uri_map), 300)
+        self.assertGreater(len(p.ds.statement_uri_map), 300)
 
         # ensure that no residuals are left from last test
-        non_builtin_rledges = [k for k in p.ds.relation_edge_uri_map.keys() if not k.startswith(p.BUILTINS_URI)]
-        self.assertEqual(len(non_builtin_rledges), 0)
+        non_builtin_stms = [k for k in p.ds.statement_uri_map.keys() if not k.startswith(p.BUILTINS_URI)]
+        self.assertEqual(len(non_builtin_stms), 0)
 
         non_builtin_entities = [k for k in p.ds.items.keys() if not k.startswith(p.BUILTINS_URI)]
         non_builtin_entities += [k for k in p.ds.relations.keys() if not k.startswith(p.BUILTINS_URI)]
         self.assertEqual(len(non_builtin_entities), 0)
 
     # noinspection PyUnresolvedReferences
     # (above noinspection is necessary because of the @-operator which is undecleared for strings)
@@ -364,20 +310,19 @@
         """
         test how to create items with labels in multiple languages
         """
 
         with p.uri_context(uri=TEST_BASE_URI):
             itm = p.create_item(
                 key_str=p.pop_uri_based_key("I"),
-
                 # multiple values to R1 can be passed using a list
                 R1__has_label=[
-                    "test-label in english"@p.en,  # `@p.en` is recommended, if you use multiple languages
-                    "test-label auf deutsch"@p.de
-                    ],
+                    "test-label in english" @ p.en,  # `@p.en` is recommended, if you use multiple languages
+                    "test-label auf deutsch" @ p.de,
+                ],
                 R2__has_description="test-description in english",
             )
 
         # this returns only one label according to the default language
         default_label = itm.R1
 
         # to access all labels use this:
@@ -387,15 +332,15 @@
         self.assertEqual(label1.language, "en")
         self.assertEqual(label2.value, "test-label auf deutsch")
         self.assertEqual(label2.language, "de")
 
         # add another language later
 
         with p.uri_context(uri=TEST_BASE_URI):
-            itm.set_relation(p.R2, "test-beschreibung auf deutsch"@p.de)
+            itm.set_relation(p.R2, "test-beschreibung auf deutsch" @ p.de)
 
         desc1, desc2 = itm.get_relations("R2", return_obj=True)
 
         self.assertTrue(isinstance(desc1, str))
         self.assertTrue(isinstance(desc2, p.Literal))
 
         self.assertEqual(desc2.language, "de")
@@ -406,97 +351,114 @@
         tmp1 = itm["test-label in english"]
         self.assertTrue(tmp1 is itm)
 
         tmp2 = itm["test-label auf deutsch"]
         self.assertTrue(tmp2 is itm)
 
         # second: with explicitly specifying the language
-        tmp3 = itm["test-label in english"@p.en]
+        tmp3 = itm["test-label in english" @ p.en]
         self.assertTrue(tmp3 is itm)
 
-        tmp4 = itm["test-label auf deutsch"@p.de]
+        tmp4 = itm["test-label auf deutsch" @ p.de]
         self.assertTrue(tmp4 is itm)
 
         with self.assertRaises(ValueError):
             tmp5 = itm["wrong label"]
 
         with self.assertRaises(ValueError):
-            tmp5 = itm["wrong label"@p.de]
+            tmp5 = itm["wrong label" @ p.de]
 
         with self.assertRaises(ValueError):
-            tmp5 = itm["wrong label"@p.en]  # noqa
+            tmp5 = itm["wrong label" @ p.en]  # noqa
 
         # change the default language
 
         p.settings.DEFAULT_DATA_LANGUAGE = "de"
 
         new_default_label = itm.R1
         self.assertEqual(new_default_label, label2)
         self.assertEqual(new_default_label.language, "de")
 
         new_default_description = itm.R2
-        self.assertEqual(new_default_description, "test-beschreibung auf deutsch"@p.de)
+        self.assertEqual(new_default_description, "test-beschreibung auf deutsch" @ p.de)
 
         with p.uri_context(uri=TEST_BASE_URI):
             itm2 = p.create_item(
                 key_str=p.pop_uri_based_key("I"),
-
                 # multiple values to R1 can be passed using a list
-                R1__has_label=["test-label2", "test-label2-de"@p.de],
+                R1__has_label=["test-label2", "test-label2-de" @ p.de],
                 R2__has_description="test-description2 in english",
             )
 
         # in case of ordinary strings they should be used if no value is available for current language
 
         self.assertEqual(p.settings.DEFAULT_DATA_LANGUAGE, "de")
-        self.assertEqual(itm2.R1, "test-label2-de"@p.de)
+        self.assertEqual(itm2.R1, "test-label2-de" @ p.de)
         self.assertEqual(itm2.R2, "test-description2 in english")
 
         p.settings.DEFAULT_DATA_LANGUAGE = "en"
         self.assertEqual(itm2.R1, "test-label2")
         self.assertEqual(itm2.R2, "test-description2 in english")
 
         p.settings.DEFAULT_DATA_LANGUAGE = "en"
 
+        # test for correct error message
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm1 = p.instance_of(p.I1["general item"])
+
+            # this should cause no error (because of differnt language)
+            itm1.set_relation(p.R1["has label"], "neues Label" @ p.de)
+
+            with self.assertRaises(p.aux.FunctionalRelationError):
+                itm1.set_relation(p.R1["has label"], "new label")
+
     def test_c03__nontrivial_metaclasses(self):
         with p.uri_context(uri=TEST_BASE_URI):
             i1 = p.instance_of(p.I34["complex number"])
 
         self.assertTrue(i1.R4, p.I34)
 
     def test_c04__evaluated_mapping(self):
 
-        res = p.ds.relation_edges.get("RE6229")
+        res = p.ds.statements.get("S6229")
         self.assertIsNone(res)
 
-        mod1 = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
+        ct = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
         with p.uri_context(uri=TEST_BASE_URI):
-            poly1 = p.instance_of(mod1.I4239["monovariate polynomial"])
+            poly1 = p.instance_of(ct.I4239["monovariate polynomial"])
 
         # test that an arbitrary item is *not* callable
-        self.assertRaises(TypeError, mod1.ma.I2738["field of complex numbers"], 0)
+        self.assertRaises(TypeError, ct.ma.I2738["field of complex numbers"], 0)
 
         # test that some special items are callable (note that its parent class is a subclass of one which has
         # a _custom_call-method defined)
         with p.uri_context(uri=TEST_BASE_URI):
             # this creates new items and thus must be executed inside a context
             res = poly1(0)
 
         self.assertEqual(res.R4__is_instance_of, p.I32["evaluated mapping"])
 
+        with p.uri_context(uri=TEST_BASE_URI):
+            x = p.instance_of(p.I35["real number"])
+            s1 = ct.ma.I5807["sign"](x)
+            s2 = ct.ma.I5807["sign"](x)
+            self.assertTrue(s1 is s2)
+
+
     def test_c05__evaluated_mapping2(self):
         mod1 = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
 
         with p.uri_context(uri=TEST_BASE_URI):
             h = p.instance_of(mod1.I9923["scalar field"])
             f = p.instance_of(mod1.I9841["vector field"])
             x = p.instance_of(mod1.I1168["point in state space"])
 
             Lderiv = mod1.I1347["Lie derivative of scalar field"]
-            
+
             # this creates a new item (and thus must be executed with a non-empty uri stack, i.e. within this context)
             h2 = Lderiv(h, f, x)
 
         self.assertEqual(h2.R4__is_instance_of, mod1.I9923["scalar field"])
 
         arg_tup = h2.R36__has_argument_tuple
         self.assertEqual(arg_tup.R4__is_instance_of, p.I33["tuple"])
@@ -523,14 +485,122 @@
 
         # this tests for a bug with labels of scope vars
         _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
         def_itm = p.ds.get_entity_by_key_str("ct__I9907__definition_of_square_matrix")
         matrix_instance = def_itm.M
         self.assertEqual(matrix_instance.R1, "M")
 
+    def test_c07b__nested_scopes_of_propositions(self):
+        """
+        Test existentially and universally quantified conditions as nested scopes in scopes of propositions/definitions
+        """
+        with p.uri_context(uri=TEST_BASE_URI):
+            I7324 = p.create_item(
+                R1__has_label = "definition of something",
+                R4__is_instance_of =p.I20["mathematical definition"],
+            )
+
+            my_set = p.instance_of(p.I13["mathematical set"])
+            my_prop = p.instance_of(p.I11["mathematical property"])
+
+            with I7324["definition of something"].scope("setting") as cm:
+                x = cm.new_var(x=p.instance_of(p.I39["positive integer"]))
+                y = cm.new_var(y=p.instance_of(p.I39["positive integer"]))
+
+            with I7324["definition of something"].scope("premise") as cm:
+                with cm.universally_quantified() as cm2:
+                    cm2.add_condition_statement(cm.x, p.R15["is element of"], my_set)
+                    cm2.add_condition_statement(cm.y, p.R15["is element of"], my_set)
+
+                    # note: the meaning of this equation is pointless, we just test the implementation of subscopes
+                    cm2.new_equation(lhs=cm.x, rhs=cm.y)
+
+            with I7324["definition of something"].scope("assertion") as cm:
+                cm.new_rel(cm.x, p.R16["has property"], my_prop)
+                cm.new_rel(cm.y, p.R16["has property"], my_prop)
+
+                # also pointless direct meaning, only to test contexts
+                with cm.existentially_quantified() as cm2:
+                    z = cm2.new_condition_var(z=p.instance_of(p.I39["positive integer"]))
+                    cm2.add_condition_statement(cm2.z, p.R15["is element of"], my_set)
+                    cm2.add_condition_statement(cm.y, p.R15["is element of"], my_set)
+                    cm2.add_condition_math_relation(cm2.z, "<", cm.x)
+
+                    cm2.new_math_relation(cm2.z, ">", cm.y)
+
+            # universally quantified scope
+
+            scp_prem = I7324.get_subscopes()[1]
+            prem_sub_scopes = scp_prem.get_subscopes()
+            self.assertEqual(len(prem_sub_scopes), 1)
+            uq_scp = prem_sub_scopes[0]
+            self.assertEqual(uq_scp.R64__has_scope_type, "UNIV_QUANT")
+
+            # check the condition
+            cond_sc = uq_scp.get_subscopes()[0]
+            cond_stms = cond_sc.get_statements_for_scope()
+            stm1: p.Statement = cond_stms[0]
+            self.assertEqual(stm1.subject, x)
+            self.assertEqual(stm1.predicate, p.R15["is element of"])
+            self.assertEqual(stm1.object, my_set)
+
+            # check the actual statement (which is an equation)
+            stm1, = uq_scp.get_statements_for_scope()
+            self.assertEqual(stm1.subject, x)
+            self.assertEqual(stm1.predicate, p.R31["is in mathematical relation with"])
+            self.assertEqual(stm1.object, y)
+
+            proxy_item = stm1.get_first_qualifier_obj_with_rel("R34__has_proxy_item")
+            self.assertEqual(proxy_item.R4__is_instance_of, p.I23["equation"])
+            self.assertEqual(proxy_item.R26__has_lhs, x)
+            self.assertEqual(proxy_item.R27__has_rhs, y)
+
+            # existentially quantified scope
+
+            scp_asstn = I7324.get_subscopes()[2]
+            self.assertEqual(len(scp_asstn.get_subscopes()), 1)
+            ex_scp = scp_asstn.get_subscopes()[0]
+            self.assertEqual(ex_scp.R64__has_scope_type, "EXIS_QUANT")
+
+            # check the conditions
+            cond_sc = ex_scp.get_subscopes()[0]
+            cond_itms = cond_sc.get_items_for_scope()
+            self.assertEqual(len(cond_itms), 2)
+            self.assertIn(z, cond_itms)
+            # apart from z there is also the cond_proxy_item, see below
+
+            cond_stms = cond_sc.get_statements_for_scope()
+            self.assertEqual(len(cond_stms), 3)
+            stm1: p.Statement = cond_stms[0]
+            self.assertEqual(stm1.subject, z)
+            self.assertEqual(stm1.predicate, p.R15["is element of"])
+            self.assertEqual(stm1.object, my_set)
+
+            stm3: p.Statement = cond_stms[2]
+            self.assertEqual(stm3.subject, z)
+            self.assertEqual(stm3.predicate, p.R31["is in mathematical relation with"])
+            self.assertEqual(stm3.object, x)
+
+            cond_proxy_item = stm3.get_first_qualifier_obj_with_rel("R34__has_proxy_item")
+            self.assertIn(cond_proxy_item, cond_itms)
+            self.assertEqual(cond_proxy_item.R4__is_instance_of, p.I29["less-than-relation"])
+            self.assertEqual(cond_proxy_item.R26__has_lhs, z)
+            self.assertEqual(cond_proxy_item.R27__has_rhs, x)
+
+            # check the actual statement (which is an equation)
+            stm1, = ex_scp.get_statements_for_scope()
+            self.assertEqual(stm1.subject, z)
+            self.assertEqual(stm1.predicate, p.R31["is in mathematical relation with"])
+            self.assertEqual(stm1.object, y)
+
+            proxy_item = stm1.get_first_qualifier_obj_with_rel("R34__has_proxy_item")
+            self.assertEqual(proxy_item.R4__is_instance_of, p.I28["greater-than-relation"])
+            self.assertEqual(proxy_item.R26__has_lhs, z)
+            self.assertEqual(proxy_item.R27__has_rhs, y)
+
     def test_c08__relations_with_sequence_as_argument(self):
         with p.uri_context(uri=TEST_BASE_URI):
             Ia001 = p.create_item(R1__has_label="test item")
 
         # check that assigning sequences is not allowed
         with self.assertRaises(TypeError):
             Ia001.set_relation(p.R5["is part of"], [p.I4["Mathematics"], p.I5["Engineering"]])
@@ -551,15 +621,15 @@
         self.assertIn(p.I5["Engineering"], res)
 
     def test_c09__is_instance_of_generalized_metaclass(self):
         _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
 
         itm1 = p.ds.get_entity_by_key_str("I2__Metaclass")
         itm2 = p.ds.get_entity_by_key_str("I12__mathematical_object")
-        itm3 = p.ds.get_entity_by_key_str("ct__I4239__monovariate_polynomial")
+        itm3 = p.ds.get_entity_by_key_str("ma__I4239__monovariate_polynomial")
 
         # metaclass could be considered as an instance of itself because metaclasses are allowed to have
         # subclasses and instances (which is both true for I2__metaclass)
         self.assertTrue(p.allows_instantiation(itm1))
 
         self.assertTrue(p.allows_instantiation(itm2))
         self.assertTrue(p.allows_instantiation(itm3))
@@ -570,49 +640,60 @@
         self.assertFalse(p.allows_instantiation(itm4))
 
     def test_c10__qualifiers(self):
         _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
         _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH3, prefix="ag")
 
         itm1: p.Item = p.ds.get_entity_by_key_str("ag__I2746__Rudolf_Kalman")
-        rel1, rel2 = itm1.get_relations("ag__R1833__has_employer")[:2]
-        self.assertEqual(len(rel1.qualifiers), 2)
-        self.assertEqual(len(rel2.qualifiers), 2)
+        stm1, stm2 = itm1.get_relations("ag__R1833__has_employer")[:2]
+        self.assertEqual(len(stm1.qualifiers), 2)
+        self.assertEqual(len(stm2.qualifiers), 2)
+
+        self.assertEqual(len(stm2.dual_statement.qualifiers), 2)
+
+        qf1, qf2 = stm2.qualifiers
+
+        qf1.unlink()
+        self.assertEqual(len(stm2.qualifiers), 1)
+        self.assertEqual(len(stm2.dual_statement.qualifiers), 1)
 
     def test_c11__equation(self):
         mod1 = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct")
 
         # get item via prefix and key
-        itm1: p.Item = p.ds.get_entity_by_key_str("ct__I3749__Cayley-Hamilton_theorem")
+        itm1: p.Item = p.ds.get_entity_by_key_str("ct__I3749__Cayley_Hamilton_theorem")
 
         # get item via key and uri
-        itm2: p.Item = p.ds.get_entity_by_key_str("I3749__Cayley-Hamilton_theorem", mod_uri=mod1.__URI__)
+        itm2: p.Item = p.ds.get_entity_by_key_str("I3749__Cayley_Hamilton_theorem", mod_uri=mod1.__URI__)
 
         self.assertEqual(itm1, itm2)
 
-        Z: p.Item = itm1.scope("context").namespace["Z"]
+        itm1_setting_namespace = itm1._ns_context
+        # alternative way to access names (graph based but bulky): itm1.scp__context.get_inv_relations("R20"), ...
+
+        Z: p.Item = itm1_setting_namespace["Z"]
 
         r31_list = Z.get_inv_relations("R31__is_in_mathematical_relation_with")
-        re: p.RelationEdge = r31_list[0]
+        stm: p.Statement = r31_list[0].dual_statement  # taking the dual because we got it via the inverse relation
         self.assertEqual(len(r31_list), 1)
 
         # test the expected qualifier
-        q = re.qualifiers[0]
-        self.assertEqual(q.relation_tuple[0], re)
-        self.assertEqual(q.relation_tuple[1], p.R34["has proxy item"])
+        q = stm.qualifiers[0]
+        self.assertEqual(q.subject, stm)  # here it is relevant that we used the dual_relation above
+        self.assertEqual(q.predicate, p.R34["has proxy item"])
 
         # this is the proxy item
-        eq = q.relation_tuple[2]
+        eq = q.object
         rhs = eq.R27__has_rhs
         self.assertEqual(rhs, Z)
 
         # ensure reproducible results of applied mappings
         lhs = eq.R26__has_lhs
-        P: p.Item = itm1.scope("context").namespace["P"]
-        A: p.Item = itm1.scope("context").namespace["A"]
+        P: p.Item = itm1_setting_namespace["P"]
+        A: p.Item = itm1_setting_namespace["A"]
         tmp = P(A)
         self.assertEqual(lhs, tmp)
 
     def test_c12__process_key_str(self):
 
         # first, check label consistency in builtin_enities
         # note these keys do not to exist
@@ -741,33 +822,319 @@
         s1 = '<a href="">R35</a>'
         s2 = '<a href="">["is applied</a>'
         s3 = '<a href="">mapping of"]</a>'
         self.assertIn(s1, res)
         self.assertIn(s2, res)
         self.assertIn(s3, res)
 
+    def test_d01__wrap_function_with_uri_context(self):
+        ma = p.erkloader.load_mod_from_path(TEST_DATA_PATH_MA, prefix="ma")
 
-class Test_02_ruleengine(HouskeeperMixin, unittest.TestCase):
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            A = p.instance_of(ma.I9906["square matrix"])
+            A.set_relation("ma__R5939__has_column_number", 7)
+
+        def test_func():
+            """
+            docstring
+            """
+            # this fails outside uri-context of math
+            n = A.R5939__has_column_number
+            return n
+
+        with self.assertRaises(AttributeError):
+            test_func()
+
+        wrapped_func = p.wrap_function_with_search_uri_context(test_func, ma.__URI__)
+
+        self.assertEqual(wrapped_func.__doc__, test_func.__doc__)
+
+        # now this call works as expected
+        res = wrapped_func()
+        self.assertEqual(res, 7)
+
+    def test_d02__custom_call_post_process1(self):
+
+        ma = p.erkloader.load_mod_from_path(TEST_DATA_PATH_MA, prefix="ma")
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            A = p.instance_of(ma.I9906["square matrix"])
+            s = p.instance_of(ma.I5030["variable"])
+
+            # construct sI - A
+            M = ma.I6324["canonical first order monic polynomial matrix"](A, s)
+            d = ma.I5359["determinant"](M)
+
+        self.assertTrue(M.R4__is_instance_of, ma.I1935["polynomial matrix"])
+        self.assertTrue(M.ma__R8736__depends_polyonomially_on, s)
+
+        self.assertTrue(d.ma__R8736__depends_polyonomially_on, s)
+
+    def test_d03__replace_entity(self):
+
+        ma = p.erkloader.load_mod_from_path(TEST_DATA_PATH_MA, prefix="ma")
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            A = p.instance_of(ma.I9906["square matrix"])
+            n1 = p.instance_of(p.I38["non-negative integer"])
+            n2 = p.instance_of(p.I38["non-negative integer"])
+
+            # set functional relation
+            A.set_relation(ma.R5938["has row number"], n1)
+        self.assertEqual(A.ma__R5938__has_row_number, n1)
+        self.assertNotEqual(A.ma__R5938__has_row_number, n2)
+
+        tmp = p.ds.get_entity_by_uri(n1.uri)
+        self.assertEqual(n1, tmp)
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            p.replace_and_unlink_entity(n1, n2)
+
+        self.assertEqual(A.ma__R5938__has_row_number, n2)
+        self.assertNotEqual(A.ma__R5938__has_row_number, n1)
+
+        with self.assertRaises(p.aux.UnknownURIError):
+            tmp = p.ds.get_entity_by_uri(n1.uri)
+
+    def test_d03b__replace_entity(self):
+
+        ma = p.erkloader.load_mod_from_path(TEST_DATA_PATH_MA, prefix="ma")
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            A = p.instance_of(ma.I9906["square matrix"])
+            n1 = p.instance_of(p.I38["non-negative integer"])
+            n2 = p.instance_of(p.I38["non-negative integer"])
+            n3 = p.instance_of(p.I38["non-negative integer"])
+
+            # set relations
+            A.set_relation(ma.R5938["has row number"], n1)  # n1 is object
+            n1.set_relation(p.R31["is in mathematical relation with"], n3)  # n1 is subject
+
+        self.assertEqual(n3.get_inv_relations("R31", return_subj=True)[0], n1)
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            p.replace_and_unlink_entity(n1, n2)
+
+        self.assertEqual(n3.get_inv_relations("R31", return_subj=True)[0], n2)
+
+    def test_d04__invalid_prefix(self):
+
+        n1a = len(p.ds.mod_path_mapping.a)
+        n2a = len(p.ds.entities_created_in_mod)
+        n3a = len(p.ds.stms_created_in_mod)
+        n4a = len(sys.modules)
+
+        with self.assertRaises(p.aux.InvalidPrefixError):
+            _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH_ZEBRA02, prefix="zb")
+
+        n1b = len(p.ds.mod_path_mapping.a)
+        n2b = len(p.ds.entities_created_in_mod)
+        n3b = len(p.ds.stms_created_in_mod)
+        n4b = len(sys.modules)
+
+        self.assertEqual(n1a, n1b)
+        self.assertEqual(n2a, n2b)
+        self.assertEqual(n3a, n3b)
+        self.assertEqual(n4a, n4b)
+
+    def test_d05__get_proxy_item(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            A = p.instance_of(p.I1["general item"])
+            B = p.instance_of(p.I1["general item"], qualifiers=[p.proxy_item(A)])
+
+        res = p.get_proxy_item(B.get_relations(p.R4.uri)[0])
+        self.assertEqual(res, A)
+
+    def test_d06__get_rel_props(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            R1000 = p.create_relation(
+                R1__has_label="test relation",
+                R22__is_functional=True,
+                R53__is_inverse_functional=True,
+            )
+
+            R1001 = p.create_relation(
+                R1__has_label="test relation2",
+            )
+
+            I2000 = p.instance_of(p.I40["general relation"])
+            I2000.set_relation(p.R22["is functional"], True)
+
+        res = p.get_relation_properties(R1000)
+        self.assertEqual(res, [p.R22.uri, p.R53.uri])
+
+        res = p.get_relation_properties(R1001)
+        self.assertEqual(res, [])
+
+        res = p.get_relation_properties(I2000)
+        self.assertEqual(res, [p.R22.uri])
+
+    def test_d07__replace_statement(self):
 
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm = p.instance_of(p.I1["general item"])
+
+        self.assertEqual(itm.R4__is_instance_of, p.I1["general item"])
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+            itm.overwrite_statement("R4__is_instance_of", p.I2["Metaclass"])
+        self.assertEqual(itm.R4__is_instance_of, p.I2["Metaclass"])
+
+    def test_d08__unlink_enities(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm1 = p.instance_of(p.I1["general item"])
+
+            rep_str1 = repr(itm1)
+            self.assertTrue(rep_str1.endswith('["itm1"]>'))
+
+            p.core._unlink_entity(itm1.uri, remove_from_mod=True)
+
+            rep_str2 = repr(itm1)
+            self.assertTrue(rep_str2.endswith('["!!unlinked: itm1"]>'))
+
+    def test_d09__raise_invalid_scope_name_error(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            prop = p.instance_of(p.I15["implication proposition"])
+
+            scp1 = prop.scope("setting")
+
+            with self.assertRaises(p.aux.InvalidScopeNameError):
+                prop.scope("setting")
+
+            scp2 = prop.scope("premise")
+
+        self.assertNotEqual(scp1, scp2)
+
+    def test_d10__set_multiple_statements(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm1 = p.instance_of(p.I1["general item"])
+            itm2 = p.instance_of(p.I1["general item"])
+            itm3 = p.instance_of(p.I1["general item"])
+
+            x = p.instance_of(p.I1["general item"])
+
+            self.assertEquals(itm1.R57__is_placeholder, None)
+            self.assertEquals(itm2.R57__is_placeholder, None)
+
+            stms = p.set_multiple_statements((itm1, itm2), p.R57["is placeholder"], True)
+            self.assertEquals(len(stms), 2)
+            self.assertEquals(itm1.R57__is_placeholder, True)
+            self.assertEquals(itm2.R57__is_placeholder, True)
+
+            tup = p.new_tuple(itm1, itm2, itm3)
+            stms = p.set_multiple_statements(tup.R39__has_element, p.R31["is in mathematical relation with"], x)
+
+            self.assertEquals(len(stms), 3)
+
+            self.assertEquals(itm1.R31__is_in_mathematical_relation_with, [x])
+            self.assertEquals(itm2.R31__is_in_mathematical_relation_with, [x])
+            self.assertEquals(itm3.R31__is_in_mathematical_relation_with, [x])
+
+    def test_d11__get_subjects_for_relation(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm1 = p.instance_of(p.I1["general item"])
+            itm2 = p.instance_of(p.I1["general item"])
+            itm3 = p.instance_of(p.I1["general item"])
+            itm4 = p.instance_of(p.I1["general item"])
+
+            R301 = p.create_relation(R1="test relation")
+
+            itm1.set_relation(R301, True)
+            itm2.set_relation(R301, False)
+            itm3.set_relation(R301, 15)
+
+            subj_list = p.ds.get_subjects_for_relation(R301.uri)
+
+            self.assertEqual(uri_set(*subj_list), uri_set(itm1, itm2, itm3))
+
+            itm1.set_relation(R301, 15)
+            itm4.set_relation(R301, 15)
+
+            subj_list = p.ds.get_subjects_for_relation(R301.uri, filter=15)
+            self.assertEqual(uri_set(*subj_list), uri_set(itm1, itm3, itm4))
+
+    def test_d12__prevent_duplicates(self):
+
+        with p.uri_context(uri=TEST_BASE_URI, prefix="ut"):
+
+            itm1 = p.instance_of(p.I1["general item"])
+            R301 = p.create_relation(R1="test relation")
+
+            itm1.set_relation(R301, True)
+            itm1.set_relation(R301, True)
+
+            self.assertEqual(len(itm1.R301), 2)
+            itm1.set_relation(R301, True, prevent_duplicate=True)
+            self.assertEqual(len(itm1.R301), 2)
+
+    def test_d13__check_type(self):
+
+        import json
+
+        # created with json.dumps and textwrap.fill(json_str, width=100)
+        raw_data = """
+        {"erk:/ocse/0.2/zebra_base_data#R8216": [[5, "erk:/ocse/0.2/zebra_base_data#I4037"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I9848"], [5, "erk:/ocse/0.2/zebra_base_data#I3132"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I2552"], [5, "erk:/ocse/0.2/zebra_base_data#I5931"]],
+        "erk:/ocse/0.2/zebra_base_data#R9040": [[5, "erk:/ocse/0.2/zebra_base_data#I4037"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I9848"], [5, "erk:/ocse/0.2/zebra_base_data#I3132"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I2552"], [5, "erk:/ocse/0.2/zebra_base_data#I5931"]],
+        "erk:/ocse/0.2/zebra_base_data#R5611": [[5, "erk:/ocse/0.2/zebra_base_data#I4037"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I9848"], [5, "erk:/ocse/0.2/zebra_base_data#I3132"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I2552"], [5, "erk:/ocse/0.2/zebra_base_data#I5931"]],
+        "erk:/ocse/0.2/zebra_base_data#R8098": [[5, "erk:/ocse/0.2/zebra_base_data#I4037"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I9848"], [5, "erk:/ocse/0.2/zebra_base_data#I3132"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I2552"], [5, "erk:/ocse/0.2/zebra_base_data#I5931"]],
+        "erk:/ocse/0.2/zebra_base_data#R8592": [[5, "erk:/ocse/0.2/zebra_base_data#I4037"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I9848"], [5, "erk:/ocse/0.2/zebra_base_data#I3132"], [5,
+        "erk:/ocse/0.2/zebra_base_data#I2552"], [5, "erk:/ocse/0.2/zebra_base_data#I5931"]]}
+        """.replace("\n","")
+        data = json.loads(raw_data)
+
+        self.assertFalse(p.check_type(data, Dict[str, int], strict=False))
+        self.assertFalse(p.check_type(data, Dict[str, dict], strict=False))
+        self.assertFalse(p.check_type(data, Dict[str, Dict], strict=False))
+        self.assertFalse(p.check_type(data, Dict[str, List[int]], strict=False))
+        self.assertFalse(p.check_type(data, Dict[str, List[List[int]]], strict=False))
+
+        # pydantic has nontrivial behavior abour Unions. This requires smart_unions=True
+        q = [5, 'erk:/ocse/0.2/zebra_base_data#I9848']
+        p.check_type(q, List[Union[int, str]])
+
+        # this is what we actually want to test (note that the inner list could be specified more precisely)
+        self.assertTrue(p.check_type(data, Dict[str, List[List[Union[int, str]]]], strict=False))
+
+
+class Test_02_ruleengine(HouskeeperMixin, unittest.TestCase):
     def setUp(self):
         super().setUp()
-        self.setup_data1()
 
     def tearDown(self) -> None:
         super().tearDown()
 
     def setup_data1(self):
 
         with p.uri_context(uri=TEST_BASE_URI):
             self.rule1 = p.create_item(
                 key_str="I400",
                 R1__has_label="subproperty rule 1",
                 R2__has_description=(
                     # "specifies the 'transitivity' of I11_mathematical_property-instances via R17_issubproperty_of"
-                    "specifies the 'transitivity' of R17_issubproperty_of"
+                    "specifies the 'transitivity' of R17_is_subproperty_of"
                 ),
                 R4__is_instance_of=p.I41["semantic rule"],
             )
 
             with self.rule1["subproperty rule 1"].scope("context") as cm:
                 cm.new_var(P1=p.instance_of(p.I11["mathematical property"]))
                 cm.new_var(P2=p.instance_of(p.I11["mathematical property"]))
@@ -778,95 +1145,104 @@
                 cm.new_rel(cm.P2, p.R17["is subproperty of"], cm.P1)
                 cm.new_rel(cm.P3, p.R17["is subproperty of"], cm.P2)
                 # todo: state that all variables are different from each other
 
             with self.rule1["subproperty rule 1"].scope("assertions") as cm:
                 cm.new_rel(cm.P3, p.R17["is subproperty of"], cm.P1)
 
-    def setup_data2(self):
-        pass
-
     def test_a01__basics(self):
 
+        self.setup_data1()
+
         self.assertIn(TEST_BASE_URI, p.ds.entities_created_in_mod)
         self.assertEqual(len(p.ds.entities_created_in_mod), 2)
         self.tearDown()
 
         self.assertEqual(len(p.ds.entities_created_in_mod), 1)
         self.tearDown()
 
         # would be nice to solve this more elegantly (without the need for explicitly registering the module again)
         self.register_this_module()
         self.setup_data1()
         self.assertIn(TEST_BASE_URI, p.ds.entities_created_in_mod)
         self.assertEqual(len(p.ds.entities_created_in_mod), 2)
 
     def test_c02__ruleengine01(self):
+
+        self.setup_data1()
         itm1 = p.I12["mathematical object"]
         res = p.ruleengine.get_simple_properties(itm1)
         self.assertEqual(len(res), 2)
         self.assertEqual(res[p.R1.uri], itm1.R1)
         self.assertEqual(res[p.R2.uri], itm1.R2)
 
-        all_rels = p.ruleengine.get_all_node_relations()
+        ra = p.ruleengine.RuleApplicator(self.rule1)
+        all_rels = ra.get_all_node_relations()
         self.assertGreater(len(all_rels), 30)
         key = (p.I2.uri, p.I1.uri)
-        value_container: p.ruleengine.Container = all_rels[key]
+        value_container_list = all_rels[key]
+        value_container: p.ruleengine.Container = value_container_list[0]
 
         self.assertEqual(value_container.rel_uri, p.R3.uri)
 
         all_rules = p.ruleengine.get_all_rules()
         self.assertGreater(len(all_rules), 0)
 
     def test_c03__ruleengine02(self):
-        G = p.ruleengine.create_simple_graph()
+        self.setup_data1()
+        ra = p.ruleengine.RuleApplicator(self.rule1)
+        G = ra.create_simple_graph()
         self.assertGreater(G.number_of_nodes(), 30)
         self.assertGreater(G.number_of_edges(), 30)
 
     def test_c04__ruleengine03(self):
+        self.setup_data1()
 
         ra = p.ruleengine.RuleApplicator(self.rule1)
 
-        self.assertEqual(len(ra.get_asserted_relation_templates()), 1)
+        self.assertEqual(len(ra.ra_workers), 1)
+        ra_worker = ra.ra_workers[0]
+
+        self.assertEqual(len(ra_worker.get_asserted_relation_templates()), 1)
 
-        P = ra.create_prototype_subgraph_from_rule()
-        self.assertEqual(P.number_of_nodes(), 3)
-        self.assertEqual(P.number_of_edges(), 2)
+        self.assertEqual(ra_worker.P.number_of_nodes(), 3)
+        self.assertEqual(ra_worker.P.number_of_edges(), 2)
 
-        res_graph = ra.match_subgraph_P()
+        res_graph = ra_worker.match_subgraph_P()
 
         # ensures that the rule does not match itself
         self.assertEqual(len(res_graph), 0)
 
         # in this erk module some properties have subproperties
         _ = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct", modname=TEST_MOD_NAME)
 
         # create a new RuleApplicator because the overal graph changed
         ra = p.ruleengine.RuleApplicator(self.rule1)
-        res_graph = ra.match_subgraph_P()
+        ra_worker = ra.ra_workers[0]
+        res_graph = ra_worker.match_subgraph_P()
         self.assertGreater(len(res_graph), 5)
 
     def test_c05__ruleengine04(self):
+        self.setup_data1()
 
         mod1 = p.erkloader.load_mod_from_path(TEST_DATA_PATH2, prefix="ct", modname=TEST_MOD_NAME)
         self.assertEqual(len(mod1.I9642["local exponential stability"].get_relations("R17__is_subproperty_of")), 1)
         ra = p.ruleengine.RuleApplicator(self.rule1, mod_context_uri=TEST_BASE_URI)
         res = ra.apply()
 
-        # ensure that after rule application there is at least one new relation
-        self.assertEqual(len(mod1.I9642["local exponential stability"].get_relations("R17__is_subproperty_of")), 2)
-        for r in res:
-            print(r)
+        # ensure that after rule application there new relations
+        self.assertEqual(len(mod1.I9642["local exponential stability"].get_relations("R17__is_subproperty_of")), 3)
 
     def test_c06__ruleengine05(self):
-        premises_rledgs = p.ruleengine.filter_relevant_rledgs(
+        self.setup_data1()
+        premises_stms = p.ruleengine.filter_relevant_stms(
             self.rule1.scp__premises.get_inv_relations("R20__has_defining_scope")
         )
 
-        self.assertEqual(len(premises_rledgs), 2)
+        self.assertEqual(len(premises_stms), 2)
         with self.assertRaises(p.aux.EmptyURIStackError):
             p.ruleengine.apply_all_semantic_rules()
 
         with p.uri_context(uri=TEST_BASE_URI):
             _ = p.ruleengine.apply_all_semantic_rules()
 
 
@@ -982,15 +1358,14 @@
     def test_c01__visualization(self):
         cmd = "pyerk -vis I12"
         res = os.system(cmd)
         self.assertEqual(res, 0)
 
 
 class Test_06_reportgenerator(HouskeeperMixin, unittest.TestCase):
-
     @p.erkloader.preserve_cwd
     def tearDown(self) -> None:
         super().tearDown()
         os.chdir(pjoin(TEST_DATA_DIR1, "reports"))
         try:
             os.unlink("report.tex")
         except FileNotFoundError:
@@ -1020,7 +1395,104 @@
         os.chdir(pjoin(TEST_DATA_DIR1, "reports"))
         self.assertFalse(os.path.exists(reporttex_path1))
         rg = rgen.ReportGenerator(reportconf_path1, write_file=True)
         rg.generate_report()
         self.assertTrue(os.path.exists(reporttex_path1))
 
         self.assertEqual(len(rg.authors), 2)
+
+
+class Test_07_import_export(HouskeeperMixin, unittest.TestCase):
+
+    def test_b01__rdf_export(self):
+
+        with p.uri_context(uri=TEST_BASE_URI):
+            R301 = p.create_relation(R1="relation1")
+            R302 = p.create_relation(R1="test qualifier")
+
+            QF_R302 = p.QualifierFactory(R302["test qualifier"])
+
+            x0 = p.instance_of(p.I35["real number"])
+            x1 = p.instance_of(p.I35["real number"])
+            x2 = p.instance_of(p.I35["real number"])
+
+            # create two qualifiers (one with a literal object-value and one with x2 as object-value)
+            stm = x0.set_relation(R301, x1, qualifiers=[QF_R302(True), QF_R302(x2)])  # noqa
+
+        q_stms = [v for v in p.ds.stms_created_in_mod[TEST_BASE_URI].values() if v.is_qualifier()]
+        self.assertEquals(len(q_stms), 2)
+
+        fpath = pjoin(TEST_DATA_DIR1, "tmp_test.nt")
+        p.io.export_rdf_triples(fpath, add_qualifiers=True,  modfilter=TEST_BASE_URI)
+        g = p.io.import_raw_rdf_triples(fpath)
+        os.unlink(fpath)
+
+        self.assertGreater(len(g), 40)
+
+    def test_b02__rdf_import(self):
+
+        fpath = pjoin(TEST_DATA_DIR1, "test_triples1.nt")
+
+        with p.uri_context(uri=TEST_BASE_URI):
+            # the labels will be overwritten
+            R301 = p.create_relation(R1="__foo__ relation1")
+            R302 = p.create_relation(R1="__foo__ test qualifier")  # noqa
+
+            c = p.io.import_stms_from_rdf_triples(fpath)
+
+            c.new_items.sort(key=lambda itm: itm.R1__has_label)
+
+            x0, x1, x2 = c.new_items
+            # test that overwriting worked
+            self.assertEqual(R301.R1__has_label, "relation1")
+
+            # test that a statement has been created
+            self.assertEqual(x0.R301__relation1, [x1])
+
+    def test_b03__zebra_puzzle_import(self):
+        """
+        match persons which have four negative statements of the same kind (test statement relations)
+        """
+        zb = p.erkloader.load_mod_from_path(TEST_DATA_PATH_ZEBRA_BASE_DATA, prefix="zb")
+
+        self.assertEqual(zb.I9848["Norwegian"].zb__R8098__has_house_color, None)
+        self.assertEqual(zb.I9848["Norwegian"].zb__R1055__has_not_house_color, [])
+
+        # test to load facts
+
+        fpath = pjoin(TEST_DATA_DIR1, "test_zebra_triples1.nt")
+        with p.uri_context(uri=TEST_BASE_URI):
+            c = p.io.import_stms_from_rdf_triples(fpath)  #noqa
+        self.assertEqual(zb.I9848["Norwegian"].zb__R8098__has_house_color, zb.I4118["yellow"])
+        self.assertEqual(len(zb.I9848["Norwegian"].zb__R1055__has_not_house_color), 4)
+
+    def test_b04__zebra_puzzle_unlinked_items(self):
+        zb = p.erkloader.load_mod_from_path(TEST_DATA_PATH_ZEBRA_BASE_DATA, prefix="zb")
+        zp = p.erkloader.load_mod_from_path(TEST_DATA_PATH_ZEBRA02, prefix="zp")
+
+        # persons1 ... person12 exists -> if they are unlinked within a module this is not yet reflected in the
+        # rdf-data -> TODO: introduce a "Housekeeping" item for every module
+
+        # this tests ensures that at least the unlinked item is not present in the rdfgrap
+
+        with p.uri_context(uri=TEST_BASE_URI):
+            zp.person10.set_relation(zb.R8098["has house color"], zb.I7612["ivory"])
+            zp.person11.set_relation(zb.R8098["has house color"], zb.I4118["yellow"])
+            zp.person10.set_relation(zb.R3606["lives next to"], zp.person11)
+
+
+        fpath = pjoin(TEST_DATA_DIR1, "tmp_test.nt")
+        p.io.export_rdf_triples(fpath, add_qualifiers=True,  modfilter=TEST_BASE_URI)
+        g = p.io.import_raw_rdf_triples(fpath)
+
+        self.assertTrue(rdflib.URIRef(zp.person11.uri) in g.subjects())
+        self.assertTrue(rdflib.URIRef(zp.person11.uri) in g.objects())
+
+        p.core._unlink_entity(zp.person11.uri, remove_from_mod=True)
+
+        p.io.export_rdf_triples(fpath, add_qualifiers=True,  modfilter=TEST_BASE_URI)
+        g = p.io.import_raw_rdf_triples(fpath)
+
+        self.assertFalse(rdflib.URIRef(zp.person11.uri) in g.subjects())
+        self.assertFalse(rdflib.URIRef(zp.person11.uri) in g.objects())
+
+        os.unlink(fpath)
```

### Comparing `pyerk-0.6.5/tests/test_data/reports/reportconf.toml` & `pyerk-0.8.5/tests/test_data/reports/reportconf.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 journal = "default"
 
 [load_modules]
 
 # use absolute or relative paths here
 # (to simplify unittests, a path beginning with `$` will be preprocessed accordingly)
-ct = "$__erk-root__/erk-data-for-unittests/erk-ocse/control_theory1.py"
-ag = "$__erk-root__/erk-data-for-unittests/erk-ocse/agents1.py"
+ct = "$__erk-root__/erk-data-for-unittests/ocse/control_theory1.py"
+ag = "$__erk-root__/erk-data-for-unittests/ocse/agents1.py"
 
 
 # use an obviously fictious author combinations
 [authors.1]
 item = ":ag__I2746__Rudolf_Kalman"
 affiliation = ":ag__I7301__ETH_Zürich"
```

