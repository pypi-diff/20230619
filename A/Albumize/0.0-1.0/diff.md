# Comparing `tmp/Albumize-0.0.tar.gz` & `tmp/Albumize-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Albumize-0.0.tar", last modified: Sat Jun 17 02:28:58 2023, max compression
+gzip compressed data, was "Albumize-1.0.tar", last modified: Mon Jun 19 01:06:20 2023, max compression
```

## Comparing `Albumize-0.0.tar` & `Albumize-1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 02:28:58.621140 Albumize-0.0/
-drwxrwxrwx   0        0        0        0 2023-06-17 02:28:58.620143 Albumize-0.0/Albumize.egg-info/
--rw-rw-rw-   0        0        0      107 2023-06-17 02:28:58.000000 Albumize-0.0/Albumize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-06-17 02:28:58.000000 Albumize-0.0/Albumize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 02:28:58.000000 Albumize-0.0/Albumize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 02:28:58.000000 Albumize-0.0/Albumize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-17 02:24:01.000000 Albumize-0.0/Albumize.py
--rw-rw-rw-   0        0        0      107 2023-06-17 02:28:58.620143 Albumize-0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-17 02:28:58.621140 Albumize-0.0/setup.cfg
--rw-rw-rw-   0        0        0      139 2023-06-17 02:28:19.000000 Albumize-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:06:20.789943 Albumize-1.0/
+drwxrwxrwx   0        0        0        0 2023-06-19 01:06:20.789943 Albumize-1.0/Albumize.egg-info/
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:06:20.000000 Albumize-1.0/Albumize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-06-19 01:06:20.000000 Albumize-1.0/Albumize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:06:20.000000 Albumize-1.0/Albumize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 01:06:20.000000 Albumize-1.0/Albumize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4666 2023-06-19 01:04:17.000000 Albumize-1.0/Albumize.py
+-rw-rw-rw-   0        0        0      107 2023-06-19 01:06:20.789943 Albumize-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:06:20.789943 Albumize-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      139 2023-06-19 01:05:36.000000 Albumize-1.0/setup.py
```

