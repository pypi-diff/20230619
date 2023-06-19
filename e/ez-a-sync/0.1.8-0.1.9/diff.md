# Comparing `tmp/ez-a-sync-0.1.8.tar.gz` & `tmp/ez-a-sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-a-sync-0.1.8.tar", last modified: Thu Jun  1 08:59:05 2023, max compression
+gzip compressed data, was "ez-a-sync-0.1.9.tar", last modified: Mon Jun 19 00:53:20 2023, max compression
```

## Comparing `ez-a-sync-0.1.8.tar` & `ez-a-sync-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.342256 ez-a-sync-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.338256 ez-a-sync-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.338256 ez-a-sync-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-01 08:59:05.342256 ez-a-sync-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.338256 ez-a-sync-0.1.8/a_sync/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_bound.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     2855 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modified.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.338256 ez-a-sync-0.1.8/a_sync/modifiers/
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.338256 ez-a-sync-0.1.8/a_sync/modifiers/cache/
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/limiter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/modifiers/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/property.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/a_sync/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.342256 ez-a-sync-0.1.8/ez_a_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-01 08:59:05.000000 ez-a-sync-0.1.8/ez_a_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-01 08:59:05.000000 ez-a-sync-0.1.8/ez_a_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 08:59:05.000000 ez-a-sync-0.1.8/ez_a_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-01 08:59:05.000000 ez-a-sync-0.1.8/ez_a_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-01 08:59:05.000000 ez-a-sync-0.1.8/ez_a_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-01 08:59:05.342256 ez-a-sync-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:59:05.342256 ez-a-sync-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-01 08:58:49.000000 ez-a-sync-0.1.8/tests/test_semaphore.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.110393 ez-a-sync-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6139 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4462 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_bound.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2855 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6316 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modified.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/modifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/modifiers/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/modifiers/semaphores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/_loggable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.114394 ez-a-sync-0.1.9/a_sync/primitives/locks/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/primitives/locks/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/property.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/a_sync/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/ez_a_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-19 00:53:20.000000 ez-a-sync-0.1.9/ez_a_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:20.118394 ez-a-sync-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3684 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1628 2023-06-19 00:53:01.000000 ez-a-sync-0.1.9/tests/test_semaphore.py
```

### Comparing `ez-a-sync-0.1.8/.github/workflows/codeql.yaml` & `ez-a-sync-0.1.9/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/.github/workflows/mypy.yaml` & `ez-a-sync-0.1.9/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/.github/workflows/pytest.yaml` & `ez-a-sync-0.1.9/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/.github/workflows/release.yaml` & `ez-a-sync-0.1.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/LICENSE.txt` & `ez-a-sync-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/README.md` & `ez-a-sync-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/__init__.py` & `ez-a-sync-0.1.9/a_sync/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 from a_sync import aliases
 from a_sync.base import ASyncGenericBase
 from a_sync.decorator import a_sync
 from a_sync.modifiers.semaphores import (DummySemaphore, ThreadsafeSemaphore,
-                               apply_semaphore)
+                                         apply_semaphore)
+from a_sync.primitives import *
 from a_sync.singleton import ASyncGenericSingleton
 
 # I alias the aliases for your convenience.
 # I prefer "aka" but its meaning is not intuitive when reading code so I created both aliases for you to choose from.
 # NOTE: Overkill? Maybe.
 aka = alias = aliases
 
 # alias for backward-compatability, will be removed eventually, probably in 0.1.0
-ASyncBase = ASyncGenericBase    
-
+ASyncBase = ASyncGenericBase
```

### Comparing `ez-a-sync-0.1.8/a_sync/_bound.py` & `ez-a-sync-0.1.9/a_sync/_bound.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/_flags.py` & `ez-a-sync-0.1.9/a_sync/_flags.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/_helpers.py` & `ez-a-sync-0.1.9/a_sync/_helpers.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/_kwargs.py` & `ez-a-sync-0.1.9/a_sync/_kwargs.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/_meta.py` & `ez-a-sync-0.1.9/a_sync/_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/_typing.py` & `ez-a-sync-0.1.9/a_sync/_typing.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/abstract.py` & `ez-a-sync-0.1.9/a_sync/abstract.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/base.py` & `ez-a-sync-0.1.9/a_sync/base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/config.py` & `ez-a-sync-0.1.9/a_sync/config.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/decorator.py` & `ez-a-sync-0.1.9/a_sync/decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/exceptions.py` & `ez-a-sync-0.1.9/a_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modified.py` & `ez-a-sync-0.1.9/a_sync/modified.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/__init__.py` & `ez-a-sync-0.1.9/a_sync/modifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/cache/__init__.py` & `ez-a-sync-0.1.9/a_sync/modifiers/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/cache/memory.py` & `ez-a-sync-0.1.9/a_sync/modifiers/cache/memory.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/limiter.py` & `ez-a-sync-0.1.9/a_sync/modifiers/limiter.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/manager.py` & `ez-a-sync-0.1.9/a_sync/modifiers/manager.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/modifiers/semaphores.py` & `ez-a-sync-0.1.9/a_sync/modifiers/semaphores.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/a_sync/property.py` & `ez-a-sync-0.1.9/a_sync/property.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/setup.py` & `ez-a-sync-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/fixtures.py` & `ez-a-sync-0.1.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/test_base.py` & `ez-a-sync-0.1.9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/test_cache.py` & `ez-a-sync-0.1.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/test_decorator.py` & `ez-a-sync-0.1.9/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/test_meta.py` & `ez-a-sync-0.1.9/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `ez-a-sync-0.1.8/tests/test_semaphore.py` & `ez-a-sync-0.1.9/tests/test_semaphore.py`

 * *Files identical despite different names*

