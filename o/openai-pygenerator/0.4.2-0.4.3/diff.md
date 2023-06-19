# Comparing `tmp/openai-pygenerator-0.4.2.tar.gz` & `tmp/openai-pygenerator-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.2.tar", last modified: Mon Jun 19 16:16:54 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.3.tar", last modified: Mon Jun 19 16:39:10 2023, max compression
```

## Comparing `openai-pygenerator-0.4.2.tar` & `openai-pygenerator-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.151344 openai-pygenerator-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.155345 openai-pygenerator-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.491666 openai-pygenerator-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 16:39:10.000000 openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:39:10.495666 openai-pygenerator-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 16:39:00.000000 openai-pygenerator-0.4.3/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.2/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/.pre-commit-config.yaml` & `openai-pygenerator-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/.pylintrc` & `openai-pygenerator-0.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/LICENSE.txt` & `openai-pygenerator-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/PKG-INFO` & `openai-pygenerator-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.2
+Version: 0.4.3
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.2/README.md` & `openai-pygenerator-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/pyproject.toml` & `openai-pygenerator-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.3/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.3/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 import time
 from enum import Enum, auto
 from typing import Callable, Dict, Iterable, Iterator, List, NewType, Optional, TypeVar
 
 import openai
-from openai.error import APIError, RateLimitError
+from openai.error import APIError, RateLimitError, ServiceUnavailableError
 
 Completion = Dict[str, str]
 Seconds = NewType("Seconds", int)
 Completions = Iterator[Completion]
 History = Iterable[Completion]
 Completer = Callable[[History, int], Completions]
 T = TypeVar("T")
@@ -84,16 +84,16 @@
             max_tokens=max_tokens,
             n=n,
             temperature=temperature,
         )
         logger.debug("response = %s", result)
         for choice in result.choices:
             yield choice.message
-    except (RateLimitError, APIError) as err:
-        if isinstance(err, APIError) and not (err.http_status in [524, 502, 503]):
+    except (RateLimitError, APIError, ServiceUnavailableError) as err:
+        if isinstance(err, APIError) and not (err.http_status in [524, 502]):
             raise
         logger.warning("Error returned from openai API: %s", err)
         logger.debug("retries = %d", retries)
         if retries < max_retries:
             logger.info("Retrying... ")
             time.sleep(retry_base + retry_exponent**retries)
             for completion in generate_completions(
```

### Comparing `openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.2
+Version: 0.4.3
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.3/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.2/tests/test_gpt.py` & `openai-pygenerator-0.4.3/tests/test_gpt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=redefined-outer-name
 
 from typing import Iterable
 
 import pytest
-from openai.error import APIError, RateLimitError
+from openai.error import APIError, RateLimitError, ServiceUnavailableError
 from openai.openai_object import OpenAIObject
 
 from openai_pygenerator import (
     GPT_MAX_RETRIES,
     ChatSession,
     Completer,
     Completion,
@@ -48,16 +48,19 @@
 
 
 @pytest.mark.parametrize(
     "error",
     [
         RateLimitError("rate limited", http_status=429),
         APIError("Gateway Timeout", http_status=524),
-        APIError(
-            "openai.error.ServiceUnavailableError: The server is overloaded or not ready yet",
+        ServiceUnavailableError(
+            message=(
+                "openai.error.ServiceUnavailableError:"
+                " The server is overloaded or not ready yet"
+            ),
             http_status=503,
         ),
     ],
 )
 def test_generate_completion(mock_openai, mock_sleep, error):
     mock_openai.side_effect = [
         error,
```

