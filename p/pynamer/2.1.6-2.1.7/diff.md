# Comparing `tmp/pynamer-2.1.6.tar.gz` & `tmp/pynamer-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.1.6.tar", last modified: Sat Jun 17 20:20:17 2023, max compression
+gzip compressed data, was "pynamer-2.1.7.tar", last modified: Mon Jun 19 19:04:55 2023, max compression
```

## Comparing `pynamer-2.1.6.tar` & `pynamer-2.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.534263 pynamer-2.1.6/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.6/AUTHORS.md
--rw-rw-rw-   0        0        0    11759 2023-06-17 20:20:04.000000 pynamer-2.1.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.6/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    19547 2023-06-17 20:20:17.535265 pynamer-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    17582 2023-06-17 19:07:40.000000 pynamer-2.1.6/README.md
--rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     2288 2023-06-17 20:20:17.540269 pynamer-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.289270 pynamer-2.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.398264 pynamer-2.1.6/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1989 2023-06-17 20:20:04.000000 pynamer-2.1.6/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.6/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.6/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.6/src/pynamer/config.py
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.418274 pynamer-2.1.6/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7935 2023-06-17 17:24:20.000000 pynamer-2.1.6/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.6/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.6/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0    11098 2023-06-14 17:55:57.000000 pynamer-2.1.6/src/pynamer/utils.py
--rw-rw-rw-   0        0        0    11810 2023-06-15 11:17:11.000000 pynamer-2.1.6/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.411273 pynamer-2.1.6/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    19547 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-17 20:20:17.000000 pynamer-2.1.6/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 20:20:17.531263 pynamer-2.1.6/tests/
--rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.6/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.6/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2900 2023-06-15 11:28:35.000000 pynamer-2.1.6/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1484 2023-06-14 19:03:12.000000 pynamer-2.1.6/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.6/tests/test_get_homepage.py
--rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.6/tests/test_github_meta.py
--rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.6/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.6/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.6/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1325 2023-06-14 17:55:57.000000 pynamer-2.1.6/tests/test_utils_search_json.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.6/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.6/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:55.234025 pynamer-2.1.7/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.1.7/AUTHORS.md
+-rw-rw-rw-   0        0        0    11947 2023-06-19 19:04:40.000000 pynamer-2.1.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    19784 2023-06-19 19:04:55.234025 pynamer-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    17816 2023-06-19 12:49:30.000000 pynamer-2.1.7/README.md
+-rw-rw-rw-   0        0        0     2183 2023-06-11 20:09:06.000000 pynamer-2.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     2288 2023-06-19 19:04:55.236026 pynamer-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.788031 pynamer-2.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.886027 pynamer-2.1.7/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-19 19:04:40.000000 pynamer-2.1.7/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.1.7/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2462 2023-06-12 20:06:37.000000 pynamer-2.1.7/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      863 2023-06-12 20:04:32.000000 pynamer-2.1.7/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.901026 pynamer-2.1.7/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7935 2023-06-17 17:24:20.000000 pynamer-2.1.7/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-06-04 12:15:11.000000 pynamer-2.1.7/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.1.7/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0    11098 2023-06-14 17:55:57.000000 pynamer-2.1.7/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0    11922 2023-06-19 18:58:14.000000 pynamer-2.1.7/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:54.898025 pynamer-2.1.7/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    19784 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 19:04:54.000000 pynamer-2.1.7/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 19:04:55.231044 pynamer-2.1.7/tests/
+-rw-rw-rw-   0        0        0     2159 2023-06-12 20:06:37.000000 pynamer-2.1.7/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1617 2023-06-04 12:01:20.000000 pynamer-2.1.7/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2900 2023-06-15 11:28:35.000000 pynamer-2.1.7/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1484 2023-06-14 19:03:12.000000 pynamer-2.1.7/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0     1712 2023-06-06 13:17:16.000000 pynamer-2.1.7/tests/test_get_homepage.py
+-rw-rw-rw-   0        0        0     2025 2023-06-12 20:09:06.000000 pynamer-2.1.7/tests/test_github_meta.py
+-rw-rw-rw-   0        0        0      329 2023-06-07 13:07:48.000000 pynamer-2.1.7/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     2568 2023-06-06 13:17:15.000000 pynamer-2.1.7/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.1.7/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1325 2023-06-14 17:55:57.000000 pynamer-2.1.7/tests/test_utils_search_json.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.1.7/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.1.7/tests/test_write_output_file.py
```

### Comparing `pynamer-2.1.6/CHANGELOG.md` & `pynamer-2.1.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.1.7 (2023-06-19)
+### Fix
+* Account for hompepoage beginning with http: ([`d9dcb50`](https://github.com/Stephen-RA-King/pynamer/commit/d9dcb50b4e6321d681a16aeba88bc2a2908f1005))
+
 ## v2.1.6 (2023-06-17)
 ### Fix
 * Error message regarding pypirc file before registration ([`ded4143`](https://github.com/Stephen-RA-King/pynamer/commit/ded4143062a1e2fb5cf74c2912dea692d64fac17))
 
 ### Documentation
 * Update logo ([`6be0f9a`](https://github.com/Stephen-RA-King/pynamer/commit/6be0f9ae77e6b63f382e1a490b57153a589a8920))
 * Add missing docstrings ([`1377322`](https://github.com/Stephen-RA-King/pynamer/commit/1377322620a7894bc036021c9cde50bcd4cc732b))
```

### Comparing `pynamer-2.1.6/LICENSE` & `pynamer-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/PKG-INFO` & `pynamer-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.6
+Version: 2.1.7
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -35,14 +35,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
@@ -452,15 +453,14 @@
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/b95fb617fbcd469ccfc3/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynamer/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynamer
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
@@ -468,14 +468,16 @@
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
@@ -486,16 +488,17 @@
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
-[pypi-url]: https://pypi.org/project/pynamer/
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
+[pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynamer/wiki
```

### Comparing `pynamer-2.1.6/README.md` & `pynamer-2.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
@@ -420,15 +421,14 @@
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/b95fb617fbcd469ccfc3/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynamer/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynamer
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
@@ -436,14 +436,16 @@
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
@@ -454,16 +456,17 @@
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
-[pypi-url]: https://pypi.org/project/pynamer/
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
+[pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynamer/wiki
```

### Comparing `pynamer-2.1.6/pyproject.toml` & `pynamer-2.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/setup.cfg` & `pynamer-2.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/__init__.py` & `pynamer-2.1.7/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.1.6/src/pynamer/builder.py` & `pynamer-2.1.7/src/pynamer/builder.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/cli.py` & `pynamer-2.1.7/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/config.py` & `pynamer-2.1.7/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/pynamer.py` & `pynamer-2.1.7/src/pynamer/pynamer.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/utils.py` & `pynamer-2.1.7/src/pynamer/utils.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/src/pynamer/validators.py` & `pynamer-2.1.7/src/pynamer/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,16 @@
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
 
         homepage_text, homepage_url = _get_homepage(project_json, project_name)
+        if homepage_url.startswith("http:"):
+            homepage_url = homepage_url.replace("http:", "https:")
 
         author = (
             "".join(["Author:   ", project_json["info"]["author"]])
             if project_json["info"]["author"]
             else "Author:   None"
         )
         version = (
```

### Comparing `pynamer-2.1.6/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.1.7/src/pynamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.1.6
+Version: 2.1.7
 Summary: Utility to find an available package name in the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -35,14 +35,15 @@
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
 [![CodeQl][codeql-image]][codeql-url]
+[![Docker][docker-image]][docker-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
@@ -452,15 +453,14 @@
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/b95fb617fbcd469ccfc3/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynamer/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynamer/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynamer
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynamer
@@ -468,14 +468,16 @@
 [codeql-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/github-code-scanning/codeql
 [commitizen-image]: https://img.shields.io/badge/commitizen-friendly-brightgreen.svg
 [commitizen-url]: http://commitizen.github.io/cz-cli/
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynamer/?ref=repository-badge
+[docker-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml/badge.svg
+[docker-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/docker-image.yml
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynamer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynamer
 [format-image]: https://img.shields.io/pypi/format/pynamer
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
@@ -486,16 +488,17 @@
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
-[pypi-url]: https://pypi.org/project/pynamer/
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [pypi-image]: https://img.shields.io/pypi/v/pynamer.svg
+[pypi-url]: https://pypi.org/project/pynamer/
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynamer
 [readthedocs-image]: https://readthedocs.org/projects/pynamer/badge/?version=latest
 [readthedocs-url]: https://pynamer.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynamer.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynamer/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynamer/wiki
```

### Comparing `pynamer-2.1.6/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.1.7/src/pynamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_args.py` & `pynamer-2.1.7/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_build_dist.py` & `pynamer-2.1.7/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_cleanup.py` & `pynamer-2.1.7/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_create_setup_file.py` & `pynamer-2.1.7/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_defaults.py` & `pynamer-2.1.7/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_delete_director.py` & `pynamer-2.1.7/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_feedback.py` & `pynamer-2.1.7/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_final_analysis.py` & `pynamer-2.1.7/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_find_pypirc_file.py` & `pynamer-2.1.7/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_generate_pypi_index.py` & `pynamer-2.1.7/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_get_homepage.py` & `pynamer-2.1.7/tests/test_get_homepage.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_github_meta.py` & `pynamer-2.1.7/tests/test_github_meta.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_ping_json.py` & `pynamer-2.1.7/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_ping_project.py` & `pynamer-2.1.7/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_process_input_file.py` & `pynamer-2.1.7/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_pypi_search.py` & `pynamer-2.1.7/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_pypi_search_index.py` & `pynamer-2.1.7/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_rename_project_dir.py` & `pynamer-2.1.7/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_upload_dist.py` & `pynamer-2.1.7/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_utils_search_json.py` & `pynamer-2.1.7/tests/test_utils_search_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_utils_version.py` & `pynamer-2.1.7/tests/test_utils_version.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.1.6/tests/test_write_output_file.py` & `pynamer-2.1.7/tests/test_write_output_file.py`

 * *Files identical despite different names*

