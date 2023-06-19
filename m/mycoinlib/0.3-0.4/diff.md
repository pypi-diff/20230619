# Comparing `tmp/mycoinlib-0.3.tar.gz` & `tmp/mycoinlib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-0.3.tar", last modified: Mon Jun 19 05:19:05 2023, max compression
+gzip compressed data, was "mycoinlib-0.4.tar", last modified: Mon Jun 19 06:40:20 2023, max compression
```

## Comparing `mycoinlib-0.3.tar` & `mycoinlib-0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:19:05.328698 mycoinlib-0.3/
--rw-rw-rw-   0        0        0       54 2023-06-19 05:19:05.239784 mycoinlib-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 05:19:04.238306 mycoinlib-0.3/mycoinlib/
--rw-rw-rw-   0        0        0       34 2023-06-19 05:13:48.000000 mycoinlib-0.3/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0      693 2023-06-19 05:13:50.000000 mycoinlib-0.3/mycoinlib/mycoinlib.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:19:05.172231 mycoinlib-0.3/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-19 05:19:03.000000 mycoinlib-0.3/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-19 05:19:03.000000 mycoinlib-0.3/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:19:03.000000 mycoinlib-0.3/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 05:19:03.000000 mycoinlib-0.3/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 05:19:05.333665 mycoinlib-0.3/setup.cfg
--rw-rw-rw-   0        0        0      132 2023-06-19 05:18:53.000000 mycoinlib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:40:20.226275 mycoinlib-0.4/
+-rw-rw-rw-   0        0        0       54 2023-06-19 06:40:20.215675 mycoinlib-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 06:40:19.832679 mycoinlib-0.4/mycoinlib/
+-rw-rw-rw-   0        0        0       34 2023-06-19 05:13:48.000000 mycoinlib-0.4/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     1159 2023-06-19 06:33:04.000000 mycoinlib-0.4/mycoinlib/mycoinlib.py
+drwxrwxrwx   0        0        0        0 2023-06-19 06:40:20.205415 mycoinlib-0.4/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 06:40:20.257586 mycoinlib-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-06-19 06:34:41.000000 mycoinlib-0.4/setup.py
```

