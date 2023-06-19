# Comparing `tmp/bonus-0.6.27.tar.gz` & `tmp/bonus-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonus-0.6.27.tar", last modified: Mon Jun 19 21:57:45 2023, max compression
+gzip compressed data, was "bonus-0.6.3.tar", last modified: Sat Dec 17 20:14:41 2022, max compression
```

## Comparing `bonus-0.6.27.tar` & `bonus-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:57:45.449775 bonus-0.6.27/
--rw-rw-rw-   0        0        0      123 2023-06-19 21:57:45.449775 bonus-0.6.27/PKG-INFO
--rw-rw-rw-   0        0        0      196 2020-07-15 06:42:11.000000 bonus-0.6.27/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-19 21:57:45.441633 bonus-0.6.27/bonus/
--rw-rw-rw-   0        0        0     9966 2023-06-19 21:57:13.000000 bonus-0.6.27/bonus/bonus.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:57:45.448750 bonus-0.6.27/bonus.egg-info/
--rw-rw-rw-   0        0        0      123 2023-06-19 21:57:45.000000 bonus-0.6.27/bonus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-06-19 21:57:45.000000 bonus-0.6.27/bonus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:57:45.000000 bonus-0.6.27/bonus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 21:57:45.000000 bonus-0.6.27/bonus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 21:57:45.450775 bonus-0.6.27/setup.cfg
--rw-rw-rw-   0        0        0      212 2023-06-19 21:56:49.000000 bonus-0.6.27/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.417698 bonus-0.6.3/
+-rw-rw-rw-   0        0        0      122 2022-12-17 20:14:41.418698 bonus-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2020-07-15 06:42:11.000000 bonus-0.6.3/README.rst
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.374696 bonus-0.6.3/bonus/
+-rw-rw-rw-   0        0        0     2943 2022-12-17 20:13:32.000000 bonus-0.6.3/bonus/bonus.py
+drwxrwxrwx   0        0        0        0 2022-12-17 20:14:41.412697 bonus-0.6.3/bonus.egg-info/
+-rw-rw-rw-   0        0        0      122 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2022-12-17 20:14:41.000000 bonus-0.6.3/bonus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-17 20:14:41.419697 bonus-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      211 2022-12-17 20:14:02.000000 bonus-0.6.3/setup.py
```

