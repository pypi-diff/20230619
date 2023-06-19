# Comparing `tmp/hgutilities-1.0.8.4.tar.gz` & `tmp/hgutilities-1.0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.8.4.tar", last modified: Mon Jun 19 13:18:27 2023, max compression
+gzip compressed data, was "hgutilities-1.0.8.5.tar", last modified: Mon Jun 19 13:21:55 2023, max compression
```

## Comparing `hgutilities-1.0.8.4.tar` & `hgutilities-1.0.8.5.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.581072 hgutilities-1.0.8.4/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.471411 hgutilities-1.0.8.4/.eggs/
--rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/README.txt
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.464627 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.475993 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
--rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
--rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
--rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
--rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
--rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.488090 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
--rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.496126 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
--rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.498134 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.500232 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
--rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
--rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
--rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
--rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
--rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
--rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
--rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
--rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
--rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
--rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
--rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
--rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
--rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.465512 hgutilities-1.0.8.4/.github/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.500791 hgutilities-1.0.8.4/.github/workflows/
--rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/.github/workflows/python-publish.yml
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:18:27.580703 hgutilities-1.0.8.4/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.501268 hgutilities-1.0.8.4/hgutilities/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.504770 hgutilities-1.0.8.4/hgutilities/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/Documentation/hgutilities.txt
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.505311 hgutilities-1.0.8.4/hgutilities/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/__pycache__/__init__.cpython-310.pyc
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.508033 hgutilities-1.0.8.4/hgutilities/defaults/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.511436 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/defaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/docs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/inherit.txt
--rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/Documentation/processkwargs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.514580 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.517794 hgutilities-1.0.8.4/hgutilities/plotting/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.521161 hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      830 2023-06-18 19:56:12.000000 hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      361 2023-06-18 19:56:18.000000 hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.526465 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/create_animations.txt
--rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/create_figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/Documentation/plotting.txt
--rw-r-----   0 henry     (1000) henry     (1000)    11039 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/README.md
--rw-r-----   0 henry     (1000) henry     (1000)     1132 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.530313 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     1137 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7866 2023-06-18 20:03:47.000000 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3949 2023-06-18 19:32:07.000000 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.8.4/hgutilities/plotting/animate.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.537170 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.542949 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-19 12:08:59.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.550450 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.557739 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/bar.py
--rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/bars.py
--rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/colorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/data.py
--rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/line.py
--rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/lines.py
--rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/pie.py
--rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/datatypes/surface.py
--rw-r-----   0 henry     (1000) henry     (1000)     6166 2023-06-19 13:18:08.000000 hgutilities-1.0.8.4/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2899 2023-06-18 19:31:35.000000 hgutilities-1.0.8.4/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      398 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.562013 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.563246 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.568595 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4394 2023-06-18 20:09:09.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4726 2023-06-18 20:06:55.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4997 2023-06-19 13:15:58.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plot.py
--rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotbars.py
--rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)     6981 2023-06-19 12:15:57.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotlines.py
--rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotpie.py
--rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotsurface.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.571708 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.574235 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1505 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/figuresize.py
--rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/griddimensions.py
--rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/plotshape.py
--rw-r-----   0 henry     (1000) henry     (1000)     1429 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/plotting/plotutils/savefigure.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.577051 hgutilities-1.0.8.4/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/utils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.580001 hgutilities-1.0.8.4/hgutilities/utils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.8.4/hgutilities/utils/__pycache__/groups.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.8.4/hgutilities/utils/__pycache__/paths.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.8.4/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:18:27.503738 hgutilities-1.0.8.4/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:18:27.000000 hgutilities-1.0.8.4/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     9254 2023-06-19 13:18:27.000000 hgutilities-1.0.8.4/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-19 13:18:27.000000 hgutilities-1.0.8.4/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-19 13:18:27.000000 hgutilities-1.0.8.4/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-19 13:18:27.000000 hgutilities-1.0.8.4/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-19 13:18:27.581163 hgutilities-1.0.8.4/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1455 2023-06-19 13:15:46.000000 hgutilities-1.0.8.4/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.880794 hgutilities-1.0.8.5/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.771950 hgutilities-1.0.8.5/.eggs/
+-rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/README.txt
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.765354 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.776787 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
+-rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
+-rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
+-rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
+-rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.792589 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
+-rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.800526 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.802900 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.805283 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
+-rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
+-rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
+-rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
+-rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
+-rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.766310 hgutilities-1.0.8.5/.github/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.805925 hgutilities-1.0.8.5/.github/workflows/
+-rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.github/workflows/python-publish.yml
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:21:55.880458 hgutilities-1.0.8.5/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.806460 hgutilities-1.0.8.5/hgutilities/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.810709 hgutilities-1.0.8.5/hgutilities/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/Documentation/hgutilities.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.811382 hgutilities-1.0.8.5/hgutilities/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.814641 hgutilities-1.0.8.5/hgutilities/defaults/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.818321 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/defaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/docs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/inherit.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.821906 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.826444 hgutilities-1.0.8.5/hgutilities/plotting/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.828666 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      803 2023-06-19 13:21:34.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      361 2023-06-18 19:56:18.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.832624 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_animations.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/plotting.txt
+-rw-r-----   0 henry     (1000) henry     (1000)    11039 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/README.md
+-rw-r-----   0 henry     (1000) henry     (1000)     1132 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.835976 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     1137 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7866 2023-06-18 20:03:47.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3949 2023-06-18 19:32:07.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.8.5/hgutilities/plotting/animate.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.841240 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.846667 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-19 12:08:59.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.852416 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.859221 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bar.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bars.py
+-rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/colorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/data.py
+-rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/line.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/lines.py
+-rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/pie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/surface.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6162 2023-06-19 13:21:37.000000 hgutilities-1.0.8.5/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2899 2023-06-18 19:31:35.000000 hgutilities-1.0.8.5/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      398 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.863356 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.864663 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.869289 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4394 2023-06-18 20:09:09.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4726 2023-06-18 20:06:55.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4997 2023-06-19 13:15:58.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotbars.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6981 2023-06-19 12:15:57.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotlines.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotpie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotsurface.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.872327 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.874906 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1505 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/figuresize.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/griddimensions.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/plotshape.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1429 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/savefigure.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.877553 hgutilities-1.0.8.5/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.879847 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/plots.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.809458 hgutilities-1.0.8.5/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     9254 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-19 13:21:55.880884 hgutilities-1.0.8.5/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1455 2023-06-19 13:19:57.000000 hgutilities-1.0.8.5/setup.py
```

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py` & `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/.github/workflows/python-publish.yml` & `hgutilities-1.0.8.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/LICENSE.md` & `hgutilities-1.0.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/PKG-INFO` & `hgutilities-1.0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.8.4
+Version: 1.0.8.5
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hgutilities-1.0.8.4/README.md` & `hgutilities-1.0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/Documentation/hgutilities.txt` & `hgutilities-1.0.8.5/hgutilities/Documentation/hgutilities.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/Documentation/defaults.txt` & `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/defaults.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/docs.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/Documentation/processkwargs.txt` & `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/processkwargs.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/docs.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/docs.py` & `hgutilities-1.0.8.5/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/inherit.py` & `hgutilities-1.0.8.5/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.8.5/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.8.5/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figure.txt`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9117647058823529%*

 * *Differences: {"'suptitle_x'": 'None', 'delete': "['suptitle_pad', 'suptitle_loc']"}*

