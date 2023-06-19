# Comparing `tmp/DeepLogTimedelta-0.0.3.tar.gz` & `tmp/DeepLogTimedelta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.0.3.tar", last modified: Mon Jun 19 13:28:41 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.1.0.tar", last modified: Mon Jun 19 13:29:04 2023, max compression
```

## Comparing `DeepLogTimedelta-0.0.3.tar` & `DeepLogTimedelta-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:28:41.313773 DeepLogTimedelta-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:28:41.293458 DeepLogTimedelta-0.0.3/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     1100 2023-06-19 13:11:20.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2309 2023-06-19 13:28:17.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:28:41.310768 DeepLogTimedelta-0.0.3/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-19 13:28:41.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-19 13:28:41.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:28:41.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 13:28:41.000000 DeepLogTimedelta-0.0.3/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-19 13:28:41.313773 DeepLogTimedelta-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 13:28:41.314913 DeepLogTimedelta-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-19 13:28:37.000000 DeepLogTimedelta-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.601192 DeepLogTimedelta-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.575687 DeepLogTimedelta-0.1.0/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     1100 2023-06-19 13:11:20.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2309 2023-06-19 13:28:17.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:29:04.598003 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 13:29:04.000000 DeepLogTimedelta-0.1.0/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-19 13:29:04.600188 DeepLogTimedelta-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:29:04.601192 DeepLogTimedelta-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-19 13:29:01.000000 DeepLogTimedelta-0.1.0/setup.py
```

### Comparing `DeepLogTimedelta-0.0.3/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.1.0/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files identical despite different names*

### Comparing `DeepLogTimedelta-0.0.3/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.1.0/DeepLogTimedelta/preproccesing.py`

 * *Files identical despite different names*

