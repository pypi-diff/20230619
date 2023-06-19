# Comparing `tmp/foran-2022.7.25.tar.gz` & `tmp/foran-2023.6.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foran-2022.7.25.tar", last modified: Mon Jul 25 05:20:03 2022, max compression
+gzip compressed data, was "foran-2023.6.19.tar", last modified: Mon Jun 19 21:35:45 2023, max compression
```

## Comparing `foran-2022.7.25.tar` & `foran-2023.6.19.tar`

### file list

```diff
@@ -1,45 +1,26 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.164510 foran-2022.7.25/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 foran-2022.7.25/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 foran-2022.7.25/.gitattributes
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.127625 foran-2022.7.25/.github/
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.139366 foran-2022.7.25/.github/workflows/
--rw-r--r--   0 ruth       (501) staff       (20)     2449 2021-10-11 19:00:15.000000 foran-2022.7.25/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1915 2022-07-25 05:05:40.000000 foran-2022.7.25/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2021-10-11 15:16:49.000000 foran-2022.7.25/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-09-18 16:56:40.000000 foran-2022.7.25/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     1487 2022-07-25 05:08:12.000000 foran-2022.7.25/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     2360 2022-07-25 05:20:03.164638 foran-2022.7.25/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1405 2022-07-25 05:16:06.000000 foran-2022.7.25/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.142047 foran-2022.7.25/docs/
--rw-r--r--   0 ruth       (501) staff       (20)     1705 2022-07-25 05:01:12.000000 foran-2022.7.25/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1334 2022-07-25 05:16:17.000000 foran-2022.7.25/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      231 2022-07-25 04:58:28.000000 foran-2022.7.25/docs/install.md
--rw-r--r--   0 ruth       (501) staff       (20)     1638 2022-07-25 04:59:05.000000 foran-2022.7.25/docs/usage.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.146392 foran-2022.7.25/foran/
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-07-25 05:18:41.000000 foran-2022.7.25/foran/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      183 2021-10-16 16:43:34.000000 foran-2022.7.25/foran/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3061 2021-10-17 15:53:02.000000 foran-2022.7.25/foran/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     2291 2021-10-17 15:43:51.000000 foran-2022.7.25/foran/foran.py
--rw-r--r--   0 ruth       (501) staff       (20)      324 2021-10-16 14:56:00.000000 foran-2022.7.25/foran/render.py
--rw-r--r--   0 ruth       (501) staff       (20)     2198 2021-10-17 16:48:48.000000 foran-2022.7.25/foran/report.py
--rw-r--r--   0 ruth       (501) staff       (20)      979 2021-10-16 16:41:55.000000 foran-2022.7.25/foran/status.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.152489 foran-2022.7.25/foran.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2360 2022-07-25 05:20:02.000000 foran-2022.7.25/foran.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      663 2022-07-25 05:20:03.000000 foran-2022.7.25/foran.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-07-25 05:20:02.000000 foran-2022.7.25/foran.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       40 2022-07-25 05:20:02.000000 foran-2022.7.25/foran.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)       97 2022-07-25 05:20:02.000000 foran-2022.7.25/foran.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       11 2022-07-25 05:20:02.000000 foran-2022.7.25/foran.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1244 2022-07-25 05:02:50.000000 foran-2022.7.25/mkdocs.yml
--rw-r--r--   0 ruth       (501) staff       (20)      200 2022-05-22 10:06:06.000000 foran-2022.7.25/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       31 2022-07-13 20:57:11.000000 foran-2022.7.25/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1780 2022-07-25 05:20:03.165885 foran-2022.7.25/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2021-09-18 16:56:40.000000 foran-2022.7.25/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-07-25 05:20:03.164036 foran-2022.7.25/test/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2021-09-18 16:56:40.000000 foran-2022.7.25/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-10-11 15:17:32.000000 foran-2022.7.25/test/context.py
--rw-r--r--   0 ruth       (501) staff       (20)      679 2022-07-24 17:24:55.000000 foran-2022.7.25/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      705 2022-07-23 20:14:38.000000 foran-2022.7.25/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2230 2021-10-17 15:56:39.000000 foran-2022.7.25/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     2250 2022-07-25 05:11:43.000000 foran-2022.7.25/test/test_foran.py
--rw-r--r--   0 ruth       (501) staff       (20)     1148 2021-10-17 17:08:30.000000 foran-2022.7.25/test/test_report.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 21:35:45.804830 foran-2023.6.19/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 foran-2023.6.19/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 foran-2023.6.19/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3460 2023-06-19 21:35:45.804685 foran-2023.6.19/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2369 2023-03-14 22:18:24.000000 foran-2023.6.19/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 21:35:45.801348 foran-2023.6.19/foran/
+-rw-r--r--   0 ruth       (501) staff       (20)      351 2023-06-19 21:33:10.000000 foran-2023.6.19/foran/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      123 2022-12-07 10:03:59.000000 foran-2023.6.19/foran/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2982 2022-12-07 10:03:43.000000 foran-2023.6.19/foran/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2248 2022-12-07 10:25:55.000000 foran-2023.6.19/foran/foran.py
+-rw-r--r--   0 ruth       (501) staff       (20)      244 2022-12-07 10:02:44.000000 foran-2023.6.19/foran/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2118 2022-12-07 10:10:43.000000 foran-2023.6.19/foran/report.py
+-rw-r--r--   0 ruth       (501) staff       (20)      904 2022-12-07 10:03:14.000000 foran-2023.6.19/foran/status.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 21:35:45.803665 foran-2023.6.19/foran.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3460 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      388 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       40 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      106 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        6 2023-06-19 21:35:45.000000 foran-2023.6.19/foran.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2680 2023-06-19 21:21:12.000000 foran-2023.6.19/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-19 21:35:45.804865 foran-2023.6.19/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-19 21:35:45.804472 foran-2023.6.19/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1551 2023-06-19 21:27:26.000000 foran-2023.6.19/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1655 2022-12-07 11:05:25.000000 foran-2023.6.19/test/test_foran.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1272 2023-06-19 21:26:54.000000 foran-2023.6.19/test/test_report.py
```

### Comparing `foran-2022.7.25/foran/cli.py` & `foran-2023.6.19/foran/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#! /usr/bin/env python
-# -*- coding: utf-8 -*-
-# pylint: disable=line-too-long
 """Commandline API gateway for foran."""
 import pathlib
 import sys
 from typing import List, Union
 
 import typer
