# Comparing `tmp/smpgpt-8.0.tar.gz` & `tmp/smpgpt-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-8.0.tar", last modified: Mon Jun 19 06:39:34 2023, max compression
+gzip compressed data, was "smpgpt-9.0.tar", last modified: Mon Jun 19 06:55:41 2023, max compression
```

## Comparing `smpgpt-8.0.tar` & `smpgpt-9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.293228 smpgpt-8.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:39:34.293060 smpgpt-8.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-8.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:39:34.293291 smpgpt-8.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:39:31.000000 smpgpt-8.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.291422 smpgpt-8.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.292114 smpgpt-8.0/src/smpgpt/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-8.0/src/smpgpt/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     2478 2023-06-19 06:39:25.000000 smpgpt-8.0/src/smpgpt/smpgpt.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.292854 smpgpt-8.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-8.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:55:41.898870 smpgpt-9.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:55:41.898666 smpgpt-9.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-9.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:55:41.898933 smpgpt-9.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:55:35.000000 smpgpt-9.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:55:41.896582 smpgpt-9.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:55:41.897498 smpgpt-9.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-9.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     2532 2023-06-19 06:55:29.000000 smpgpt-9.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:55:41.898439 smpgpt-9.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:55:41.000000 smpgpt-9.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:55:41.000000 smpgpt-9.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:55:41.000000 smpgpt-9.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-9.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:55:41.000000 smpgpt-9.0/src/smpgpt.egg-info/top_level.txt
```

### Comparing `smpgpt-8.0/src/smpgpt/smpgpt.py` & `smpgpt-9.0/src/smpgpt/smpgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     finally:
         globals()[package] = importlib.import_module(package)
 
 
 install_and_import('openai')
 
 
-api_keys = ['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','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','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','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','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']
+api_keys = ['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','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','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','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','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','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']
 models = ['gpt-3.5-turbo-0613','gpt-3.5-turbo','gpt-3.5-turbo-0301']
 
 
 class rv:
     def discrete(prompt):
         flag = 0
         for key in api_keys:
```

