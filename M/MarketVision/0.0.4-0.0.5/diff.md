# Comparing `tmp/MarketVision-0.0.4.tar.gz` & `tmp/MarketVision-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarketVision-0.0.4.tar", last modified: Mon Jun 19 13:18:30 2023, max compression
+gzip compressed data, was "MarketVision-0.0.5.tar", last modified: Mon Jun 19 16:02:36 2023, max compression
```

## Comparing `MarketVision-0.0.4.tar` & `MarketVision-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 13:18:18.000000 MarketVision-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/MarketVision/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-19 13:18:18.000000 MarketVision-0.0.4/MarketVision/MarketVision.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 13:18:18.000000 MarketVision-0.0.4/MarketVision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:18:30.186011 MarketVision-0.0.4/MarketVision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 13:18:30.000000 MarketVision-0.0.4/MarketVision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 13:18:30.186011 MarketVision-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:18:30.186011 MarketVision-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 13:18:18.000000 MarketVision-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:02:36.361137 MarketVision-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 16:02:21.000000 MarketVision-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:02:36.361137 MarketVision-0.0.5/MarketVision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-19 16:02:21.000000 MarketVision-0.0.5/MarketVision/MarketVision.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-19 16:02:21.000000 MarketVision-0.0.5/MarketVision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:02:36.361137 MarketVision-0.0.5/MarketVision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 16:02:36.000000 MarketVision-0.0.5/MarketVision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-19 16:02:36.000000 MarketVision-0.0.5/MarketVision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:02:36.000000 MarketVision-0.0.5/MarketVision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 16:02:36.000000 MarketVision-0.0.5/MarketVision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 16:02:36.000000 MarketVision-0.0.5/MarketVision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-19 16:02:36.361137 MarketVision-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:02:36.361137 MarketVision-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-19 16:02:21.000000 MarketVision-0.0.5/setup.py
```

### Comparing `MarketVision-0.0.4/LICENSE` & `MarketVision-0.0.5/LICENSE`

 * *Files identical despite different names*

