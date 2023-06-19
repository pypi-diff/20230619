# Comparing `tmp/hgutilities-1.0.8.5.tar.gz` & `tmp/hgutilities-1.0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.8.5.tar", last modified: Mon Jun 19 13:21:55 2023, max compression
+gzip compressed data, was "hgutilities-1.0.8.6.tar", last modified: Mon Jun 19 17:20:30 2023, max compression
```

## Comparing `hgutilities-1.0.8.5.tar` & `hgutilities-1.0.8.6.tar`

### file list

```diff
@@ -1,201 +1,207 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.880794 hgutilities-1.0.8.5/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.771950 hgutilities-1.0.8.5/.eggs/
--rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/README.txt
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.765354 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.776787 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
--rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
--rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
--rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
--rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
--rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.792589 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
--rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.800526 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
--rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.802900 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.805283 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
--rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
--rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
--rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
--rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
--rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
--rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
--rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
--rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
--rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
--rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
--rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
--rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
--rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.766310 hgutilities-1.0.8.5/.github/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.805925 hgutilities-1.0.8.5/.github/workflows/
--rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/.github/workflows/python-publish.yml
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:21:55.880458 hgutilities-1.0.8.5/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.806460 hgutilities-1.0.8.5/hgutilities/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.810709 hgutilities-1.0.8.5/hgutilities/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/Documentation/hgutilities.txt
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.811382 hgutilities-1.0.8.5/hgutilities/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/__pycache__/__init__.cpython-310.pyc
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.814641 hgutilities-1.0.8.5/hgutilities/defaults/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.818321 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/defaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/docs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/inherit.txt
--rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/Documentation/processkwargs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.821906 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.826444 hgutilities-1.0.8.5/hgutilities/plotting/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.828666 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      803 2023-06-19 13:21:34.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      361 2023-06-18 19:56:18.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.832624 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_animations.txt
--rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/Documentation/plotting.txt
--rw-r-----   0 henry     (1000) henry     (1000)    11039 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/README.md
--rw-r-----   0 henry     (1000) henry     (1000)     1132 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.835976 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     1137 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7866 2023-06-18 20:03:47.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3949 2023-06-18 19:32:07.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.8.5/hgutilities/plotting/animate.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.841240 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.846667 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-19 12:08:59.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.852416 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.859221 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bar.py
--rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bars.py
--rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/colorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/data.py
--rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/line.py
--rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/lines.py
--rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/pie.py
--rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/datatypes/surface.py
--rw-r-----   0 henry     (1000) henry     (1000)     6162 2023-06-19 13:21:37.000000 hgutilities-1.0.8.5/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2899 2023-06-18 19:31:35.000000 hgutilities-1.0.8.5/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      398 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.863356 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.864663 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.869289 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4394 2023-06-18 20:09:09.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4726 2023-06-18 20:06:55.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4997 2023-06-19 13:15:58.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plot.py
--rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotbars.py
--rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)     6981 2023-06-19 12:15:57.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotlines.py
--rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotpie.py
--rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotsurface.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.872327 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.874906 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1505 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/figuresize.py
--rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/griddimensions.py
--rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/plotshape.py
--rw-r-----   0 henry     (1000) henry     (1000)     1429 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/plotting/plotutils/savefigure.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.877553 hgutilities-1.0.8.5/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.879847 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.8.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.8.5/hgutilities/utils/plots.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 13:21:55.809458 hgutilities-1.0.8.5/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     9254 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-19 13:21:55.000000 hgutilities-1.0.8.5/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-19 13:21:55.880884 hgutilities-1.0.8.5/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1455 2023-06-19 13:19:57.000000 hgutilities-1.0.8.5/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.758204 hgutilities-1.0.8.6/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.608407 hgutilities-1.0.8.6/.eggs/
+-rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/README.txt
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.598235 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.615489 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
+-rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
+-rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
+-rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
+-rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.634556 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
+-rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.645651 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.648637 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.651453 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
+-rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
+-rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
+-rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
+-rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
+-rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.599576 hgutilities-1.0.8.6/.github/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.652040 hgutilities-1.0.8.6/.github/workflows/
+-rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.github/workflows/python-publish.yml
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 17:20:30.757745 hgutilities-1.0.8.6/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.652530 hgutilities-1.0.8.6/hgutilities/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.655966 hgutilities-1.0.8.6/hgutilities/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/Documentation/hgutilities.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.656488 hgutilities-1.0.8.6/hgutilities/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.659893 hgutilities-1.0.8.6/hgutilities/defaults/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.665316 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/defaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/docs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/inherit.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.669866 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.676108 hgutilities-1.0.8.6/hgutilities/plotting/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.680549 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      842 2023-06-19 13:58:26.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      366 2023-06-19 13:52:51.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       73 2023-06-19 17:09:56.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Quick.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.686577 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_animations.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/plotting.txt
+-rw-r-----   0 henry     (1000) henry     (1000)    12516 2023-06-19 16:24:29.000000 hgutilities-1.0.8.6/hgutilities/plotting/README.md
+-rw-r-----   0 henry     (1000) henry     (1000)     1220 2023-06-19 15:37:00.000000 hgutilities-1.0.8.6/hgutilities/plotting/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.692022 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     1193 2023-06-19 15:39:42.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7823 2023-06-19 14:01:32.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3985 2023-06-19 17:06:30.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      770 2023-06-19 17:02:15.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5885 2023-06-19 17:16:52.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/quick.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.8.6/hgutilities/plotting/animate.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.700248 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.708011 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-19 12:08:59.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.715365 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.722747 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bar.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bars.py
+-rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/colorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/data.py
+-rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/line.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/lines.py
+-rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/pie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/surface.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6162 2023-06-19 13:54:04.000000 hgutilities-1.0.8.6/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2944 2023-06-19 17:04:36.000000 hgutilities-1.0.8.6/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      545 2023-06-19 17:02:12.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.729345 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.731277 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.738251 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5316 2023-06-19 14:01:33.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4790 2023-06-19 14:01:33.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4997 2023-06-19 13:15:58.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotbars.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6981 2023-06-19 12:15:57.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotlines.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotpie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotsurface.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.742595 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.746633 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1770 2023-06-19 14:04:15.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/figuresize.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/griddimensions.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/plotshape.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1789 2023-06-19 14:04:01.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/savefigure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4591 2023-06-19 17:16:47.000000 hgutilities-1.0.8.6/hgutilities/plotting/quick.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.752362 hgutilities-1.0.8.6/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.756875 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2242 2023-06-19 16:46:20.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/readwrite.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2373 2023-06-14 13:20:48.000000 hgutilities-1.0.8.6/hgutilities/utils/filenames.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/plots.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1154 2023-06-14 13:31:22.000000 hgutilities-1.0.8.6/hgutilities/utils/readwrite.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.654995 hgutilities-1.0.8.6/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     9505 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-19 17:20:30.758332 hgutilities-1.0.8.6/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1455 2023-06-19 13:29:22.000000 hgutilities-1.0.8.6/setup.py
```

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py` & `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/.github/workflows/python-publish.yml` & `hgutilities-1.0.8.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/LICENSE.md` & `hgutilities-1.0.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/PKG-INFO` & `hgutilities-1.0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.8.5
+Version: 1.0.8.6
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hgutilities-1.0.8.5/README.md` & `hgutilities-1.0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/Documentation/hgutilities.txt` & `hgutilities-1.0.8.6/hgutilities/Documentation/hgutilities.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/defaults.txt` & `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/defaults.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/docs.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/Documentation/processkwargs.txt` & `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/processkwargs.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/docs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/docs.py` & `hgutilities-1.0.8.6/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/inherit.py` & `hgutilities-1.0.8.6/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.8.6/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.8.6/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figure.txt`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'file_name'": 'None', "'path'": 'None'}*

