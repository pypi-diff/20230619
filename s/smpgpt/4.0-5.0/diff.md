# Comparing `tmp/smpgpt-4.0.tar.gz` & `tmp/smpgpt-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-4.0.tar", last modified: Fri Jun 16 21:06:57 2023, max compression
+gzip compressed data, was "smpgpt-5.0.tar", last modified: Mon Jun 19 06:06:57 2023, max compression
```

## Comparing `smpgpt-4.0.tar` & `smpgpt-5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976959 smpgpt-4.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.976758 smpgpt-4.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-4.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 21:06:57.977017 smpgpt-4.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 21:06:53.000000 smpgpt-4.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.974766 smpgpt-4.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.975622 smpgpt-4.0/src/smpgpt/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-4.0/src/smpgpt/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     1570 2023-06-16 21:06:48.000000 smpgpt-4.0/src/smpgpt/smpgpt.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976529 smpgpt-4.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-4.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:06:57.743896 smpgpt-5.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:06:57.743726 smpgpt-5.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-5.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:06:57.743957 smpgpt-5.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:06:45.000000 smpgpt-5.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:06:57.741932 smpgpt-5.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:06:57.742668 smpgpt-5.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-5.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     1624 2023-06-19 06:06:38.000000 smpgpt-5.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:06:57.743524 smpgpt-5.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:06:57.000000 smpgpt-5.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:06:57.000000 smpgpt-5.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:06:57.000000 smpgpt-5.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-5.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:06:57.000000 smpgpt-5.0/src/smpgpt.egg-info/top_level.txt
```

### Comparing `smpgpt-4.0/src/smpgpt/smpgpt.py` & `smpgpt-5.0/src/smpgpt/smpgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     finally:
         globals()[package] = importlib.import_module(package)
 
 
 install_and_import('openai')
 
 
-api_keys = ['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','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','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']
+api_keys = ['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','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','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','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']
 models = ['gpt-3.5-turbo-0613','gpt-3.5-turbo','gpt-3.5-turbo-0301']
 
 
 class rv:
     def discrete(prompt):
         flag = 0
         for key in api_keys:
```