```diff
@@ -11,17 +11,16 @@
     "hspace": null,
     "maximise": true,
     "subplots": null,
     "suptitle_color": null,
     "suptitle_fontname": null,
     "suptitle_fontsize": null,
     "suptitle_horizontalalignment": null,
-    "suptitle_loc": null,
-    "suptitle_pad": null,
     "suptitle_verticalalignment": null,
+    "suptitle_x": null,
     "suptitle_y": null,
     "title_color": null,
     "title_fontname": null,
     "title_fontsize": null,
     "title_horizontalalignment": null,
     "title_loc": null,
     "title_pad": null,
```

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Documentation/Animate.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Animate.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Documentation/Figures.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figures.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_animations.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Documentation/create_figures.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_figures.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/plotting.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/README.md` & `hgutilities-1.0.8.5/hgutilities/plotting/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__init__.py` & `hgutilities-1.0.8.5/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/animate.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/figure.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/figures.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/animate.py` & `hgutilities-1.0.8.5/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Data.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Data.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Line.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Default Settings/Surface.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Data.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Data.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/figure.py` & `hgutilities-1.0.8.5/hgutilities/plotting/figure.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                   "horizontalalignment": self.suptitle_horizontalalignment}
         self.suptitle_fontdict = remove_none_values(kwargs)
 
     def set_suptitle(self):
         if self.figures_obj.suptitle is not None:
             self.fig.suptitle(f"{self.figures_obj.suptitle}",
                               **self.suptitle_fontdict,
-                              y=self.suptitle_y, pad=self.suptitle_pad)
+                              x=self.suptitle_x, y=self.suptitle_y)
 
     def set_universal_legend(self):
         if self.figures_obj.universal_legend:
             self.do_universal_legend()
 
     def do_universal_legend(self):
         ax = self.axes[-1]
```

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/figures.py` & `hgutilities-1.0.8.5/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotbars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotlines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/savefigure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/utils/__pycache__/groups.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/utils/__pycache__/paths.cpython-310.pyc` & `hgutilities-1.0.8.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/utils/groups.py` & `hgutilities-1.0.8.5/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/utils/paths.py` & `hgutilities-1.0.8.5/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities/utils/plots.py` & `hgutilities-1.0.8.5/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.8.5/hgutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.8.4
+Version: 1.0.8.5
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hgutilities-1.0.8.4/hgutilities.egg-info/SOURCES.txt` & `hgutilities-1.0.8.5/hgutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.4/setup.py` & `hgutilities-1.0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.8.4"
+VERSION = "1.0.8.5"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
```

