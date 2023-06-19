# Comparing `tmp/authit-0.0.1.tar.gz` & `tmp/authit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authit-0.0.1.tar", last modified: Sun Jun 18 06:13:46 2023, max compression
+gzip compressed data, was "authit-0.0.3.tar", last modified: Mon Jun 19 05:48:51 2023, max compression
```

## Comparing `authit-0.0.1.tar` & `authit-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:13:46.330126 authit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 06:13:46.330126 authit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 06:13:37.000000 authit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:13:46.330126 authit-0.0.1/authit/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-18 06:13:37.000000 authit-0.0.1/authit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 06:13:46.330126 authit-0.0.1/authit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-18 06:13:46.000000 authit-0.0.1/authit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-18 06:13:46.000000 authit-0.0.1/authit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 06:13:46.000000 authit-0.0.1/authit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 06:13:46.000000 authit-0.0.1/authit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 06:13:46.330126 authit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-18 06:13:37.000000 authit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.731024 authit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 05:48:51.731024 authit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 05:48:41.000000 authit-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.727024 authit-0.0.3/authit/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 05:48:41.000000 authit-0.0.3/authit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:48:51.731024 authit-0.0.3/authit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 05:48:51.000000 authit-0.0.3/authit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 05:48:51.731024 authit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 05:48:41.000000 authit-0.0.3/setup.py
```