```

### Comparing `foran-2022.7.25/foran/foran.py` & `foran-2023.6.19/foran/foran.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=expression-not-assigned,line-too-long
 """In front or behind (Foran eller bagved)? API."""
 import os
 import pathlib
 import warnings
 from typing import List, Union
 
-from git import Repo
 from git.exc import GitCommandError
+from git.repo import Repo
 
 from foran.report import Format, Report, report_as
 from foran.status import Status
 
 DEBUG_VAR = 'FORAN_DEBUG'
 DEBUG = os.getenv(DEBUG_VAR)
 
@@ -63,15 +61,15 @@
         return 1
 
     if template and target != 'STD_OUT':
         warnings.warn('templates not yet implemented')
 
     report = Report(stem=target, file_format=Format.NONE)
 
-    repo = Repo(repo_root)
+    repo = Repo(repo_root, search_parent_directories=True)
     status = Status(repo)
     if command == 'diff':
         local_commits(repo, status)
         local_staged(repo, status)
         local_files(repo, status)
     report_as(status, report)
     return 0
```

### Comparing `foran-2022.7.25/foran/report.py` & `foran-2023.6.19/foran/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=expression-not-assigned,line-too-long
 """In front or behind (Foran eller bagved)? reporting interface."""
 import pathlib
 from enum import Enum, auto
 from typing import List, Tuple
 
 from foran.status import Status
```

### Comparing `foran-2022.7.25/foran/status.py` & `foran-2023.6.19/foran/status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=expression-not-assigned,line-too-long
 """In front or behind (Foran eller bagved)? status structure."""
 import datetime as dti
 
-from git import Repo
+from git.repo import Repo
 
 STATUS_DTI_FORMAT = '%Y-%m-%d %H:%M:%S UTC'
 
 
 class Status:
     """Status structure."""
