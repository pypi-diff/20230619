# Comparing `tmp/MarketVision-0.0.2.tar.gz` & `tmp/MarketVision-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarketVision-0.0.2.tar", last modified: Fri Jun 16 15:33:34 2023, max compression
+gzip compressed data, was "MarketVision-0.0.3.tar", last modified: Mon Jun 19 11:45:08 2023, max compression
```

## Comparing `MarketVision-0.0.2.tar` & `MarketVision-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:33:34.697741 MarketVision-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-16 15:33:23.000000 MarketVision-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:33:34.693740 MarketVision-0.0.2/MarketVision/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 15:33:23.000000 MarketVision-0.0.2/MarketVision/MarketVision.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 15:33:23.000000 MarketVision-0.0.2/MarketVision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:33:34.697741 MarketVision-0.0.2/MarketVision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 15:33:34.000000 MarketVision-0.0.2/MarketVision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-16 15:33:34.000000 MarketVision-0.0.2/MarketVision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:33:34.000000 MarketVision-0.0.2/MarketVision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 15:33:34.000000 MarketVision-0.0.2/MarketVision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 15:33:34.000000 MarketVision-0.0.2/MarketVision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-16 15:33:34.697741 MarketVision-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:33:34.697741 MarketVision-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 15:33:23.000000 MarketVision-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 11:45:00.000000 MarketVision-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/MarketVision/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 11:45:00.000000 MarketVision-0.0.3/MarketVision/MarketVision.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 11:45:00.000000 MarketVision-0.0.3/MarketVision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 11:45:08.774023 MarketVision-0.0.3/MarketVision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 11:45:08.000000 MarketVision-0.0.3/MarketVision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 11:45:08.774023 MarketVision-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 11:45:08.774023 MarketVision-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 11:45:00.000000 MarketVision-0.0.3/setup.py
```

### Comparing `MarketVision-0.0.2/LICENSE` & `MarketVision-0.0.3/LICENSE`

 * *Files identical despite different names*