```diff
@@ -3,17 +3,19 @@
     "axis_fontname": null,
     "axis_fontsize": null,
     "axis_labelpad": null,
     "axis_loc": null,
     "dark": false,
     "dpi": null,
     "figure_size": null,
+    "file_name": null,
     "h_pad": 0.3,
     "hspace": null,
     "maximise": true,
+    "path": null,
     "subplots": null,
     "suptitle_color": null,
     "suptitle_fontname": null,
     "suptitle_fontsize": null,
     "suptitle_horizontalalignment": null,
     "suptitle_verticalalignment": null,
     "suptitle_x": null,
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Animate.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Animate.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/Figures.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Figures.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_animations.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/create_figures.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_figures.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/plotting.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/README.md` & `hgutilities-1.0.8.6/hgutilities/plotting/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     1. [Figure](#figure)
     1. [Plot](#plot)
     1. [Data](#data)
 1. [Usage](#usage)
 1. [Features](#features)
     1. [Universal Legend](#universal-legend)
     1. [Subplot Adjustment](#subplot-adjustment)
+    1. [Quick Plot](#quick-plot)
 
 ## Overview and Structure
 
 This is a tool designed to make creating figures with multiple subplots easier. The data is prescribed, and the creation of the figures is handled by the package.
 
 ### Figures
 
@@ -194,8 +195,22 @@
 
 ### Universal Legend
 
 The universal legend is a tool that can be used if all subplots in a figure have the same legend. An extra blank subplot is created and the space is used to show a legend that corresponds to all plots. This can be activated by passing `universal_legend=True` as a keyword-value pair into the `create_figures` function, and any individual legends will be overruled. Exception handling not implemented, will crash or get unexpected results if not used properly.
 
 ### Subplot Adjustment
 
-Note: this feature has not been implemented yet. If the optional keyword argument, `adjust_subplots=True` is passed in to `create_figures` (or `create_animation`), then the matplotlib subplot adjustment tool will appear when the figures are created. The subplots are usually plotted with using the constrained layout, but in this case that will be turned off and tight layout used instead.
+Note: this feature has not been implemented yet. If the optional keyword argument, `adjust_subplots=True` is passed in to `create_figures` (or `create_animation`), then the matplotlib subplot adjustment tool will appear when the figures are created. The subplots are usually plotted with using the constrained layout, but in this case that will be turned off and tight layout used instead.
+
+### Quick Plot
+
+This generates a figure from saved data with a single line of code. It gives very little control and the aim is to get an idea of what the data looks like very fast. The format of the files with the data are expected to have a single line header with the names of the variables and these will be used as the axis labels. The columns are assumed to be separated by tabs, but this is controllable with the `separator` keyword. The independent and dependent variables are assumed to be the 0'th and 1st columns, but these can be changed with the `x` and `y` keyword arguments. The main control is given by the form of the input of the data to plot, detailed below.
+
+- Path to file. A single plot with a single line on it.
+- Path to folder with `one_line_per_plot=True`. Each file within the folder will be plotted on it's own subplot.
+- Path to folder with `one_line_per_plot=False`. All files within the folder will be plotted on one subplot.
+- List of paths to files with `one_line_per_plot=True`. Each file plotting on it's own subplot.
+- List of paths to files with `one_line_per_plot=False`. All files plotting on one subplot.
+- Two dimensional list of paths to files. Each outer list corresponds to one subplot.
+- List of paths to folders. The contents of each folder will be plotted on one subplot each.
+
+If a dictionary is given in place of a list/tuple/array then the values will be used and not the keys.
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/__init__.py` & `hgutilities-1.0.8.6/hgutilities/plotting/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from ..defaults import docs
 
-# Functions and classes to be accessed by the user
+# Functions to be accessed by the user
 from .plotfunctions import create_figures
 from .plotfunctions import create_animations
+from .plotfunctions import quick
+
+# Classes to be accessed by the user
 from .datatypes.line import Line as line
 from .datatypes.lines import Lines as lines
 from .datatypes.bars import Bars as bars
 from .datatypes.bar import Bar as bar
 from .datatypes.pie import Pie as pie
 from .datatypes.surface import Surface as surface
 from .datatypes.colorplot import Colorplot as colorplot
@@ -26,9 +29,10 @@
 PlotPie.set_function_dict()
 PlotSurface.set_function_dict()
 PlotColorplot.set_function_dict()
 
 # Importing other classes that have documentation
 # files so they can be detected by defaults.doc
 from .animate import Animate
+from .quick import Quick
 
 docs()
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 19:06:03 2023 UTC, .py size: 1132 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-00000000: 6f0d 0d0a 0000 0000 9b55 8f64 6c04 0000  o........U.dl...
+00000000: 6f0d 0d0a 0000 0000 1c76 9064 c404 0000  o........v.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
-00000050: 0100 6402 6405 6c05 6d06 5a07 0100 6402  ..d.d.l.m.Z...d.
-00000060: 6406 6c08 6d09 5a0a 0100 6402 6407 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0d 0100 6402 6408 6c0e 6d0f 5a10  m.Z...d.d.l.m.Z.
-00000080: 0100 6402 6409 6c11 6d12 5a13 0100 6402  ..d.d.l.m.Z...d.
-00000090: 640a 6c14 6d15 5a16 0100 6402 640b 6c17  d.l.m.Z...d.d.l.
-000000a0: 6d18 5a19 0100 6402 640c 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
-000000b0: 0100 6402 640d 6c1c 6d1d 5a1d 0100 6402  ..d.d.l.m.Z...d.
-000000c0: 640e 6c1e 6d1f 5a1f 0100 6402 640f 6c20  d.l.m.Z...d.d.l 
-000000d0: 6d21 5a21 0100 6402 6410 6c22 6d23 5a23  m!Z!..d.d.l"m#Z#
-000000e0: 0100 6402 6411 6c24 6d25 5a25 0100 651b  ..d.d.l$m%Z%..e.
-000000f0: a026 a100 0100 651d a027 a100 0100 651f  .&....e..'....e.
-00000100: a027 a100 0100 6521 a027 a100 0100 6523  .'....e!.'....e#
-00000110: a027 a100 0100 6525 a027 a100 0100 6402  .'....e%.'....d.
-00000120: 6412 6c28 6d29 5a29 0100 6501 8300 0100  d.l(m)Z)..e.....
-00000130: 6413 5300 2914 e902 0000 0029 01da 0464  d.S.)......)...d
-00000140: 6f63 73e9 0100 0000 2901 da0e 6372 6561  ocs.....)...crea
-00000150: 7465 5f66 6967 7572 6573 2901 da11 6372  te_figures)...cr
-00000160: 6561 7465 5f61 6e69 6d61 7469 6f6e 7329  eate_animations)
-00000170: 01da 044c 696e 6529 01da 054c 696e 6573  ...Line)...Lines
-00000180: 2901 da04 4261 7273 2901 da03 4261 7229  )...Bars)...Bar)
-00000190: 01da 0350 6965 2901 da07 5375 7266 6163  ...Pie)...Surfac
-000001a0: 6529 01da 0943 6f6c 6f72 706c 6f74 2901  e)...Colorplot).
-000001b0: da06 4669 6775 7265 2901 da09 506c 6f74  ..Figure)...Plot
-000001c0: 4c69 6e65 7329 01da 0850 6c6f 7442 6172  Lines)...PlotBar
-000001d0: 7329 01da 0750 6c6f 7450 6965 2901 da0b  s)...PlotPie)...
-000001e0: 506c 6f74 5375 7266 6163 6529 01da 0d50  PlotSurface)...P
-000001f0: 6c6f 7443 6f6c 6f72 706c 6f74 2901 da07  lotColorplot)...
-00000200: 416e 696d 6174 654e 292a da08 6465 6661  AnimateN)*..defa
-00000210: 756c 7473 7202 0000 00da 0d70 6c6f 7466  ultsr......plotf
-00000220: 756e 6374 696f 6e73 7204 0000 0072 0500  unctionsr....r..
-00000230: 0000 da0e 6461 7461 7479 7065 732e 6c69  ....datatypes.li
-00000240: 6e65 7206 0000 00da 046c 696e 65da 0f64  ner......line..d
-00000250: 6174 6174 7970 6573 2e6c 696e 6573 7207  atatypes.linesr.
-00000260: 0000 00da 056c 696e 6573 da0e 6461 7461  .....lines..data
-00000270: 7479 7065 732e 6261 7273 7208 0000 00da  types.barsr.....
-00000280: 0462 6172 73da 0d64 6174 6174 7970 6573  .bars..datatypes
-00000290: 2e62 6172 7209 0000 00da 0362 6172 da0d  .barr......bar..
-000002a0: 6461 7461 7479 7065 732e 7069 6572 0a00  datatypes.pier..
-000002b0: 0000 da03 7069 65da 1164 6174 6174 7970  ....pie..datatyp
-000002c0: 6573 2e73 7572 6661 6365 720b 0000 00da  es.surfacer.....
-000002d0: 0773 7572 6661 6365 da13 6461 7461 7479  .surface..dataty
-000002e0: 7065 732e 636f 6c6f 7270 6c6f 7472 0c00  pes.colorplotr..
-000002f0: 0000 da09 636f 6c6f 7270 6c6f 74da 0666  ....colorplot..f
-00000300: 6967 7572 6572 0d00 0000 da13 706c 6f74  igurer......plot
-00000310: 7479 7065 732e 706c 6f74 6c69 6e65 7372  types.plotlinesr
-00000320: 0e00 0000 da12 706c 6f74 7479 7065 732e  ......plottypes.
-00000330: 706c 6f74 6261 7273 720f 0000 00da 1170  plotbarsr......p
-00000340: 6c6f 7474 7970 6573 2e70 6c6f 7470 6965  lottypes.plotpie
-00000350: 7210 0000 00da 1570 6c6f 7474 7970 6573  r......plottypes
-00000360: 2e70 6c6f 7473 7572 6661 6365 7211 0000  .plotsurfacer...
-00000370: 00da 1770 6c6f 7474 7970 6573 2e70 6c6f  ...plottypes.plo
-00000380: 7463 6f6c 6f72 706c 6f74 7212 0000 00da  tcolorplotr.....
-00000390: 1073 6574 5f70 6c6f 745f 636c 6173 7365  .set_plot_classe
-000003a0: 73da 1173 6574 5f66 756e 6374 696f 6e5f  s..set_function_
-000003b0: 6469 6374 da07 616e 696d 6174 6572 1300  dict..animater..
-000003c0: 0000 a900 722d 0000 0072 2d00 0000 fa5e  ....r-...r-....^
-000003d0: 2f6d 6e74 2f32 5442 2f44 6f63 756d 656e  /mnt/2TB/Documen
-000003e0: 7473 2f50 7974 686f 6e2f 5265 616c 2057  ts/Python/Real W
-000003f0: 6f72 6c64 2041 7070 6c69 6361 7469 6f6e  orld Application
-00000400: 732f 6867 7574 696c 6974 6965 732f 6867  s/hgutilities/hg
-00000410: 7574 696c 6974 6965 732f 706c 6f74 7469  utilities/plotti
-00000420: 6e67 2f5f 5f69 6e69 745f 5f2e 7079 da08  ng/__init__.py..
-00000430: 3c6d 6f64 756c 653e 0100 0000 7330 0000  <module>....s0..
-00000440: 000c 000c 030c 010c 010c 010c 010c 010c  ................
-00000450: 010c 010c 010c 030c 010c 010c 010c 010c  ................
-00000460: 0108 0308 0108 0108 0108 0108 010c 040a  ................
-00000470: 02                                       .
+00000050: 0100 6402 6405 6c02 6d05 5a05 0100 6402  ..d.d.l.m.Z...d.
+00000060: 6406 6c06 6d07 5a08 0100 6402 6407 6c09  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0b 0100 6402 6408 6c0c 6d0d 5a0e  m.Z...d.d.l.m.Z.
+00000080: 0100 6402 6409 6c0f 6d10 5a11 0100 6402  ..d.d.l.m.Z...d.
+00000090: 640a 6c12 6d13 5a14 0100 6402 640b 6c15  d.l.m.Z...d.d.l.
+000000a0: 6d16 5a17 0100 6402 640c 6c18 6d19 5a1a  m.Z...d.d.l.m.Z.
+000000b0: 0100 6402 640d 6c1b 6d1c 5a1c 0100 6402  ..d.d.l.m.Z...d.
+000000c0: 640e 6c1d 6d1e 5a1e 0100 6402 640f 6c1f  d.l.m.Z...d.d.l.
+000000d0: 6d20 5a20 0100 6402 6410 6c21 6d22 5a22  m Z ..d.d.l!m"Z"
+000000e0: 0100 6402 6411 6c23 6d24 5a24 0100 6402  ..d.d.l#m$Z$..d.
+000000f0: 6412 6c25 6d26 5a26 0100 651c a027 a100  d.l%m&Z&..e..'..
+00000100: 0100 651e a028 a100 0100 6520 a028 a100  ..e..(....e .(..
+00000110: 0100 6522 a028 a100 0100 6524 a028 a100  ..e".(....e$.(..
+00000120: 0100 6526 a028 a100 0100 6402 6413 6c29  ..e&.(....d.d.l)
+00000130: 6d2a 5a2a 0100 6402 6414 6c05 6d2b 5a2b  m*Z*..d.d.l.m+Z+
+00000140: 0100 6501 8300 0100 6415 5300 2916 e902  ..e.....d.S.)...
+00000150: 0000 0029 01da 0464 6f63 73e9 0100 0000  ...)...docs.....
+00000160: 2901 da0e 6372 6561 7465 5f66 6967 7572  )...create_figur
+00000170: 6573 2901 da11 6372 6561 7465 5f61 6e69  es)...create_ani
+00000180: 6d61 7469 6f6e 7329 01da 0571 7569 636b  mations)...quick
+00000190: 2901 da04 4c69 6e65 2901 da05 4c69 6e65  )...Line)...Line
+000001a0: 7329 01da 0442 6172 7329 01da 0342 6172  s)...Bars)...Bar
+000001b0: 2901 da03 5069 6529 01da 0753 7572 6661  )...Pie)...Surfa
+000001c0: 6365 2901 da09 436f 6c6f 7270 6c6f 7429  ce)...Colorplot)
+000001d0: 01da 0646 6967 7572 6529 01da 0950 6c6f  ...Figure)...Plo
+000001e0: 744c 696e 6573 2901 da08 506c 6f74 4261  tLines)...PlotBa
+000001f0: 7273 2901 da07 506c 6f74 5069 6529 01da  rs)...PlotPie)..
+00000200: 0b50 6c6f 7453 7572 6661 6365 2901 da0d  .PlotSurface)...
+00000210: 506c 6f74 436f 6c6f 7270 6c6f 7429 01da  PlotColorplot)..
+00000220: 0741 6e69 6d61 7465 2901 da05 5175 6963  .Animate)...Quic
+00000230: 6b4e 292c da08 6465 6661 756c 7473 7202  kN),..defaultsr.
+00000240: 0000 00da 0d70 6c6f 7466 756e 6374 696f  .....plotfunctio
+00000250: 6e73 7204 0000 0072 0500 0000 7206 0000  nsr....r....r...
+00000260: 00da 0e64 6174 6174 7970 6573 2e6c 696e  ...datatypes.lin
+00000270: 6572 0700 0000 da04 6c69 6e65 da0f 6461  er......line..da
+00000280: 7461 7479 7065 732e 6c69 6e65 7372 0800  tatypes.linesr..
+00000290: 0000 da05 6c69 6e65 73da 0e64 6174 6174  ....lines..datat
+000002a0: 7970 6573 2e62 6172 7372 0900 0000 da04  ypes.barsr......
+000002b0: 6261 7273 da0d 6461 7461 7479 7065 732e  bars..datatypes.
+000002c0: 6261 7272 0a00 0000 da03 6261 72da 0d64  barr......bar..d
+000002d0: 6174 6174 7970 6573 2e70 6965 720b 0000  atatypes.pier...
+000002e0: 00da 0370 6965 da11 6461 7461 7479 7065  ...pie..datatype
+000002f0: 732e 7375 7266 6163 6572 0c00 0000 da07  s.surfacer......
+00000300: 7375 7266 6163 65da 1364 6174 6174 7970  surface..datatyp
+00000310: 6573 2e63 6f6c 6f72 706c 6f74 720d 0000  es.colorplotr...
+00000320: 00da 0963 6f6c 6f72 706c 6f74 da06 6669  ...colorplot..fi
+00000330: 6775 7265 720e 0000 00da 1370 6c6f 7474  gurer......plott
+00000340: 7970 6573 2e70 6c6f 746c 696e 6573 720f  ypes.plotlinesr.
+00000350: 0000 00da 1270 6c6f 7474 7970 6573 2e70  .....plottypes.p
+00000360: 6c6f 7462 6172 7372 1000 0000 da11 706c  lotbarsr......pl
+00000370: 6f74 7479 7065 732e 706c 6f74 7069 6572  ottypes.plotpier
+00000380: 1100 0000 da15 706c 6f74 7479 7065 732e  ......plottypes.
+00000390: 706c 6f74 7375 7266 6163 6572 1200 0000  plotsurfacer....
+000003a0: da17 706c 6f74 7479 7065 732e 706c 6f74  ..plottypes.plot
+000003b0: 636f 6c6f 7270 6c6f 7472 1300 0000 da10  colorplotr......
+000003c0: 7365 745f 706c 6f74 5f63 6c61 7373 6573  set_plot_classes
+000003d0: da11 7365 745f 6675 6e63 7469 6f6e 5f64  ..set_function_d
+000003e0: 6963 74da 0761 6e69 6d61 7465 7214 0000  ict..animater...
+000003f0: 0072 1500 0000 a900 722f 0000 0072 2f00  .r......r/...r/.
+00000400: 0000 fa5e 2f6d 6e74 2f32 5442 2f44 6f63  ...^/mnt/2TB/Doc
+00000410: 756d 656e 7473 2f50 7974 686f 6e2f 5265  uments/Python/Re
+00000420: 616c 2057 6f72 6c64 2041 7070 6c69 6361  al World Applica
+00000430: 7469 6f6e 732f 6867 7574 696c 6974 6965  tions/hgutilitie
+00000440: 732f 6867 7574 696c 6974 6965 732f 706c  s/hgutilities/pl
+00000450: 6f74 7469 6e67 2f5f 5f69 6e69 745f 5f2e  otting/__init__.
+00000460: 7079 da08 3c6d 6f64 756c 653e 0100 0000  py..<module>....
+00000470: 7334 0000 000c 000c 030c 010c 010c 030c  s4..............
+00000480: 010c 010c 010c 010c 010c 010c 030c 010c  ................
+00000490: 010c 010c 010c 0108 0308 0108 0108 0108  ................
+000004a0: 0108 010c 040c 010a 02                   .........
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/animate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 20:02:49 2023 UTC, .py size: 6189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e962 8f64 2d18 0000  o........b.d-...
+00000000: 6f0d 0d0a 0000 0000 fc5d 9064 1218 0000  o........].d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a06 0100 6400 6401 6c07 5a08 6403  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6405 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6405 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -48,445 +48,442 @@
 000002f0: 0074 0074 0174 0274 0374 0464 019c 057c  .t.t.t.t.t.d...|
 00000300: 005f 0564 0053 0029 024e 2905 da05 4c69  ._.d.S.).N)...Li
 00000310: 6e65 73da 0442 6172 73da 0350 6965 da09  nes..Bars..Pie..
 00000320: 436f 6c6f 7270 6c6f 74da 0753 7572 6661  Colorplot..Surfa
 00000330: 6365 2906 7206 0000 0072 0700 0000 7208  ce).r....r....r.
 00000340: 0000 0072 0900 0000 720a 0000 00da 0c70  ...r....r......p
 00000350: 6c6f 745f 636c 6173 7365 7329 01da 0363  lot_classes)...c
-00000360: 6c73 a900 7217 0000 00fa 5c2f 6d6e 742f  ls..r.....\/mnt/
-00000370: 3254 422f 446f 6375 6d65 6e74 732f 5079  2TB/Documents/Py
-00000380: 7468 6f6e 2f52 6561 6c20 576f 726c 6420  thon/Real World 
-00000390: 4170 706c 6963 6174 696f 6e73 2f68 6775  Applications/hgu
-000003a0: 7469 6c69 7469 6573 2f68 6775 7469 6c69  tilities/hgutili
-000003b0: 7469 6573 2f70 6c6f 7474 696e 672f 6669  ties/plotting/fi
-000003c0: 6775 7265 2e70 79da 1073 6574 5f70 6c6f  gure.py..set_plo
-000003d0: 745f 636c 6173 7365 7315 0000 0073 0c00  t_classes....s..
-000003e0: 0000 0202 0201 0201 0201 0201 0cfc 7a17  ..............z.
-000003f0: 4669 6775 7265 2e73 6574 5f70 6c6f 745f  Figure.set_plot_
-00000400: 636c 6173 7365 7363 0400 0000 0000 0000  classesc........
-00000410: 0000 0000 0500 0000 0400 0000 4b00 0000  ............K...
-00000420: 7336 0000 0074 00a0 017c 007c 04a1 0201  s6...t...|.|....
-00000430: 007c 017c 005f 027c 037c 005f 037c 00a0  .|.|._.|.|._.|..
-00000440: 047c 02a1 0101 007c 00a0 05a1 0001 007c  .|.....|.......|
-00000450: 00a0 06a1 0001 0064 0053 00a9 014e 2907  .......d.S...N).
-00000460: 7204 0000 00da 066b 7761 7267 73da 0b66  r......kwargs..f
-00000470: 6967 7572 6573 5f6f 626a da0a 706c 6f74  igures_obj..plot
-00000480: 5f69 6e64 6578 da17 696e 6974 6961 6c69  _index..initiali
-00000490: 7365 5f64 6174 615f 6f62 6a65 6374 73da  se_data_objects.
-000004a0: 0d73 6574 5f67 7269 645f 7369 7a65 da15  .set_grid_size..
-000004b0: 7072 6f63 6573 735f 6c69 6768 745f 6f72  process_light_or
-000004c0: 5f64 6172 6b29 05da 0473 656c 6672 1c00  _dark)...selfr..
-000004d0: 0000 da0c 6461 7461 5f6f 626a 6563 7473  ....data_objects
-000004e0: 721d 0000 0072 1b00 0000 7217 0000 0072  r....r....r....r
-000004f0: 1700 0000 7218 0000 00da 085f 5f69 6e69  ....r......__ini
-00000500: 745f 5f1d 0000 0073 0c00 0000 0c01 0601  t__....s........
-00000510: 0601 0a01 0801 0c01 7a0f 4669 6775 7265  ........z.Figure
-00000520: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000530: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000540: 0000 731a 0000 007c 006a 0072 0b74 016a  ..s....|.j.r.t.j
-00000550: 02a0 0364 01a1 0101 0064 0053 0064 0053  ...d.....d.S.d.S
-00000560: 0029 024e da0f 6461 726b 5f62 6163 6b67  .).N..dark_backg
-00000570: 726f 756e 6429 04da 0464 6172 6bda 0370  round)...dark..p
-00000580: 6c74 da05 7374 796c 65da 0375 7365 a901  lt..style..use..
-00000590: 7221 0000 0072 1700 0000 7217 0000 0072  r!...r....r....r
-000005a0: 1800 0000 7220 0000 0025 0000 0073 0600  ....r ...%...s..
-000005b0: 0000 0601 1001 04ff 7a1c 4669 6775 7265  ........z.Figure
-000005c0: 2e70 726f 6365 7373 5f6c 6967 6874 5f6f  .process_light_o
-000005d0: 725f 6461 726b 6302 0000 0000 0000 0000  r_darkc.........
-000005e0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-000005f0: 2e00 0000 7c01 7c00 5f00 7401 7c01 8301  ....|.|._.t.|...
-00000600: 7c00 5f02 7c00 6a03 6a04 7215 7c00 0400  |._.|.j.j.r.|...
-00000610: 6a02 6401 3700 0200 5f02 6400 5300 6400  j.d.7..._.d.S.d.
-00000620: 5300 2902 4e72 0500 0000 2905 7222 0000  S.).Nr....).r"..
-00000630: 00da 036c 656e da05 636f 756e 7472 1c00  ...len..countr..
-00000640: 0000 da10 756e 6976 6572 7361 6c5f 6c65  ....universal_le
-00000650: 6765 6e64 2902 7221 0000 0072 2200 0000  gend).r!...r"...
-00000660: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00000670: 1e00 0000 2900 0000 730a 0000 0006 010a  ....)...s.......
-00000680: 0108 0112 0104 ff7a 1e46 6967 7572 652e  .......z.Figure.
-00000690: 696e 6974 6961 6c69 7365 5f64 6174 615f  initialise_data_
-000006a0: 6f62 6a65 6374 7363 0100 0000 0000 0000  objectsc........
-000006b0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000006c0: 7320 0000 007c 006a 006a 017d 0174 027c  s ...|.j.j.}.t.|
-000006d0: 006a 037c 0183 025c 027c 005f 047c 005f  .j.|...\.|._.|._
-000006e0: 0564 0053 0072 1a00 0000 2906 721c 0000  .d.S.r....).r...
-000006f0: 00da 0c61 7370 6563 745f 7261 7469 6f72  ...aspect_ratior
-00000700: 0b00 0000 722b 0000 00da 0472 6f77 73da  ....r+.....rows.
-00000710: 0763 6f6c 756d 6e73 2902 7221 0000 0072  .columns).r!...r
-00000720: 2d00 0000 7217 0000 0072 1700 0000 7218  -...r....r....r.
-00000730: 0000 0072 1f00 0000 2f00 0000 7304 0000  ...r..../...s...
-00000740: 0008 0118 017a 1446 6967 7572 652e 7365  .....z.Figure.se
-00000750: 745f 6772 6964 5f73 697a 6563 0100 0000  t_grid_sizec....
-00000760: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000770: 4300 0000 f324 0000 007c 00a0 00a1 0001  C....$...|......
-00000780: 007c 00a0 01a1 0001 007c 00a0 02a1 0001  .|.......|......
-00000790: 007c 00a0 03a1 0001 0064 0053 0072 1a00  .|.......d.S.r..
-000007a0: 0000 2904 da11 696e 6974 6961 6c69 7365  ..)...initialise
-000007b0: 5f66 6967 7572 65da 0c63 7265 6174 655f  _figure..create_
-000007c0: 706c 6f74 73da 1661 6464 5f66 6967 7572  plots..add_figur
-000007d0: 655f 7065 7269 7068 6572 616c 73da 0d6f  e_peripherals..o
-000007e0: 7574 7075 745f 6669 6775 7265 7229 0000  utput_figurer)..
-000007f0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000800: da0d 6372 6561 7465 5f66 6967 7572 6533  ..create_figure3
-00000810: 0000 00f3 0800 0000 0801 0801 0801 0c01  ................
-00000820: 7a14 4669 6775 7265 2e63 7265 6174 655f  z.Figure.create_
-00000830: 6669 6775 7265 6301 0000 0000 0000 0000  figurec.........
-00000840: 0000 0001 0000 0002 0000 0043 0000 00f3  ...........C....
-00000850: 1c00 0000 7c00 a000 a100 0100 7c00 a001  ....|.......|...
-00000860: a100 0100 7c00 a002 a100 0100 6400 5300  ....|.......d.S.
-00000870: 721a 0000 0029 03da 0a73 6574 5f66 6967  r....)...set_fig
-00000880: 7572 65da 0b63 7265 6174 655f 6178 6573  ure..create_axes
-00000890: da11 7265 6d6f 7665 5f65 7874 7261 5f61  ..remove_extra_a
-000008a0: 7865 7372 2900 0000 7217 0000 0072 1700  xesr)...r....r..
-000008b0: 0000 7218 0000 0072 3100 0000 3900 0000  ..r....r1...9...
-000008c0: f306 0000 0008 0108 010c 017a 1846 6967  ...........z.Fig
-000008d0: 7572 652e 696e 6974 6961 6c69 7365 5f66  ure.initialise_f
-000008e0: 6967 7572 6563 0100 0000 0000 0000 0000  igurec..........
-000008f0: 0000 0100 0000 0600 0000 4300 0000 7332  ..........C...s2
-00000900: 0000 0074 006a 0164 017c 006a 0264 028d  ...t.j.d.|.j.d..
-00000910: 027c 005f 037c 006a 036a 047c 006a 057c  .|._.|.j.j.|.j.|
-00000920: 006a 067c 006a 077c 006a 0864 038d 0401  .j.|.j.|.j.d....
-00000930: 0064 0053 0029 044e 5429 02da 1263 6f6e  .d.S.).NT)...con
-00000940: 7374 7261 696e 6564 5f6c 6179 6f75 74da  strained_layout.
-00000950: 0364 7069 2904 da05 775f 7061 64da 0568  .dpi)...w_pad..h
-00000960: 5f70 6164 da06 6873 7061 6365 da06 7773  _pad..hspace..ws
-00000970: 7061 6365 2909 7226 0000 00da 0666 6967  pace).r&.....fig
-00000980: 7572 6572 3d00 0000 da03 6669 67da 1b73  urer=.....fig..s
-00000990: 6574 5f63 6f6e 7374 7261 696e 6564 5f6c  et_constrained_l
-000009a0: 6179 6f75 745f 7061 6473 723e 0000 0072  ayout_padsr>...r
-000009b0: 3f00 0000 7240 0000 0072 4100 0000 7229  ?...r@...rA...r)
-000009c0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-000009d0: 0000 7238 0000 003e 0000 0073 0800 0000  ..r8...>...s....
-000009e0: 1201 0e01 0801 0aff 7a11 4669 6775 7265  ........z.Figure
-000009f0: 2e73 6574 5f66 6967 7572 6563 0100 0000  .set_figurec....
-00000a00: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000a10: 0300 0000 731e 0000 0087 0066 0164 0164  ....s......f.d.d
-00000a20: 0284 0874 0088 006a 0183 0144 0083 0188  ...t...j...D....
-00000a30: 005f 0264 0053 0029 034e 6301 0000 0000  ._.d.S.).Nc.....
-00000a40: 0000 0000 0000 0003 0000 0006 0000 0013  ................
-00000a50: 0000 00f3 1c00 0000 6700 7c00 5d0a 5c02  ........g.|.].\.
-00000a60: 7d01 7d02 8800 a000 7c01 7c02 a102 9102  }.}.....|.|.....
-00000a70: 7102 5300 7217 0000 0029 01da 0867 6574  q.S.r....)...get
-00000a80: 5f61 7869 7329 03da 022e 30da 0569 6e64  _axis)....0..ind
-00000a90: 6578 da08 6461 7461 5f6f 626a 7229 0000  ex..data_objr)..
-00000aa0: 0072 1700 0000 7218 0000 00da 0a3c 6c69  .r....r......<li
-00000ab0: 7374 636f 6d70 3e44 0000 00f3 0600 0000  stcomp>D........
-00000ac0: 0600 0601 10ff 7a26 4669 6775 7265 2e63  ......z&Figure.c
-00000ad0: 7265 6174 655f 6178 6573 2e3c 6c6f 6361  reate_axes.<loca
-00000ae0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2903  ls>.<listcomp>).
-00000af0: da09 656e 756d 6572 6174 6572 2200 0000  ..enumerater"...
-00000b00: da04 6178 6573 7229 0000 0072 1700 0000  ..axesr)...r....
-00000b10: 7229 0000 0072 1800 0000 7239 0000 0043  r)...r....r9...C
-00000b20: 0000 0073 0600 0000 0a01 0801 0cff 7a12  ...s..........z.
-00000b30: 4669 6775 7265 2e63 7265 6174 655f 6178  Figure.create_ax
-00000b40: 6573 6303 0000 0000 0000 0000 0000 0004  esc.............
-00000b50: 0000 0006 0000 0043 0000 0073 2200 0000  .......C...s"...
-00000b60: 7c00 6a00 6a01 7c00 6a02 7c00 6a03 7c01  |.j.j.|.j.|.j.|.
-00000b70: 6401 1700 7c02 6a04 6402 8d04 7d03 7c03  d...|.j.d...}.|.
-00000b80: 5300 2903 4e72 0500 0000 2901 da0a 7072  S.).Nr....)...pr
-00000b90: 6f6a 6563 7469 6f6e 2905 7243 0000 00da  ojection).rC....
-00000ba0: 0b61 6464 5f73 7562 706c 6f74 722e 0000  .add_subplotr...
-00000bb0: 0072 2f00 0000 724e 0000 0029 0472 2100  .r/...rN...).r!.
-00000bc0: 0000 7248 0000 0072 4900 0000 da04 6178  ..rH...rI.....ax
-00000bd0: 6973 7217 0000 0072 1700 0000 7218 0000  isr....r....r...
-00000be0: 0072 4600 0000 4700 0000 7308 0000 0014  .rF...G...s.....
-00000bf0: 0104 0106 ff04 027a 0f46 6967 7572 652e  .......z.Figure.
-00000c00: 6765 745f 6178 6973 6301 0000 0000 0000  get_axisc.......
-00000c10: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-00000c20: 0073 4000 0000 7400 7c00 6a01 8301 7c00  .s@...t.|.j...|.
-00000c30: 6a02 1800 7d01 7403 7c00 6a01 6400 6400  j...}.t.|.j.d.d.
-00000c40: 6401 8503 1900 7404 7c01 8301 8302 4400  d.....t.|.....D.
-00000c50: 5d08 5c02 7d02 7d03 7c02 a005 a100 0100  ].\.}.}.|.......
-00000c60: 7115 6400 5300 2902 4ee9 ffff ffff 2906  q.d.S.).N.....).
-00000c70: 722a 0000 0072 4d00 0000 722b 0000 00da  r*...rM...r+....
-00000c80: 037a 6970 da05 7261 6e67 65da 0672 656d  .zip..range..rem
-00000c90: 6f76 6529 0472 2100 0000 da10 6578 7472  ove).r!.....extr
-00000ca0: 615f 6178 6573 5f63 6f75 6e74 da02 6178  a_axes_count..ax
-00000cb0: da01 5f72 1700 0000 7217 0000 0072 1800  .._r....r....r..
-00000cc0: 0000 723a 0000 004c 0000 0073 0800 0000  ..r:...L...s....
-00000cd0: 1001 2201 0a01 04ff 7a18 4669 6775 7265  ..".....z.Figure
-00000ce0: 2e72 656d 6f76 655f 6578 7472 615f 6178  .remove_extra_ax
-00000cf0: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
-00000d00: 0000 0002 0000 0043 0000 0072 3000 0000  .......C...r0...
-00000d10: 721a 0000 0029 04da 1573 6574 5f73 7570  r....)...set_sup
-00000d20: 7469 746c 655f 666f 6e74 6469 6374 da0c  title_fontdict..
-00000d30: 7365 745f 7375 7074 6974 6c65 da14 7365  set_suptitle..se
-00000d40: 745f 756e 6976 6572 7361 6c5f 6c65 6765  t_universal_lege
-00000d50: 6e64 da0f 7365 745f 6669 6775 7265 5f73  nd..set_figure_s
-00000d60: 697a 6572 2900 0000 7217 0000 0072 1700  izer)...r....r..
-00000d70: 0000 7218 0000 0072 3300 0000 5100 0000  ..r....r3...Q...
-00000d80: 7236 0000 007a 1d46 6967 7572 652e 6164  r6...z.Figure.ad
-00000d90: 645f 6669 6775 7265 5f70 6572 6970 6865  d_figure_periphe
-00000da0: 7261 6c73 6301 0000 0000 0000 0000 0000  ralsc...........
-00000db0: 0002 0000 0006 0000 0043 0000 0073 2800  .........C...s(.
-00000dc0: 0000 7c00 6a00 7c00 6a01 7c00 6a02 7c00  ..|.j.|.j.|.j.|.
-00000dd0: 6a03 7c00 6a04 6401 9c05 7d01 7405 7c01  j.|.j.d...}.t.|.
-00000de0: 8301 7c00 5f06 6400 5300 2902 4e29 05da  ..|._.d.S.).N)..
-00000df0: 0866 6f6e 746e 616d 65da 0866 6f6e 7473  .fontname..fonts
-00000e00: 697a 65da 0563 6f6c 6f72 da11 7665 7274  ize..color..vert
-00000e10: 6963 616c 616c 6967 6e6d 656e 74da 1368  icalalignment..h
-00000e20: 6f72 697a 6f6e 7461 6c61 6c69 676e 6d65  orizontalalignme
-00000e30: 6e74 2907 da11 7375 7074 6974 6c65 5f66  nt)...suptitle_f
-00000e40: 6f6e 746e 616d 65da 1173 7570 7469 746c  ontname..suptitl
-00000e50: 655f 666f 6e74 7369 7a65 da0e 7375 7074  e_fontsize..supt
-00000e60: 6974 6c65 5f63 6f6c 6f72 da1a 7375 7074  itle_color..supt
-00000e70: 6974 6c65 5f76 6572 7469 6361 6c61 6c69  itle_verticalali
-00000e80: 676e 6d65 6e74 da1c 7375 7074 6974 6c65  gnment..suptitle
-00000e90: 5f68 6f72 697a 6f6e 7461 6c61 6c69 676e  _horizontalalign
-00000ea0: 6d65 6e74 720e 0000 00da 1173 7570 7469  mentr......supti
-00000eb0: 746c 655f 666f 6e74 6469 6374 2902 7221  tle_fontdict).r!
-00000ec0: 0000 0072 1b00 0000 7217 0000 0072 1700  ...r....r....r..
-00000ed0: 0000 7218 0000 0072 5800 0000 5700 0000  ..r....rX...W...
-00000ee0: 730e 0000 0004 0104 0104 0104 0104 0106  s...............
-00000ef0: fc0e 057a 1c46 6967 7572 652e 7365 745f  ...z.Figure.set_
-00000f00: 7375 7074 6974 6c65 5f66 6f6e 7464 6963  suptitle_fontdic
-00000f10: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00000f20: 0000 0700 0000 4300 0000 7342 0000 007c  ......C...sB...|
-00000f30: 006a 006a 0164 0075 0172 1f7c 006a 026a  .j.j.d.u.r.|.j.j
-00000f40: 017c 006a 006a 019b 0066 0169 007c 006a  .|.j.j...f.i.|.j
-00000f50: 03a4 017c 006a 047c 006a 057c 006a 0664  ...|.j.|.j.|.j.d
-00000f60: 019c 03a4 018e 0101 0064 0053 0064 0053  .........d.S.d.S
-00000f70: 0029 024e 2903 da03 6c6f 63da 0179 da03  .).N)...loc..y..
-00000f80: 7061 6429 0772 1c00 0000 da08 7375 7074  pad).r......supt
-00000f90: 6974 6c65 7243 0000 0072 6600 0000 da0c  itlerC...rf.....
-00000fa0: 7375 7074 6974 6c65 5f6c 6f63 da0a 7375  suptitle_loc..su
-00000fb0: 7074 6974 6c65 5f79 da0c 7375 7074 6974  ptitle_y..suptit
-00000fc0: 6c65 5f70 6164 7229 0000 0072 1700 0000  le_padr)...r....
-00000fd0: 7217 0000 0072 1800 0000 7259 0000 005f  r....r....rY..._
-00000fe0: 0000 0073 1000 0000 0c01 1201 0401 02ff  ...s............
-00000ff0: 0401 0801 0efe 04ff 7a13 4669 6775 7265  ........z.Figure
-00001000: 2e73 6574 5f73 7570 7469 746c 6563 0100  .set_suptitlec..
-00001010: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001020: 0000 4300 0000 7318 0000 007c 006a 006a  ..C...s....|.j.j
-00001030: 0172 0a7c 00a0 02a1 0001 0064 0053 0064  .r.|.......d.S.d
-00001040: 0053 0072 1a00 0000 2903 721c 0000 0072  .S.r....).r....r
-00001050: 2c00 0000 da13 646f 5f75 6e69 7665 7273  ,.....do_univers
-00001060: 616c 5f6c 6567 656e 6472 2900 0000 7217  al_legendr)...r.
-00001070: 0000 0072 1700 0000 7218 0000 0072 5a00  ...r....r....rZ.
-00001080: 0000 6500 0000 7306 0000 0008 010c 0104  ..e...s.........
-00001090: ff7a 1b46 6967 7572 652e 7365 745f 756e  .z.Figure.set_un
-000010a0: 6976 6572 7361 6c5f 6c65 6765 6e64 6301  iversal_legendc.
-000010b0: 0000 0000 0000 0000 0000 0003 0000 0007  ................
-000010c0: 0000 0043 0000 0073 5000 0000 7c00 6a00  ...C...sP...|.j.
-000010d0: 6401 1900 7d01 7c00 6a01 6402 1900 6a01  d...}.|.j.d...j.
-000010e0: 4400 5d0d 7d02 7c01 6a02 6403 6403 7c02  D.].}.|.j.d.d.|.
-000010f0: 6a03 7c02 6a04 6404 8d04 0100 710b 7c01  j.|.j.d.....q.|.
-00001100: 6a05 6405 6406 6403 6407 8d03 0100 7c01  j.d.d.d.d.....|.
-00001110: a006 6408 a101 0100 6400 5300 2909 4e72  ..d.....d.S.).Nr
-00001120: 5100 0000 7201 0000 0072 0500 0000 2902  Q...r....r....).
-00001130: da05 6c61 6265 6c72 5e00 0000 da06 6365  ..labelr^.....ce
-00001140: 6e74 6572 7203 0000 0029 0372 6700 0000  nterr....).rg...
-00001150: da09 626f 7264 6572 7061 64da 0c6c 6162  ..borderpad..lab
-00001160: 656c 7370 6163 696e 67da 036f 6666 2907  elspacing..off).
-00001170: 724d 0000 0072 2200 0000 da04 706c 6f74  rM...r".....plot
-00001180: 726f 0000 00da 0663 6f6c 6f75 72da 066c  ro.....colour..l
-00001190: 6567 656e 6472 5000 0000 2903 7221 0000  egendrP...).r!..
-000011a0: 0072 5600 0000 7249 0000 0072 1700 0000  .rV...rI...r....
-000011b0: 7217 0000 0072 1800 0000 726e 0000 0069  r....r....rn...i
-000011c0: 0000 0073 0a00 0000 0a01 1001 1801 1001  ...s............
-000011d0: 0e01 7a1a 4669 6775 7265 2e64 6f5f 756e  ..z.Figure.do_un
-000011e0: 6976 6572 7361 6c5f 6c65 6765 6e64 6301  iversal_legendc.
-000011f0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001200: 0000 0043 0000 0073 1400 0000 7c00 a000  ...C...s....|...
-00001210: a100 0100 7c00 a001 a100 0100 6400 5300  ....|.......d.S.
-00001220: 721a 0000 0029 02da 0b75 7064 6174 655f  r....)...update_
-00001230: 7369 7a65 da16 7365 745f 6669 6775 7265  size..set_figure
-00001240: 5f73 697a 655f 7069 7865 6c73 7229 0000  _size_pixelsr)..
-00001250: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00001260: 725b 0000 0070 0000 00f3 0400 0000 0801  r[...p..........
-00001270: 0c01 7a16 4669 6775 7265 2e73 6574 5f66  ..z.Figure.set_f
-00001280: 6967 7572 655f 7369 7a65 6301 0000 0000  igure_sizec.....
-00001290: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-000012a0: 0000 0072 3700 0000 721a 0000 0029 03da  ...r7...r....)..
-000012b0: 1973 6574 5f6d 6178 696d 6973 6564 5f66  .set_maximised_f
-000012c0: 6967 7572 655f 7369 7a65 da11 7365 745f  igure_size..set_
-000012d0: 6669 6775 7265 5f69 6e63 6865 7372 0d00  figure_inchesr..
-000012e0: 0000 7229 0000 0072 1700 0000 7217 0000  ..r)...r....r...
-000012f0: 0072 1800 0000 7277 0000 0074 0000 0072  .r....rw...t...r
-00001300: 3b00 0000 7a12 4669 6775 7265 2e75 7064  ;...z.Figure.upd
-00001310: 6174 655f 7369 7a65 6301 0000 0000 0000  ate_sizec.......
-00001320: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
-00001330: 0073 3200 0000 7c00 6a00 7217 7401 8300  .s2...|.j.r.t...
-00001340: 6401 1900 7d01 7c01 6a02 6402 1b00 7c01  d...}.|.j.d...|.
-00001350: 6a03 6402 1b00 6702 7d02 7c02 7c00 5f04  j.d...g.}.|.|._.
-00001360: 6400 5300 6400 5300 2903 4e72 0100 0000  d.S.d.S.).Nr....
-00001370: 6766 6666 6666 6639 4029 05da 086d 6178  gffffff9@)...max
-00001380: 696d 6973 6572 0200 0000 da08 7769 6474  imiser......widt
-00001390: 685f 6d6d da09 6865 6967 6874 5f6d 6dda  h_mm..height_mm.
-000013a0: 0b66 6967 7572 655f 7369 7a65 2903 7221  .figure_size).r!
-000013b0: 0000 00da 076d 6f6e 6974 6f72 727f 0000  .....monitorr...
-000013c0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-000013d0: 727a 0000 0079 0000 0073 0a00 0000 0601  rz...y...s......
-000013e0: 0a01 1401 0a01 04fd 7a20 4669 6775 7265  ........z Figure
-000013f0: 2e73 6574 5f6d 6178 696d 6973 6564 5f66  .set_maximised_f
-00001400: 6967 7572 655f 7369 7a65 6301 0000 0000  igure_sizec.....
-00001410: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001420: 0000 0073 1400 0000 7c00 6a00 7208 7401  ...s....|.j.r.t.
-00001430: 8300 0100 6400 5300 6400 5300 721a 0000  ....d.S.d.S.r...
-00001440: 0029 0272 7c00 0000 720d 0000 0072 2900  .).r|...r....r).
-00001450: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001460: 0072 0d00 0000 7f00 0000 7306 0000 0006  .r........s.....
-00001470: 010a 0104 ff7a 1646 6967 7572 652e 6d61  .....z.Figure.ma
-00001480: 7869 6d69 7365 5f66 6967 7572 6563 0100  ximise_figurec..
-00001490: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000014a0: 0000 4300 0000 7320 0000 007c 006a 0064  ..C...s ...|.j.d
-000014b0: 0075 0172 0e7c 006a 01a0 027c 006a 00a1  .u.r.|.j...|.j..
-000014c0: 0101 0064 0053 0064 0053 0072 1a00 0000  ...d.S.d.S.r....
-000014d0: 2903 727f 0000 0072 4300 0000 da0f 7365  ).r....rC.....se
-000014e0: 745f 7369 7a65 5f69 6e63 6865 7372 2900  t_size_inchesr).
-000014f0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001500: 0072 7b00 0000 8300 0000 7306 0000 000a  .r{.......s.....
-00001510: 0112 0104 ff7a 1846 6967 7572 652e 7365  .....z.Figure.se
-00001520: 745f 6669 6775 7265 5f69 6e63 6865 7363  t_figure_inchesc
-00001530: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001540: 0200 0000 4300 0000 732a 0000 007c 006a  ....C...s*...|.j
-00001550: 00a0 01a1 007c 006a 006a 0214 007c 005f  .....|.j.j...|._
-00001560: 0364 0164 0284 007c 006a 0344 0083 017c  .d.d...|.j.D...|
-00001570: 005f 0364 0053 0029 034e 6301 0000 0000  ._.d.S.).Nc.....
-00001580: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00001590: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-000015a0: 7400 7c01 8301 9102 7102 5300 7217 0000  t.|.....q.S.r...
-000015b0: 0029 01da 0369 6e74 2902 7247 0000 00da  .)...int).rG....
-000015c0: 0576 616c 7565 7217 0000 0072 1700 0000  .valuer....r....
-000015d0: 7218 0000 0072 4a00 0000 8900 0000 7302  r....rJ.......s.
-000015e0: 0000 0014 007a 3146 6967 7572 652e 7365  .....z1Figure.se
-000015f0: 745f 6669 6775 7265 5f73 697a 655f 7069  t_figure_size_pi
-00001600: 7865 6c73 2e3c 6c6f 6361 6c73 3e2e 3c6c  xels.<locals>.<l
-00001610: 6973 7463 6f6d 703e 2904 7243 0000 00da  istcomp>).rC....
-00001620: 0f67 6574 5f73 697a 655f 696e 6368 6573  .get_size_inches
-00001630: 723d 0000 00da 1266 6967 7572 655f 7369  r=.....figure_si
-00001640: 7a65 5f70 6978 656c 7372 2900 0000 7217  ze_pixelsr)...r.
-00001650: 0000 0072 1700 0000 7218 0000 0072 7800  ...r....r....rx.
-00001660: 0000 8700 0000 7304 0000 0014 0116 017a  ......s........z
-00001670: 1d46 6967 7572 652e 7365 745f 6669 6775  .Figure.set_figu
-00001680: 7265 5f73 697a 655f 7069 7865 6c73 6301  re_size_pixelsc.
-00001690: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000016a0: 0000 0003 0000 0073 2200 0000 8700 6601  .......s".....f.
-000016b0: 6401 6402 8408 7400 8800 6a01 8800 6a02  d.d...t...j...j.
-000016c0: 8302 4400 8301 8800 5f03 6400 5300 2903  ..D....._.d.S.).
-000016d0: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-000016e0: 0000 0600 0000 1300 0000 7245 0000 0072  ..........rE...r
-000016f0: 1700 0000 2901 da0f 6372 6561 7465 5f70  ....)...create_p
-00001700: 6c6f 745f 6f62 6a29 0372 4700 0000 7256  lot_obj).rG...rV
-00001710: 0000 0072 4900 0000 7229 0000 0072 1700  ...rI...r)...r..
-00001720: 0000 7218 0000 0072 4a00 0000 8c00 0000  ..r....rJ.......
-00001730: 724b 0000 007a 2746 6967 7572 652e 6372  rK...z'Figure.cr
-00001740: 6561 7465 5f70 6c6f 7473 2e3c 6c6f 6361  eate_plots.<loca
-00001750: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2904  ls>.<listcomp>).
-00001760: 7252 0000 0072 4d00 0000 7222 0000 00da  rR...rM...r"....
-00001770: 0c70 6c6f 745f 6f62 6a65 6374 7372 2900  .plot_objectsr).
-00001780: 0000 7217 0000 0072 2900 0000 7218 0000  ..r....r)...r...
-00001790: 0072 3200 0000 8b00 0000 7306 0000 000a  .r2.......s.....
-000017a0: 010c 010c ff7a 1346 6967 7572 652e 6372  .....z.Figure.cr
-000017b0: 6561 7465 5f70 6c6f 7473 6303 0000 0000  eate_plotsc.....
-000017c0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-000017d0: 0000 0073 2600 0000 7c00 6a00 7c02 6a01  ...s&...|.j.|.j.
-000017e0: 6a02 1900 7d03 7c03 7c00 7c01 7c02 8303  j...}.|.|.|.|...
-000017f0: 7d04 7c04 a003 a100 0100 7c04 5300 721a  }.|.......|.S.r.
-00001800: 0000 0029 0472 1500 0000 da09 5f5f 636c  ...).r......__cl
-00001810: 6173 735f 5fda 085f 5f6e 616d 655f 5fda  ass__..__name__.
-00001820: 0b63 7265 6174 655f 706c 6f74 2905 7221  .create_plot).r!
-00001830: 0000 0072 5600 0000 7249 0000 00da 0a70  ...rV...rI.....p
-00001840: 6c6f 745f 636c 6173 73da 0870 6c6f 745f  lot_class..plot_
-00001850: 6f62 6a72 1700 0000 7217 0000 0072 1800  objr....r....r..
-00001860: 0000 7286 0000 008f 0000 0073 0800 0000  ..r........s....
-00001870: 0e01 0c01 0801 0401 7a16 4669 6775 7265  ........z.Figure
-00001880: 2e63 7265 6174 655f 706c 6f74 5f6f 626a  .create_plot_obj
-00001890: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000018a0: 0002 0000 0043 0000 0073 3400 0000 7c00  .....C...s4...|.
-000018b0: 6a00 6a01 6401 6b02 720c 7c00 a002 a100  j.j.d.k.r.|.....
-000018c0: 0100 6400 5300 7c00 6a00 6a01 6402 6b02  ..d.S.|.j.j.d.k.
-000018d0: 7218 7403 7c00 8301 0100 6400 5300 6400  r.t.|.....d.S.d.
-000018e0: 5300 2903 4eda 0453 686f 77da 0453 6176  S.).N..Show..Sav
-000018f0: 6529 0472 1c00 0000 da06 6f75 7470 7574  e).r......output
-00001900: da0b 7368 6f77 5f66 6967 7572 6572 0c00  ..show_figurer..
-00001910: 0000 7229 0000 0072 1700 0000 7217 0000  ..r)...r....r...
-00001920: 0072 1800 0000 7234 0000 0095 0000 0073  .r....r4.......s
-00001930: 0a00 0000 0c01 0c01 0c01 0c01 04ff 7a14  ..............z.
-00001940: 4669 6775 7265 2e6f 7574 7075 745f 6669  Figure.output_fi
-00001950: 6775 7265 6301 0000 0000 0000 0000 0000  gurec...........
-00001960: 0001 0000 0002 0000 0043 0000 0073 1400  .........C...s..
-00001970: 0000 7400 a001 a100 0100 7400 a002 a100  ..t.......t.....
-00001980: 0100 6400 5300 721a 0000 0029 0372 2600  ..d.S.r....).r&.
-00001990: 0000 da04 7368 6f77 da05 636c 6f73 6572  ....show..closer
-000019a0: 2900 0000 7217 0000 0072 1700 0000 7218  )...r....r....r.
-000019b0: 0000 0072 9000 0000 9b00 0000 7279 0000  ...r........ry..
-000019c0: 007a 1246 6967 7572 652e 7368 6f77 5f66  .z.Figure.show_f
-000019d0: 6967 7572 6563 0100 0000 0000 0000 0000  igurec..........
-000019e0: 0000 0200 0000 0300 0000 4300 0000 7318  ..........C...s.
-000019f0: 0000 007c 006a 0044 005d 067d 017c 01a0  ...|.j.D.].}.|..
-00001a00: 01a1 0001 0071 0364 0053 0072 1a00 0000  .....q.d.S.r....
-00001a10: 2902 7222 0000 00da 1973 6574 5f61 6e69  ).r".....set_ani
-00001a20: 6d61 7469 6f6e 5f61 7869 735f 6c69 6d69  mation_axis_limi
-00001a30: 7473 2902 7221 0000 0072 4900 0000 7217  ts).r!...rI...r.
-00001a40: 0000 0072 1700 0000 7218 0000 0072 9300  ...r....r....r..
-00001a50: 0000 9f00 0000 7306 0000 000a 010a 0104  ......s.........
-00001a60: ff7a 2046 6967 7572 652e 7365 745f 616e  .z Figure.set_an
-00001a70: 696d 6174 696f 6e5f 6178 6973 5f6c 696d  imation_axis_lim
-00001a80: 6974 7363 0100 0000 0000 0000 0000 0000  itsc............
-00001a90: 0200 0000 0200 0000 4300 0000 7312 0000  ........C...s...
-00001aa0: 007c 006a 0064 0119 00a0 01a1 007d 017c  .|.j.d.......}.|
-00001ab0: 0153 0029 024e 7201 0000 0029 0272 2200  .S.).Nr....).r".
-00001ac0: 0000 da0f 6765 745f 6672 616d 655f 636f  ....get_frame_co
-00001ad0: 756e 7429 0272 2100 0000 da0b 6672 616d  unt).r!.....fram
-00001ae0: 655f 636f 756e 7472 1700 0000 7217 0000  e_countr....r...
-00001af0: 0072 1800 0000 7294 0000 00a3 0000 0073  .r....r........s
-00001b00: 0400 0000 0e01 0401 7a16 4669 6775 7265  ........z.Figure
-00001b10: 2e67 6574 5f66 7261 6d65 5f63 6f75 6e74  .get_frame_count
-00001b20: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00001b30: 0004 0000 0043 0000 0073 2e00 0000 7400  .....C...s....t.
-00001b40: 7c00 6a01 7c00 6a02 8302 4400 5d0d 5c02  |.j.|.j...D.].\.
-00001b50: 7d02 7d03 7c03 7c01 1900 7d04 7c02 a003  }.}.|.|...}.|...
-00001b60: 7c04 a101 0100 7107 6400 5300 721a 0000  |.....q.d.S.r...
-00001b70: 0029 0472 5200 0000 7222 0000 00da 0f61  .).rR...r".....a
-00001b80: 6c6c 5f64 6174 615f 7661 6c75 6573 da0e  ll_data_values..
-00001b90: 7365 745f 6461 7461 5f76 616c 7565 2905  set_data_value).
-00001ba0: 7221 0000 0072 4800 0000 7249 0000 00da  r!...rH...rI....
-00001bb0: 0b64 6174 615f 7661 6c75 6573 da0a 6461  .data_values..da
-00001bc0: 7461 5f76 616c 7565 7217 0000 0072 1700  ta_valuer....r..
-00001bd0: 0000 7218 0000 0072 9700 0000 a700 0000  ..r....r........
-00001be0: 7308 0000 0016 0108 010c 0104 fe7a 1546  s............z.F
-00001bf0: 6967 7572 652e 7365 745f 6461 7461 5f76  igure.set_data_v
-00001c00: 616c 7565 4e29 2172 8900 0000 da0a 5f5f  alueN)!r......__
-00001c10: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001c20: 6e61 6d65 5f5f da0b 636c 6173 736d 6574  name__..classmet
-00001c30: 686f 6472 1900 0000 7223 0000 0072 2000  hodr....r#...r .
-00001c40: 0000 721e 0000 0072 1f00 0000 7235 0000  ..r....r....r5..
-00001c50: 0072 3100 0000 7238 0000 0072 3900 0000  .r1...r8...r9...
-00001c60: 7246 0000 0072 3a00 0000 7233 0000 0072  rF...r:...r3...r
-00001c70: 5800 0000 7259 0000 0072 5a00 0000 726e  X...rY...rZ...rn
-00001c80: 0000 0072 5b00 0000 7277 0000 0072 7a00  ...r[...rw...rz.
-00001c90: 0000 720d 0000 0072 7b00 0000 7278 0000  ..r....r{...rx..
-00001ca0: 0072 3200 0000 7286 0000 0072 3400 0000  .r2...r....r4...
-00001cb0: 7290 0000 0072 9300 0000 7294 0000 0072  r....r....r....r
-00001cc0: 9700 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-00001cd0: 0000 0072 1800 0000 720f 0000 0013 0000  ...r....r.......
-00001ce0: 0073 3e00 0000 0800 0202 0a01 0807 0808  .s>.............
-00001cf0: 0804 0806 0804 0806 0805 0805 0804 0805  ................
-00001d00: 0805 0806 0808 0806 0804 0807 0804 0805  ................
-00001d10: 0806 0804 0804 0804 0804 0806 0806 0804  ................
-00001d20: 0804 0c04 720f 0000 0029 1fda 026f 73da  ....r....)...os.
-00001d30: 046d 6174 68da 0a73 6372 6565 6e69 6e66  .math..screeninf
-00001d40: 6f72 0200 0000 da11 6d61 7470 6c6f 746c  or......matplotl
-00001d50: 6962 2e70 7970 6c6f 74da 0670 7970 6c6f  ib.pyplot..pyplo
-00001d60: 7472 2600 0000 da05 6e75 6d70 79da 026e  tr&.....numpy..n
-00001d70: 70da 0072 0400 0000 da13 706c 6f74 7479  p..r......plotty
-00001d80: 7065 732e 706c 6f74 6c69 6e65 7372 0600  pes.plotlinesr..
-00001d90: 0000 da12 706c 6f74 7479 7065 732e 706c  ....plottypes.pl
-00001da0: 6f74 6261 7273 7207 0000 00da 1170 6c6f  otbarsr......plo
-00001db0: 7474 7970 6573 2e70 6c6f 7470 6965 7208  ttypes.plotpier.
-00001dc0: 0000 00da 1770 6c6f 7474 7970 6573 2e70  .....plottypes.p
-00001dd0: 6c6f 7463 6f6c 6f72 706c 6f74 7209 0000  lotcolorplotr...
-00001de0: 00da 1570 6c6f 7474 7970 6573 2e70 6c6f  ...plottypes.plo
-00001df0: 7473 7572 6661 6365 720a 0000 00da 1870  tsurfacer......p
-00001e00: 6c6f 7475 7469 6c73 2e67 7269 6464 696d  lotutils.griddim
-00001e10: 656e 7369 6f6e 7372 0b00 0000 da14 706c  ensionsr......pl
-00001e20: 6f74 7574 696c 732e 7361 7665 6669 6775  otutils.savefigu
-00001e30: 7265 720c 0000 00da 1470 6c6f 7475 7469  rer......plotuti
-00001e40: 6c73 2e66 6967 7572 6573 697a 6572 0d00  ls.figuresizer..
-00001e50: 0000 da0b 7574 696c 732e 6469 6374 7372  ....utils.dictsr
-00001e60: 0e00 0000 720f 0000 00da 046c 6f61 6472  ....r......loadr
-00001e70: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00001e80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00001e90: 0073 2400 0000 0800 0801 0c01 0c02 0801  .s$.............
-00001ea0: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001eb0: 0c01 0c01 0e02 007f 0e1a                 ..........
+00000360: 6c73 a900 7217 0000 00fa 4e2f 686f 6d65  ls..r.....N/home
+00000370: 2f68 656e 7279 2f2e 6c6f 6361 6c2f 6c69  /henry/.local/li
+00000380: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
+00000390: 652d 7061 636b 6167 6573 2f68 6775 7469  e-packages/hguti
+000003a0: 6c69 7469 6573 2f70 6c6f 7474 696e 672f  lities/plotting/
+000003b0: 6669 6775 7265 2e70 79da 1073 6574 5f70  figure.py..set_p
+000003c0: 6c6f 745f 636c 6173 7365 7315 0000 0073  lot_classes....s
+000003d0: 0c00 0000 0202 0201 0201 0201 0201 0cfc  ................
+000003e0: 7a17 4669 6775 7265 2e73 6574 5f70 6c6f  z.Figure.set_plo
+000003f0: 745f 636c 6173 7365 7363 0400 0000 0000  t_classesc......
+00000400: 0000 0000 0000 0500 0000 0400 0000 4b00  ..............K.
+00000410: 0000 7336 0000 0074 00a0 017c 007c 04a1  ..s6...t...|.|..
+00000420: 0201 007c 017c 005f 027c 037c 005f 037c  ...|.|._.|.|._.|
+00000430: 00a0 047c 02a1 0101 007c 00a0 05a1 0001  ...|.....|......
+00000440: 007c 00a0 06a1 0001 0064 0053 00a9 014e  .|.......d.S...N
+00000450: 2907 7204 0000 00da 066b 7761 7267 73da  ).r......kwargs.
+00000460: 0b66 6967 7572 6573 5f6f 626a da0a 706c  .figures_obj..pl
+00000470: 6f74 5f69 6e64 6578 da17 696e 6974 6961  ot_index..initia
+00000480: 6c69 7365 5f64 6174 615f 6f62 6a65 6374  lise_data_object
+00000490: 73da 0d73 6574 5f67 7269 645f 7369 7a65  s..set_grid_size
+000004a0: da15 7072 6f63 6573 735f 6c69 6768 745f  ..process_light_
+000004b0: 6f72 5f64 6172 6b29 05da 0473 656c 6672  or_dark)...selfr
+000004c0: 1c00 0000 da0c 6461 7461 5f6f 626a 6563  ......data_objec
+000004d0: 7473 721d 0000 0072 1b00 0000 7217 0000  tsr....r....r...
+000004e0: 0072 1700 0000 7218 0000 00da 085f 5f69  .r....r......__i
+000004f0: 6e69 745f 5f1d 0000 0073 0c00 0000 0c01  nit__....s......
+00000500: 0601 0601 0a01 0801 0c01 7a0f 4669 6775  ..........z.Figu
+00000510: 7265 2e5f 5f69 6e69 745f 5f63 0100 0000  re.__init__c....
+00000520: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000530: 4300 0000 731a 0000 007c 006a 0072 0b74  C...s....|.j.r.t
+00000540: 016a 02a0 0364 01a1 0101 0064 0053 0064  .j...d.....d.S.d
+00000550: 0053 0029 024e da0f 6461 726b 5f62 6163  .S.).N..dark_bac
+00000560: 6b67 726f 756e 6429 04da 0464 6172 6bda  kground)...dark.
+00000570: 0370 6c74 da05 7374 796c 65da 0375 7365  .plt..style..use
+00000580: a901 7221 0000 0072 1700 0000 7217 0000  ..r!...r....r...
+00000590: 0072 1800 0000 7220 0000 0025 0000 0073  .r....r ...%...s
+000005a0: 0600 0000 0601 1001 04ff 7a1c 4669 6775  ..........z.Figu
+000005b0: 7265 2e70 726f 6365 7373 5f6c 6967 6874  re.process_light
+000005c0: 5f6f 725f 6461 726b 6302 0000 0000 0000  _or_darkc.......
+000005d0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+000005e0: 0073 2e00 0000 7c01 7c00 5f00 7401 7c01  .s....|.|._.t.|.
+000005f0: 8301 7c00 5f02 7c00 6a03 6a04 7215 7c00  ..|._.|.j.j.r.|.
+00000600: 0400 6a02 6401 3700 0200 5f02 6400 5300  ..j.d.7..._.d.S.
+00000610: 6400 5300 2902 4e72 0500 0000 2905 7222  d.S.).Nr....).r"
+00000620: 0000 00da 036c 656e da05 636f 756e 7472  .....len..countr
+00000630: 1c00 0000 da10 756e 6976 6572 7361 6c5f  ......universal_
+00000640: 6c65 6765 6e64 2902 7221 0000 0072 2200  legend).r!...r".
+00000650: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000660: 0072 1e00 0000 2900 0000 730a 0000 0006  .r....)...s.....
+00000670: 010a 0108 0112 0104 ff7a 1e46 6967 7572  .........z.Figur
+00000680: 652e 696e 6974 6961 6c69 7365 5f64 6174  e.initialise_dat
+00000690: 615f 6f62 6a65 6374 7363 0100 0000 0000  a_objectsc......
+000006a0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000006b0: 0000 7320 0000 007c 006a 006a 017d 0174  ..s ...|.j.j.}.t
+000006c0: 027c 006a 037c 0183 025c 027c 005f 047c  .|.j.|...\.|._.|
+000006d0: 005f 0564 0053 0072 1a00 0000 2906 721c  ._.d.S.r....).r.
+000006e0: 0000 00da 0c61 7370 6563 745f 7261 7469  .....aspect_rati
+000006f0: 6f72 0b00 0000 722b 0000 00da 0472 6f77  or....r+.....row
+00000700: 73da 0763 6f6c 756d 6e73 2902 7221 0000  s..columns).r!..
+00000710: 0072 2d00 0000 7217 0000 0072 1700 0000  .r-...r....r....
+00000720: 7218 0000 0072 1f00 0000 2f00 0000 7304  r....r..../...s.
+00000730: 0000 0008 0118 017a 1446 6967 7572 652e  .......z.Figure.
+00000740: 7365 745f 6772 6964 5f73 697a 6563 0100  set_grid_sizec..
+00000750: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000760: 0000 4300 0000 f324 0000 007c 00a0 00a1  ..C....$...|....
+00000770: 0001 007c 00a0 01a1 0001 007c 00a0 02a1  ...|.......|....
+00000780: 0001 007c 00a0 03a1 0001 0064 0053 0072  ...|.......d.S.r
+00000790: 1a00 0000 2904 da11 696e 6974 6961 6c69  ....)...initiali
+000007a0: 7365 5f66 6967 7572 65da 0c63 7265 6174  se_figure..creat
+000007b0: 655f 706c 6f74 73da 1661 6464 5f66 6967  e_plots..add_fig
+000007c0: 7572 655f 7065 7269 7068 6572 616c 73da  ure_peripherals.
+000007d0: 0d6f 7574 7075 745f 6669 6775 7265 7229  .output_figurer)
+000007e0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+000007f0: 0000 da0d 6372 6561 7465 5f66 6967 7572  ....create_figur
+00000800: 6533 0000 00f3 0800 0000 0801 0801 0801  e3..............
+00000810: 0c01 7a14 4669 6775 7265 2e63 7265 6174  ..z.Figure.creat
+00000820: 655f 6669 6775 7265 6301 0000 0000 0000  e_figurec.......
+00000830: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000840: 00f3 1c00 0000 7c00 a000 a100 0100 7c00  ......|.......|.
+00000850: a001 a100 0100 7c00 a002 a100 0100 6400  ......|.......d.
+00000860: 5300 721a 0000 0029 03da 0a73 6574 5f66  S.r....)...set_f
+00000870: 6967 7572 65da 0b63 7265 6174 655f 6178  igure..create_ax
+00000880: 6573 da11 7265 6d6f 7665 5f65 7874 7261  es..remove_extra
+00000890: 5f61 7865 7372 2900 0000 7217 0000 0072  _axesr)...r....r
+000008a0: 1700 0000 7218 0000 0072 3100 0000 3900  ....r....r1...9.
+000008b0: 0000 f306 0000 0008 0108 010c 017a 1846  .............z.F
+000008c0: 6967 7572 652e 696e 6974 6961 6c69 7365  igure.initialise
+000008d0: 5f66 6967 7572 6563 0100 0000 0000 0000  _figurec........
+000008e0: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
+000008f0: 7332 0000 0074 006a 0164 017c 006a 0264  s2...t.j.d.|.j.d
+00000900: 028d 027c 005f 037c 006a 036a 047c 006a  ...|._.|.j.j.|.j
+00000910: 057c 006a 067c 006a 077c 006a 0864 038d  .|.j.|.j.|.j.d..
+00000920: 0401 0064 0053 0029 044e 5429 02da 1263  ...d.S.).NT)...c
+00000930: 6f6e 7374 7261 696e 6564 5f6c 6179 6f75  onstrained_layou
+00000940: 74da 0364 7069 2904 da05 775f 7061 64da  t..dpi)...w_pad.
+00000950: 0568 5f70 6164 da06 6873 7061 6365 da06  .h_pad..hspace..
+00000960: 7773 7061 6365 2909 7226 0000 00da 0666  wspace).r&.....f
+00000970: 6967 7572 6572 3d00 0000 da03 6669 67da  igurer=.....fig.
+00000980: 1b73 6574 5f63 6f6e 7374 7261 696e 6564  .set_constrained
+00000990: 5f6c 6179 6f75 745f 7061 6473 723e 0000  _layout_padsr>..
+000009a0: 0072 3f00 0000 7240 0000 0072 4100 0000  .r?...r@...rA...
+000009b0: 7229 0000 0072 1700 0000 7217 0000 0072  r)...r....r....r
+000009c0: 1800 0000 7238 0000 003e 0000 0073 0800  ....r8...>...s..
+000009d0: 0000 1201 0e01 0801 0aff 7a11 4669 6775  ..........z.Figu
+000009e0: 7265 2e73 6574 5f66 6967 7572 6563 0100  re.set_figurec..
+000009f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000a00: 0000 0300 0000 731e 0000 0087 0066 0164  ......s......f.d
+00000a10: 0164 0284 0874 0088 006a 0183 0144 0083  .d...t...j...D..
+00000a20: 0188 005f 0264 0053 0029 034e 6301 0000  ..._.d.S.).Nc...
+00000a30: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+00000a40: 0013 0000 00f3 1c00 0000 6700 7c00 5d0a  ..........g.|.].
+00000a50: 5c02 7d01 7d02 8800 a000 7c01 7c02 a102  \.}.}.....|.|...
+00000a60: 9102 7102 5300 7217 0000 0029 01da 0867  ..q.S.r....)...g
+00000a70: 6574 5f61 7869 7329 03da 022e 30da 0569  et_axis)....0..i
+00000a80: 6e64 6578 da08 6461 7461 5f6f 626a 7229  ndex..data_objr)
+00000a90: 0000 0072 1700 0000 7218 0000 00da 0a3c  ...r....r......<
+00000aa0: 6c69 7374 636f 6d70 3e44 0000 00f3 0600  listcomp>D......
+00000ab0: 0000 0600 0601 10ff 7a26 4669 6775 7265  ........z&Figure
+00000ac0: 2e63 7265 6174 655f 6178 6573 2e3c 6c6f  .create_axes.<lo
+00000ad0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000ae0: 2903 da09 656e 756d 6572 6174 6572 2200  )...enumerater".
+00000af0: 0000 da04 6178 6573 7229 0000 0072 1700  ....axesr)...r..
+00000b00: 0000 7229 0000 0072 1800 0000 7239 0000  ..r)...r....r9..
+00000b10: 0043 0000 0073 0600 0000 0a01 0801 0cff  .C...s..........
+00000b20: 7a12 4669 6775 7265 2e63 7265 6174 655f  z.Figure.create_
+00000b30: 6178 6573 6303 0000 0000 0000 0000 0000  axesc...........
+00000b40: 0004 0000 0006 0000 0043 0000 0073 2200  .........C...s".
+00000b50: 0000 7c00 6a00 6a01 7c00 6a02 7c00 6a03  ..|.j.j.|.j.|.j.
+00000b60: 7c01 6401 1700 7c02 6a04 6402 8d04 7d03  |.d...|.j.d...}.
+00000b70: 7c03 5300 2903 4e72 0500 0000 2901 da0a  |.S.).Nr....)...
+00000b80: 7072 6f6a 6563 7469 6f6e 2905 7243 0000  projection).rC..
+00000b90: 00da 0b61 6464 5f73 7562 706c 6f74 722e  ...add_subplotr.
+00000ba0: 0000 0072 2f00 0000 724e 0000 0029 0472  ...r/...rN...).r
+00000bb0: 2100 0000 7248 0000 0072 4900 0000 da04  !...rH...rI.....
+00000bc0: 6178 6973 7217 0000 0072 1700 0000 7218  axisr....r....r.
+00000bd0: 0000 0072 4600 0000 4700 0000 7308 0000  ...rF...G...s...
+00000be0: 0014 0104 0106 ff04 027a 0f46 6967 7572  .........z.Figur
+00000bf0: 652e 6765 745f 6178 6973 6301 0000 0000  e.get_axisc.....
+00000c00: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
+00000c10: 0000 0073 4000 0000 7400 7c00 6a01 8301  ...s@...t.|.j...
+00000c20: 7c00 6a02 1800 7d01 7403 7c00 6a01 6400  |.j...}.t.|.j.d.
+00000c30: 6400 6401 8503 1900 7404 7c01 8301 8302  d.d.....t.|.....
+00000c40: 4400 5d08 5c02 7d02 7d03 7c02 a005 a100  D.].\.}.}.|.....
+00000c50: 0100 7115 6400 5300 2902 4ee9 ffff ffff  ..q.d.S.).N.....
+00000c60: 2906 722a 0000 0072 4d00 0000 722b 0000  ).r*...rM...r+..
+00000c70: 00da 037a 6970 da05 7261 6e67 65da 0672  ...zip..range..r
+00000c80: 656d 6f76 6529 0472 2100 0000 da10 6578  emove).r!.....ex
+00000c90: 7472 615f 6178 6573 5f63 6f75 6e74 da02  tra_axes_count..
+00000ca0: 6178 da01 5f72 1700 0000 7217 0000 0072  ax.._r....r....r
+00000cb0: 1800 0000 723a 0000 004c 0000 0073 0800  ....r:...L...s..
+00000cc0: 0000 1001 2201 0a01 04ff 7a18 4669 6775  ....".....z.Figu
+00000cd0: 7265 2e72 656d 6f76 655f 6578 7472 615f  re.remove_extra_
+00000ce0: 6178 6573 6301 0000 0000 0000 0000 0000  axesc...........
+00000cf0: 0001 0000 0002 0000 0043 0000 0072 3000  .........C...r0.
+00000d00: 0000 721a 0000 0029 04da 1573 6574 5f73  ..r....)...set_s
+00000d10: 7570 7469 746c 655f 666f 6e74 6469 6374  uptitle_fontdict
+00000d20: da0c 7365 745f 7375 7074 6974 6c65 da14  ..set_suptitle..
+00000d30: 7365 745f 756e 6976 6572 7361 6c5f 6c65  set_universal_le
+00000d40: 6765 6e64 da0f 7365 745f 6669 6775 7265  gend..set_figure
+00000d50: 5f73 697a 6572 2900 0000 7217 0000 0072  _sizer)...r....r
+00000d60: 1700 0000 7218 0000 0072 3300 0000 5100  ....r....r3...Q.
+00000d70: 0000 7236 0000 007a 1d46 6967 7572 652e  ..r6...z.Figure.
+00000d80: 6164 645f 6669 6775 7265 5f70 6572 6970  add_figure_perip
+00000d90: 6865 7261 6c73 6301 0000 0000 0000 0000  heralsc.........
+00000da0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+00000db0: 2800 0000 7c00 6a00 7c00 6a01 7c00 6a02  (...|.j.|.j.|.j.
+00000dc0: 7c00 6a03 7c00 6a04 6401 9c05 7d01 7405  |.j.|.j.d...}.t.
+00000dd0: 7c01 8301 7c00 5f06 6400 5300 2902 4e29  |...|._.d.S.).N)
+00000de0: 05da 0866 6f6e 746e 616d 65da 0866 6f6e  ...fontname..fon
+00000df0: 7473 697a 65da 0563 6f6c 6f72 da11 7665  tsize..color..ve
+00000e00: 7274 6963 616c 616c 6967 6e6d 656e 74da  rticalalignment.
+00000e10: 1368 6f72 697a 6f6e 7461 6c61 6c69 676e  .horizontalalign
+00000e20: 6d65 6e74 2907 da11 7375 7074 6974 6c65  ment)...suptitle
+00000e30: 5f66 6f6e 746e 616d 65da 1173 7570 7469  _fontname..supti
+00000e40: 746c 655f 666f 6e74 7369 7a65 da0e 7375  tle_fontsize..su
+00000e50: 7074 6974 6c65 5f63 6f6c 6f72 da1a 7375  ptitle_color..su
+00000e60: 7074 6974 6c65 5f76 6572 7469 6361 6c61  ptitle_verticala
+00000e70: 6c69 676e 6d65 6e74 da1c 7375 7074 6974  lignment..suptit
+00000e80: 6c65 5f68 6f72 697a 6f6e 7461 6c61 6c69  le_horizontalali
+00000e90: 676e 6d65 6e74 720e 0000 00da 1173 7570  gnmentr......sup
+00000ea0: 7469 746c 655f 666f 6e74 6469 6374 2902  title_fontdict).
+00000eb0: 7221 0000 0072 1b00 0000 7217 0000 0072  r!...r....r....r
+00000ec0: 1700 0000 7218 0000 0072 5800 0000 5700  ....r....rX...W.
+00000ed0: 0000 730e 0000 0004 0104 0104 0104 0104  ..s.............
+00000ee0: 0106 fc0e 057a 1c46 6967 7572 652e 7365  .....z.Figure.se
+00000ef0: 745f 7375 7074 6974 6c65 5f66 6f6e 7464  t_suptitle_fontd
+00000f00: 6963 7463 0100 0000 0000 0000 0000 0000  ictc............
+00000f10: 0100 0000 0600 0000 4300 0000 733e 0000  ........C...s>..
+00000f20: 007c 006a 006a 0164 0075 0172 1d7c 006a  .|.j.j.d.u.r.|.j
+00000f30: 026a 017c 006a 006a 019b 0066 0169 007c  .j.|.j.j...f.i.|
+00000f40: 006a 03a4 017c 006a 047c 006a 0564 019c  .j...|.j.|.j.d..
+00000f50: 02a4 018e 0101 0064 0053 0064 0053 0029  .......d.S.d.S.)
+00000f60: 024e 2902 da01 78da 0179 2906 721c 0000  .N)...x..y).r...
+00000f70: 00da 0873 7570 7469 746c 6572 4300 0000  ...suptitlerC...
+00000f80: 7266 0000 00da 0a73 7570 7469 746c 655f  rf.....suptitle_
+00000f90: 78da 0a73 7570 7469 746c 655f 7972 2900  x..suptitle_yr).
+00000fa0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000fb0: 0072 5900 0000 5f00 0000 730e 0000 000c  .rY..._...s.....
+00000fc0: 0112 0104 0102 ff08 020e fe04 ff7a 1346  .............z.F
+00000fd0: 6967 7572 652e 7365 745f 7375 7074 6974  igure.set_suptit
+00000fe0: 6c65 6301 0000 0000 0000 0000 0000 0001  lec.............
+00000ff0: 0000 0002 0000 0043 0000 0073 1800 0000  .......C...s....
+00001000: 7c00 6a00 6a01 720a 7c00 a002 a100 0100  |.j.j.r.|.......
+00001010: 6400 5300 6400 5300 721a 0000 0029 0372  d.S.d.S.r....).r
+00001020: 1c00 0000 722c 0000 00da 1364 6f5f 756e  ....r,.....do_un
+00001030: 6976 6572 7361 6c5f 6c65 6765 6e64 7229  iversal_legendr)
+00001040: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00001050: 0000 725a 0000 0065 0000 0073 0600 0000  ..rZ...e...s....
+00001060: 0801 0c01 04ff 7a1b 4669 6775 7265 2e73  ......z.Figure.s
+00001070: 6574 5f75 6e69 7665 7273 616c 5f6c 6567  et_universal_leg
+00001080: 656e 6463 0100 0000 0000 0000 0000 0000  endc............
+00001090: 0300 0000 0700 0000 4300 0000 7350 0000  ........C...sP..
+000010a0: 007c 006a 0064 0119 007d 017c 006a 0164  .|.j.d...}.|.j.d
+000010b0: 0219 006a 0144 005d 0d7d 027c 016a 0264  ...j.D.].}.|.j.d
+000010c0: 0364 037c 026a 037c 026a 0464 048d 0401  .d.|.j.|.j.d....
+000010d0: 0071 0b7c 016a 0564 0564 0664 0364 078d  .q.|.j.d.d.d.d..
+000010e0: 0301 007c 01a0 0664 08a1 0101 0064 0053  ...|...d.....d.S
+000010f0: 0029 094e 7251 0000 0072 0100 0000 7205  .).NrQ...r....r.
+00001100: 0000 0029 02da 056c 6162 656c 725e 0000  ...)...labelr^..
+00001110: 00da 0663 656e 7465 7272 0300 0000 2903  ...centerr....).
+00001120: da03 6c6f 63da 0962 6f72 6465 7270 6164  ..loc..borderpad
+00001130: da0c 6c61 6265 6c73 7061 6369 6e67 da03  ..labelspacing..
+00001140: 6f66 6629 0772 4d00 0000 7222 0000 00da  off).rM...r"....
+00001150: 0470 6c6f 7472 6d00 0000 da06 636f 6c6f  .plotrm.....colo
+00001160: 7572 da06 6c65 6765 6e64 7250 0000 0029  ur..legendrP...)
+00001170: 0372 2100 0000 7256 0000 0072 4900 0000  .r!...rV...rI...
+00001180: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001190: 6c00 0000 6900 0000 730a 0000 000a 0110  l...i...s.......
+000011a0: 0118 0110 010e 017a 1a46 6967 7572 652e  .......z.Figure.
+000011b0: 646f 5f75 6e69 7665 7273 616c 5f6c 6567  do_universal_leg
+000011c0: 656e 6463 0100 0000 0000 0000 0000 0000  endc............
+000011d0: 0100 0000 0200 0000 4300 0000 7314 0000  ........C...s...
+000011e0: 007c 00a0 00a1 0001 007c 00a0 01a1 0001  .|.......|......
+000011f0: 0064 0053 0072 1a00 0000 2902 da0b 7570  .d.S.r....)...up
+00001200: 6461 7465 5f73 697a 65da 1673 6574 5f66  date_size..set_f
+00001210: 6967 7572 655f 7369 7a65 5f70 6978 656c  igure_size_pixel
+00001220: 7372 2900 0000 7217 0000 0072 1700 0000  sr)...r....r....
+00001230: 7218 0000 0072 5b00 0000 7000 0000 f304  r....r[...p.....
+00001240: 0000 0008 010c 017a 1646 6967 7572 652e  .......z.Figure.
+00001250: 7365 745f 6669 6775 7265 5f73 697a 6563  set_figure_sizec
+00001260: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001270: 0200 0000 4300 0000 7237 0000 0072 1a00  ....C...r7...r..
+00001280: 0000 2903 da19 7365 745f 6d61 7869 6d69  ..)...set_maximi
+00001290: 7365 645f 6669 6775 7265 5f73 697a 65da  sed_figure_size.
+000012a0: 1173 6574 5f66 6967 7572 655f 696e 6368  .set_figure_inch
+000012b0: 6573 720d 0000 0072 2900 0000 7217 0000  esr....r)...r...
+000012c0: 0072 1700 0000 7218 0000 0072 7600 0000  .r....r....rv...
+000012d0: 7400 0000 723b 0000 007a 1246 6967 7572  t...r;...z.Figur
+000012e0: 652e 7570 6461 7465 5f73 697a 6563 0100  e.update_sizec..
+000012f0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00001300: 0000 4300 0000 7332 0000 007c 006a 0072  ..C...s2...|.j.r
+00001310: 1774 0183 0064 0119 007d 017c 016a 0264  .t...d...}.|.j.d
+00001320: 021b 007c 016a 0364 021b 0067 027d 027c  ...|.j.d...g.}.|
+00001330: 027c 005f 0464 0053 0064 0053 0029 034e  .|._.d.S.d.S.).N
+00001340: 7201 0000 0067 6666 6666 6666 3940 2905  r....gffffff9@).
+00001350: da08 6d61 7869 6d69 7365 7202 0000 00da  ..maximiser.....
+00001360: 0877 6964 7468 5f6d 6dda 0968 6569 6768  .width_mm..heigh
+00001370: 745f 6d6d da0b 6669 6775 7265 5f73 697a  t_mm..figure_siz
+00001380: 6529 0372 2100 0000 da07 6d6f 6e69 746f  e).r!.....monito
+00001390: 7272 7e00 0000 7217 0000 0072 1700 0000  rr~...r....r....
+000013a0: 7218 0000 0072 7900 0000 7900 0000 730a  r....ry...y...s.
+000013b0: 0000 0006 010a 0114 010a 0104 fd7a 2046  .............z F
+000013c0: 6967 7572 652e 7365 745f 6d61 7869 6d69  igure.set_maximi
+000013d0: 7365 645f 6669 6775 7265 5f73 697a 6563  sed_figure_sizec
+000013e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000013f0: 0100 0000 4300 0000 7314 0000 007c 006a  ....C...s....|.j
+00001400: 0072 0874 0183 0001 0064 0053 0064 0053  .r.t.....d.S.d.S
+00001410: 0072 1a00 0000 2902 727b 0000 0072 0d00  .r....).r{...r..
+00001420: 0000 7229 0000 0072 1700 0000 7217 0000  ..r)...r....r...
+00001430: 0072 1800 0000 720d 0000 007f 0000 0073  .r....r........s
+00001440: 0600 0000 0601 0a01 04ff 7a16 4669 6775  ..........z.Figu
+00001450: 7265 2e6d 6178 696d 6973 655f 6669 6775  re.maximise_figu
+00001460: 7265 6301 0000 0000 0000 0000 0000 0001  rec.............
+00001470: 0000 0003 0000 0043 0000 0073 2000 0000  .......C...s ...
+00001480: 7c00 6a00 6400 7501 720e 7c00 6a01 a002  |.j.d.u.r.|.j...
+00001490: 7c00 6a00 a101 0100 6400 5300 6400 5300  |.j.....d.S.d.S.
+000014a0: 721a 0000 0029 0372 7e00 0000 7243 0000  r....).r~...rC..
+000014b0: 00da 0f73 6574 5f73 697a 655f 696e 6368  ...set_size_inch
+000014c0: 6573 7229 0000 0072 1700 0000 7217 0000  esr)...r....r...
+000014d0: 0072 1800 0000 727a 0000 0083 0000 0073  .r....rz.......s
+000014e0: 0600 0000 0a01 1201 04ff 7a18 4669 6775  ..........z.Figu
+000014f0: 7265 2e73 6574 5f66 6967 7572 655f 696e  re.set_figure_in
+00001500: 6368 6573 6301 0000 0000 0000 0000 0000  chesc...........
+00001510: 0001 0000 0002 0000 0043 0000 0073 2a00  .........C...s*.
+00001520: 0000 7c00 6a00 a001 a100 7c00 6a00 6a02  ..|.j.....|.j.j.
+00001530: 1400 7c00 5f03 6401 6402 8400 7c00 6a03  ..|._.d.d...|.j.
+00001540: 4400 8301 7c00 5f03 6400 5300 2903 4e63  D...|._.d.S.).Nc
+00001550: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001560: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00001570: 005d 067d 0174 007c 0183 0191 0271 0253  .].}.t.|.....q.S
+00001580: 0072 1700 0000 2901 da03 696e 7429 0272  .r....)...int).r
+00001590: 4700 0000 da05 7661 6c75 6572 1700 0000  G.....valuer....
+000015a0: 7217 0000 0072 1800 0000 724a 0000 0089  r....r....rJ....
+000015b0: 0000 0073 0200 0000 1400 7a31 4669 6775  ...s......z1Figu
+000015c0: 7265 2e73 6574 5f66 6967 7572 655f 7369  re.set_figure_si
+000015d0: 7a65 5f70 6978 656c 732e 3c6c 6f63 616c  ze_pixels.<local
+000015e0: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
+000015f0: 4300 0000 da0f 6765 745f 7369 7a65 5f69  C.....get_size_i
+00001600: 6e63 6865 7372 3d00 0000 da12 6669 6775  nchesr=.....figu
+00001610: 7265 5f73 697a 655f 7069 7865 6c73 7229  re_size_pixelsr)
+00001620: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00001630: 0000 7277 0000 0087 0000 0073 0400 0000  ..rw.......s....
+00001640: 1401 1601 7a1d 4669 6775 7265 2e73 6574  ....z.Figure.set
+00001650: 5f66 6967 7572 655f 7369 7a65 5f70 6978  _figure_size_pix
+00001660: 656c 7363 0100 0000 0000 0000 0000 0000  elsc............
+00001670: 0100 0000 0400 0000 0300 0000 7322 0000  ............s"..
+00001680: 0087 0066 0164 0164 0284 0874 0088 006a  ...f.d.d...t...j
+00001690: 0188 006a 0283 0244 0083 0188 005f 0364  ...j...D....._.d
+000016a0: 0053 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
+000016b0: 0000 0003 0000 0006 0000 0013 0000 0072  ...............r
+000016c0: 4500 0000 7217 0000 0029 01da 0f63 7265  E...r....)...cre
+000016d0: 6174 655f 706c 6f74 5f6f 626a 2903 7247  ate_plot_obj).rG
+000016e0: 0000 0072 5600 0000 7249 0000 0072 2900  ...rV...rI...r).
+000016f0: 0000 7217 0000 0072 1800 0000 724a 0000  ..r....r....rJ..
+00001700: 008c 0000 0072 4b00 0000 7a27 4669 6775  .....rK...z'Figu
+00001710: 7265 2e63 7265 6174 655f 706c 6f74 732e  re.create_plots.
+00001720: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001730: 6d70 3e29 0472 5200 0000 724d 0000 0072  mp>).rR...rM...r
+00001740: 2200 0000 da0c 706c 6f74 5f6f 626a 6563  ".....plot_objec
+00001750: 7473 7229 0000 0072 1700 0000 7229 0000  tsr)...r....r)..
+00001760: 0072 1800 0000 7232 0000 008b 0000 0073  .r....r2.......s
+00001770: 0600 0000 0a01 0c01 0cff 7a13 4669 6775  ..........z.Figu
+00001780: 7265 2e63 7265 6174 655f 706c 6f74 7363  re.create_plotsc
+00001790: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+000017a0: 0400 0000 4300 0000 7326 0000 007c 006a  ....C...s&...|.j
+000017b0: 007c 026a 016a 0219 007d 037c 037c 007c  .|.j.j...}.|.|.|
+000017c0: 017c 0283 037d 047c 04a0 03a1 0001 007c  .|...}.|.......|
+000017d0: 0453 0072 1a00 0000 2904 7215 0000 00da  .S.r....).r.....
+000017e0: 095f 5f63 6c61 7373 5f5f da08 5f5f 6e61  .__class__..__na
+000017f0: 6d65 5f5f da0b 6372 6561 7465 5f70 6c6f  me__..create_plo
+00001800: 7429 0572 2100 0000 7256 0000 0072 4900  t).r!...rV...rI.
+00001810: 0000 da0a 706c 6f74 5f63 6c61 7373 da08  ....plot_class..
+00001820: 706c 6f74 5f6f 626a 7217 0000 0072 1700  plot_objr....r..
+00001830: 0000 7218 0000 0072 8500 0000 8f00 0000  ..r....r........
+00001840: 7308 0000 000e 010c 0108 0104 017a 1646  s............z.F
+00001850: 6967 7572 652e 6372 6561 7465 5f70 6c6f  igure.create_plo
+00001860: 745f 6f62 6a63 0100 0000 0000 0000 0000  t_objc..........
+00001870: 0000 0100 0000 0200 0000 4300 0000 7334  ..........C...s4
+00001880: 0000 007c 006a 006a 0164 016b 0272 0c7c  ...|.j.j.d.k.r.|
+00001890: 00a0 02a1 0001 0064 0053 007c 006a 006a  .......d.S.|.j.j
+000018a0: 0164 026b 0272 1874 037c 0083 0101 0064  .d.k.r.t.|.....d
+000018b0: 0053 0064 0053 0029 034e da04 5368 6f77  .S.d.S.).N..Show
+000018c0: da04 5361 7665 2904 721c 0000 00da 066f  ..Save).r......o
+000018d0: 7574 7075 74da 0b73 686f 775f 6669 6775  utput..show_figu
+000018e0: 7265 720c 0000 0072 2900 0000 7217 0000  rer....r)...r...
+000018f0: 0072 1700 0000 7218 0000 0072 3400 0000  .r....r....r4...
+00001900: 9500 0000 730a 0000 000c 010c 010c 010c  ....s...........
+00001910: 0104 ff7a 1446 6967 7572 652e 6f75 7470  ...z.Figure.outp
+00001920: 7574 5f66 6967 7572 6563 0100 0000 0000  ut_figurec......
+00001930: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00001940: 0000 7314 0000 0074 00a0 01a1 0001 0074  ..s....t.......t
+00001950: 00a0 02a1 0001 0064 0053 0072 1a00 0000  .......d.S.r....
+00001960: 2903 7226 0000 00da 0473 686f 77da 0563  ).r&.....show..c
+00001970: 6c6f 7365 7229 0000 0072 1700 0000 7217  loser)...r....r.
+00001980: 0000 0072 1800 0000 728f 0000 009b 0000  ...r....r.......
+00001990: 0072 7800 0000 7a12 4669 6775 7265 2e73  .rx...z.Figure.s
+000019a0: 686f 775f 6669 6775 7265 6301 0000 0000  how_figurec.....
+000019b0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+000019c0: 0000 0073 1800 0000 7c00 6a00 4400 5d06  ...s....|.j.D.].
+000019d0: 7d01 7c01 a001 a100 0100 7103 6400 5300  }.|.......q.d.S.
+000019e0: 721a 0000 0029 0272 2200 0000 da19 7365  r....).r".....se
+000019f0: 745f 616e 696d 6174 696f 6e5f 6178 6973  t_animation_axis
+00001a00: 5f6c 696d 6974 7329 0272 2100 0000 7249  _limits).r!...rI
+00001a10: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00001a20: 0000 7292 0000 009f 0000 0073 0600 0000  ..r........s....
+00001a30: 0a01 0a01 04ff 7a20 4669 6775 7265 2e73  ......z Figure.s
+00001a40: 6574 5f61 6e69 6d61 7469 6f6e 5f61 7869  et_animation_axi
+00001a50: 735f 6c69 6d69 7473 6301 0000 0000 0000  s_limitsc.......
+00001a60: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00001a70: 0073 1200 0000 7c00 6a00 6401 1900 a001  .s....|.j.d.....
+00001a80: a100 7d01 7c01 5300 2902 4e72 0100 0000  ..}.|.S.).Nr....
+00001a90: 2902 7222 0000 00da 0f67 6574 5f66 7261  ).r".....get_fra
+00001aa0: 6d65 5f63 6f75 6e74 2902 7221 0000 00da  me_count).r!....
+00001ab0: 0b66 7261 6d65 5f63 6f75 6e74 7217 0000  .frame_countr...
+00001ac0: 0072 1700 0000 7218 0000 0072 9300 0000  .r....r....r....
+00001ad0: a300 0000 7304 0000 000e 0104 017a 1646  ....s........z.F
+00001ae0: 6967 7572 652e 6765 745f 6672 616d 655f  igure.get_frame_
+00001af0: 636f 756e 7463 0200 0000 0000 0000 0000  countc..........
+00001b00: 0000 0500 0000 0400 0000 4300 0000 732e  ..........C...s.
+00001b10: 0000 0074 007c 006a 017c 006a 0283 0244  ...t.|.j.|.j...D
+00001b20: 005d 0d5c 027d 027d 037c 037c 0119 007d  .].\.}.}.|.|...}
+00001b30: 047c 02a0 037c 04a1 0101 0071 0764 0053  .|...|.....q.d.S
+00001b40: 0072 1a00 0000 2904 7252 0000 0072 2200  .r....).rR...r".
+00001b50: 0000 da0f 616c 6c5f 6461 7461 5f76 616c  ....all_data_val
+00001b60: 7565 73da 0e73 6574 5f64 6174 615f 7661  ues..set_data_va
+00001b70: 6c75 6529 0572 2100 0000 7248 0000 0072  lue).r!...rH...r
+00001b80: 4900 0000 da0b 6461 7461 5f76 616c 7565  I.....data_value
+00001b90: 73da 0a64 6174 615f 7661 6c75 6572 1700  s..data_valuer..
+00001ba0: 0000 7217 0000 0072 1800 0000 7296 0000  ..r....r....r...
+00001bb0: 00a7 0000 0073 0800 0000 1601 0801 0c01  .....s..........
+00001bc0: 04fe 7a15 4669 6775 7265 2e73 6574 5f64  ..z.Figure.set_d
+00001bd0: 6174 615f 7661 6c75 654e 2921 7288 0000  ata_valueN)!r...
+00001be0: 00da 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  ...__module__.._
+00001bf0: 5f71 7561 6c6e 616d 655f 5fda 0b63 6c61  _qualname__..cla
+00001c00: 7373 6d65 7468 6f64 7219 0000 0072 2300  ssmethodr....r#.
+00001c10: 0000 7220 0000 0072 1e00 0000 721f 0000  ..r ...r....r...
+00001c20: 0072 3500 0000 7231 0000 0072 3800 0000  .r5...r1...r8...
+00001c30: 7239 0000 0072 4600 0000 723a 0000 0072  r9...rF...r:...r
+00001c40: 3300 0000 7258 0000 0072 5900 0000 725a  3...rX...rY...rZ
+00001c50: 0000 0072 6c00 0000 725b 0000 0072 7600  ...rl...r[...rv.
+00001c60: 0000 7279 0000 0072 0d00 0000 727a 0000  ..ry...r....rz..
+00001c70: 0072 7700 0000 7232 0000 0072 8500 0000  .rw...r2...r....
+00001c80: 7234 0000 0072 8f00 0000 7292 0000 0072  r4...r....r....r
+00001c90: 9300 0000 7296 0000 0072 1700 0000 7217  ....r....r....r.
+00001ca0: 0000 0072 1700 0000 7218 0000 0072 0f00  ...r....r....r..
+00001cb0: 0000 1300 0000 733e 0000 0008 0002 020a  ......s>........
+00001cc0: 0108 0708 0808 0408 0608 0408 0608 0508  ................
+00001cd0: 0508 0408 0508 0508 0608 0808 0608 0408  ................
+00001ce0: 0708 0408 0508 0608 0408 0408 0408 0408  ................
+00001cf0: 0608 0608 0408 040c 0472 0f00 0000 291f  .........r....).
+00001d00: da02 6f73 da04 6d61 7468 da0a 7363 7265  ..os..math..scre
+00001d10: 656e 696e 666f 7202 0000 00da 116d 6174  eninfor......mat
+00001d20: 706c 6f74 6c69 622e 7079 706c 6f74 da06  plotlib.pyplot..
+00001d30: 7079 706c 6f74 7226 0000 00da 056e 756d  pyplotr&.....num
+00001d40: 7079 da02 6e70 da00 7204 0000 00da 1370  py..np..r......p
+00001d50: 6c6f 7474 7970 6573 2e70 6c6f 746c 696e  lottypes.plotlin
+00001d60: 6573 7206 0000 00da 1270 6c6f 7474 7970  esr......plottyp
+00001d70: 6573 2e70 6c6f 7462 6172 7372 0700 0000  es.plotbarsr....
+00001d80: da11 706c 6f74 7479 7065 732e 706c 6f74  ..plottypes.plot
+00001d90: 7069 6572 0800 0000 da17 706c 6f74 7479  pier......plotty
+00001da0: 7065 732e 706c 6f74 636f 6c6f 7270 6c6f  pes.plotcolorplo
+00001db0: 7472 0900 0000 da15 706c 6f74 7479 7065  tr......plottype
+00001dc0: 732e 706c 6f74 7375 7266 6163 6572 0a00  s.plotsurfacer..
+00001dd0: 0000 da18 706c 6f74 7574 696c 732e 6772  ....plotutils.gr
+00001de0: 6964 6469 6d65 6e73 696f 6e73 720b 0000  iddimensionsr...
+00001df0: 00da 1470 6c6f 7475 7469 6c73 2e73 6176  ...plotutils.sav
+00001e00: 6566 6967 7572 6572 0c00 0000 da14 706c  efigurer......pl
+00001e10: 6f74 7574 696c 732e 6669 6775 7265 7369  otutils.figuresi
+00001e20: 7a65 720d 0000 00da 0b75 7469 6c73 2e64  zer......utils.d
+00001e30: 6963 7473 720e 0000 0072 0f00 0000 da04  ictsr....r......
+00001e40: 6c6f 6164 7217 0000 0072 1700 0000 7217  loadr....r....r.
+00001e50: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
+00001e60: 653e 0100 0000 7324 0000 0008 0008 010c  e>....s$........
+00001e70: 010c 0208 010c 020c 010c 010c 010c 010c  ................
+00001e80: 010c 010c 010c 010c 010e 0200 7f0e 1a    ...............
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figures.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 19:31:35 2023 UTC, .py size: 2899 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 975b 8f64 530b 0000  o........[.dS...
+00000000: 6f0d 0d0a 0000 0000 a48a 9064 800b 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6404 6405 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6402 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6402 6408 6c0a 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -117,131 +117,134 @@
 00000740: 7572 6573 2900 0000 7306 0000 0008 0108  ures)...s.......
 00000750: 0114 017a 1646 6967 7572 6573 2e63 7265  ...z.Figures.cre
 00000760: 6174 655f 6669 6775 7265 7363 0100 0000  ate_figuresc....
 00000770: 0000 0000 0000 0000 0100 0000 0200 0000  ................
 00000780: 4300 0000 731a 0000 007c 006a 0064 016b  C...s....|.j.d.k
 00000790: 0272 0b7c 00a0 01a1 0001 0064 0053 0064  .r.|.......d.S.d
 000007a0: 0053 0029 024e da04 5361 7665 2902 da06  .S.).N..Save)...
-000007b0: 6f75 7470 7574 da08 7365 745f 7061 7468  output..set_path
-000007c0: a901 7212 0000 0072 1300 0000 7213 0000  ..r....r....r...
-000007d0: 0072 1400 0000 7225 0000 002e 0000 0073  .r....r%.......s
-000007e0: 0600 0000 0a01 0c01 04ff 7a1b 4669 6775  ..........z.Figu
-000007f0: 7265 732e 7072 6f63 6573 735f 6f75 7470  res.process_outp
-00000800: 7574 5f6d 6f64 65da 0550 6c6f 7473 6302  ut_mode..Plotsc.
-00000810: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000820: 0000 0043 0000 0073 1600 0000 7c00 a000  ...C...s....|...
-00000830: a100 0100 7c00 a001 7c01 a101 0100 6400  ....|...|.....d.
-00000840: 5300 720c 0000 0029 02da 1073 6574 5f64  S.r....)...set_d
-00000850: 6566 6175 6c74 5f70 6174 68da 1573 706c  efault_path..spl
-00000860: 6974 5f6f 6e5f 706c 6f74 735f 666f 6c64  it_on_plots_fold
-00000870: 6572 a902 7212 0000 00da 1170 6c6f 7473  er..r......plots
-00000880: 5f66 6f6c 6465 725f 6e61 6d65 7213 0000  _folder_namer...
-00000890: 0072 1300 0000 7214 0000 0072 2a00 0000  .r....r....r*...
-000008a0: 3200 0000 7304 0000 0008 010e 017a 1046  2...s........z.F
-000008b0: 6967 7572 6573 2e73 6574 5f70 6174 6863  igures.set_pathc
-000008c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000008d0: 0300 0000 4300 0000 7326 0000 007c 006a  ....C...s&...|.j
-000008e0: 0064 0075 0072 1174 016a 00a0 0274 036a  .d.u.r.t.j...t.j
-000008f0: 04a1 0164 0119 007c 005f 0064 0053 0064  ...d...|._.d.S.d
-00000900: 0053 0029 024e 7201 0000 0029 05da 0470  .S.).Nr....)...p
-00000910: 6174 68da 026f 73da 0573 706c 6974 da08  ath..os..split..
-00000920: 5f5f 6d61 696e 5f5f da08 5f5f 6669 6c65  __main__..__file
-00000930: 5f5f 722b 0000 0072 1300 0000 7213 0000  __r+...r....r...
-00000940: 0072 1400 0000 722d 0000 0036 0000 0073  .r....r-...6...s
-00000950: 0600 0000 0a01 1801 04ff 7a18 4669 6775  ..........z.Figu
-00000960: 7265 732e 7365 745f 6465 6661 756c 745f  res.set_default_
-00000970: 7061 7468 6302 0000 0000 0000 0000 0000  pathc...........
-00000980: 0002 0000 0004 0000 0043 0000 0073 2a00  .........C...s*.
-00000990: 0000 7c00 6a00 7213 7401 6a02 a003 7c00  ..|.j.r.t.j...|.
-000009a0: 6a02 7c01 a102 7c00 5f02 7404 7c00 6a02  j.|...|._.t.|.j.
-000009b0: 8301 0100 6400 5300 6400 5300 720c 0000  ....d.S.d.S.r...
-000009c0: 0029 05da 0c70 6c6f 7473 5f66 6f6c 6465  .)...plots_folde
-000009d0: 7272 3200 0000 7231 0000 00da 046a 6f69  rr2...r1.....joi
-000009e0: 6e72 0a00 0000 722f 0000 0072 1300 0000  nr....r/...r....
-000009f0: 7213 0000 0072 1400 0000 722e 0000 003a  r....r....r....:
-00000a00: 0000 0073 0800 0000 0601 1201 0e01 04fe  ...s............
-00000a10: 7a1d 4669 6775 7265 732e 7370 6c69 745f  z.Figures.split_
-00000a20: 6f6e 5f70 6c6f 7473 5f66 6f6c 6465 7263  on_plots_folderc
-00000a30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000a40: 0300 0000 0300 0000 7336 0000 0074 0088  ........s6...t..
-00000a50: 006a 0188 006a 0283 0288 005f 0174 0388  .j...j....._.t..
-00000a60: 006a 0488 006a 0183 027d 0187 0066 0164  .j...j...}...f.d
-00000a70: 0164 0284 087c 0144 0083 0188 005f 0564  .d...|.D....._.d
-00000a80: 0053 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00000a90: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00000aa0: 1600 0000 6700 7c00 5d07 7d01 8800 6a00  ....g.|.].}...j.
-00000ab0: 7c01 1900 9102 7102 5300 7213 0000 0029  |.....q.S.r....)
-00000ac0: 0172 0f00 0000 2902 721b 0000 00da 0769  .r....).r......i
-00000ad0: 6e64 6578 6573 722b 0000 0072 1300 0000  ndexesr+...r....
-00000ae0: 7214 0000 0072 1d00 0000 4200 0000 721e  r....r....B...r.
-00000af0: 0000 007a 3046 6967 7572 6573 2e70 726f  ...z0Figures.pro
-00000b00: 6365 7373 5f64 6174 615f 6f62 6a65 6374  cess_data_object
-00000b10: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-00000b20: 636f 6d70 3e29 0672 0900 0000 da08 7375  comp>).r......su
-00000b30: 6270 6c6f 7473 720f 0000 0072 0800 0000  bplotsr....r....
-00000b40: 7211 0000 00da 1264 6174 615f 6f62 6a65  r......data_obje
-00000b50: 6374 5f67 726f 7570 7329 0272 1200 0000  ct_groups).r....
-00000b60: da0d 6772 6f75 705f 696e 6465 7865 7372  ..group_indexesr
-00000b70: 1300 0000 722b 0000 0072 1400 0000 7224  ....r+...r....r$
-00000b80: 0000 003f 0000 0073 0a00 0000 1001 0e01  ...?...s........
-00000b90: 0a01 0201 0cff 7a1c 4669 6775 7265 732e  ......z.Figures.
-00000ba0: 7072 6f63 6573 735f 6461 7461 5f6f 626a  process_data_obj
-00000bb0: 6563 7473 6301 0000 0000 0000 0000 0000  ectsc...........
-00000bc0: 0003 0000 0004 0000 004b 0000 0073 2800  .........K...s(.
-00000bd0: 0000 7c00 6a00 6401 6900 7c01 a401 8e01  ..|.j.d.i.|.....
-00000be0: 0100 7c00 6a01 4400 5d06 7d02 7c02 a002  ..|.j.D.].}.|...
-00000bf0: a100 0100 710b 6400 5300 7223 0000 0029  ....q.d.S.r#...)
-00000c00: 03da 1273 6574 5f66 6967 7572 655f 6f62  ...set_figure_ob
-00000c10: 6a65 6374 73da 0e66 6967 7572 655f 6f62  jects..figure_ob
-00000c20: 6a65 6374 73da 0d63 7265 6174 655f 6669  jects..create_fi
-00000c30: 6775 7265 2903 7212 0000 0072 0d00 0000  gure).r....r....
-00000c40: da0a 6669 6775 7265 5f6f 626a 7213 0000  ..figure_objr...
-00000c50: 0072 1300 0000 7214 0000 0072 2600 0000  .r....r....r&...
-00000c60: 4500 0000 7308 0000 0010 010a 010a 0104  E...s...........
-00000c70: ff7a 1946 6967 7572 6573 2e70 6c6f 745f  .z.Figures.plot_
-00000c80: 6461 7461 5f6f 626a 6563 7473 6301 0000  data_objectsc...
-00000c90: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000ca0: 000b 0000 0073 2400 0000 7400 8801 6a01  .....s$...t...j.
-00000cb0: 8301 7d02 8700 8701 6602 6401 6402 8408  ..}.....f.d.d...
-00000cc0: 7c02 4400 8301 8801 5f02 6400 5300 2903  |.D....._.d.S.).
-00000cd0: 4e63 0100 0000 0000 0000 0000 0000 0300  Nc..............
-00000ce0: 0000 0600 0000 1300 0000 7324 0000 0067  ..........s$...g
-00000cf0: 007c 005d 0e5c 027d 017d 0274 0088 017c  .|.].\.}.}.t...|
-00000d00: 027c 0166 0369 0088 00a4 018e 0191 0271  .|.f.i.........q
-00000d10: 0253 0072 1300 0000 7205 0000 0029 0372  .S.r....r....).r
-00000d20: 1b00 0000 da05 696e 6465 78da 1164 6174  ......index..dat
-00000d30: 615f 6f62 6a65 6374 5f67 726f 7570 a902  a_object_group..
-00000d40: 720d 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000d50: 1400 0000 721d 0000 004c 0000 0073 0600  ....r....L...s..
-00000d60: 0000 0600 0601 18ff 7a2e 4669 6775 7265  ........z.Figure
-00000d70: 732e 7365 745f 6669 6775 7265 5f6f 626a  s.set_figure_obj
-00000d80: 6563 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c  ects.<locals>.<l
-00000d90: 6973 7463 6f6d 703e 2903 da09 656e 756d  istcomp>)...enum
-00000da0: 6572 6174 6572 3a00 0000 723d 0000 0029  erater:...r=...)
-00000db0: 0372 1200 0000 720d 0000 00da 1164 6174  .r....r......dat
-00000dc0: 615f 6f62 6a5f 6974 6572 6162 6c65 7213  a_obj_iterabler.
-00000dd0: 0000 0072 4200 0000 7214 0000 0072 3c00  ...rB...r....r<.
-00000de0: 0000 4a00 0000 7308 0000 000a 010c 0102  ..J...s.........
-00000df0: 010c ff7a 1a46 6967 7572 6573 2e73 6574  ...z.Figures.set
-00000e00: 5f66 6967 7572 655f 6f62 6a65 6374 734e  _figure_objectsN
-00000e10: 2901 722c 0000 0029 0fda 085f 5f6e 616d  ).r,...)...__nam
-00000e20: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000e30: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1500  .__qualname__r..
-00000e40: 0000 720e 0000 0072 1900 0000 7220 0000  ..r....r....r ..
-00000e50: 0072 2700 0000 7225 0000 0072 2a00 0000  .r'...r%...r*...
-00000e60: 722d 0000 0072 2e00 0000 7224 0000 0072  r-...r....r$...r
-00000e70: 2600 0000 723c 0000 0072 1300 0000 7213  &...r<...r....r.
-00000e80: 0000 0072 1300 0000 7214 0000 0072 0b00  ...r....r....r..
-00000e90: 0000 0d00 0000 731a 0000 0008 0008 0208  ......s.........
-00000ea0: 0508 0608 0708 0808 050a 0408 0408 0408  ................
-00000eb0: 0508 060c 0572 0b00 0000 2911 7232 0000  .....r....).r2..
-00000ec0: 0072 3400 0000 da05 6e75 6d70 7972 1700  .r4.....numpyr..
-00000ed0: 0000 da00 7203 0000 00da 0666 6967 7572  ....r......figur
-00000ee0: 6572 0600 0000 da0e 6461 7461 7479 7065  er......datatype
-00000ef0: 732e 6461 7461 7207 0000 00da 0c75 7469  s.datar......uti
-00000f00: 6c73 2e67 726f 7570 7372 0800 0000 7209  ls.groupsr....r.
-00000f10: 0000 00da 0b75 7469 6c73 2e70 6174 6873  .....utils.paths
-00000f20: 720a 0000 0072 0b00 0000 da04 6c6f 6164  r....r......load
-00000f30: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-00000f40: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000f50: 0000 7316 0000 0008 0008 0108 020c 020c  ..s.............
-00000f60: 010c 010c 010c 010c 010e 020e 42         ............B
+000007b0: 6f75 7470 7574 da0d 7365 745f 6261 7365  output..set_base
+000007c0: 5f70 6174 68a9 0172 1200 0000 7213 0000  _path..r....r...
+000007d0: 0072 1300 0000 7214 0000 0072 2500 0000  .r....r....r%...
+000007e0: 2e00 0000 7306 0000 000a 010c 0104 ff7a  ....s..........z
+000007f0: 1b46 6967 7572 6573 2e70 726f 6365 7373  .Figures.process
+00000800: 5f6f 7574 7075 745f 6d6f 6465 da05 506c  _output_mode..Pl
+00000810: 6f74 7363 0200 0000 0000 0000 0000 0000  otsc............
+00000820: 0200 0000 0300 0000 4300 0000 7316 0000  ........C...s...
+00000830: 007c 00a0 00a1 0001 007c 00a0 017c 01a1  .|.......|...|..
+00000840: 0101 0064 0053 0072 0c00 0000 2902 da15  ...d.S.r....)...
+00000850: 7365 745f 6465 6661 756c 745f 6261 7365  set_default_base
+00000860: 5f70 6174 68da 1573 706c 6974 5f6f 6e5f  _path..split_on_
+00000870: 706c 6f74 735f 666f 6c64 6572 a902 7212  plots_folder..r.
+00000880: 0000 00da 1170 6c6f 7473 5f66 6f6c 6465  .....plots_folde
+00000890: 725f 6e61 6d65 7213 0000 0072 1300 0000  r_namer....r....
+000008a0: 7214 0000 0072 2a00 0000 3200 0000 7304  r....r*...2...s.
+000008b0: 0000 0008 010e 017a 1546 6967 7572 6573  .......z.Figures
+000008c0: 2e73 6574 5f62 6173 655f 7061 7468 6301  .set_base_pathc.
+000008d0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000008e0: 0000 0043 0000 0073 2600 0000 7c00 6a00  ...C...s&...|.j.
+000008f0: 6400 7500 7211 7401 6a02 a003 7404 6a05  d.u.r.t.j...t.j.
+00000900: a101 6401 1900 7c00 5f00 6400 5300 6400  ..d...|._.d.S.d.
+00000910: 5300 2902 4e72 0100 0000 2906 da09 6261  S.).Nr....)...ba
+00000920: 7365 5f70 6174 68da 026f 73da 0470 6174  se_path..os..pat
+00000930: 68da 0573 706c 6974 da08 5f5f 6d61 696e  h..split..__main
+00000940: 5f5f da08 5f5f 6669 6c65 5f5f 722b 0000  __..__file__r+..
+00000950: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000960: 722d 0000 0036 0000 0073 0600 0000 0a01  r-...6...s......
+00000970: 1801 04ff 7a1d 4669 6775 7265 732e 7365  ....z.Figures.se
+00000980: 745f 6465 6661 756c 745f 6261 7365 5f70  t_default_base_p
+00000990: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
+000009a0: 0200 0000 0400 0000 4300 0000 732a 0000  ........C...s*..
+000009b0: 007c 006a 0072 1374 016a 02a0 037c 006a  .|.j.r.t.j...|.j
+000009c0: 047c 01a1 027c 005f 0474 057c 006a 0483  .|...|._.t.|.j..
+000009d0: 0101 0064 0053 0064 0053 0072 0c00 0000  ...d.S.d.S.r....
+000009e0: 2906 da0c 706c 6f74 735f 666f 6c64 6572  )...plots_folder
+000009f0: 7232 0000 0072 3300 0000 da04 6a6f 696e  r2...r3.....join
+00000a00: 7231 0000 0072 0a00 0000 722f 0000 0072  r1...r....r/...r
+00000a10: 1300 0000 7213 0000 0072 1400 0000 722e  ....r....r....r.
+00000a20: 0000 003a 0000 0073 0800 0000 0601 1201  ...:...s........
+00000a30: 0e01 04fe 7a1d 4669 6775 7265 732e 7370  ....z.Figures.sp
+00000a40: 6c69 745f 6f6e 5f70 6c6f 7473 5f66 6f6c  lit_on_plots_fol
+00000a50: 6465 7263 0100 0000 0000 0000 0000 0000  derc............
+00000a60: 0200 0000 0300 0000 0300 0000 7336 0000  ............s6..
+00000a70: 0074 0088 006a 0188 006a 0283 0288 005f  .t...j...j....._
+00000a80: 0174 0388 006a 0488 006a 0183 027d 0187  .t...j...j...}..
+00000a90: 0066 0164 0164 0284 087c 0144 0083 0188  .f.d.d...|.D....
+00000aa0: 005f 0564 0053 0029 034e 6301 0000 0000  ._.d.S.).Nc.....
+00000ab0: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00000ac0: 0000 0073 1600 0000 6700 7c00 5d07 7d01  ...s....g.|.].}.
+00000ad0: 8800 6a00 7c01 1900 9102 7102 5300 7213  ..j.|.....q.S.r.
+00000ae0: 0000 0029 0172 0f00 0000 2902 721b 0000  ...).r....).r...
+00000af0: 00da 0769 6e64 6578 6573 722b 0000 0072  ...indexesr+...r
+00000b00: 1300 0000 7214 0000 0072 1d00 0000 4200  ....r....r....B.
+00000b10: 0000 721e 0000 007a 3046 6967 7572 6573  ..r....z0Figures
+00000b20: 2e70 726f 6365 7373 5f64 6174 615f 6f62  .process_data_ob
+00000b30: 6a65 6374 732e 3c6c 6f63 616c 733e 2e3c  jects.<locals>.<
+00000b40: 6c69 7374 636f 6d70 3e29 0672 0900 0000  listcomp>).r....
+00000b50: da08 7375 6270 6c6f 7473 720f 0000 0072  ..subplotsr....r
+00000b60: 0800 0000 7211 0000 00da 1264 6174 615f  ....r......data_
+00000b70: 6f62 6a65 6374 5f67 726f 7570 7329 0272  object_groups).r
+00000b80: 1200 0000 da0d 6772 6f75 705f 696e 6465  ......group_inde
+00000b90: 7865 7372 1300 0000 722b 0000 0072 1400  xesr....r+...r..
+00000ba0: 0000 7224 0000 003f 0000 0073 0a00 0000  ..r$...?...s....
+00000bb0: 1001 0e01 0a01 0201 0cff 7a1c 4669 6775  ..........z.Figu
+00000bc0: 7265 732e 7072 6f63 6573 735f 6461 7461  res.process_data
+00000bd0: 5f6f 626a 6563 7473 6301 0000 0000 0000  _objectsc.......
+00000be0: 0000 0000 0003 0000 0004 0000 004b 0000  .............K..
+00000bf0: 0073 2800 0000 7c00 6a00 6401 6900 7c01  .s(...|.j.d.i.|.
+00000c00: a401 8e01 0100 7c00 6a01 4400 5d06 7d02  ......|.j.D.].}.
+00000c10: 7c02 a002 a100 0100 710b 6400 5300 7223  |.......q.d.S.r#
+00000c20: 0000 0029 03da 1273 6574 5f66 6967 7572  ...)...set_figur
+00000c30: 655f 6f62 6a65 6374 73da 0e66 6967 7572  e_objects..figur
+00000c40: 655f 6f62 6a65 6374 73da 0d63 7265 6174  e_objects..creat
+00000c50: 655f 6669 6775 7265 2903 7212 0000 0072  e_figure).r....r
+00000c60: 0d00 0000 da0a 6669 6775 7265 5f6f 626a  ......figure_obj
+00000c70: 7213 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000c80: 2600 0000 4500 0000 7308 0000 0010 010a  &...E...s.......
+00000c90: 010a 0104 ff7a 1946 6967 7572 6573 2e70  .....z.Figures.p
+00000ca0: 6c6f 745f 6461 7461 5f6f 626a 6563 7473  lot_data_objects
+00000cb0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00000cc0: 0003 0000 000b 0000 0073 2400 0000 7400  .........s$...t.
+00000cd0: 8801 6a01 8301 7d02 8700 8701 6602 6401  ..j...}.....f.d.
+00000ce0: 6402 8408 7c02 4400 8301 8801 5f02 6400  d...|.D....._.d.
+00000cf0: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000d00: 0000 0300 0000 0600 0000 1300 0000 7324  ..............s$
+00000d10: 0000 0067 007c 005d 0e5c 027d 017d 0274  ...g.|.].\.}.}.t
+00000d20: 0088 017c 027c 0166 0369 0088 00a4 018e  ...|.|.f.i......
+00000d30: 0191 0271 0253 0072 1300 0000 7205 0000  ...q.S.r....r...
+00000d40: 0029 0372 1b00 0000 da05 696e 6465 78da  .).r......index.
+00000d50: 1164 6174 615f 6f62 6a65 6374 5f67 726f  .data_object_gro
+00000d60: 7570 a902 720d 0000 0072 1200 0000 7213  up..r....r....r.
+00000d70: 0000 0072 1400 0000 721d 0000 004c 0000  ...r....r....L..
+00000d80: 0073 0600 0000 0600 0601 18ff 7a2e 4669  .s..........z.Fi
+00000d90: 6775 7265 732e 7365 745f 6669 6775 7265  gures.set_figure
+00000da0: 5f6f 626a 6563 7473 2e3c 6c6f 6361 6c73  _objects.<locals
+00000db0: 3e2e 3c6c 6973 7463 6f6d 703e 2903 da09  >.<listcomp>)...
+00000dc0: 656e 756d 6572 6174 6572 3b00 0000 723e  enumerater;...r>
+00000dd0: 0000 0029 0372 1200 0000 720d 0000 00da  ...).r....r.....
+00000de0: 1164 6174 615f 6f62 6a5f 6974 6572 6162  .data_obj_iterab
+00000df0: 6c65 7213 0000 0072 4300 0000 7214 0000  ler....rC...r...
+00000e00: 0072 3d00 0000 4a00 0000 7308 0000 000a  .r=...J...s.....
+00000e10: 010c 0102 010c ff7a 1a46 6967 7572 6573  .......z.Figures
+00000e20: 2e73 6574 5f66 6967 7572 655f 6f62 6a65  .set_figure_obje
+00000e30: 6374 734e 2901 722c 0000 0029 0fda 085f  ctsN).r,...)..._
+00000e40: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000e50: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000e60: 5f72 1500 0000 720e 0000 0072 1900 0000  _r....r....r....
+00000e70: 7220 0000 0072 2700 0000 7225 0000 0072  r ...r'...r%...r
+00000e80: 2a00 0000 722d 0000 0072 2e00 0000 7224  *...r-...r....r$
+00000e90: 0000 0072 2600 0000 723d 0000 0072 1300  ...r&...r=...r..
+00000ea0: 0000 7213 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000eb0: 0072 0b00 0000 0d00 0000 731a 0000 0008  .r........s.....
+00000ec0: 0008 0208 0508 0608 0708 0808 050a 0408  ................
+00000ed0: 0408 0408 0508 060c 0572 0b00 0000 2911  .........r....).
+00000ee0: 7232 0000 0072 3500 0000 da05 6e75 6d70  r2...r5.....nump
+00000ef0: 7972 1700 0000 da00 7203 0000 00da 0666  yr......r......f
+00000f00: 6967 7572 6572 0600 0000 da0e 6461 7461  igurer......data
+00000f10: 7479 7065 732e 6461 7461 7207 0000 00da  types.datar.....
+00000f20: 0c75 7469 6c73 2e67 726f 7570 7372 0800  .utils.groupsr..
+00000f30: 0000 7209 0000 00da 0b75 7469 6c73 2e70  ..r......utils.p
+00000f40: 6174 6873 720a 0000 0072 0b00 0000 da04  athsr....r......
+00000f50: 6c6f 6164 7213 0000 0072 1300 0000 7213  loadr....r....r.
+00000f60: 0000 0072 1400 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000f70: 653e 0100 0000 7316 0000 0008 0008 0108  e>....s.........
+00000f80: 020c 020c 010c 010c 010c 010c 010e 020e  ................
+00000f90: 42                                       B
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/animate.py` & `hgutilities-1.0.8.6/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Data.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Data.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Line.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Data.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Data.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/figure.py` & `hgutilities-1.0.8.6/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/figures.py` & `hgutilities-1.0.8.6/hgutilities/plotting/figures.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,28 +41,28 @@
     def create_figures(self, **kwargs):
         self.process_data_objects()
         self.process_output_mode()
         self.plot_data_objects(**kwargs)
 
     def process_output_mode(self):
         if self.output == "Save":
-            self.set_path()
+            self.set_base_path()
 
-    def set_path(self, plots_folder_name="Plots"):
-        self.set_default_path()
+    def set_base_path(self, plots_folder_name="Plots"):
+        self.set_default_base_path()
         self.split_on_plots_folder(plots_folder_name)
 
-    def set_default_path(self):
-        if self.path is None:
-            self.path = os.path.split(__main__.__file__)[0]
+    def set_default_base_path(self):
+        if self.base_path is None:
+            self.base_path = os.path.split(__main__.__file__)[0]
 
     def split_on_plots_folder(self, plots_folder_name):
         if self.plots_folder:
-            self.path = os.path.join(self.path, plots_folder_name)
-            make_folder(self.path)
+            self.base_path = os.path.join(self.base_path, plots_folder_name)
+            make_folder(self.base_path)
 
     def process_data_objects(self):
         self.subplots = get_group_size(self.subplots, self.data_objects)
         group_indexes = get_group_indexes(self.data_obj_count, self.subplots)
         self.data_object_groups = [self.data_objects[indexes]
                                     for indexes in group_indexes]
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 20:09:06 2023 UTC, .py size: 4054 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,275 +1,333 @@
-00000000: 6f0d 0d0a 0000 0000 6264 8f64 d60f 0000  o.......bd.d....
+00000000: 6f0d 0d0a 0000 0000 0e55 9064 8513 0000  o........U.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 5a04 6400 6401 6c05 5a06 6402 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000050: 6d08 5a08 0100 6402 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 8302 5a0b  ..G.d.d...d...Z.
 00000070: 6508 a00c 650b a101 0100 6401 5300 2907  e...e.....d.S.).
 00000080: e900 0000 004e e903 0000 0029 01da 0864  .....N.....)...d
 00000090: 6566 6175 6c74 7329 01da 1272 656d 6f76  efaults)...remov
 000000a0: 655f 6e6f 6e65 5f76 616c 7565 7363 0000  e_none_valuesc..
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000000c0: 0000 4000 0000 73a0 0000 0065 005a 0164  ..@...s....e.Z.d
+000000c0: 0000 4000 0000 73d0 0000 0065 005a 0164  ..@...s....e.Z.d
 000000d0: 005a 0265 0364 0164 0284 0083 015a 0464  .Z.e.d.d.....Z.d
 000000e0: 0364 0484 005a 0564 0564 0684 005a 0664  .d...Z.d.d...Z.d
 000000f0: 0764 0884 005a 0764 0964 0a84 005a 0864  .d...Z.d.d...Z.d
 00000100: 0b64 0c84 005a 0964 0d64 0e84 005a 0a64  .d...Z.d.d...Z.d
 00000110: 0f64 1084 005a 0b64 1164 1284 005a 0c64  .d...Z.d.d...Z.d
 00000120: 1364 1484 005a 0d64 1564 1684 005a 0e64  .d...Z.d.d...Z.d
 00000130: 1764 1884 005a 0f64 1964 1a84 005a 1064  .d...Z.d.d...Z.d
 00000140: 1b64 1c84 005a 1164 1d64 1e84 005a 1264  .d...Z.d.d...Z.d
 00000150: 1f64 2084 005a 1364 2164 2284 005a 1464  .d ..Z.d!d"..Z.d
-00000160: 2364 2484 005a 1564 2553 0029 26da 0450  #d$..Z.d%S.)&..P
-00000170: 6c6f 7463 0100 0000 0000 0000 0000 0000  lotc............
-00000180: 0100 0000 0100 0000 4300 0000 f304 0000  ........C.......
-00000190: 0064 0053 00a9 014e a900 2901 da03 636c  .d.S...N..)...cl
-000001a0: 7372 0800 0000 7208 0000 00fa 642f 6d6e  sr....r.....d/mn
-000001b0: 742f 3254 422f 446f 6375 6d65 6e74 732f  t/2TB/Documents/
-000001c0: 5079 7468 6f6e 2f52 6561 6c20 576f 726c  Python/Real Worl
-000001d0: 6420 4170 706c 6963 6174 696f 6e73 2f68  d Applications/h
-000001e0: 6775 7469 6c69 7469 6573 2f68 6775 7469  gutilities/hguti
-000001f0: 6c69 7469 6573 2f70 6c6f 7474 696e 672f  lities/plotting/
-00000200: 706c 6f74 7479 7065 732f 706c 6f74 2e70  plottypes/plot.p
-00000210: 79da 1173 6574 5f66 756e 6374 696f 6e5f  y..set_function_
-00000220: 6469 6374 0a00 0000 7302 0000 0004 027a  dict....s......z
-00000230: 1650 6c6f 742e 7365 745f 6675 6e63 7469  .Plot.set_functi
-00000240: 6f6e 5f64 6963 7463 0400 0000 0000 0000  on_dictc........
-00000250: 0000 0000 0500 0000 0400 0000 4b00 0000  ............K...
-00000260: 732e 0000 007c 00a0 007c 01a1 0101 007c  s....|...|.....|
-00000270: 027c 005f 017c 037c 005f 0274 03a0 047c  .|._.|.|._.t...|
-00000280: 007c 04a1 0201 007c 00a0 05a1 0001 0064  .|.....|.......d
-00000290: 0053 0072 0700 0000 2906 da0e 7365 745f  .S.r....)...set_
-000002a0: 6669 6775 7265 5f6f 626a da02 6178 da08  figure_obj..ax..
-000002b0: 6461 7461 5f6f 626a 7203 0000 00da 066b  data_objr......k
-000002c0: 7761 7267 73da 0a73 6574 5f6b 7761 7267  wargs..set_kwarg
-000002d0: 7329 05da 0473 656c 66da 0a66 6967 7572  s)...self..figur
-000002e0: 655f 6f62 6a72 0d00 0000 720e 0000 0072  e_objr....r....r
-000002f0: 0f00 0000 7208 0000 0072 0800 0000 720a  ....r....r....r.
-00000300: 0000 00da 085f 5f69 6e69 745f 5f0e 0000  .....__init__...
-00000310: 0073 0a00 0000 0a01 0601 0601 0c01 0c01  .s..............
-00000320: 7a0d 506c 6f74 2e5f 5f69 6e69 745f 5f63  z.Plot.__init__c
-00000330: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000340: 0200 0000 4300 0000 f314 0000 007c 00a0  ....C........|..
-00000350: 00a1 0001 007c 00a0 01a1 0001 0064 0053  .....|.......d.S
-00000360: 0072 0700 0000 2902 da0e 696e 6865 7269  .r....)...inheri
-00000370: 745f 6b77 6172 6773 da0f 7365 745f 666f  t_kwargs..set_fo
-00000380: 6e74 5f6b 7761 7267 73a9 0172 1100 0000  nt_kwargs..r....
-00000390: 7208 0000 0072 0800 0000 720a 0000 0072  r....r....r....r
-000003a0: 1000 0000 1500 0000 f304 0000 0008 010c  ................
-000003b0: 017a 0f50 6c6f 742e 7365 745f 6b77 6172  .z.Plot.set_kwar
-000003c0: 6773 6301 0000 0000 0000 0000 0000 0002  gsc.............
-000003d0: 0000 0005 0000 0043 0000 0073 1e00 0000  .......C...s....
-000003e0: 6700 6401 a201 7d01 7400 a001 7c00 6a02  g.d...}.t...|.j.
-000003f0: 7c00 6a03 7c01 a103 0100 6400 5300 2902  |.j.|.....d.S.).
-00000400: 4e29 10da 0e74 6974 6c65 5f66 6f6e 746e  N)...title_fontn
-00000410: 616d 65da 0e74 6974 6c65 5f66 6f6e 7473  ame..title_fonts
-00000420: 697a 65da 0b74 6974 6c65 5f63 6f6c 6f72  ize..title_color
-00000430: da17 7469 746c 655f 7665 7274 6963 616c  ..title_vertical
-00000440: 616c 6967 6e6d 656e 74da 1974 6974 6c65  alignment..title
-00000450: 5f68 6f72 697a 6f6e 7461 6c61 6c69 676e  _horizontalalign
-00000460: 6d65 6e74 da07 7469 746c 655f 79da 0974  ment..title_y..t
-00000470: 6974 6c65 5f70 6164 da09 7469 746c 655f  itle_pad..title_
-00000480: 6c6f 63da 0d61 7869 735f 666f 6e74 6e61  loc..axis_fontna
-00000490: 6d65 da0d 6178 6973 5f66 6f6e 7473 697a  me..axis_fontsiz
-000004a0: 65da 0a61 7869 735f 636f 6c6f 72da 0d61  e..axis_color..a
-000004b0: 7869 735f 6c61 6265 6c70 6164 da08 6178  xis_labelpad..ax
-000004c0: 6973 5f6c 6f63 da0f 785f 6178 6973 5f72  is_loc..x_axis_r
-000004d0: 6f74 6174 696f 6eda 0f79 5f61 7869 735f  otation..y_axis_
-000004e0: 726f 7461 7469 6f6e da0f 7a5f 6178 6973  rotation..z_axis
-000004f0: 5f72 6f74 6174 696f 6e29 0472 0300 0000  _rotation).r....
-00000500: da07 696e 6865 7269 7472 0e00 0000 7212  ..inheritr....r.
-00000510: 0000 0029 0272 1100 0000 da0a 6174 7472  ...).r......attr
-00000520: 6962 7574 6573 7208 0000 0072 0800 0000  ibutesr....r....
-00000530: 720a 0000 0072 1500 0000 1900 0000 7304  r....r........s.
-00000540: 0000 0008 0116 077a 1350 6c6f 742e 696e  .......z.Plot.in
-00000550: 6865 7269 745f 6b77 6172 6773 6301 0000  herit_kwargsc...
-00000560: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000570: 0043 0000 0072 1400 0000 7207 0000 0029  .C...r....r....)
-00000580: 02da 1273 6574 5f74 6974 6c65 5f66 6f6e  ...set_title_fon
-00000590: 7464 6963 74da 1173 6574 5f61 7869 735f  tdict..set_axis_
-000005a0: 666f 6e74 6469 6374 7217 0000 0072 0800  fontdictr....r..
-000005b0: 0000 7208 0000 0072 0a00 0000 7216 0000  ..r....r....r...
-000005c0: 0023 0000 0072 1800 0000 7a14 506c 6f74  .#...r....z.Plot
-000005d0: 2e73 6574 5f66 6f6e 745f 6b77 6172 6773  .set_font_kwargs
-000005e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000005f0: 0006 0000 0043 0000 0073 3200 0000 7c00  .....C...s2...|.
-00000600: 6a00 6a01 7c00 6a00 6a02 7c00 6a00 6a03  j.j.|.j.j.|.j.j.
-00000610: 7c00 6a00 6a04 7c00 6a00 6a05 6401 9c05  |.j.j.|.j.j.d...
-00000620: 7d01 7406 7c01 8301 7c00 5f07 6400 5300  }.t.|...|._.d.S.
-00000630: 2902 4e29 05da 0866 6f6e 746e 616d 65da  ).N)...fontname.
-00000640: 0866 6f6e 7473 697a 65da 0563 6f6c 6f72  .fontsize..color
-00000650: da11 7665 7274 6963 616c 616c 6967 6e6d  ..verticalalignm
-00000660: 656e 74da 1368 6f72 697a 6f6e 7461 6c61  ent..horizontala
-00000670: 6c69 676e 6d65 6e74 2908 720e 0000 0072  lignment).r....r
-00000680: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00000690: 0000 0072 1d00 0000 7204 0000 00da 0e74  ...r....r......t
-000006a0: 6974 6c65 5f66 6f6e 7464 6963 74a9 0272  itle_fontdict..r
-000006b0: 1100 0000 720f 0000 0072 0800 0000 7208  ....r....r....r.
-000006c0: 0000 0072 0a00 0000 722b 0000 0027 0000  ...r....r+...'..
-000006d0: 0073 0e00 0000 0601 0601 0601 0601 0601  .s..............
-000006e0: 06fc 0e05 7a17 506c 6f74 2e73 6574 5f74  ....z.Plot.set_t
-000006f0: 6974 6c65 5f66 6f6e 7464 6963 7463 0100  itle_fontdictc..
-00000700: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000710: 0000 4300 0000 7326 0000 007c 006a 006a  ..C...s&...|.j.j
-00000720: 017c 006a 006a 027c 006a 006a 0364 019c  .|.j.j.|.j.j.d..
-00000730: 037d 0174 047c 0183 017c 005f 0564 0053  .}.t.|...|._.d.S
-00000740: 0029 024e 2903 722d 0000 0072 2e00 0000  .).N).r-...r....
-00000750: 722f 0000 0029 0672 0e00 0000 7221 0000  r/...).r....r!..
-00000760: 0072 2200 0000 7223 0000 0072 0400 0000  .r"...r#...r....
-00000770: da0d 6178 6973 5f66 6f6e 7464 6963 7472  ..axis_fontdictr
-00000780: 3300 0000 7208 0000 0072 0800 0000 720a  3...r....r....r.
-00000790: 0000 0072 2c00 0000 2f00 0000 730a 0000  ...r,.../...s...
-000007a0: 0006 0106 0106 0106 fe0e 037a 1650 6c6f  ...........z.Plo
-000007b0: 742e 7365 745f 6178 6973 5f66 6f6e 7464  t.set_axis_fontd
-000007c0: 6963 7463 0200 0000 0000 0000 0000 0000  ictc............
-000007d0: 0200 0000 0200 0000 4300 0000 7312 0000  ........C...s...
-000007e0: 007c 017c 005f 007c 016a 017c 005f 0164  .|.|._.|.j.|._.d
-000007f0: 0053 0072 0700 0000 2902 7212 0000 00da  .S.r....).r.....
-00000800: 0b66 6967 7572 6573 5f6f 626a 2902 7211  .figures_obj).r.
-00000810: 0000 0072 1200 0000 7208 0000 0072 0800  ...r....r....r..
-00000820: 0000 720a 0000 0072 0c00 0000 3500 0000  ..r....r....5...
-00000830: 7304 0000 0006 010c 017a 1350 6c6f 742e  s........z.Plot.
-00000840: 7365 745f 6669 6775 7265 5f6f 626a 6301  set_figure_objc.
-00000850: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000860: 0000 0043 0000 0073 2400 0000 7c00 a000  ...C...s$...|...
-00000870: a100 0100 7c00 a001 a100 0100 7c00 a002  ....|.......|...
-00000880: a100 0100 7c00 a003 a100 0100 6400 5300  ....|.......d.S.
-00000890: 7207 0000 0029 04da 0970 6c6f 745f 6461  r....)...plot_da
-000008a0: 7461 da09 7365 745f 7469 746c 65da 0a61  ta..set_title..a
-000008b0: 6464 5f6c 6567 656e 64da 0f61 6464 5f61  dd_legend..add_a
-000008c0: 7869 735f 6c61 6265 6c73 7217 0000 0072  xis_labelsr....r
-000008d0: 0800 0000 7208 0000 0072 0a00 0000 da0b  ....r....r......
-000008e0: 6372 6561 7465 5f70 6c6f 7439 0000 0073  create_plot9...s
-000008f0: 0800 0000 0801 0801 0801 0c01 7a10 506c  ............z.Pl
-00000900: 6f74 2e63 7265 6174 655f 706c 6f74 6301  ot.create_plotc.
-00000910: 0000 0000 0000 0000 0000 0001 0000 0007  ................
-00000920: 0000 0043 0000 0073 4600 0000 7c00 6a00  ...C...sF...|.j.
-00000930: 6a01 6400 7501 7221 7c00 6a02 6a03 7c00  j.d.u.r!|.j.j.|.
-00000940: 6a00 6a01 6601 6900 7c00 6a04 a401 7c00  j.j.f.i.|.j...|.
-00000950: 6a00 6a05 7c00 6a00 6a06 7c00 6a00 6a07  j.j.|.j.j.|.j.j.
-00000960: 6401 9c03 a401 8e01 0100 6400 5300 6400  d.........d.S.d.
-00000970: 5300 2902 4e29 03da 036c 6f63 da01 79da  S.).N)...loc..y.
-00000980: 0370 6164 2908 720e 0000 00da 0574 6974  .pad).r......tit
-00000990: 6c65 720d 0000 0072 3700 0000 7232 0000  ler....r7...r2..
-000009a0: 0072 2000 0000 721e 0000 0072 1f00 0000  .r ...r....r....
-000009b0: 7217 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-000009c0: 0a00 0000 7237 0000 003f 0000 0073 0c00  ....r7...?...s..
-000009d0: 0000 0c01 1601 0c01 0601 0efe 04ff 7a0e  ..............z.
-000009e0: 506c 6f74 2e73 6574 5f74 6974 6c65 6301  Plot.set_titlec.
-000009f0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000a00: 0000 0043 0000 0073 2e00 0000 7c00 6a00  ...C...s....|.j.
-00000a10: 6a01 7313 7c00 6a02 6a03 7215 7c00 6a04  j.s.|.j.j.r.|.j.
-00000a20: 6a03 7c00 6a02 6a05 6401 8d01 0100 6400  j.|.j.j.d.....d.
-00000a30: 5300 6400 5300 6400 5300 2902 4e29 0172  S.d.S.d.S.).N).r
-00000a40: 3b00 0000 2906 7235 0000 00da 1075 6e69  ;...).r5.....uni
-00000a50: 7665 7273 616c 5f6c 6567 656e 6472 0e00  versal_legendr..
-00000a60: 0000 da06 6c65 6765 6e64 720d 0000 00da  ....legendr.....
-00000a70: 0a6c 6567 656e 645f 6c6f 6372 1700 0000  .legend_locr....
-00000a80: 7208 0000 0072 0800 0000 720a 0000 0072  r....r....r....r
-00000a90: 3800 0000 4500 0000 730a 0000 0008 0108  8...E...s.......
-00000aa0: 0116 0104 fe04 017a 0f50 6c6f 742e 6164  .......z.Plot.ad
-00000ab0: 645f 6c65 6765 6e64 6301 0000 0000 0000  d_legendc.......
-00000ac0: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00000ad0: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000ae0: 7217 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00000af0: 0a00 0000 7239 0000 004a 0000 0073 0200  ....r9...J...s..
-00000b00: 0000 0401 7a14 506c 6f74 2e61 6464 5f61  ....z.Plot.add_a
-00000b10: 7869 735f 6c61 6265 6c73 6301 0000 0000  xis_labelsc.....
-00000b20: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00000b30: 0000 00f3 2e00 0000 7c00 6a00 6a01 6400  ........|.j.j.d.
-00000b40: 7501 7215 7c00 6a02 6a03 7c00 6a00 6a01  u.r.|.j.j.|.j.j.
-00000b50: 6601 6900 7c00 6a04 a401 8e01 0100 6400  f.i.|.j.......d.
-00000b60: 5300 6400 5300 7207 0000 0029 0572 0e00  S.d.S.r....).r..
-00000b70: 0000 da07 785f 6c61 6265 6c72 0d00 0000  ....x_labelr....
-00000b80: da0a 7365 745f 786c 6162 656c 7234 0000  ..set_xlabelr4..
-00000b90: 0072 1700 0000 7208 0000 0072 0800 0000  .r....r....r....
-00000ba0: 720a 0000 00da 0b61 6464 5f78 5f6c 6162  r......add_x_lab
-00000bb0: 656c 4d00 0000 f30a 0000 000c 0110 0104  elM.............
-00000bc0: 010a ff04 ff7a 1050 6c6f 742e 6164 645f  .....z.Plot.add_
-00000bd0: 785f 6c61 6265 6c63 0100 0000 0000 0000  x_labelc........
-00000be0: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000bf0: 7242 0000 0072 0700 0000 2905 720e 0000  rB...r....).r...
-00000c00: 00da 0779 5f6c 6162 656c 720d 0000 00da  ...y_labelr.....
-00000c10: 0a73 6574 5f79 6c61 6265 6c72 3400 0000  .set_ylabelr4...
-00000c20: 7217 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00000c30: 0a00 0000 da0b 6164 645f 795f 6c61 6265  ......add_y_labe
-00000c40: 6c52 0000 0072 4600 0000 7a10 506c 6f74  lR...rF...z.Plot
-00000c50: 2e61 6464 5f79 5f6c 6162 656c 6301 0000  .add_y_labelc...
-00000c60: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000c70: 0043 0000 0072 4200 0000 7207 0000 0029  .C...rB...r....)
-00000c80: 0572 0e00 0000 da07 7a5f 6c61 6265 6c72  .r......z_labelr
-00000c90: 0d00 0000 da0a 7365 745f 7a6c 6162 656c  ......set_zlabel
-00000ca0: 7234 0000 0072 1700 0000 7208 0000 0072  r4...r....r....r
-00000cb0: 0800 0000 720a 0000 00da 0b61 6464 5f7a  ....r......add_z
-00000cc0: 5f6c 6162 656c 5700 0000 7246 0000 007a  _labelW...rF...z
-00000cd0: 1050 6c6f 742e 6164 645f 7a5f 6c61 6265  .Plot.add_z_labe
-00000ce0: 6c63 0100 0000 0000 0000 0000 0000 0100  lc..............
-00000cf0: 0000 0200 0000 4300 0000 7214 0000 0072  ......C...r....r
-00000d00: 0700 0000 2902 da11 7365 745f 785f 7469  ....)...set_x_ti
-00000d10: 636b 5f6c 6162 656c 73da 1173 6574 5f79  ck_labels..set_y
-00000d20: 5f74 6963 6b5f 6c61 6265 6c73 7217 0000  _tick_labelsr...
-00000d30: 0072 0800 0000 7208 0000 0072 0a00 0000  .r....r....r....
-00000d40: da0f 7365 745f 7469 636b 5f6c 6162 656c  ..set_tick_label
-00000d50: 735c 0000 0072 1800 0000 7a14 506c 6f74  s\...r....z.Plot
-00000d60: 2e73 6574 5f74 6963 6b5f 6c61 6265 6c73  .set_tick_labels
-00000d70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000d80: 0007 0000 0043 0000 0073 4e00 0000 7400  .....C...sN...t.
-00000d90: 7c00 6a01 6401 8302 7225 7402 7c00 6a03  |.j.d...r%t.|.j.
-00000da0: 6a04 8301 0100 7c00 6a01 6a05 7c00 6a01  j.....|.j.j.|.j.
-00000db0: a006 a100 7c00 6a01 a007 a100 7c00 6a03  ....|.j.....|.j.
-00000dc0: 6a08 7c00 6a03 6a04 7c00 6a03 6a09 6402  j.|.j.j.|.j.j.d.
-00000dd0: 8d05 0100 6400 5300 6400 5300 2903 4eda  ....d.S.d.S.).N.
-00000de0: 0a73 6574 5f78 7469 636b 73a9 03da 0872  .set_xticks....r
-00000df0: 6f74 6174 696f 6eda 0268 61da 0276 6129  otation..ha..va)
-00000e00: 0ada 0768 6173 6174 7472 720d 0000 00da  ...hasattrr.....
-00000e10: 0570 7269 6e74 720e 0000 00da 0478 5f68  .printr......x_h
-00000e20: 6172 5000 0000 da0a 6765 745f 7874 6963  arP.....get_xtic
-00000e30: 6b73 da0f 6765 745f 7874 6963 6b6c 6162  ks..get_xticklab
-00000e40: 656c 73da 0a78 5f72 6f74 6174 696f 6eda  els..x_rotation.
-00000e50: 0478 5f76 6172 1700 0000 7208 0000 0072  .x_var....r....r
-00000e60: 0800 0000 720a 0000 0072 4d00 0000 6000  ....r....rM...`.
-00000e70: 0000 730e 0000 000c 010c 0116 010c 0106  ..s.............
-00000e80: 010a fe04 fe7a 1650 6c6f 742e 7365 745f  .....z.Plot.set_
-00000e90: 785f 7469 636b 5f6c 6162 656c 7363 0100  x_tick_labelsc..
-00000ea0: 0000 0000 0000 0000 0000 0100 0000 0700  ................
-00000eb0: 0000 4300 0000 7342 0000 0074 007c 006a  ..C...sB...t.|.j
-00000ec0: 0164 0183 0272 1f7c 006a 016a 027c 006a  .d...r.|.j.j.|.j
-00000ed0: 01a0 03a1 007c 006a 01a0 04a1 007c 006a  .....|.j.....|.j
-00000ee0: 056a 067c 006a 056a 077c 006a 056a 0864  .j.|.j.j.|.j.j.d
-00000ef0: 028d 0501 0064 0053 0064 0053 0029 034e  .....d.S.d.S.).N
-00000f00: da0a 7365 745f 7974 6963 6b73 7251 0000  ..set_yticksrQ..
-00000f10: 0029 0972 5500 0000 720d 0000 0072 5c00  .).rU...r....r\.
-00000f20: 0000 da0a 6765 745f 7974 6963 6b73 da0f  ....get_yticks..
-00000f30: 6765 745f 7974 6963 6b6c 6162 656c 7372  get_yticklabelsr
-00000f40: 0e00 0000 da0a 795f 726f 7461 7469 6f6e  ......y_rotation
-00000f50: da04 795f 6861 da04 795f 7661 7217 0000  ..y_ha..y_var...
-00000f60: 0072 0800 0000 7208 0000 0072 0a00 0000  .r....r....r....
-00000f70: 724e 0000 0067 0000 0073 0c00 0000 0c01  rN...g...s......
-00000f80: 1601 0c01 0601 0afe 04ff 7a16 506c 6f74  ..........z.Plot
-00000f90: 2e73 6574 5f79 5f74 6963 6b5f 6c61 6265  .set_y_tick_labe
-00000fa0: 6c73 4e29 16da 085f 5f6e 616d 655f 5fda  lsN)...__name__.
-00000fb0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000fc0: 7561 6c6e 616d 655f 5fda 0b63 6c61 7373  ualname__..class
-00000fd0: 6d65 7468 6f64 720b 0000 0072 1300 0000  methodr....r....
-00000fe0: 7210 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000ff0: 2b00 0000 722c 0000 0072 0c00 0000 723a  +...r,...r....r:
-00001000: 0000 0072 3700 0000 7238 0000 0072 3900  ...r7...r8...r9.
-00001010: 0000 7245 0000 0072 4900 0000 724c 0000  ..rE...rI...rL..
-00001020: 0072 4f00 0000 724d 0000 0072 4e00 0000  .rO...rM...rN...
-00001030: 7208 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
-00001040: 0a00 0000 7205 0000 0008 0000 0073 2800  ....r........s(.
-00001050: 0000 0800 0202 0a01 0803 0807 0804 080a  ................
-00001060: 0804 0808 0806 0804 0806 0806 0805 0803  ................
-00001070: 0805 0805 0805 0804 0c07 7205 0000 0029  ..........r....)
-00001080: 0dda 116d 6174 706c 6f74 6c69 622e 7079  ...matplotlib.py
-00001090: 706c 6f74 da06 7079 706c 6f74 da03 706c  plot..pyplot..pl
-000010a0: 74da 176d 6174 706c 6f74 6c69 622e 666f  t..matplotlib.fo
-000010b0: 6e74 5f6d 616e 6167 6572 da0a 6d61 7470  nt_manager..matp
-000010c0: 6c6f 746c 6962 da05 6e75 6d70 79da 026e  lotlib..numpy..n
-000010d0: 70da 0072 0300 0000 da0b 7574 696c 732e  p..r......utils.
-000010e0: 6469 6374 7372 0400 0000 7205 0000 00da  dictsr....r.....
-000010f0: 046c 6f61 6472 0800 0000 7208 0000 0072  .loadr....r....r
-00001100: 0800 0000 720a 0000 00da 083c 6d6f 6475  ....r......<modu
-00001110: 6c65 3e01 0000 0073 0e00 0000 0c00 0801  le>....s........
-00001120: 0801 0c02 0c01 0e02 0e65                 .........e
+00000160: 2364 2484 005a 1564 2564 2684 005a 1664  #d$..Z.d%d&..Z.d
+00000170: 2764 2884 005a 1764 2964 2a84 005a 1864  'd(..Z.d)d*..Z.d
+00000180: 2b64 2c84 005a 1964 2d64 2e84 005a 1a64  +d,..Z.d-d...Z.d
+00000190: 2f64 3084 005a 1b64 3153 0029 32da 0450  /d0..Z.d1S.)2..P
+000001a0: 6c6f 7463 0100 0000 0000 0000 0000 0000  lotc............
+000001b0: 0100 0000 0100 0000 4300 0000 f304 0000  ........C.......
+000001c0: 0064 0053 00a9 014e a900 2901 da03 636c  .d.S...N..)...cl
+000001d0: 7372 0800 0000 7208 0000 00fa 562f 686f  sr....r.....V/ho
+000001e0: 6d65 2f68 656e 7279 2f2e 6c6f 6361 6c2f  me/henry/.local/
+000001f0: 6c69 622f 7079 7468 6f6e 332e 3130 2f73  lib/python3.10/s
+00000200: 6974 652d 7061 636b 6167 6573 2f68 6775  ite-packages/hgu
+00000210: 7469 6c69 7469 6573 2f70 6c6f 7474 696e  tilities/plottin
+00000220: 672f 706c 6f74 7479 7065 732f 706c 6f74  g/plottypes/plot
+00000230: 2e70 79da 1173 6574 5f66 756e 6374 696f  .py..set_functio
+00000240: 6e5f 6469 6374 0a00 0000 7302 0000 0004  n_dict....s.....
+00000250: 027a 1650 6c6f 742e 7365 745f 6675 6e63  .z.Plot.set_func
+00000260: 7469 6f6e 5f64 6963 7463 0400 0000 0000  tion_dictc......
+00000270: 0000 0000 0000 0500 0000 0400 0000 4b00  ..............K.
+00000280: 0000 732e 0000 007c 00a0 007c 01a1 0101  ..s....|...|....
+00000290: 007c 027c 005f 017c 037c 005f 0274 03a0  .|.|._.|.|._.t..
+000002a0: 047c 007c 04a1 0201 007c 00a0 05a1 0001  .|.|.....|......
+000002b0: 0064 0053 0072 0700 0000 2906 da0e 7365  .d.S.r....)...se
+000002c0: 745f 6669 6775 7265 5f6f 626a da02 6178  t_figure_obj..ax
+000002d0: da08 6461 7461 5f6f 626a 7203 0000 00da  ..data_objr.....
+000002e0: 066b 7761 7267 73da 0a73 6574 5f6b 7761  .kwargs..set_kwa
+000002f0: 7267 7329 05da 0473 656c 66da 0a66 6967  rgs)...self..fig
+00000300: 7572 655f 6f62 6a72 0d00 0000 720e 0000  ure_objr....r...
+00000310: 0072 0f00 0000 7208 0000 0072 0800 0000  .r....r....r....
+00000320: 720a 0000 00da 085f 5f69 6e69 745f 5f0e  r......__init__.
+00000330: 0000 0073 0a00 0000 0a01 0601 0601 0c01  ...s............
+00000340: 0c01 7a0d 506c 6f74 2e5f 5f69 6e69 745f  ..z.Plot.__init_
+00000350: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000360: 0000 0200 0000 4300 0000 f314 0000 007c  ......C........|
+00000370: 00a0 00a1 0001 007c 00a0 01a1 0001 0064  .......|.......d
+00000380: 0053 0072 0700 0000 2902 da0e 696e 6865  .S.r....)...inhe
+00000390: 7269 745f 6b77 6172 6773 da0f 7365 745f  rit_kwargs..set_
+000003a0: 666f 6e74 5f6b 7761 7267 73a9 0172 1100  font_kwargs..r..
+000003b0: 0000 7208 0000 0072 0800 0000 720a 0000  ..r....r....r...
+000003c0: 0072 1000 0000 1500 0000 f304 0000 0008  .r..............
+000003d0: 010c 017a 0f50 6c6f 742e 7365 745f 6b77  ...z.Plot.set_kw
+000003e0: 6172 6773 6301 0000 0000 0000 0000 0000  argsc...........
+000003f0: 0002 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
+00000400: 0000 6700 6401 a201 7d01 7400 a001 7c00  ..g.d...}.t...|.
+00000410: 6a02 7c00 6a03 7c01 a103 0100 6400 5300  j.|.j.|.....d.S.
+00000420: 2902 4e29 10da 0e74 6974 6c65 5f66 6f6e  ).N)...title_fon
+00000430: 746e 616d 65da 0e74 6974 6c65 5f66 6f6e  tname..title_fon
+00000440: 7473 697a 65da 0b74 6974 6c65 5f63 6f6c  tsize..title_col
+00000450: 6f72 da17 7469 746c 655f 7665 7274 6963  or..title_vertic
+00000460: 616c 616c 6967 6e6d 656e 74da 1974 6974  alalignment..tit
+00000470: 6c65 5f68 6f72 697a 6f6e 7461 6c61 6c69  le_horizontalali
+00000480: 676e 6d65 6e74 da07 7469 746c 655f 79da  gnment..title_y.
+00000490: 0974 6974 6c65 5f70 6164 da09 7469 746c  .title_pad..titl
+000004a0: 655f 6c6f 63da 0d61 7869 735f 666f 6e74  e_loc..axis_font
+000004b0: 6e61 6d65 da0d 6178 6973 5f66 6f6e 7473  name..axis_fonts
+000004c0: 697a 65da 0a61 7869 735f 636f 6c6f 72da  ize..axis_color.
+000004d0: 0d61 7869 735f 6c61 6265 6c70 6164 da08  .axis_labelpad..
+000004e0: 6178 6973 5f6c 6f63 da0f 785f 6178 6973  axis_loc..x_axis
+000004f0: 5f72 6f74 6174 696f 6eda 0f79 5f61 7869  _rotation..y_axi
+00000500: 735f 726f 7461 7469 6f6e da0f 7a5f 6178  s_rotation..z_ax
+00000510: 6973 5f72 6f74 6174 696f 6e29 0472 0300  is_rotation).r..
+00000520: 0000 da07 696e 6865 7269 7472 0e00 0000  ....inheritr....
+00000530: 7212 0000 0029 0272 1100 0000 da0a 6174  r....).r......at
+00000540: 7472 6962 7574 6573 7208 0000 0072 0800  tributesr....r..
+00000550: 0000 720a 0000 0072 1500 0000 1900 0000  ..r....r........
+00000560: 7304 0000 0008 0116 077a 1350 6c6f 742e  s........z.Plot.
+00000570: 696e 6865 7269 745f 6b77 6172 6773 6301  inherit_kwargsc.
+00000580: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000590: 0000 0043 0000 0072 1400 0000 7207 0000  ...C...r....r...
+000005a0: 0029 02da 1273 6574 5f74 6974 6c65 5f66  .)...set_title_f
+000005b0: 6f6e 7464 6963 74da 1173 6574 5f61 7869  ontdict..set_axi
+000005c0: 735f 666f 6e74 6469 6374 7217 0000 0072  s_fontdictr....r
+000005d0: 0800 0000 7208 0000 0072 0a00 0000 7216  ....r....r....r.
+000005e0: 0000 0023 0000 0072 1800 0000 7a14 506c  ...#...r....z.Pl
+000005f0: 6f74 2e73 6574 5f66 6f6e 745f 6b77 6172  ot.set_font_kwar
+00000600: 6773 6301 0000 0000 0000 0000 0000 0002  gsc.............
+00000610: 0000 0006 0000 0043 0000 0073 3200 0000  .......C...s2...
+00000620: 7c00 6a00 6a01 7c00 6a00 6a02 7c00 6a00  |.j.j.|.j.j.|.j.
+00000630: 6a03 7c00 6a00 6a04 7c00 6a00 6a05 6401  j.|.j.j.|.j.j.d.
+00000640: 9c05 7d01 7406 7c01 8301 7c00 5f07 6400  ..}.t.|...|._.d.
+00000650: 5300 2902 4e29 05da 0866 6f6e 746e 616d  S.).N)...fontnam
+00000660: 65da 0866 6f6e 7473 697a 65da 0563 6f6c  e..fontsize..col
+00000670: 6f72 da11 7665 7274 6963 616c 616c 6967  or..verticalalig
+00000680: 6e6d 656e 74da 1368 6f72 697a 6f6e 7461  nment..horizonta
+00000690: 6c61 6c69 676e 6d65 6e74 2908 720e 0000  lalignment).r...
+000006a0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000006b0: 721c 0000 0072 1d00 0000 7204 0000 00da  r....r....r.....
+000006c0: 0e74 6974 6c65 5f66 6f6e 7464 6963 74a9  .title_fontdict.
+000006d0: 0272 1100 0000 720f 0000 0072 0800 0000  .r....r....r....
+000006e0: 7208 0000 0072 0a00 0000 722b 0000 0027  r....r....r+...'
+000006f0: 0000 0073 0e00 0000 0601 0601 0601 0601  ...s............
+00000700: 0601 06fc 0e05 7a17 506c 6f74 2e73 6574  ......z.Plot.set
+00000710: 5f74 6974 6c65 5f66 6f6e 7464 6963 7463  _title_fontdictc
+00000720: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000730: 0400 0000 4300 0000 7326 0000 007c 006a  ....C...s&...|.j
+00000740: 006a 017c 006a 006a 027c 006a 006a 0364  .j.|.j.j.|.j.j.d
+00000750: 019c 037d 0174 047c 0183 017c 005f 0564  ...}.t.|...|._.d
+00000760: 0053 0029 024e 2903 722d 0000 0072 2e00  .S.).N).r-...r..
+00000770: 0000 722f 0000 0029 0672 0e00 0000 7221  ..r/...).r....r!
+00000780: 0000 0072 2200 0000 7223 0000 0072 0400  ...r"...r#...r..
+00000790: 0000 da0d 6178 6973 5f66 6f6e 7464 6963  ....axis_fontdic
+000007a0: 7472 3300 0000 7208 0000 0072 0800 0000  tr3...r....r....
+000007b0: 720a 0000 0072 2c00 0000 2f00 0000 730a  r....r,.../...s.
+000007c0: 0000 0006 0106 0106 0106 fe0e 037a 1650  .............z.P
+000007d0: 6c6f 742e 7365 745f 6178 6973 5f66 6f6e  lot.set_axis_fon
+000007e0: 7464 6963 7463 0200 0000 0000 0000 0000  tdictc..........
+000007f0: 0000 0200 0000 0200 0000 4300 0000 7312  ..........C...s.
+00000800: 0000 007c 017c 005f 007c 016a 017c 005f  ...|.|._.|.j.|._
+00000810: 0164 0053 0072 0700 0000 2902 7212 0000  .d.S.r....).r...
+00000820: 00da 0b66 6967 7572 6573 5f6f 626a 2902  ...figures_obj).
+00000830: 7211 0000 0072 1200 0000 7208 0000 0072  r....r....r....r
+00000840: 0800 0000 720a 0000 0072 0c00 0000 3500  ....r....r....5.
+00000850: 0000 7304 0000 0006 010c 017a 1350 6c6f  ..s........z.Plo
+00000860: 742e 7365 745f 6669 6775 7265 5f6f 626a  t.set_figure_obj
+00000870: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000880: 0002 0000 0043 0000 0073 2400 0000 7c00  .....C...s$...|.
+00000890: a000 a100 0100 7c00 a001 a100 0100 7c00  ......|.......|.
+000008a0: a002 a100 0100 7c00 a003 a100 0100 6400  ......|.......d.
+000008b0: 5300 7207 0000 0029 04da 0970 6c6f 745f  S.r....)...plot_
+000008c0: 6461 7461 da09 7365 745f 7469 746c 65da  data..set_title.
+000008d0: 0a61 6464 5f6c 6567 656e 64da 0f61 6464  .add_legend..add
+000008e0: 5f61 7869 735f 6c61 6265 6c73 7217 0000  _axis_labelsr...
+000008f0: 0072 0800 0000 7208 0000 0072 0a00 0000  .r....r....r....
+00000900: da0b 6372 6561 7465 5f70 6c6f 7439 0000  ..create_plot9..
+00000910: 0073 0800 0000 0801 0801 0801 0c01 7a10  .s............z.
+00000920: 506c 6f74 2e63 7265 6174 655f 706c 6f74  Plot.create_plot
+00000930: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000940: 0007 0000 0043 0000 0073 4600 0000 7c00  .....C...sF...|.
+00000950: 6a00 6a01 6400 7501 7221 7c00 6a02 6a03  j.j.d.u.r!|.j.j.
+00000960: 7c00 6a00 6a01 6601 6900 7c00 6a04 a401  |.j.j.f.i.|.j...
+00000970: 7c00 6a00 6a05 7c00 6a00 6a06 7c00 6a00  |.j.j.|.j.j.|.j.
+00000980: 6a07 6401 9c03 a401 8e01 0100 6400 5300  j.d.........d.S.
+00000990: 6400 5300 2902 4e29 03da 036c 6f63 da01  d.S.).N)...loc..
+000009a0: 79da 0370 6164 2908 720e 0000 00da 0574  y..pad).r......t
+000009b0: 6974 6c65 720d 0000 0072 3700 0000 7232  itler....r7...r2
+000009c0: 0000 0072 2000 0000 721e 0000 0072 1f00  ...r ...r....r..
+000009d0: 0000 7217 0000 0072 0800 0000 7208 0000  ..r....r....r...
+000009e0: 0072 0a00 0000 7237 0000 003f 0000 0073  .r....r7...?...s
+000009f0: 0c00 0000 0c01 1601 0c01 0601 0efe 04ff  ................
+00000a00: 7a0e 506c 6f74 2e73 6574 5f74 6974 6c65  z.Plot.set_title
+00000a10: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000a20: 0003 0000 0043 0000 0073 2e00 0000 7c00  .....C...s....|.
+00000a30: 6a00 6a01 7313 7c00 6a02 6a03 7215 7c00  j.j.s.|.j.j.r.|.
+00000a40: 6a04 6a03 7c00 6a02 6a05 6401 8d01 0100  j.j.|.j.j.d.....
+00000a50: 6400 5300 6400 5300 6400 5300 2902 4e29  d.S.d.S.d.S.).N)
+00000a60: 0172 3b00 0000 2906 7235 0000 00da 1075  .r;...).r5.....u
+00000a70: 6e69 7665 7273 616c 5f6c 6567 656e 6472  niversal_legendr
+00000a80: 0e00 0000 da06 6c65 6765 6e64 720d 0000  ......legendr...
+00000a90: 00da 0a6c 6567 656e 645f 6c6f 6372 1700  ...legend_locr..
+00000aa0: 0000 7208 0000 0072 0800 0000 720a 0000  ..r....r....r...
+00000ab0: 0072 3800 0000 4500 0000 730a 0000 0008  .r8...E...s.....
+00000ac0: 0108 0116 0104 fe04 017a 0f50 6c6f 742e  .........z.Plot.
+00000ad0: 6164 645f 6c65 6765 6e64 6301 0000 0000  add_legendc.....
+00000ae0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000af0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
+00000b00: 0000 7217 0000 0072 0800 0000 7208 0000  ..r....r....r...
+00000b10: 0072 0a00 0000 7239 0000 004a 0000 0073  .r....r9...J...s
+00000b20: 0200 0000 0401 7a14 506c 6f74 2e61 6464  ......z.Plot.add
+00000b30: 5f61 7869 735f 6c61 6265 6c73 6301 0000  _axis_labelsc...
+00000b40: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000b50: 0043 0000 00f3 2e00 0000 7c00 6a00 6a01  .C........|.j.j.
+00000b60: 6400 7501 7215 7c00 6a02 6a03 7c00 6a00  d.u.r.|.j.j.|.j.
+00000b70: 6a01 6601 6900 7c00 6a04 a401 8e01 0100  j.f.i.|.j.......
+00000b80: 6400 5300 6400 5300 7207 0000 0029 0572  d.S.d.S.r....).r
+00000b90: 0e00 0000 da07 785f 6c61 6265 6c72 0d00  ......x_labelr..
+00000ba0: 0000 da0a 7365 745f 786c 6162 656c 7234  ....set_xlabelr4
+00000bb0: 0000 0072 1700 0000 7208 0000 0072 0800  ...r....r....r..
+00000bc0: 0000 720a 0000 00da 0b61 6464 5f78 5f6c  ..r......add_x_l
+00000bd0: 6162 656c 4d00 0000 f30a 0000 000c 0110  abelM...........
+00000be0: 0104 010a ff04 ff7a 1050 6c6f 742e 6164  .......z.Plot.ad
+00000bf0: 645f 785f 6c61 6265 6c63 0100 0000 0000  d_x_labelc......
+00000c00: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000c10: 0000 7242 0000 0072 0700 0000 2905 720e  ..rB...r....).r.
+00000c20: 0000 00da 0779 5f6c 6162 656c 720d 0000  .....y_labelr...
+00000c30: 00da 0a73 6574 5f79 6c61 6265 6c72 3400  ...set_ylabelr4.
+00000c40: 0000 7217 0000 0072 0800 0000 7208 0000  ..r....r....r...
+00000c50: 0072 0a00 0000 da0b 6164 645f 795f 6c61  .r......add_y_la
+00000c60: 6265 6c52 0000 0072 4600 0000 7a10 506c  belR...rF...z.Pl
+00000c70: 6f74 2e61 6464 5f79 5f6c 6162 656c 6301  ot.add_y_labelc.
+00000c80: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000c90: 0000 0043 0000 0072 4200 0000 7207 0000  ...C...rB...r...
+00000ca0: 0029 0572 0e00 0000 da07 7a5f 6c61 6265  .).r......z_labe
+00000cb0: 6c72 0d00 0000 da0a 7365 745f 7a6c 6162  lr......set_zlab
+00000cc0: 656c 7234 0000 0072 1700 0000 7208 0000  elr4...r....r...
+00000cd0: 0072 0800 0000 720a 0000 00da 0b61 6464  .r....r......add
+00000ce0: 5f7a 5f6c 6162 656c 5700 0000 7246 0000  _z_labelW...rF..
+00000cf0: 007a 1050 6c6f 742e 6164 645f 7a5f 6c61  .z.Plot.add_z_la
+00000d00: 6265 6c63 0100 0000 0000 0000 0000 0000  belc............
+00000d10: 0100 0000 0200 0000 4300 0000 7214 0000  ........C...r...
+00000d20: 0072 0700 0000 2902 da11 7365 745f 785f  .r....)...set_x_
+00000d30: 7469 636b 5f6c 6162 656c 73da 1173 6574  tick_labels..set
+00000d40: 5f79 5f74 6963 6b5f 6c61 6265 6c73 7217  _y_tick_labelsr.
+00000d50: 0000 0072 0800 0000 7208 0000 0072 0a00  ...r....r....r..
+00000d60: 0000 da0f 7365 745f 7469 636b 5f6c 6162  ....set_tick_lab
+00000d70: 656c 735c 0000 0072 1800 0000 7a14 506c  els\...r....z.Pl
+00000d80: 6f74 2e73 6574 5f74 6963 6b5f 6c61 6265  ot.set_tick_labe
+00000d90: 6c73 6301 0000 0000 0000 0000 0000 0001  lsc.............
+00000da0: 0000 0007 0000 0043 0000 00f3 4200 0000  .......C....B...
+00000db0: 7400 7c00 6a01 6401 8302 721f 7c00 6a01  t.|.j.d...r.|.j.
+00000dc0: 6a02 7c00 6a01 a003 a100 7c00 6a01 a004  j.|.j.....|.j...
+00000dd0: a100 7c00 6a05 6a06 7c00 6a05 6a07 7c00  ..|.j.j.|.j.j.|.
+00000de0: 6a05 6a08 6402 8d05 0100 6400 5300 6400  j.j.d.....d.S.d.
+00000df0: 5300 2903 4eda 0a73 6574 5f78 7469 636b  S.).N..set_xtick
+00000e00: 73a9 03da 0872 6f74 6174 696f 6eda 0268  s....rotation..h
+00000e10: 61da 0276 6129 09da 0768 6173 6174 7472  a..va)...hasattr
+00000e20: 720d 0000 0072 5100 0000 da0a 6765 745f  r....rQ.....get_
+00000e30: 7874 6963 6b73 da0f 6765 745f 7874 6963  xticks..get_xtic
+00000e40: 6b6c 6162 656c 7372 0e00 0000 da0a 785f  klabelsr......x_
+00000e50: 726f 7461 7469 6f6e da04 785f 6861 da04  rotation..x_ha..
+00000e60: 785f 7661 7217 0000 0072 0800 0000 7208  x_var....r....r.
+00000e70: 0000 0072 0a00 0000 724d 0000 0060 0000  ...r....rM...`..
+00000e80: 00f3 0c00 0000 0c01 1601 0c01 0601 0afe  ................
+00000e90: 04ff 7a16 506c 6f74 2e73 6574 5f78 5f74  ..z.Plot.set_x_t
+00000ea0: 6963 6b5f 6c61 6265 6c73 6301 0000 0000  ick_labelsc.....
+00000eb0: 0000 0000 0000 0001 0000 0007 0000 0043  ...............C
+00000ec0: 0000 0072 5000 0000 2903 4eda 0a73 6574  ...rP...).N..set
+00000ed0: 5f79 7469 636b 7372 5200 0000 2909 7256  _yticksrR...).rV
+00000ee0: 0000 0072 0d00 0000 725d 0000 00da 0a67  ...r....r].....g
+00000ef0: 6574 5f79 7469 636b 73da 0f67 6574 5f79  et_yticks..get_y
+00000f00: 7469 636b 6c61 6265 6c73 720e 0000 00da  ticklabelsr.....
+00000f10: 0a79 5f72 6f74 6174 696f 6eda 0479 5f68  .y_rotation..y_h
+00000f20: 61da 0479 5f76 6172 1700 0000 7208 0000  a..y_var....r...
+00000f30: 0072 0800 0000 720a 0000 0072 4e00 0000  .r....r....rN...
+00000f40: 6600 0000 725c 0000 007a 1650 6c6f 742e  f...r\...z.Plot.
+00000f50: 7365 745f 795f 7469 636b 5f6c 6162 656c  set_y_tick_label
+00000f60: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+00000f70: 0000 0200 0000 4300 0000 7214 0000 0072  ......C...r....r
+00000f80: 0700 0000 2902 da0b 7365 745f 786c 696d  ....)...set_xlim
+00000f90: 6974 73da 0b73 6574 5f79 6c69 6d69 7473  its..set_ylimits
+00000fa0: 7217 0000 0072 0800 0000 7208 0000 0072  r....r....r....r
+00000fb0: 0a00 0000 da0f 7365 745f 6178 6973 5f6c  ......set_axis_l
+00000fc0: 696d 6974 736c 0000 0072 1800 0000 7a14  imitsl...r....z.
+00000fd0: 506c 6f74 2e73 6574 5f61 7869 735f 6c69  Plot.set_axis_li
+00000fe0: 6d69 7473 6301 0000 0000 0000 0000 0000  mitsc...........
+00000ff0: 0001 0000 0004 0000 0043 0000 00f3 2c00  .........C....,.
+00001000: 0000 7400 7c00 6a01 6401 8302 7214 7c00  ..t.|.j.d...r.|.
+00001010: 6a01 6a02 7c00 6a03 6a04 7c00 6a03 6a05  j.j.|.j.j.|.j.j.
+00001020: 6402 8d02 0100 6400 5300 6400 5300 2903  d.....d.S.d.S.).
+00001030: 4eda 0873 6574 5f78 6c69 6d29 02da 046c  N..set_xlim)...l
+00001040: 6566 74da 0572 6967 6874 2906 7256 0000  eft..right).rV..
+00001050: 0072 0d00 0000 7267 0000 0072 0e00 0000  .r....rg...r....
+00001060: da0a 786c 696d 5f6c 6f77 6572 da0a 786c  ..xlim_lower..xl
+00001070: 696d 5f75 7070 6572 7217 0000 0072 0800  im_upperr....r..
+00001080: 0000 7208 0000 0072 0a00 0000 7263 0000  ..r....r....rc..
+00001090: 0070 0000 00f3 0a00 0000 0c01 0c01 0601  .p..............
+000010a0: 0aff 04ff 7a10 506c 6f74 2e73 6574 5f78  ....z.Plot.set_x
+000010b0: 6c69 6d69 7473 6301 0000 0000 0000 0000  limitsc.........
+000010c0: 0000 0001 0000 0004 0000 0043 0000 0072  ...........C...r
+000010d0: 6600 0000 2903 4eda 0873 6574 5f79 6c69  f...).N..set_yli
+000010e0: 6d29 02da 0662 6f74 746f 6dda 0374 6f70  m)...bottom..top
+000010f0: 2906 7256 0000 0072 0d00 0000 726d 0000  ).rV...r....rm..
+00001100: 0072 0e00 0000 da0a 796c 696d 5f6c 6f77  .r......ylim_low
+00001110: 6572 da0a 796c 696d 5f75 7070 6572 7217  er..ylim_upperr.
+00001120: 0000 0072 0800 0000 7208 0000 0072 0a00  ...r....r....r..
+00001130: 0000 7264 0000 0075 0000 0072 6c00 0000  ..rd...u...rl...
+00001140: 7a10 506c 6f74 2e73 6574 5f79 6c69 6d69  z.Plot.set_ylimi
+00001150: 7473 6301 0000 0000 0000 0000 0000 0001  tsc.............
+00001160: 0000 0002 0000 0043 0000 0072 1400 0000  .......C...r....
+00001170: 7207 0000 0029 02da 0b73 6574 5f78 626f  r....)...set_xbo
+00001180: 756e 6473 da0b 7365 745f 7962 6f75 6e64  unds..set_ybound
+00001190: 7372 1700 0000 7208 0000 0072 0800 0000  sr....r....r....
+000011a0: 720a 0000 00da 0f73 6574 5f61 7869 735f  r......set_axis_
+000011b0: 626f 756e 6473 7a00 0000 7218 0000 007a  boundsz...r....z
+000011c0: 1450 6c6f 742e 7365 745f 6178 6973 5f62  .Plot.set_axis_b
+000011d0: 6f75 6e64 7363 0100 0000 0000 0000 0000  oundsc..........
+000011e0: 0000 0100 0000 0400 0000 4300 0000 7266  ..........C...rf
+000011f0: 0000 0029 034e da0a 7365 745f 7862 6f75  ...).N..set_xbou
+00001200: 6e64 a902 da05 6c6f 7765 72da 0575 7070  nd....lower..upp
+00001210: 6572 2906 7256 0000 0072 0d00 0000 7275  er).rV...r....ru
+00001220: 0000 0072 0e00 0000 da0c 7862 6f75 6e64  ...r......xbound
+00001230: 5f6c 6f77 6572 da0c 7862 6f75 6e64 5f75  _lower..xbound_u
+00001240: 7070 6572 7217 0000 0072 0800 0000 7208  pperr....r....r.
+00001250: 0000 0072 0a00 0000 7272 0000 007e 0000  ...r....rr...~..
+00001260: 0072 6c00 0000 7a10 506c 6f74 2e73 6574  .rl...z.Plot.set
+00001270: 5f78 626f 756e 6473 6301 0000 0000 0000  _xboundsc.......
+00001280: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001290: 0072 6600 0000 2903 4eda 0a73 6574 5f79  .rf...).N..set_y
+000012a0: 626f 756e 6472 7600 0000 2906 7256 0000  boundrv...).rV..
+000012b0: 0072 0d00 0000 727b 0000 0072 0e00 0000  .r....r{...r....
+000012c0: da0c 7962 6f75 6e64 5f6c 6f77 6572 da0c  ..ybound_lower..
+000012d0: 7962 6f75 6e64 5f75 7070 6572 7217 0000  ybound_upperr...
+000012e0: 0072 0800 0000 7208 0000 0072 0a00 0000  .r....r....r....
+000012f0: 7273 0000 0083 0000 0072 6c00 0000 7a10  rs.......rl...z.
+00001300: 506c 6f74 2e73 6574 5f79 626f 756e 6473  Plot.set_ybounds
+00001310: 4e29 1cda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00001320: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001330: 6c6e 616d 655f 5fda 0b63 6c61 7373 6d65  lname__..classme
+00001340: 7468 6f64 720b 0000 0072 1300 0000 7210  thodr....r....r.
+00001350: 0000 0072 1500 0000 7216 0000 0072 2b00  ...r....r....r+.
+00001360: 0000 722c 0000 0072 0c00 0000 723a 0000  ..r,...r....r:..
+00001370: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
+00001380: 7245 0000 0072 4900 0000 724c 0000 0072  rE...rI...rL...r
+00001390: 4f00 0000 724d 0000 0072 4e00 0000 7265  O...rM...rN...re
+000013a0: 0000 0072 6300 0000 7264 0000 0072 7400  ...rc...rd...rt.
+000013b0: 0000 7272 0000 0072 7300 0000 7208 0000  ..rr...rs...r...
+000013c0: 0072 0800 0000 7208 0000 0072 0a00 0000  .r....r....r....
+000013d0: 7205 0000 0008 0000 0073 3400 0000 0800  r........s4.....
+000013e0: 0202 0a01 0803 0807 0804 080a 0804 0808  ................
+000013f0: 0806 0804 0806 0806 0805 0803 0805 0805  ................
+00001400: 0805 0804 0806 0806 0804 0805 0805 0804  ................
+00001410: 0c05 7205 0000 0029 0dda 116d 6174 706c  ..r....)...matpl
+00001420: 6f74 6c69 622e 7079 706c 6f74 da06 7079  otlib.pyplot..py
+00001430: 706c 6f74 da03 706c 74da 176d 6174 706c  plot..plt..matpl
+00001440: 6f74 6c69 622e 666f 6e74 5f6d 616e 6167  otlib.font_manag
+00001450: 6572 da0a 6d61 7470 6c6f 746c 6962 da05  er..matplotlib..
+00001460: 6e75 6d70 79da 026e 70da 0072 0300 0000  numpy..np..r....
+00001470: da0b 7574 696c 732e 6469 6374 7372 0400  ..utils.dictsr..
+00001480: 0000 7205 0000 00da 046c 6f61 6472 0800  ..r......loadr..
+00001490: 0000 7208 0000 0072 0800 0000 720a 0000  ..r....r....r...
+000014a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000014b0: 1000 0000 0c00 0801 0801 0c02 0c01 0e02  ................
+000014c0: 007f 0e01                                ....
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 20:06:26 2023 UTC, .py size: 6917 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c263 8f64 051b 0000  o........c.d....
+00000000: 6f0d 0d0a 0000 0000 fd46 9064 451b 0000  o........F.dE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
 00000040: 5a04 6402 6403 6c05 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000050: 6405 6c07 6d08 5a08 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000060: 8400 6407 6508 8303 5a09 6506 a00a 6509  ..d.e...Z.e...e.
 00000070: a101 0100 6401 5300 2908 e900 0000 004e  ....d.S.)......N
@@ -24,273 +24,277 @@
 00000170: 7365 6d69 6c6f 6778 da08 7365 6d69 6c6f  semilogx..semilo
 00000180: 6779 da06 6c6f 676c 6f67 da08 6572 726f  gy..loglog..erro
 00000190: 7262 6172 da07 7363 6174 7465 7229 04da  rbar..scatter)..
 000001a0: 0c70 6c6f 745f 7265 6775 6c61 72da 0e70  .plot_regular..p
 000001b0: 6c6f 745f 6572 726f 7262 6172 73da 0c70  lot_errorbars..p
 000001c0: 6c6f 745f 7363 6174 7465 72da 0d66 756e  lot_scatter..fun
 000001d0: 6374 696f 6e5f 6469 6374 2901 da03 636c  ction_dict)...cl
-000001e0: 73a9 0072 1200 0000 fa69 2f6d 6e74 2f32  s..r.....i/mnt/2
-000001f0: 5442 2f44 6f63 756d 656e 7473 2f50 7974  TB/Documents/Pyt
-00000200: 686f 6e2f 5265 616c 2057 6f72 6c64 2041  hon/Real World A
-00000210: 7070 6c69 6361 7469 6f6e 732f 6867 7574  pplications/hgut
-00000220: 696c 6974 6965 732f 6867 7574 696c 6974  ilities/hgutilit
-00000230: 6965 732f 706c 6f74 7469 6e67 2f70 6c6f  ies/plotting/plo
-00000240: 7474 7970 6573 2f70 6c6f 746c 696e 6573  ttypes/plotlines
-00000250: 2e70 79da 1173 6574 5f66 756e 6374 696f  .py..set_functio
-00000260: 6e5f 6469 6374 0900 0000 730e 0000 0004  n_dict....s.....
-00000270: 0204 0104 0104 0104 0104 010c fb7a 1b50  .............z.P
-00000280: 6c6f 744c 696e 6573 2e73 6574 5f66 756e  lotLines.set_fun
-00000290: 6374 696f 6e5f 6469 6374 6304 0000 0000  ction_dictc.....
-000002a0: 0000 0000 0000 0005 0000 0005 0000 004b  ...............K
-000002b0: 0000 0073 2e00 0000 7400 6a01 7c00 7c01  ...s....t.j.|.|.
-000002c0: 7c02 7c03 6604 6900 7c04 a401 8e01 0100  |.|.f.i.|.......
-000002d0: 7c03 7c00 5f02 7403 a004 7c00 7c04 a102  |.|._.t...|.|...
-000002e0: 0100 6400 5300 a901 4e29 0572 0500 0000  ..d.S...N).r....
-000002f0: da08 5f5f 696e 6974 5f5f da09 6c69 6e65  ..__init__..line
-00000300: 735f 6f62 6a72 0300 0000 da06 6b77 6172  s_objr......kwar
-00000310: 6773 2905 da04 7365 6c66 da0a 6669 6775  gs)...self..figu
-00000320: 7265 5f6f 626a da02 6178 7217 0000 0072  re_obj..axr....r
-00000330: 1800 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000340: 0000 0072 1600 0000 1200 0000 7306 0000  ...r........s...
-00000350: 0018 0106 0110 017a 1250 6c6f 744c 696e  .......z.PlotLin
-00000360: 6573 2e5f 5f69 6e69 745f 5f63 0100 0000  es.__init__c....
-00000370: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000380: 4300 0000 f314 0000 007c 00a0 00a1 0001  C........|......
-00000390: 007c 00a0 01a1 0001 0064 0053 0072 1500  .|.......d.S.r..
-000003a0: 0000 2902 da0a 706c 6f74 5f6c 696e 6573  ..)...plot_lines
-000003b0: da0f 7365 745f 7469 636b 5f6c 6162 656c  ..set_tick_label
-000003c0: 73a9 0172 1900 0000 7212 0000 0072 1200  s..r....r....r..
-000003d0: 0000 7213 0000 00da 0970 6c6f 745f 6461  ..r......plot_da
-000003e0: 7461 1700 0000 f304 0000 0008 010c 017a  ta.............z
-000003f0: 1350 6c6f 744c 696e 6573 2e70 6c6f 745f  .PlotLines.plot_
-00000400: 6461 7461 6301 0000 0000 0000 0000 0000  datac...........
-00000410: 0004 0000 0005 0000 0043 0000 0073 3600  .........C...s6.
-00000420: 0000 7c00 a000 a100 7d01 7401 7c00 6a02  ..|.....}.t.|.j.
-00000430: 7c00 6a03 6a04 8302 7d02 7c00 6a03 6a05  |.j.j...}.|.j.j.
-00000440: 4400 5d08 7d03 7c01 7c00 7c02 7c03 8303  D.].}.|.|.|.|...
-00000450: 0100 7110 6400 5300 7215 0000 0029 06da  ..q.d.S.r....)..
-00000460: 1667 6574 5f70 6c6f 745f 7479 7065 5f66  .get_plot_type_f
-00000470: 756e 6374 696f 6eda 0767 6574 6174 7472  unction..getattr
-00000480: 721b 0000 0072 1700 0000 da09 706c 6f74  r....r......plot
-00000490: 5f74 7970 65da 0c6c 696e 655f 6f62 6a65  _type..line_obje
-000004a0: 6374 7329 0472 1900 0000 da12 706c 6f74  cts).r......plot
-000004b0: 5f74 7970 655f 6675 6e63 7469 6f6e da0d  _type_function..
-000004c0: 706c 6f74 5f66 756e 6374 696f 6eda 086c  plot_function..l
-000004d0: 696e 655f 6f62 6a72 1200 0000 7212 0000  ine_objr....r...
-000004e0: 0072 1300 0000 721d 0000 001b 0000 0073  .r....r........s
-000004f0: 0a00 0000 0801 1001 0c01 0e01 04ff 7a14  ..............z.
-00000500: 506c 6f74 4c69 6e65 732e 706c 6f74 5f6c  PlotLines.plot_l
-00000510: 696e 6573 6301 0000 0000 0000 0000 0000  inesc...........
-00000520: 0003 0000 0002 0000 0043 0000 0073 1600  .........C...s..
-00000530: 0000 7c00 6a00 6a01 7d01 7c00 6a02 7c01  ..|.j.j.}.|.j.|.
-00000540: 1900 7d02 7c02 5300 7215 0000 0029 0372  ..}.|.S.r....).r
-00000550: 1700 0000 7224 0000 0072 1000 0000 2903  ....r$...r....).
-00000560: 7219 0000 0072 2400 0000 7226 0000 0072  r....r$...r&...r
-00000570: 1200 0000 7212 0000 0072 1300 0000 7222  ....r....r....r"
-00000580: 0000 0021 0000 0073 0600 0000 0801 0a01  ...!...s........
-00000590: 0401 7a20 506c 6f74 4c69 6e65 732e 6765  ..z PlotLines.ge
-000005a0: 745f 706c 6f74 5f74 7970 655f 6675 6e63  t_plot_type_func
-000005b0: 7469 6f6e 6303 0000 0000 0000 0000 0000  tionc...........
-000005c0: 0003 0000 0006 0000 0043 0000 0073 4201  .........C...sB.
-000005d0: 0000 7c01 7c02 6a00 7c02 6a01 6602 6900  ..|.|.j.|.j.f.i.
-000005e0: 6401 7c02 6a02 9301 6402 7c02 6a03 9301  d.|.j...d.|.j...
-000005f0: 6403 7c00 6a04 6a05 9301 6404 7c02 6a06  d.|.j.j...d.|.j.
-00000600: 9301 6405 7c00 6a04 6a07 9301 6406 7c00  ..d.|.j.j...d.|.
-00000610: 6a04 6a08 9301 6407 7c00 6a04 6a09 9301  j.j...d.|.j.j...
-00000620: 6408 7c02 6a0a 9301 6409 7c02 6a0b 9301  d.|.j...d.|.j...
-00000630: 640a 7c02 6a0c 9301 640b 7c02 6a0d 9301  d.|.j...d.|.j...
-00000640: 640c 740e 7c02 6a0f 8301 9301 640d 7c02  d.t.|.j.....d.|.
-00000650: 6a10 9301 640e 7c02 6a11 9301 640f 7c02  j...d.|.j...d.|.
-00000660: 6a12 9301 6410 7c02 6a13 9301 6411 7c02  j...d.|.j...d.|.
-00000670: 6a14 9301 6412 7c02 6a15 9301 6413 7c02  j...d.|.j...d.|.
-00000680: 6a16 9301 6414 7c02 6a17 9301 6415 7c02  j...d.|.j...d.|.
-00000690: 6a18 9301 6416 7c02 6a19 9301 6417 7c02  j...d.|.j...d.|.
-000006a0: 6a1a 9301 6418 7c02 6a1b 9301 6419 7c02  j...d.|.j...d.|.
-000006b0: 6a1c 9301 641a 7c02 6a1d 9301 641b 7c02  j...d.|.j...d.|.
-000006c0: 6a1e 9301 641c 7c02 6a1f 9301 641d 7c02  j...d.|.j...d.|.
-000006d0: 6a20 9301 641e 7c02 6a21 9301 641f 7c02  j ..d.|.j!..d.|.
-000006e0: 6a22 9301 6420 7c02 6a23 9301 6421 7c02  j"..d |.j#..d!|.
-000006f0: 6a24 9301 6422 7c02 6a25 9301 6423 7c02  j$..d"|.j%..d#|.
-00000700: 6a26 9301 6424 7c02 6a27 9301 8e01 0100  j&..d$|.j'......
-00000710: 6400 5300 2925 4eda 0a61 6767 5f66 696c  d.S.)%N..agg_fil
-00000720: 7465 72da 0561 6c70 6861 da08 616e 696d  ter..alpha..anim
-00000730: 6174 6564 da0b 616e 7469 616c 6961 7365  ated..antialiase
-00000740: 64da 0863 6c69 705f 626f 78da 0763 6c69  d..clip_box..cli
-00000750: 705f 6f6e da09 636c 6970 5f70 6174 68da  p_on..clip_path.
-00000760: 0563 6f6c 6f72 da0d 6461 7368 5f63 6170  .color..dash_cap
-00000770: 7374 796c 65da 0e64 6173 685f 6a6f 696e  style..dash_join
-00000780: 7374 796c 65da 0964 7261 7773 7479 6c65  style..drawstyle
-00000790: da06 6461 7368 6573 da09 6669 6c6c 7374  ..dashes..fillst
-000007a0: 796c 65da 0867 6170 636f 6c6f 72da 0367  yle..gapcolor..g
-000007b0: 6964 da09 696e 5f6c 6179 6f75 74da 056c  id..in_layout..l
-000007c0: 6162 656c da09 6c69 6e65 7374 796c 65da  abel..linestyle.
-000007d0: 096c 696e 6577 6964 7468 da06 6d61 726b  .linewidth..mark
-000007e0: 6572 da0f 6d61 726b 6572 6564 6765 636f  er..markeredgeco
-000007f0: 6c6f 72da 0f6d 6172 6b65 7265 6467 6577  lor..markeredgew
-00000800: 6964 7468 da0f 6d61 726b 6572 6661 6365  idth..markerface
-00000810: 636f 6c6f 72da 126d 6172 6b65 7266 6163  color..markerfac
-00000820: 6563 6f6c 6f72 616c 74da 0a6d 6172 6b65  ecoloralt..marke
-00000830: 7273 697a 65da 096d 6172 6b65 7665 7279  rsize..markevery
-00000840: da09 6d6f 7573 656f 7665 72da 0c70 6174  ..mouseover..pat
-00000850: 685f 6566 6665 6374 73da 0a72 6173 7465  h_effects..raste
-00000860: 7269 7a65 64da 0d73 6b65 7463 685f 7061  rized..sketch_pa
-00000870: 7261 6d73 da04 736e 6170 da0e 736f 6c69  rams..snap..soli
-00000880: 645f 6361 7073 7479 6c65 da0f 736f 6c69  d_capstyle..soli
-00000890: 645f 6a6f 696e 7374 796c 65da 0375 726c  d_joinstyle..url
-000008a0: da07 7669 7369 626c 65da 067a 6f72 6465  ..visible..zorde
-000008b0: 7229 28da 0878 5f76 616c 7565 73da 0879  r)(..x_values..y
-000008c0: 5f76 616c 7565 7372 2900 0000 722a 0000  _valuesr)...r*..
-000008d0: 0072 1700 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
-000008e0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-000008f0: 3000 0000 7231 0000 0072 3200 0000 7233  0...r1...r2...r3
-00000900: 0000 00da 0574 7570 6c65 7234 0000 0072  .....tupler4...r
-00000910: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
-00000920: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
-00000930: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
-00000940: 0072 3f00 0000 7240 0000 0072 4100 0000  .r?...r@...rA...
-00000950: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00000960: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
-00000970: 0000 0072 4900 0000 724a 0000 0072 4b00  ...rI...rJ...rK.
-00000980: 0000 724c 0000 0029 0372 1900 0000 7227  ..rL...).r....r'
-00000990: 0000 0072 2800 0000 7212 0000 0072 1200  ...r(...r....r..
-000009a0: 0000 7213 0000 0072 0d00 0000 2600 0000  ..r....r....&...
-000009b0: 7396 0000 0006 0104 0106 ff06 0202 fe06  s...............
-000009c0: 0302 fd08 0402 fc06 0502 fb08 0602 fa08  ................
-000009d0: 0702 f908 0802 f806 0902 f706 0a02 f606  ................
-000009e0: 0b02 f506 0c02 f40a 0d02 f306 0e02 f206  ................
-000009f0: 0f02 f106 1002 f006 1102 ef06 1202 ee06  ................
-00000a00: 1302 ed06 1402 ec06 1502 eb06 1602 ea06  ................
-00000a10: 1702 e906 1802 e806 1902 e706 1a02 e606  ................
-00000a20: 1b02 e506 1c02 e406 1d02 e306 1e02 e206  ................
-00000a30: 1f02 e106 2002 e006 2102 df06 2202 de06  .... ...!..."...
-00000a40: 2302 dd06 2402 dc06 2508 db7a 1650 6c6f  #...$...%..z.Plo
-00000a50: 744c 696e 6573 2e70 6c6f 745f 7265 6775  tLines.plot_regu
-00000a60: 6c61 7263 0200 0000 0000 0000 0000 0000  larc............
-00000a70: 0200 0000 0600 0000 4300 0000 73aa 0100  ........C...s...
-00000a80: 007c 0174 006a 0174 006a 0266 0269 0064  .|.t.j.t.j.f.i.d
-00000a90: 0174 006a 0393 0164 0274 006a 0493 0164  .t.j...d.t.j...d
-00000aa0: 0374 006a 0593 0164 0474 006a 0693 0164  .t.j...d.t.j...d
-00000ab0: 0574 006a 0793 0164 0674 006a 0893 0164  .t.j...d.t.j...d
-00000ac0: 0774 006a 0993 0164 0874 006a 0a93 0164  .t.j...d.t.j...d
-00000ad0: 0974 006a 0b93 0164 0a74 006a 0c93 0164  .t.j...d.t.j...d
-00000ae0: 0b74 006a 0d93 0164 0c74 006a 0e93 0164  .t.j...d.t.j...d
-00000af0: 0d74 006a 0f93 0164 0e74 006a 1093 0164  .t.j...d.t.j...d
-00000b00: 0f7c 006a 116a 1293 0164 1074 006a 1393  .|.j.j...d.t.j..
-00000b10: 0164 117c 006a 116a 1493 0164 127c 006a  .d.|.j.j...d.|.j
-00000b20: 116a 1593 0164 137c 006a 116a 1693 0164  .j...d.|.j.j...d
-00000b30: 1474 006a 1793 0164 1574 006a 1893 0164  .t.j...d.t.j...d
-00000b40: 1674 006a 1993 0164 1774 1a74 006a 1b83  .t.j...d.t.t.j..
-00000b50: 0193 0164 1874 006a 1c93 0164 1974 006a  ...d.t.j...d.t.j
-00000b60: 1d93 0164 1a74 006a 1e93 0164 1b74 006a  ...d.t.j...d.t.j
-00000b70: 1f93 0164 1c74 006a 2093 0164 1d74 006a  ...d.t.j ..d.t.j
-00000b80: 2193 0164 1e74 006a 2293 0164 1f74 006a  !..d.t.j"..d.t.j
-00000b90: 2393 0164 2074 006a 2493 0164 2174 006a  #..d t.j$..d!t.j
-00000ba0: 2593 0164 2274 006a 2693 0164 2374 006a  %..d"t.j&..d#t.j
-00000bb0: 2793 0164 2474 006a 2893 0164 2574 006a  '..d$t.j(..d%t.j
-00000bc0: 2993 0164 2674 006a 2a93 0164 2774 006a  )..d&t.j*..d't.j
-00000bd0: 2b93 0164 2874 006a 2c93 0164 2974 006a  +..d(t.j,..d)t.j
-00000be0: 2d93 0164 2a74 006a 2e93 0164 2b74 006a  -..d*t.j...d+t.j
-00000bf0: 2f93 0164 2c74 006a 3093 0164 2d74 006a  /..d,t.j0..d-t.j
-00000c00: 3193 0164 2e74 006a 3293 0164 2f74 006a  1..d.t.j2..d/t.j
-00000c10: 3393 0164 3074 006a 3493 0164 3174 006a  3..d0t.j4..d1t.j
-00000c20: 3593 018e 0101 0064 0053 0029 324e da04  5......d.S.)2N..
-00000c30: 7965 7272 da05 785f 6572 72da 0665 636f  yerr..x_err..eco
-00000c40: 6c6f 72da 0a65 6c69 6e65 7769 6474 68da  lor..elinewidth.
-00000c50: 0763 6170 7369 7a65 da09 6261 7273 6162  .capsize..barsab
-00000c60: 6f76 65da 066c 6f6c 696d 73da 0675 706c  ove..lolims..upl
-00000c70: 696d 73da 0778 6c6f 6c69 6d73 da07 7875  ims..xlolims..xu
-00000c80: 706c 696d 73da 0a65 7272 6f72 6576 6572  plims..errorever
-00000c90: 79da 0863 6170 7468 6963 6b72 2900 0000  y..capthickr)...
-00000ca0: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
-00000cb0: 2d00 0000 722e 0000 0072 2f00 0000 7230  -...r....r/...r0
-00000cc0: 0000 0072 3100 0000 7232 0000 0072 3400  ...r1...r2...r4.
-00000cd0: 0000 7233 0000 0072 3500 0000 7236 0000  ..r3...r5...r6..
-00000ce0: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
-00000cf0: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
-00000d00: 3d00 0000 723e 0000 0072 3f00 0000 7240  =...r>...r?...r@
-00000d10: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
-00000d20: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
-00000d30: 0072 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
-00000d40: da09 7472 616e 7366 6f72 6d72 4a00 0000  ..transformrJ...
-00000d50: 724b 0000 0072 4c00 0000 2936 7228 0000  rK...rL...)6r(..
-00000d60: 0072 4d00 0000 724e 0000 0072 5000 0000  .rM...rN...rP...
-00000d70: 7251 0000 0072 5200 0000 7253 0000 0072  rQ...rR...rS...r
-00000d80: 5400 0000 7255 0000 0072 5600 0000 7257  T...rU...rV...rW
-00000d90: 0000 0072 5800 0000 7259 0000 0072 5a00  ...rX...rY...rZ.
-00000da0: 0000 725b 0000 0072 2900 0000 722a 0000  ..r[...r)...r*..
-00000db0: 0072 1700 0000 722b 0000 0072 2c00 0000  .r....r+...r,...
-00000dc0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-00000dd0: 3000 0000 7231 0000 0072 3200 0000 724f  0...r1...r2...rO
-00000de0: 0000 0072 3400 0000 7233 0000 0072 3500  ...r4...r3...r5.
-00000df0: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-00000e00: 0072 3900 0000 723a 0000 0072 3b00 0000  .r9...r:...r;...
-00000e10: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
-00000e20: 3f00 0000 7240 0000 0072 4100 0000 7242  ?...r@...rA...rB
-00000e30: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
-00000e40: 0000 7246 0000 0072 4700 0000 7248 0000  ..rF...rG...rH..
-00000e50: 0072 4900 0000 725c 0000 0072 4a00 0000  .rI...r\...rJ...
-00000e60: 724b 0000 0072 4c00 0000 a902 7219 0000  rK...rL.....r...
-00000e70: 0072 2700 0000 7212 0000 0072 1200 0000  .r'...r....r....
-00000e80: 7213 0000 0072 0e00 0000 4e00 0000 73ca  r....r....N...s.
-00000e90: 0000 0006 0104 0106 ff06 0202 fe06 0302  ................
-00000ea0: fd06 0402 fc06 0502 fb06 0602 fa06 0702  ................
-00000eb0: f906 0802 f806 0902 f706 0a02 f606 0b02  ................
-00000ec0: f506 0c02 f406 0d02 f306 0e02 f206 0f02  ................
-00000ed0: f108 1002 f006 1102 ef08 1202 ee08 1302  ................
-00000ee0: ed08 1402 ec06 1502 eb06 1602 ea06 1702  ................
-00000ef0: e90a 1802 e806 1902 e706 1a02 e606 1b02  ................
-00000f00: e506 1c02 e406 1d02 e306 1e02 e206 1f02  ................
-00000f10: e106 2002 e006 2102 df06 2202 de06 2302  .. ...!..."...#.
-00000f20: dd06 2402 dc06 2502 db06 2602 da06 2702  ..$...%...&...'.
-00000f30: d906 2802 d806 2902 d706 2a02 d606 2b02  ..(...)...*...+.
-00000f40: d506 2c02 d406 2d02 d306 2e02 d206 2f02  ..,...-......./.
-00000f50: d106 3002 d006 3102 cf06 3208 ce7a 1850  ..0...1...2..z.P
-00000f60: 6c6f 744c 696e 6573 2e70 6c6f 745f 6572  lotLines.plot_er
-00000f70: 726f 7262 6172 7363 0200 0000 0000 0000  rorbarsc........
-00000f80: 0000 0000 0200 0000 0f00 0000 4300 0000  ............C...
-00000f90: 7340 0000 007c 0174 006a 0174 006a 0274  s@...|.t.j.t.j.t
-00000fa0: 006a 0374 006a 0474 006a 0574 006a 0674  .j.t.j.t.j.t.j.t
-00000fb0: 006a 0774 006a 0874 006a 0974 006a 0a74  .j.t.j.t.j.t.j.t
-00000fc0: 006a 0b74 006a 0c74 006a 0d64 018d 0d01  .j.t.j.t.j.d....
-00000fd0: 0064 0053 0029 024e 290b da01 73da 0163  .d.S.).N)...s..c
-00000fe0: 723c 0000 00da 0463 6d61 70da 046e 6f72  r<.....cmap..nor
-00000ff0: 6dda 0476 6d69 6eda 0476 6d61 7872 2a00  m..vmin..vmaxr*.
-00001000: 0000 da0a 6c69 6e65 7769 6474 6873 da0a  ....linewidths..
-00001010: 6564 6765 636f 6c6f 7273 da0d 706c 6f74  edgecolors..plot
-00001020: 6e6f 6e66 696e 6974 6529 0e72 2800 0000  nonfinite).r(...
-00001030: 724d 0000 0072 4e00 0000 7241 0000 0072  rM...rN...rA...r
-00001040: 3000 0000 723c 0000 0072 6000 0000 7261  0...r<...r`...ra
-00001050: 0000 0072 6200 0000 7263 0000 0072 2a00  ...rb...rc...r*.
-00001060: 0000 7264 0000 0072 6500 0000 7266 0000  ..rd...re...rf..
-00001070: 0072 5d00 0000 7212 0000 0072 1200 0000  .r]...r....r....
-00001080: 7213 0000 0072 0f00 0000 8300 0000 731c  r....r........s.
-00001090: 0000 0006 0104 0104 0104 0104 0104 0104  ................
-000010a0: 0104 0104 0104 0104 0104 0104 010a f47a  ...............z
-000010b0: 1650 6c6f 744c 696e 6573 2e70 6c6f 745f  .PlotLines.plot_
-000010c0: 7363 6174 7465 7263 0100 0000 0000 0000  scatterc........
-000010d0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-000010e0: 721c 0000 0072 1500 0000 2902 da0b 6164  r....r....)...ad
-000010f0: 645f 785f 6c61 6265 6cda 0b61 6464 5f79  d_x_label..add_y
-00001100: 5f6c 6162 656c 721f 0000 0072 1200 0000  _labelr....r....
-00001110: 7212 0000 0072 1300 0000 da0f 6164 645f  r....r......add_
-00001120: 6178 6973 5f6c 6162 656c 7392 0000 0072  axis_labels....r
-00001130: 2100 0000 7a19 506c 6f74 4c69 6e65 732e  !...z.PlotLines.
-00001140: 6164 645f 6178 6973 5f6c 6162 656c 734e  add_axis_labelsN
-00001150: 290d da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00001160: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001170: 6e61 6d65 5f5f da0b 636c 6173 736d 6574  name__..classmet
-00001180: 686f 6472 1400 0000 7216 0000 0072 2000  hodr....r....r .
-00001190: 0000 721d 0000 0072 2200 0000 720d 0000  ..r....r"...r...
-000011a0: 0072 0e00 0000 720f 0000 0072 6900 0000  .r....r....ri...
-000011b0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000011c0: 1300 0000 7206 0000 0007 0000 0073 1600  ....r........s..
-000011d0: 0000 0800 0202 0a01 0808 0805 0804 0806  ................
-000011e0: 0805 0828 0835 0c0f 7206 0000 0029 0bda  ...(.5..r....)..
-000011f0: 116d 6174 706c 6f74 6c69 622e 7079 706c  .matplotlib.pypl
-00001200: 6f74 da06 7079 706c 6f74 da03 706c 74da  ot..pyplot..plt.
-00001210: 056e 756d 7079 da02 6e70 da00 7203 0000  .numpy..np..r...
-00001220: 00da 0e70 6c6f 7474 7970 6573 2e70 6c6f  ...plottypes.plo
-00001230: 7472 0500 0000 7206 0000 00da 046c 6f61  tr....r......loa
-00001240: 6472 1200 0000 7212 0000 0072 1200 0000  dr....r....r....
-00001250: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00001260: 0000 0073 0e00 0000 0c00 0801 0c02 0c01  ...s............
-00001270: 1002 007f 0e10                           ......
+000001e0: 73a9 0072 1200 0000 fa5b 2f68 6f6d 652f  s..r.....[/home/
+000001f0: 6865 6e72 792f 2e6c 6f63 616c 2f6c 6962  henry/.local/lib
+00000200: 2f70 7974 686f 6e33 2e31 302f 7369 7465  /python3.10/site
+00000210: 2d70 6163 6b61 6765 732f 6867 7574 696c  -packages/hgutil
+00000220: 6974 6965 732f 706c 6f74 7469 6e67 2f70  ities/plotting/p
+00000230: 6c6f 7474 7970 6573 2f70 6c6f 746c 696e  lottypes/plotlin
+00000240: 6573 2e70 79da 1173 6574 5f66 756e 6374  es.py..set_funct
+00000250: 696f 6e5f 6469 6374 0900 0000 730e 0000  ion_dict....s...
+00000260: 0004 0204 0104 0104 0104 0104 010c fb7a  ...............z
+00000270: 1b50 6c6f 744c 696e 6573 2e73 6574 5f66  .PlotLines.set_f
+00000280: 756e 6374 696f 6e5f 6469 6374 6304 0000  unction_dictc...
+00000290: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000002a0: 004b 0000 0073 2e00 0000 7400 6a01 7c00  .K...s....t.j.|.
+000002b0: 7c01 7c02 7c03 6604 6900 7c04 a401 8e01  |.|.|.f.i.|.....
+000002c0: 0100 7c03 7c00 5f02 7403 a004 7c00 7c04  ..|.|._.t...|.|.
+000002d0: a102 0100 6400 5300 a901 4e29 0572 0500  ....d.S...N).r..
+000002e0: 0000 da08 5f5f 696e 6974 5f5f da09 6c69  ....__init__..li
+000002f0: 6e65 735f 6f62 6a72 0300 0000 da06 6b77  nes_objr......kw
+00000300: 6172 6773 2905 da04 7365 6c66 da0a 6669  args)...self..fi
+00000310: 6775 7265 5f6f 626a da02 6178 7217 0000  gure_obj..axr...
+00000320: 0072 1800 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000330: 7213 0000 0072 1600 0000 1200 0000 7306  r....r........s.
+00000340: 0000 0018 0106 0110 017a 1250 6c6f 744c  .........z.PlotL
+00000350: 696e 6573 2e5f 5f69 6e69 745f 5f63 0100  ines.__init__c..
+00000360: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000370: 0000 4300 0000 7324 0000 007c 00a0 00a1  ..C...s$...|....
+00000380: 0001 007c 00a0 01a1 0001 007c 00a0 02a1  ...|.......|....
+00000390: 0001 007c 00a0 03a1 0001 0064 0053 0072  ...|.......d.S.r
+000003a0: 1500 0000 2904 da0a 706c 6f74 5f6c 696e  ....)...plot_lin
+000003b0: 6573 da0f 7365 745f 7469 636b 5f6c 6162  es..set_tick_lab
+000003c0: 656c 73da 0f73 6574 5f61 7869 735f 6c69  els..set_axis_li
+000003d0: 6d69 7473 da0f 7365 745f 6178 6973 5f62  mits..set_axis_b
+000003e0: 6f75 6e64 73a9 0172 1900 0000 7212 0000  ounds..r....r...
+000003f0: 0072 1200 0000 7213 0000 00da 0970 6c6f  .r....r......plo
+00000400: 745f 6461 7461 1700 0000 7308 0000 0008  t_data....s.....
+00000410: 0108 0108 010c 017a 1350 6c6f 744c 696e  .......z.PlotLin
+00000420: 6573 2e70 6c6f 745f 6461 7461 6301 0000  es.plot_datac...
+00000430: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00000440: 0043 0000 0073 3600 0000 7c00 a000 a100  .C...s6...|.....
+00000450: 7d01 7401 7c00 6a02 7c00 6a03 6a04 8302  }.t.|.j.|.j.j...
+00000460: 7d02 7c00 6a03 6a05 4400 5d08 7d03 7c01  }.|.j.j.D.].}.|.
+00000470: 7c00 7c02 7c03 8303 0100 7110 6400 5300  |.|.|.....q.d.S.
+00000480: 7215 0000 0029 06da 1667 6574 5f70 6c6f  r....)...get_plo
+00000490: 745f 7479 7065 5f66 756e 6374 696f 6eda  t_type_function.
+000004a0: 0767 6574 6174 7472 721b 0000 0072 1700  .getattrr....r..
+000004b0: 0000 da09 706c 6f74 5f74 7970 65da 0c6c  ....plot_type..l
+000004c0: 696e 655f 6f62 6a65 6374 7329 0472 1900  ine_objects).r..
+000004d0: 0000 da12 706c 6f74 5f74 7970 655f 6675  ....plot_type_fu
+000004e0: 6e63 7469 6f6e da0d 706c 6f74 5f66 756e  nction..plot_fun
+000004f0: 6374 696f 6eda 086c 696e 655f 6f62 6a72  ction..line_objr
+00000500: 1200 0000 7212 0000 0072 1300 0000 721c  ....r....r....r.
+00000510: 0000 001d 0000 0073 0a00 0000 0801 1001  .......s........
+00000520: 0c01 0e01 04ff 7a14 506c 6f74 4c69 6e65  ......z.PlotLine
+00000530: 732e 706c 6f74 5f6c 696e 6573 6301 0000  s.plot_linesc...
+00000540: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00000550: 0043 0000 0073 1600 0000 7c00 6a00 6a01  .C...s....|.j.j.
+00000560: 7d01 7c00 6a02 7c01 1900 7d02 7c02 5300  }.|.j.|...}.|.S.
+00000570: 7215 0000 0029 0372 1700 0000 7224 0000  r....).r....r$..
+00000580: 0072 1000 0000 2903 7219 0000 0072 2400  .r....).r....r$.
+00000590: 0000 7226 0000 0072 1200 0000 7212 0000  ..r&...r....r...
+000005a0: 0072 1300 0000 7222 0000 0023 0000 0073  .r....r"...#...s
+000005b0: 0600 0000 0801 0a01 0401 7a20 506c 6f74  ..........z Plot
+000005c0: 4c69 6e65 732e 6765 745f 706c 6f74 5f74  Lines.get_plot_t
+000005d0: 7970 655f 6675 6e63 7469 6f6e 6303 0000  ype_functionc...
+000005e0: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+000005f0: 0043 0000 0073 4201 0000 7c01 7c02 6a00  .C...sB...|.|.j.
+00000600: 7c02 6a01 6602 6900 6401 7c02 6a02 9301  |.j.f.i.d.|.j...
+00000610: 6402 7c02 6a03 9301 6403 7c00 6a04 6a05  d.|.j...d.|.j.j.
+00000620: 9301 6404 7c02 6a06 9301 6405 7c00 6a04  ..d.|.j...d.|.j.
+00000630: 6a07 9301 6406 7c00 6a04 6a08 9301 6407  j...d.|.j.j...d.
+00000640: 7c00 6a04 6a09 9301 6408 7c02 6a0a 9301  |.j.j...d.|.j...
+00000650: 6409 7c02 6a0b 9301 640a 7c02 6a0c 9301  d.|.j...d.|.j...
+00000660: 640b 7c02 6a0d 9301 640c 740e 7c02 6a0f  d.|.j...d.t.|.j.
+00000670: 8301 9301 640d 7c02 6a10 9301 640e 7c02  ....d.|.j...d.|.
+00000680: 6a11 9301 640f 7c02 6a12 9301 6410 7c02  j...d.|.j...d.|.
+00000690: 6a13 9301 6411 7c02 6a14 9301 6412 7c02  j...d.|.j...d.|.
+000006a0: 6a15 9301 6413 7c02 6a16 9301 6414 7c02  j...d.|.j...d.|.
+000006b0: 6a17 9301 6415 7c02 6a18 9301 6416 7c02  j...d.|.j...d.|.
+000006c0: 6a19 9301 6417 7c02 6a1a 9301 6418 7c02  j...d.|.j...d.|.
+000006d0: 6a1b 9301 6419 7c02 6a1c 9301 641a 7c02  j...d.|.j...d.|.
+000006e0: 6a1d 9301 641b 7c02 6a1e 9301 641c 7c02  j...d.|.j...d.|.
+000006f0: 6a1f 9301 641d 7c02 6a20 9301 641e 7c02  j...d.|.j ..d.|.
+00000700: 6a21 9301 641f 7c02 6a22 9301 6420 7c02  j!..d.|.j"..d |.
+00000710: 6a23 9301 6421 7c02 6a24 9301 6422 7c02  j#..d!|.j$..d"|.
+00000720: 6a25 9301 6423 7c02 6a26 9301 6424 7c02  j%..d#|.j&..d$|.
+00000730: 6a27 9301 8e01 0100 6400 5300 2925 4eda  j'......d.S.)%N.
+00000740: 0a61 6767 5f66 696c 7465 72da 0561 6c70  .agg_filter..alp
+00000750: 6861 da08 616e 696d 6174 6564 da0b 616e  ha..animated..an
+00000760: 7469 616c 6961 7365 64da 0863 6c69 705f  tialiased..clip_
+00000770: 626f 78da 0763 6c69 705f 6f6e da09 636c  box..clip_on..cl
+00000780: 6970 5f70 6174 68da 0563 6f6c 6f72 da0d  ip_path..color..
+00000790: 6461 7368 5f63 6170 7374 796c 65da 0e64  dash_capstyle..d
+000007a0: 6173 685f 6a6f 696e 7374 796c 65da 0964  ash_joinstyle..d
+000007b0: 7261 7773 7479 6c65 da06 6461 7368 6573  rawstyle..dashes
+000007c0: da09 6669 6c6c 7374 796c 65da 0867 6170  ..fillstyle..gap
+000007d0: 636f 6c6f 72da 0367 6964 da09 696e 5f6c  color..gid..in_l
+000007e0: 6179 6f75 74da 056c 6162 656c da09 6c69  ayout..label..li
+000007f0: 6e65 7374 796c 65da 096c 696e 6577 6964  nestyle..linewid
+00000800: 7468 da06 6d61 726b 6572 da0f 6d61 726b  th..marker..mark
+00000810: 6572 6564 6765 636f 6c6f 72da 0f6d 6172  eredgecolor..mar
+00000820: 6b65 7265 6467 6577 6964 7468 da0f 6d61  keredgewidth..ma
+00000830: 726b 6572 6661 6365 636f 6c6f 72da 126d  rkerfacecolor..m
+00000840: 6172 6b65 7266 6163 6563 6f6c 6f72 616c  arkerfacecoloral
+00000850: 74da 0a6d 6172 6b65 7273 697a 65da 096d  t..markersize..m
+00000860: 6172 6b65 7665 7279 da09 6d6f 7573 656f  arkevery..mouseo
+00000870: 7665 72da 0c70 6174 685f 6566 6665 6374  ver..path_effect
+00000880: 73da 0a72 6173 7465 7269 7a65 64da 0d73  s..rasterized..s
+00000890: 6b65 7463 685f 7061 7261 6d73 da04 736e  ketch_params..sn
+000008a0: 6170 da0e 736f 6c69 645f 6361 7073 7479  ap..solid_capsty
+000008b0: 6c65 da0f 736f 6c69 645f 6a6f 696e 7374  le..solid_joinst
+000008c0: 796c 65da 0375 726c da07 7669 7369 626c  yle..url..visibl
+000008d0: 65da 067a 6f72 6465 7229 28da 0878 5f76  e..zorder)(..x_v
+000008e0: 616c 7565 73da 0879 5f76 616c 7565 7372  alues..y_valuesr
+000008f0: 2900 0000 722a 0000 0072 1700 0000 722b  )...r*...r....r+
+00000900: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00000910: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
+00000920: 0072 3200 0000 7233 0000 00da 0574 7570  .r2...r3.....tup
+00000930: 6c65 7234 0000 0072 3500 0000 7236 0000  ler4...r5...r6..
+00000940: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
+00000950: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
+00000960: 3d00 0000 723e 0000 0072 3f00 0000 7240  =...r>...r?...r@
+00000970: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
+00000980: 0000 7244 0000 0072 4500 0000 7246 0000  ..rD...rE...rF..
+00000990: 0072 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
+000009a0: 724a 0000 0072 4b00 0000 724c 0000 0029  rJ...rK...rL...)
+000009b0: 0372 1900 0000 7227 0000 0072 2800 0000  .r....r'...r(...
+000009c0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000009d0: 0d00 0000 2800 0000 7396 0000 0006 0104  ....(...s.......
+000009e0: 0106 ff06 0202 fe06 0302 fd08 0402 fc06  ................
+000009f0: 0502 fb08 0602 fa08 0702 f908 0802 f806  ................
+00000a00: 0902 f706 0a02 f606 0b02 f506 0c02 f40a  ................
+00000a10: 0d02 f306 0e02 f206 0f02 f106 1002 f006  ................
+00000a20: 1102 ef06 1202 ee06 1302 ed06 1402 ec06  ................
+00000a30: 1502 eb06 1602 ea06 1702 e906 1802 e806  ................
+00000a40: 1902 e706 1a02 e606 1b02 e506 1c02 e406  ................
+00000a50: 1d02 e306 1e02 e206 1f02 e106 2002 e006  ............ ...
+00000a60: 2102 df06 2202 de06 2302 dd06 2402 dc06  !..."...#...$...
+00000a70: 2508 db7a 1650 6c6f 744c 696e 6573 2e70  %..z.PlotLines.p
+00000a80: 6c6f 745f 7265 6775 6c61 7263 0200 0000  lot_regularc....
+00000a90: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000aa0: 4300 0000 73aa 0100 007c 0174 006a 0174  C...s....|.t.j.t
+00000ab0: 006a 0266 0269 0064 0174 006a 0393 0164  .j.f.i.d.t.j...d
+00000ac0: 0274 006a 0493 0164 0374 006a 0593 0164  .t.j...d.t.j...d
+00000ad0: 0474 006a 0693 0164 0574 006a 0793 0164  .t.j...d.t.j...d
+00000ae0: 0674 006a 0893 0164 0774 006a 0993 0164  .t.j...d.t.j...d
+00000af0: 0874 006a 0a93 0164 0974 006a 0b93 0164  .t.j...d.t.j...d
+00000b00: 0a74 006a 0c93 0164 0b74 006a 0d93 0164  .t.j...d.t.j...d
+00000b10: 0c74 006a 0e93 0164 0d74 006a 0f93 0164  .t.j...d.t.j...d
+00000b20: 0e74 006a 1093 0164 0f7c 006a 116a 1293  .t.j...d.|.j.j..
+00000b30: 0164 1074 006a 1393 0164 117c 006a 116a  .d.t.j...d.|.j.j
+00000b40: 1493 0164 127c 006a 116a 1593 0164 137c  ...d.|.j.j...d.|
+00000b50: 006a 116a 1693 0164 1474 006a 1793 0164  .j.j...d.t.j...d
+00000b60: 1574 006a 1893 0164 1674 006a 1993 0164  .t.j...d.t.j...d
+00000b70: 1774 1a74 006a 1b83 0193 0164 1874 006a  .t.t.j.....d.t.j
+00000b80: 1c93 0164 1974 006a 1d93 0164 1a74 006a  ...d.t.j...d.t.j
+00000b90: 1e93 0164 1b74 006a 1f93 0164 1c74 006a  ...d.t.j...d.t.j
+00000ba0: 2093 0164 1d74 006a 2193 0164 1e74 006a   ..d.t.j!..d.t.j
+00000bb0: 2293 0164 1f74 006a 2393 0164 2074 006a  "..d.t.j#..d t.j
+00000bc0: 2493 0164 2174 006a 2593 0164 2274 006a  $..d!t.j%..d"t.j
+00000bd0: 2693 0164 2374 006a 2793 0164 2474 006a  &..d#t.j'..d$t.j
+00000be0: 2893 0164 2574 006a 2993 0164 2674 006a  (..d%t.j)..d&t.j
+00000bf0: 2a93 0164 2774 006a 2b93 0164 2874 006a  *..d't.j+..d(t.j
+00000c00: 2c93 0164 2974 006a 2d93 0164 2a74 006a  ,..d)t.j-..d*t.j
+00000c10: 2e93 0164 2b74 006a 2f93 0164 2c74 006a  ...d+t.j/..d,t.j
+00000c20: 3093 0164 2d74 006a 3193 0164 2e74 006a  0..d-t.j1..d.t.j
+00000c30: 3293 0164 2f74 006a 3393 0164 3074 006a  2..d/t.j3..d0t.j
+00000c40: 3493 0164 3174 006a 3593 018e 0101 0064  4..d1t.j5......d
+00000c50: 0053 0029 324e da04 7965 7272 da05 785f  .S.)2N..yerr..x_
+00000c60: 6572 72da 0665 636f 6c6f 72da 0a65 6c69  err..ecolor..eli
+00000c70: 6e65 7769 6474 68da 0763 6170 7369 7a65  newidth..capsize
+00000c80: da09 6261 7273 6162 6f76 65da 066c 6f6c  ..barsabove..lol
+00000c90: 696d 73da 0675 706c 696d 73da 0778 6c6f  ims..uplims..xlo
+00000ca0: 6c69 6d73 da07 7875 706c 696d 73da 0a65  lims..xuplims..e
+00000cb0: 7272 6f72 6576 6572 79da 0863 6170 7468  rrorevery..capth
+00000cc0: 6963 6b72 2900 0000 722a 0000 0072 2b00  ickr)...r*...r+.
+00000cd0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00000ce0: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
+00000cf0: 7232 0000 0072 3400 0000 7233 0000 0072  r2...r4...r3...r
+00000d00: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000d10: 0000 0072 3900 0000 723a 0000 0072 3b00  ...r9...r:...r;.
+00000d20: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00000d30: 0072 3f00 0000 7240 0000 0072 4100 0000  .r?...r@...rA...
+00000d40: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+00000d50: 4500 0000 7246 0000 0072 4700 0000 7248  E...rF...rG...rH
+00000d60: 0000 0072 4900 0000 da09 7472 616e 7366  ...rI.....transf
+00000d70: 6f72 6d72 4a00 0000 724b 0000 0072 4c00  ormrJ...rK...rL.
+00000d80: 0000 2936 7228 0000 0072 4d00 0000 724e  ..)6r(...rM...rN
+00000d90: 0000 0072 5000 0000 7251 0000 0072 5200  ...rP...rQ...rR.
+00000da0: 0000 7253 0000 0072 5400 0000 7255 0000  ..rS...rT...rU..
+00000db0: 0072 5600 0000 7257 0000 0072 5800 0000  .rV...rW...rX...
+00000dc0: 7259 0000 0072 5a00 0000 725b 0000 0072  rY...rZ...r[...r
+00000dd0: 2900 0000 722a 0000 0072 1700 0000 722b  )...r*...r....r+
+00000de0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00000df0: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
+00000e00: 0072 3200 0000 724f 0000 0072 3400 0000  .r2...rO...r4...
+00000e10: 7233 0000 0072 3500 0000 7236 0000 0072  r3...r5...r6...r
+00000e20: 3700 0000 7238 0000 0072 3900 0000 723a  7...r8...r9...r:
+00000e30: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
+00000e40: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
+00000e50: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
+00000e60: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
+00000e70: 4700 0000 7248 0000 0072 4900 0000 725c  G...rH...rI...r\
+00000e80: 0000 0072 4a00 0000 724b 0000 0072 4c00  ...rJ...rK...rL.
+00000e90: 0000 a902 7219 0000 0072 2700 0000 7212  ....r....r'...r.
+00000ea0: 0000 0072 1200 0000 7213 0000 0072 0e00  ...r....r....r..
+00000eb0: 0000 5000 0000 73ca 0000 0006 0104 0106  ..P...s.........
+00000ec0: ff06 0202 fe06 0302 fd06 0402 fc06 0502  ................
+00000ed0: fb06 0602 fa06 0702 f906 0802 f806 0902  ................
+00000ee0: f706 0a02 f606 0b02 f506 0c02 f406 0d02  ................
+00000ef0: f306 0e02 f206 0f02 f108 1002 f006 1102  ................
+00000f00: ef08 1202 ee08 1302 ed08 1402 ec06 1502  ................
+00000f10: eb06 1602 ea06 1702 e90a 1802 e806 1902  ................
+00000f20: e706 1a02 e606 1b02 e506 1c02 e406 1d02  ................
+00000f30: e306 1e02 e206 1f02 e106 2002 e006 2102  .......... ...!.
+00000f40: df06 2202 de06 2302 dd06 2402 dc06 2502  .."...#...$...%.
+00000f50: db06 2602 da06 2702 d906 2802 d806 2902  ..&...'...(...).
+00000f60: d706 2a02 d606 2b02 d506 2c02 d406 2d02  ..*...+...,...-.
+00000f70: d306 2e02 d206 2f02 d106 3002 d006 3102  ....../...0...1.
+00000f80: cf06 3208 ce7a 1850 6c6f 744c 696e 6573  ..2..z.PlotLines
+00000f90: 2e70 6c6f 745f 6572 726f 7262 6172 7363  .plot_errorbarsc
+00000fa0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000fb0: 0f00 0000 4300 0000 7340 0000 007c 0174  ....C...s@...|.t
+00000fc0: 006a 0174 006a 0274 006a 0374 006a 0474  .j.t.j.t.j.t.j.t
+00000fd0: 006a 0574 006a 0674 006a 0774 006a 0874  .j.t.j.t.j.t.j.t
+00000fe0: 006a 0974 006a 0a74 006a 0b74 006a 0c74  .j.t.j.t.j.t.j.t
+00000ff0: 006a 0d64 018d 0d01 0064 0053 0029 024e  .j.d.....d.S.).N
+00001000: 290b da01 73da 0163 723c 0000 00da 0463  )...s..cr<.....c
+00001010: 6d61 70da 046e 6f72 6dda 0476 6d69 6eda  map..norm..vmin.
+00001020: 0476 6d61 7872 2a00 0000 da0a 6c69 6e65  .vmaxr*.....line
+00001030: 7769 6474 6873 da0a 6564 6765 636f 6c6f  widths..edgecolo
+00001040: 7273 da0d 706c 6f74 6e6f 6e66 696e 6974  rs..plotnonfinit
+00001050: 6529 0e72 2800 0000 724d 0000 0072 4e00  e).r(...rM...rN.
+00001060: 0000 7241 0000 0072 3000 0000 723c 0000  ..rA...r0...r<..
+00001070: 0072 6000 0000 7261 0000 0072 6200 0000  .r`...ra...rb...
+00001080: 7263 0000 0072 2a00 0000 7264 0000 0072  rc...r*...rd...r
+00001090: 6500 0000 7266 0000 0072 5d00 0000 7212  e...rf...r]...r.
+000010a0: 0000 0072 1200 0000 7213 0000 0072 0f00  ...r....r....r..
+000010b0: 0000 8500 0000 731c 0000 0006 0104 0104  ......s.........
+000010c0: 0104 0104 0104 0104 0104 0104 0104 0104  ................
+000010d0: 0104 0104 010a f47a 1650 6c6f 744c 696e  .......z.PlotLin
+000010e0: 6573 2e70 6c6f 745f 7363 6174 7465 7263  es.plot_scatterc
+000010f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001100: 0200 0000 4300 0000 7314 0000 007c 00a0  ....C...s....|..
+00001110: 00a1 0001 007c 00a0 01a1 0001 0064 0053  .....|.......d.S
+00001120: 0072 1500 0000 2902 da0b 6164 645f 785f  .r....)...add_x_
+00001130: 6c61 6265 6cda 0b61 6464 5f79 5f6c 6162  label..add_y_lab
+00001140: 656c 7220 0000 0072 1200 0000 7212 0000  elr ...r....r...
+00001150: 0072 1300 0000 da0f 6164 645f 6178 6973  .r......add_axis
+00001160: 5f6c 6162 656c 7394 0000 0073 0400 0000  _labels....s....
+00001170: 0801 0c01 7a19 506c 6f74 4c69 6e65 732e  ....z.PlotLines.
+00001180: 6164 645f 6178 6973 5f6c 6162 656c 734e  add_axis_labelsN
+00001190: 290d da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000011a0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000011b0: 6e61 6d65 5f5f da0b 636c 6173 736d 6574  name__..classmet
+000011c0: 686f 6472 1400 0000 7216 0000 0072 2100  hodr....r....r!.
+000011d0: 0000 721c 0000 0072 2200 0000 720d 0000  ..r....r"...r...
+000011e0: 0072 0e00 0000 720f 0000 0072 6900 0000  .r....r....ri...
+000011f0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00001200: 1300 0000 7206 0000 0007 0000 0073 1600  ....r........s..
+00001210: 0000 0800 0202 0a01 0808 0805 0806 0806  ................
+00001220: 0805 0828 0835 0c0f 7206 0000 0029 0bda  ...(.5..r....)..
+00001230: 116d 6174 706c 6f74 6c69 622e 7079 706c  .matplotlib.pypl
+00001240: 6f74 da06 7079 706c 6f74 da03 706c 74da  ot..pyplot..plt.
+00001250: 056e 756d 7079 da02 6e70 da00 7203 0000  .numpy..np..r...
+00001260: 00da 0e70 6c6f 7474 7970 6573 2e70 6c6f  ...plottypes.plo
+00001270: 7472 0500 0000 7206 0000 00da 046c 6f61  tr....r......loa
+00001280: 6472 1200 0000 7212 0000 0072 1200 0000  dr....r....r....
+00001290: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000012a0: 0000 0073 0e00 0000 0c00 0801 0c02 0c01  ...s............
+000012b0: 1002 007f 0e12                           ......
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotbars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotlines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 18 19:06:03 2023 UTC, .py size: 1429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,111 @@
-00000000: 6f0d 0d0a 0000 0000 9b55 8f64 9505 0000  o........U.d....
+00000000: 6f0d 0d0a 0000 0000 5160 9064 fd06 0000  o.......Q`.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
+00000020: 0002 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 6d02 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6403 8400 5a04 6404 6405 8400  ..d.d...Z.d.d...
 00000050: 5a05 6406 6407 8400 5a06 6408 6409 8400  Z.d.d...Z.d.d...
 00000060: 5a07 640a 640b 8400 5a08 640c 640d 8400  Z.d.d...Z.d.d...
-00000070: 5a09 6401 5300 290e e900 0000 004e 6301  Z.d.S.)......Nc.
-00000080: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000090: 0000 0043 0000 0073 2400 0000 7400 7c00  ...C...s$...t.|.
-000000a0: 8301 7d01 7c00 6a01 7d02 7402 7c01 7c02  ..}.|.j.}.t.|.|.
-000000b0: 8302 0100 7403 a004 a100 0100 6400 5300  ....t.......d.S.
-000000c0: 2901 4e29 05da 0f67 6574 5f66 6967 7572  ).N)...get_figur
-000000d0: 655f 7061 7468 da0b 6669 6775 7265 735f  e_path..figures_
-000000e0: 6f62 6ada 0873 6176 655f 6669 67da 0370  obj..save_fig..p
-000000f0: 6c74 da05 636c 6f73 6529 03da 0a66 6967  lt..close)...fig
-00000100: 7572 655f 6f62 6ada 0470 6174 6872 0300  ure_obj..pathr..
-00000110: 0000 a900 7209 0000 00fa 6a2f 6d6e 742f  ....r.....j/mnt/
-00000120: 3254 422f 446f 6375 6d65 6e74 732f 5079  2TB/Documents/Py
-00000130: 7468 6f6e 2f52 6561 6c20 576f 726c 6420  thon/Real World 
-00000140: 4170 706c 6963 6174 696f 6e73 2f68 6775  Applications/hgu
-00000150: 7469 6c69 7469 6573 2f68 6775 7469 6c69  tilities/hgutili
-00000160: 7469 6573 2f70 6c6f 7474 696e 672f 706c  ties/plotting/pl
-00000170: 6f74 7574 696c 732f 7361 7665 6669 6775  otutils/savefigu
-00000180: 7265 2e70 79da 0b73 6176 655f 6669 6775  re.py..save_figu
-00000190: 7265 0500 0000 7308 0000 0008 0106 010a  re....s.........
-000001a0: 010c 0172 0b00 0000 6301 0000 0000 0000  ...r....c.......
-000001b0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-000001c0: 0073 3000 0000 7400 7c00 8301 7d01 7c01  .s0...t.|...}.|.
-000001d0: 9b00 6401 7c00 6a01 6a02 9b00 9d03 7d01  ..d.|.j.j.....}.
-000001e0: 7403 6a04 a005 7c00 6a01 6a04 7c01 a102  t.j...|.j.j.|...
-000001f0: 7d02 7c02 5300 2902 4eda 012e 2906 da0d  }.|.S.).N...)...
-00000200: 6765 745f 6669 6c65 5f6e 616d 6572 0300  get_file_namer..
-00000210: 0000 da06 666f 726d 6174 da02 6f73 7208  ....format..osr.
-00000220: 0000 00da 046a 6f69 6e29 0372 0700 0000  .....join).r....
-00000230: da09 6669 6c65 5f6e 616d 6572 0800 0000  ..file_namer....
-00000240: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000250: 0200 0000 0b00 0000 7308 0000 0008 0112  ........s.......
-00000260: 0112 0104 0172 0200 0000 6301 0000 0000  .....r....c.....
-00000270: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000280: 0000 0073 2200 0000 7400 7c00 6a01 6a02  ...s"...t.|.j.j.
-00000290: 8301 6401 6b02 720d 7403 7c00 6a01 8301  ..d.k.r.t.|.j...
-000002a0: 5300 7404 7c00 8301 5300 2902 4ee9 0100  S.t.|...S.).N...
-000002b0: 0000 2905 da03 6c65 6e72 0300 0000 da12  ..)...lenr......
-000002c0: 6461 7461 5f6f 626a 6563 745f 6772 6f75  data_object_grou
-000002d0: 7073 da12 6765 745f 6261 7365 5f66 696c  ps..get_base_fil
-000002e0: 655f 6e61 6d65 da16 6765 745f 6e75 6d62  e_name..get_numb
-000002f0: 6572 6564 5f66 696c 655f 6e61 6d65 2901  ered_file_name).
-00000300: 7207 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000310: 0a00 0000 720d 0000 0011 0000 0073 0600  ....r........s..
-00000320: 0000 1001 0a01 0802 720d 0000 0063 0100  ........r....c..
-00000330: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000340: 0000 4300 0000 7318 0000 007c 006a 0064  ..C...s....|.j.d
-00000350: 0075 0072 0764 0153 0074 017c 006a 0083  .u.r.d.S.t.|.j..
-00000360: 0153 0029 024e da06 4669 6775 7265 2902  .S.).N..Figure).
-00000370: da05 7469 746c 65da 0373 7472 2901 da0b  ..title..str)...
-00000380: 6669 6775 7265 5f6f 626a 7372 0900 0000  figure_objsr....
-00000390: 7209 0000 0072 0a00 0000 7215 0000 0017  r....r....r.....
-000003a0: 0000 0073 0600 0000 0a01 0401 0a02 7215  ...s..........r.
-000003b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000003c0: 0200 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-000003d0: 0074 007c 006a 0183 017d 017c 019b 0064  .t.|.j...}.|...d
-000003e0: 017c 006a 0264 0217 009b 009d 037d 017c  .|.j.d.......}.|
-000003f0: 0153 0029 034e fa01 2072 1200 0000 2903  .S.).N.. r....).
-00000400: 7215 0000 0072 1a00 0000 da0c 6669 6775  r....r......figu
-00000410: 7265 5f69 6e64 6578 2902 7207 0000 0072  re_index).r....r
-00000420: 1100 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00000430: 0000 0072 1600 0000 1d00 0000 7306 0000  ...r........s...
-00000440: 000a 0114 0104 0172 1600 0000 6302 0000  .......r....c...
-00000450: 0000 0000 0000 0000 0002 0000 000b 0000  ................
-00000460: 0043 0000 0073 3000 0000 7400 6a01 7c00  .C...s0...t.j.|.
-00000470: 7c01 6a02 7c01 6a03 7c01 6a04 7c01 6a05  |.j.|.j.|.j.|.j.
-00000480: 7c01 6a06 7c01 6a07 7c01 6a08 7c01 6a09  |.j.|.j.|.j.|.j.
-00000490: 6401 8d09 0100 6400 5300 2902 4e29 08da  d.....d.S.).N)..
-000004a0: 0364 7069 720e 0000 00da 086d 6574 6164  .dpir......metad
-000004b0: 6174 61da 0b62 626f 785f 696e 6368 6573  ata..bbox_inches
-000004c0: da0a 7061 645f 696e 6368 6573 da09 6661  ..pad_inches..fa
-000004d0: 6365 636f 6c6f 72da 0965 6467 6563 6f6c  cecolor..edgecol
-000004e0: 6f72 da07 6261 636b 656e 6429 0a72 0500  or..backend).r..
-000004f0: 0000 da07 7361 7665 6669 6772 1d00 0000  ....savefigr....
-00000500: 720e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000510: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00000520: 0000 0029 0272 0800 0000 7203 0000 0072  ...).r....r....r
-00000530: 0900 0000 7209 0000 0072 0a00 0000 7204  ....r....r....r.
-00000540: 0000 0022 0000 0073 1400 0000 0601 0401  ..."...s........
-00000550: 0401 0401 0401 0401 0401 0401 0401 0af8  ................
-00000560: 7204 0000 0029 0a72 0f00 0000 da11 6d61  r....).r......ma
-00000570: 7470 6c6f 746c 6962 2e70 7970 6c6f 74da  tplotlib.pyplot.
-00000580: 0670 7970 6c6f 7472 0500 0000 720b 0000  .pyplotr....r...
-00000590: 0072 0200 0000 720d 0000 0072 1500 0000  .r....r....r....
-000005a0: 7216 0000 0072 0400 0000 7209 0000 0072  r....r....r....r
-000005b0: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
-000005c0: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
-000005d0: 0008 000c 0208 0208 0608 0608 0608 060c  ................
-000005e0: 05                                       .
+00000070: 5a09 640e 640f 8400 5a0a 6410 6411 8400  Z.d.d...Z.d.d...
+00000080: 5a0b 6401 5300 2912 e900 0000 004e 6301  Z.d.S.)......Nc.
+00000090: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000000a0: 0000 0043 0000 0073 2400 0000 7400 7c00  ...C...s$...t.|.
+000000b0: 8301 7d01 7c00 6a01 7d02 7402 7c01 7c02  ..}.|.j.}.t.|.|.
+000000c0: 8302 0100 7403 a004 a100 0100 6400 5300  ....t.......d.S.
+000000d0: a901 4e29 05da 0f67 6574 5f66 6967 7572  ..N)...get_figur
+000000e0: 655f 7061 7468 da0b 6669 6775 7265 735f  e_path..figures_
+000000f0: 6f62 6ada 0873 6176 655f 6669 67da 0370  obj..save_fig..p
+00000100: 6c74 da05 636c 6f73 6529 03da 0a66 6967  lt..close)...fig
+00000110: 7572 655f 6f62 6ada 0470 6174 6872 0400  ure_obj..pathr..
+00000120: 0000 a900 720a 0000 00fa 5c2f 686f 6d65  ....r.....\/home
+00000130: 2f68 656e 7279 2f2e 6c6f 6361 6c2f 6c69  /henry/.local/li
+00000140: 622f 7079 7468 6f6e 332e 3130 2f73 6974  b/python3.10/sit
+00000150: 652d 7061 636b 6167 6573 2f68 6775 7469  e-packages/hguti
+00000160: 6c69 7469 6573 2f70 6c6f 7474 696e 672f  lities/plotting/
+00000170: 706c 6f74 7574 696c 732f 7361 7665 6669  plotutils/savefi
+00000180: 6775 7265 2e70 79da 0b73 6176 655f 6669  gure.py..save_fi
+00000190: 6775 7265 0500 0000 7308 0000 0008 0106  gure....s.......
+000001a0: 010a 010c 0172 0c00 0000 6301 0000 0000  .....r....c.....
+000001b0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000001c0: 0000 00f3 1800 0000 7c00 6a00 6400 7501  ........|.j.d.u.
+000001d0: 7208 7c00 6a00 5300 7401 7c00 8301 5300  r.|.j.S.t.|...S.
+000001e0: 7202 0000 0029 0272 0900 0000 da17 6765  r....).r......ge
+000001f0: 745f 6465 6661 756c 745f 6669 6775 7265  t_default_figure
+00000200: 5f70 6174 68a9 0172 0800 0000 720a 0000  _path..r....r...
+00000210: 0072 0a00 0000 720b 0000 0072 0300 0000  .r....r....r....
+00000220: 0b00 0000 f306 0000 000a 0106 0108 0272  ...............r
+00000230: 0300 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000240: 0003 0000 0004 0000 0043 0000 0073 3000  .........C...s0.
+00000250: 0000 7400 7c00 8301 7d01 7c01 9b00 6401  ..t.|...}.|...d.
+00000260: 7c00 6a01 6a02 9b00 9d03 7d01 7403 6a04  |.j.j.....}.t.j.
+00000270: a005 7c00 6a01 6a06 7c01 a102 7d02 7c02  ..|.j.j.|...}.|.
+00000280: 5300 2902 4eda 012e 2907 da0d 6765 745f  S.).N...)...get_
+00000290: 6669 6c65 5f6e 616d 6572 0400 0000 da06  file_namer......
+000002a0: 666f 726d 6174 da02 6f73 7209 0000 00da  format..osr.....
+000002b0: 046a 6f69 6eda 0962 6173 655f 7061 7468  .join..base_path
+000002c0: 2903 7208 0000 00da 0966 696c 655f 6e61  ).r......file_na
+000002d0: 6d65 7209 0000 0072 0a00 0000 720a 0000  mer....r....r...
+000002e0: 0072 0b00 0000 720e 0000 0011 0000 0073  .r....r........s
+000002f0: 0800 0000 0801 1201 1201 0401 720e 0000  ............r...
+00000300: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000310: 0000 0200 0000 4300 0000 720d 0000 0072  ......C...r....r
+00000320: 0200 0000 2902 7217 0000 00da 1567 6574  ....).r......get
+00000330: 5f64 6566 6175 6c74 5f66 696c 655f 6e61  _default_file_na
+00000340: 6d65 720f 0000 0072 0a00 0000 720a 0000  mer....r....r...
+00000350: 0072 0b00 0000 7212 0000 0017 0000 0072  .r....r........r
+00000360: 1000 0000 7212 0000 0063 0100 0000 0000  ....r....c......
+00000370: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000380: 0000 7322 0000 0074 007c 006a 016a 0283  ..s"...t.|.j.j..
+00000390: 0164 016b 0272 0d74 037c 006a 0183 0153  .d.k.r.t.|.j...S
+000003a0: 0074 047c 0083 0153 0029 024e e901 0000  .t.|...S.).N....
+000003b0: 0029 05da 036c 656e 7204 0000 00da 1264  .)...lenr......d
+000003c0: 6174 615f 6f62 6a65 6374 5f67 726f 7570  ata_object_group
+000003d0: 73da 1267 6574 5f62 6173 655f 6669 6c65  s..get_base_file
+000003e0: 5f6e 616d 65da 1667 6574 5f6e 756d 6265  _name..get_numbe
+000003f0: 7265 645f 6669 6c65 5f6e 616d 6572 0f00  red_file_namer..
+00000400: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000410: 0072 1800 0000 1d00 0000 7306 0000 0010  .r........s.....
+00000420: 010a 0108 0272 1800 0000 6301 0000 0000  .....r....c.....
+00000430: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000440: 0000 0073 1800 0000 7c00 6a00 6400 7500  ...s....|.j.d.u.
+00000450: 7207 6401 5300 7401 7c00 6a00 8301 5300  r.d.S.t.|.j...S.
+00000460: 2902 4eda 0646 6967 7572 6529 02da 0574  ).N..Figure)...t
+00000470: 6974 6c65 da03 7374 7272 0f00 0000 720a  itle..strr....r.
+00000480: 0000 0072 0a00 0000 720b 0000 0072 1c00  ...r....r....r..
+00000490: 0000 2300 0000 7306 0000 000a 0104 010a  ..#...s.........
+000004a0: 0272 1c00 0000 6301 0000 0000 0000 0000  .r....c.........
+000004b0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+000004c0: 2200 0000 7400 7c00 6a01 8301 7d01 7c01  "...t.|.j...}.|.
+000004d0: 9b00 6401 7c00 6a02 6402 1700 9b00 9d03  ..d.|.j.d.......
+000004e0: 7d01 7c01 5300 2903 4efa 0120 7219 0000  }.|.S.).N.. r...
+000004f0: 0029 0372 1c00 0000 da0b 6669 6775 7265  .).r......figure
+00000500: 5f6f 626a 73da 0c66 6967 7572 655f 696e  _objs..figure_in
+00000510: 6465 7829 0272 0800 0000 7217 0000 0072  dex).r....r....r
+00000520: 0a00 0000 720a 0000 0072 0b00 0000 721d  ....r....r....r.
+00000530: 0000 0029 0000 0073 0600 0000 0a01 1401  ...)...s........
+00000540: 0401 721d 0000 0063 0200 0000 0000 0000  ..r....c........
+00000550: 0000 0000 0200 0000 0b00 0000 4300 0000  ............C...
+00000560: 7330 0000 0074 006a 017c 007c 016a 027c  s0...t.j.|.|.j.|
+00000570: 016a 037c 016a 047c 016a 057c 016a 067c  .j.|.j.|.j.|.j.|
+00000580: 016a 077c 016a 087c 016a 0964 018d 0901  .j.|.j.|.j.d....
+00000590: 0064 0053 0029 024e 2908 da03 6470 6972  .d.S.).N)...dpir
+000005a0: 1300 0000 da08 6d65 7461 6461 7461 da0b  ......metadata..
+000005b0: 6262 6f78 5f69 6e63 6865 73da 0a70 6164  bbox_inches..pad
+000005c0: 5f69 6e63 6865 73da 0966 6163 6563 6f6c  _inches..facecol
+000005d0: 6f72 da09 6564 6765 636f 6c6f 72da 0762  or..edgecolor..b
+000005e0: 6163 6b65 6e64 290a 7206 0000 00da 0773  ackend).r......s
+000005f0: 6176 6566 6967 7224 0000 0072 1300 0000  avefigr$...r....
+00000600: 7225 0000 0072 2600 0000 7227 0000 0072  r%...r&...r'...r
+00000610: 2800 0000 7229 0000 0072 2a00 0000 2902  (...r)...r*...).
+00000620: 7209 0000 0072 0400 0000 720a 0000 0072  r....r....r....r
+00000630: 0a00 0000 720b 0000 0072 0500 0000 2e00  ....r....r......
+00000640: 0000 7314 0000 0006 0104 0104 0104 0104  ..s.............
+00000650: 0104 0104 0104 0104 010a f872 0500 0000  ...........r....
+00000660: 290c 7214 0000 00da 116d 6174 706c 6f74  ).r......matplot
+00000670: 6c69 622e 7079 706c 6f74 da06 7079 706c  lib.pyplot..pypl
+00000680: 6f74 7206 0000 0072 0c00 0000 7203 0000  otr....r....r...
+00000690: 0072 0e00 0000 7212 0000 0072 1800 0000  .r....r....r....
+000006a0: 721c 0000 0072 1d00 0000 7205 0000 0072  r....r....r....r
+000006b0: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000006c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000006d0: 0073 1400 0000 0800 0c02 0802 0806 0806  .s..............
+000006e0: 0806 0806 0806 0806 0c05                 ..........
```

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/savefigure.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,30 +5,42 @@
 def save_figure(figure_obj):
     path = get_figure_path(figure_obj)
     figures_obj = figure_obj.figures_obj
     save_fig(path, figures_obj)
     plt.close()
 
 def get_figure_path(figure_obj):
+    if figure_obj.path is not None:
+        return figure_obj.path
+    else:
+        return get_default_figure_path(figure_obj)
+
+def get_default_figure_path(figure_obj):
     file_name = get_file_name(figure_obj)
     file_name = f"{file_name}.{figure_obj.figures_obj.format}"
-    path = os.path.join(figure_obj.figures_obj.path, file_name)
+    path = os.path.join(figure_obj.figures_obj.base_path, file_name)
     return path
 
 def get_file_name(figure_obj):
+    if figure_obj.file_name is not None:
+        return figure_obj.file_name
+    else:
+        return get_default_file_name(figure_obj)
+
+def get_default_file_name(figure_obj):
     if len(figure_obj.figures_obj.data_object_groups) == 1:
         return get_base_file_name(figure_obj.figures_obj)
     else:
         return get_numbered_file_name(figure_obj)
 
-def get_base_file_name(figure_objs):
-    if figure_objs.title is None:
+def get_base_file_name(figure_obj):
+    if figure_obj.title is None:
         return "Figure"
     else:
-        return str(figure_objs.title)
+        return str(figure_obj.title)
 
 def get_numbered_file_name(figure_obj):
     file_name = get_base_file_name(figure_obj.figure_objs)
     file_name = f"{file_name} {figure_obj.figure_index + 1}"
     return file_name
 
 def save_fig(path, figures_obj):
```

