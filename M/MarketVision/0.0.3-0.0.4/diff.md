# Comparing `tmp/MarketVision-0.0.3.tar.gz` & `tmp/MarketVision-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarketVision-0.0.3.tar", last modified: Mon Jun 19 11:45:08 2023, max compression
+gzip compressed data, was "MarketVision-0.0.4.tar", last modified: Mon Jun 19 13:18:30 2023, max compression
```

## Comparing `MarketVision-0.0.3.tar` & `MarketVision-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 11:45:00.000000 MarketVision-0.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/MarketVision/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 11:45:00.000000 MarketVision-0.0.3/MarketVision/MarketVision.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 11:45:00.000000 MarketVision-0.0.3/MarketVision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/MarketVision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 11:45:08.774023 MarketVision-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:45:08.774023 MarketVision-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 11:45:00.000000 MarketVision-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 13:18:18.000000 MarketVision-0.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/MarketVision/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-19 13:18:18.000000 MarketVision-0.0.4/MarketVision/MarketVision.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 13:18:18.000000 MarketVision-0.0.4/MarketVision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/MarketVision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 13:18:30.186011 MarketVision-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:18:30.186011 MarketVision-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 13:18:18.000000 MarketVision-0.0.4/setup.py
```

### Comparing `MarketVision-0.0.3/LICENSE` & `MarketVision-0.0.4/LICENSE`

 * *Files identical despite different names*

