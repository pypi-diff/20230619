# Comparing `tmp/authit-0.0.3.tar.gz` & `tmp/authit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authit-0.0.3.tar", last modified: Mon Jun 19 05:48:51 2023, max compression
+gzip compressed data, was "authit-0.0.4.tar", last modified: Mon Jun 19 05:56:38 2023, max compression
```

## Comparing `authit-0.0.3.tar` & `authit-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.731024 authit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 05:48:51.731024 authit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 05:48:41.000000 authit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.727024 authit-0.0.3/authit/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 05:48:41.000000 authit-0.0.3/authit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.731024 authit-0.0.3/authit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 05:48:51.731024 authit-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 05:48:41.000000 authit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:56:38.342905 authit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 05:56:38.342905 authit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-19 05:56:30.000000 authit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:56:38.342905 authit-0.0.4/authit/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 05:56:30.000000 authit-0.0.4/authit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:56:38.342905 authit-0.0.4/authit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 05:56:38.000000 authit-0.0.4/authit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 05:56:38.000000 authit-0.0.4/authit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:56:38.000000 authit-0.0.4/authit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:56:38.000000 authit-0.0.4/authit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:56:38.000000 authit-0.0.4/authit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 05:56:38.342905 authit-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 05:56:30.000000 authit-0.0.4/setup.py
```