### Comparing `hgutilities-1.0.8.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/utils/__pycache__/groups.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc` & `hgutilities-1.0.8.6/hgutilities/utils/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/utils/groups.py` & `hgutilities-1.0.8.6/hgutilities/utils/groups.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/utils/paths.py` & `hgutilities-1.0.8.6/hgutilities/utils/paths.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities/utils/plots.py` & `hgutilities-1.0.8.6/hgutilities/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.5/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.8.6/hgutilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgutilities
-Version: 1.0.8.5
+Version: 1.0.8.6
 Summary: A triple of tools used for plotting, handling key-words, and utilities
 Author: Henry Ginn
 Author-email: <henryginn137@gmail.com>
 Keywords: python,matplotlib,plotting,default,keywords,utils
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hgutilities-1.0.8.5/hgutilities.egg-info/SOURCES.txt` & `hgutilities-1.0.8.6/hgutilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,30 +75,33 @@
 hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
 hgutilities/plotting/README.md
 hgutilities/plotting/__init__.py
 hgutilities/plotting/animate.py
 hgutilities/plotting/figure.py
 hgutilities/plotting/figures.py
 hgutilities/plotting/plotfunctions.py
+hgutilities/plotting/quick.py
 hgutilities/plotting/Default Settings/Animate.txt
 hgutilities/plotting/Default Settings/Figure.txt
 hgutilities/plotting/Default Settings/Figures.txt