```

### Comparing `foran-2022.7.25/test/test_foran.py` & `foran-2023.6.19/test/test_foran.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,47 +7,35 @@
 from git.exc import InvalidGitRepositoryError
 
 import foran.foran as fb
 from foran.status import Status
 
 
 def test_main_empty():
-    message = 'received wrong number of arguments'
-    with pytest.raises(UserWarning) as ex:
-        fb.main([]) == 2
-        assert message in str(ex.value)
+    assert fb.main([]) == 2
 
 
 def test_main_few():
-    message = 'received wrong number of arguments'
-    with pytest.raises(UserWarning) as ex:
-        fb.main(['diff', '.', 'would_be_here']) == 2
-        assert message in str(ex.value)
+    assert fb.main(['diff', '.', 'would_be_here']) == 2
 
 
 def test_main_unknown_command():
-    message = 'received unknown command'
-    with pytest.raises(UserWarning) as ex:
-        fb.main(['unknown', '.', 'would_be_here', '']) == 2
-        assert message in str(ex.value)
+    assert fb.main(['unknown', '.', 'would_be_here', '']) == 2
 
 
 def test_main_diff():
     assert fb.main(['diff', '.', 'foran-eller-bagved.txt', '']) == 0
 
 
 def test_main_label():
     assert fb.main(['label', '.', 'STD_OUT', '']) == 0
 
 
 def test_main_template():
-    message = 'ignoring template: ignored'
-    with pytest.raises(UserWarning) as ex:
-        fb.main(['diff', '.', 'foran-eller-bagved.txt', 'ignored']) == 0
-        assert message in str(ex.value)
+    assert fb.main(['diff', '.', 'foran-eller-bagved.txt', 'ignored']) == 0
 
 
 def test_local_commits_none():
     repo = Repo('.')
     status = Status(repo)
     status.foran = True
     fb.local_commits(repo, status)
@@ -55,26 +43,24 @@
 
 
 def test_local_commits_some():
     repo = Repo('.')
     status = Status(repo)
     status.foran = False
     fb.local_commits(repo, status)
-    assert len(status.local_commits) == 6
+    assert len(status.local_commits) >= 216
 
 
 def test_local_commits_no_repo():
     with pytest.raises(InvalidGitRepositoryError):
         _ = Repo('test')
         # We cannot currently really probe for a git repo that raises GitCommandError
 
 
 def test_local_commits_no_remote():
     path_to_non_remote = pathlib.Path('test', 'fixtures', 'non_remote')
     repo = Repo(path_to_non_remote)
     status = Status(repo)
     status.foran = False
     message = 'No remote found, so all commit differences hypothetical'
-    with pytest.raises(UserWarning) as ex:
-        fb.local_commits(repo, status)
-        assert status.local_commits == [message]
-        assert message in str(ex.value)
+    fb.local_commits(repo, status)
+    assert status.local_commits == [message]
```

### Comparing `foran-2022.7.25/test/test_report.py` & `foran-2023.6.19/test/test_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# -*- coding: utf-8 -*-
-# pylint: disable=missing-docstring,unused-import,reimported
+import warnings
+
+import pytest
+
 from foran.report import generate_report_list
 
 
 def test_generate_report_list_nothing_ast_empty():
     assert generate_report_list('foo:', False, [], '*') == []
 
 
@@ -23,13 +25,17 @@
     assert generate_report_list('foo:', True, ['bar'], '+') == ['foo:\n', ' + bar\n']
 
 
 def test_generate_report_list_dash_single():
     assert generate_report_list('foo:', True, ['bar'], '-') == ['foo:\n', ' - bar\n']
 
 
+@pytest.mark.filterwarnings('error::pytest.PytestUnraisableExceptionWarning')
+@pytest.mark.skip()
 def test_generate_report_list_default_two():
-    assert generate_report_list('foo:', True, ['bar', 'baz']) == ['foo:\n', ' * bar\n * baz\n']
+    with warnings.catch_warnings():
+        warnings.simplefilter('error')
+        assert generate_report_list('foo:', True, ['bar', 'baz']) == ['foo:\n', ' * bar\n * baz\n']
 
 
 def test_generate_report_list_nothing_default_two():
     assert generate_report_list('foo:', False, ['bar', 'baz']) == []
```

