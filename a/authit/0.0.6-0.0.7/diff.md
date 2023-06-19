# Comparing `tmp/authit-0.0.6.tar.gz` & `tmp/authit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authit-0.0.6.tar", last modified: Mon Jun 19 06:46:01 2023, max compression
+gzip compressed data, was "authit-0.0.7.tar", last modified: Mon Jun 19 06:49:12 2023, max compression
```

## Comparing `authit-0.0.6.tar` & `authit-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:46:01.520742 authit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 06:46:01.520742 authit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-19 06:45:50.000000 authit-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:46:01.516742 authit-0.0.6/authit/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 06:45:50.000000 authit-0.0.6/authit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:46:01.520742 authit-0.0.6/authit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 06:46:01.000000 authit-0.0.6/authit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 06:46:01.000000 authit-0.0.6/authit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:46:01.000000 authit-0.0.6/authit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:46:01.000000 authit-0.0.6/authit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:46:01.000000 authit-0.0.6/authit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 06:46:01.520742 authit-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 06:45:50.000000 authit-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:12.152349 authit-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-19 06:49:12.152349 authit-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-19 06:49:00.000000 authit-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:12.152349 authit-0.0.7/authit/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 06:49:00.000000 authit-0.0.7/authit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:49:12.152349 authit-0.0.7/authit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-19 06:49:12.000000 authit-0.0.7/authit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-19 06:49:12.000000 authit-0.0.7/authit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:49:12.000000 authit-0.0.7/authit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:49:12.000000 authit-0.0.7/authit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:49:12.000000 authit-0.0.7/authit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 06:49:12.152349 authit-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-19 06:49:00.000000 authit-0.0.7/setup.py
```

