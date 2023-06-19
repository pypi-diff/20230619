# Comparing `tmp/openai-pygenerator-0.4.1.tar.gz` & `tmp/openai-pygenerator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.1.tar", last modified: Tue Jun  6 18:45:23 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.2.tar", last modified: Mon Jun 19 16:16:54 2023, max compression
```

## Comparing `openai-pygenerator-0.4.1.tar` & `openai-pygenerator-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.662352 openai-pygenerator-0.4.1/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 18:45:23.000000 openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:45:23.666353 openai-pygenerator-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-06 18:45:12.000000 openai-pygenerator-0.4.1/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.151344 openai-pygenerator-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.155345 openai-pygenerator-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.159345 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 16:16:54.000000 openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:16:54.163344 openai-pygenerator-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-19 16:16:39.000000 openai-pygenerator-0.4.2/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.1/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/.pre-commit-config.yaml` & `openai-pygenerator-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/.pylintrc` & `openai-pygenerator-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/LICENSE.txt` & `openai-pygenerator-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/PKG-INFO` & `openai-pygenerator-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 ~~~bash
 pip install openai-pygenerator
 ~~~
 
 ## Basic usage
 
-In the example below we will retry automatically if there is a rate limit error.
+In the example below we will retry automatically if there is a `RateLimitError`.
 
 ~~~python
 from openai_pygenerator import ChatSession
  
 session = ChatSession()
 solution = session.ask("What is the square root of 256?")
 print(solution)
```

### Comparing `openai-pygenerator-0.4.1/README.md` & `openai-pygenerator-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ~~~bash
 pip install openai-pygenerator
 ~~~
 
 ## Basic usage
 
-In the example below we will retry automatically if there is a rate limit error.
+In the example below we will retry automatically if there is a `RateLimitError`.
 
 ~~~python
 from openai_pygenerator import ChatSession
  
 session = ChatSession()
 solution = session.ask("What is the square root of 256?")
 print(solution)
```

### Comparing `openai-pygenerator-0.4.1/pyproject.toml` & `openai-pygenerator-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.2/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.2/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             n=n,
             temperature=temperature,
         )
         logger.debug("response = %s", result)
         for choice in result.choices:
             yield choice.message
     except (RateLimitError, APIError) as err:
-        if isinstance(err, APIError) and not (err.http_status in [524, 502]):
+        if isinstance(err, APIError) and not (err.http_status in [524, 502, 503]):
             raise
         logger.warning("Error returned from openai API: %s", err)
         logger.debug("retries = %d", retries)
         if retries < max_retries:
             logger.info("Retrying... ")
             time.sleep(retry_base + retry_exponent**retries)
             for completion in generate_completions(
```

### Comparing `openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.1
+Version: 0.4.2
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 
 ~~~bash
 pip install openai-pygenerator
 ~~~
 
 ## Basic usage
 
-In the example below we will retry automatically if there is a rate limit error.
+In the example below we will retry automatically if there is a `RateLimitError`.
 
 ~~~python
 from openai_pygenerator import ChatSession
  
 session = ChatSession()
 solution = session.ask("What is the square root of 256?")
 print(solution)
```

### Comparing `openai-pygenerator-0.4.1/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.2/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.1/tests/test_gpt.py` & `openai-pygenerator-0.4.2/tests/test_gpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 
 
 @pytest.mark.parametrize(
     "error",
     [
         RateLimitError("rate limited", http_status=429),
         APIError("Gateway Timeout", http_status=524),
+        APIError(
+            "openai.error.ServiceUnavailableError: The server is overloaded or not ready yet",
+            http_status=503,
+        ),
     ],
 )
 def test_generate_completion(mock_openai, mock_sleep, error):
     mock_openai.side_effect = [
         error,
         error,
         MockChoices(["Test completion 1", "Test completion 2"]),
```