+hgutilities/plotting/Default Settings/Quick.txt
 hgutilities/plotting/Default Settings/__init__.py
 hgutilities/plotting/Documentation/Animate.txt
 hgutilities/plotting/Documentation/Figure.txt
 hgutilities/plotting/Documentation/Figures.txt
 hgutilities/plotting/Documentation/__init__.py
 hgutilities/plotting/Documentation/create_animations.txt
 hgutilities/plotting/Documentation/create_figures.txt
 hgutilities/plotting/Documentation/plotting.txt
 hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
 hgutilities/plotting/__pycache__/animate.cpython-310.pyc
 hgutilities/plotting/__pycache__/figure.cpython-310.pyc
 hgutilities/plotting/__pycache__/figures.cpython-310.pyc
 hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+hgutilities/plotting/__pycache__/quick.cpython-310.pyc
 hgutilities/plotting/datatypes/__init__.py
 hgutilities/plotting/datatypes/bar.py
 hgutilities/plotting/datatypes/bars.py
 hgutilities/plotting/datatypes/colorplot.py
 hgutilities/plotting/datatypes/data.py
 hgutilities/plotting/datatypes/line.py
 hgutilities/plotting/datatypes/lines.py
@@ -154,14 +157,17 @@
 hgutilities/plotting/plotutils/savefigure.py
 hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
 hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
 hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
 hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
 hgutilities/utils/__init__.py
 hgutilities/utils/dicts.py
+hgutilities/utils/filenames.py
 hgutilities/utils/groups.py
 hgutilities/utils/paths.py
 hgutilities/utils/plots.py
+hgutilities/utils/readwrite.py
 hgutilities/utils/__pycache__/__init__.cpython-310.pyc
 hgutilities/utils/__pycache__/dicts.cpython-310.pyc
 hgutilities/utils/__pycache__/groups.cpython-310.pyc
-hgutilities/utils/__pycache__/paths.cpython-310.pyc
+hgutilities/utils/__pycache__/paths.cpython-310.pyc
+hgutilities/utils/__pycache__/readwrite.cpython-310.pyc
```

### Comparing `hgutilities-1.0.8.5/setup.py` & `hgutilities-1.0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.8.5"
+VERSION = "1.0.8.6"
 DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
 LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
                     "Plotting: a front end for matplotlib to easily create subplots.\n"
                     "Utils: a collection of generally useful functions")
 
 # Setting up
 setup(
```

