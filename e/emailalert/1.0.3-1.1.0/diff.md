# Comparing `tmp/emailalert-1.0.3.tar.gz` & `tmp/emailalert-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.0.3.tar", last modified: Thu Jun 15 04:55:00 2023, max compression
+gzip compressed data, was "emailalert-1.1.0.tar", last modified: Mon Jun 19 01:58:41 2023, max compression
```

## Comparing `emailalert-1.0.3.tar` & `emailalert-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 04:55:00.209182 emailalert-1.0.3/
--rw-rw-rw-   0        0        0      161 2023-06-15 04:55:00.206682 emailalert-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-15 02:00:10.000000 emailalert-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 04:55:00.197008 emailalert-1.0.3/emailalert.egg-info/
--rw-rw-rw-   0        0        0      161 2023-06-15 04:55:00.000000 emailalert-1.0.3/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-15 04:55:00.000000 emailalert-1.0.3/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 04:55:00.000000 emailalert-1.0.3/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-15 04:55:00.000000 emailalert-1.0.3/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 04:55:00.203022 emailalert-1.0.3/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 01:35:00.000000 emailalert-1.0.3/sck/__init__.py
--rw-rw-rw-   0        0        0      804 2023-06-15 04:34:59.000000 emailalert-1.0.3/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-15 04:55:00.209182 emailalert-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      236 2023-06-15 04:54:34.000000 emailalert-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.684465 emailalert-1.1.0/
+-rw-rw-rw-   0        0        0      178 2023-06-19 01:58:41.682466 emailalert-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-15 05:04:18.000000 emailalert-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.644687 emailalert-1.1.0/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.675462 emailalert-1.1.0/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.0/sck/__init__.py
+-rw-rw-rw-   0        0        0     2056 2023-06-19 01:56:58.000000 emailalert-1.1.0/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:58:41.685462 emailalert-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 01:57:35.000000 emailalert-1.1.0/setup.py
```

