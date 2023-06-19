# Comparing `tmp/mycoinlib-0.4.tar.gz` & `tmp/mycoinlib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-0.4.tar", last modified: Mon Jun 19 06:40:20 2023, max compression
+gzip compressed data, was "mycoinlib-0.5.tar", last modified: Mon Jun 19 09:27:46 2023, max compression
```

## Comparing `mycoinlib-0.4.tar` & `mycoinlib-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 06:40:20.226275 mycoinlib-0.4/
--rw-rw-rw-   0        0        0       54 2023-06-19 06:40:20.215675 mycoinlib-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 06:40:19.832679 mycoinlib-0.4/mycoinlib/
--rw-rw-rw-   0        0        0       34 2023-06-19 05:13:48.000000 mycoinlib-0.4/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0     1159 2023-06-19 06:33:04.000000 mycoinlib-0.4/mycoinlib/mycoinlib.py
-drwxrwxrwx   0        0        0        0 2023-06-19 06:40:20.205415 mycoinlib-0.4/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 06:40:19.000000 mycoinlib-0.4/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 06:40:20.257586 mycoinlib-0.4/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-06-19 06:34:41.000000 mycoinlib-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:27:46.004103 mycoinlib-0.5/
+-rw-rw-rw-   0        0        0       54 2023-06-19 09:27:45.970331 mycoinlib-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 09:27:45.659882 mycoinlib-0.5/mycoinlib/
+-rw-rw-rw-   0        0        0       34 2023-06-19 05:13:48.000000 mycoinlib-0.5/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     2540 2023-06-19 09:25:13.000000 mycoinlib-0.5/mycoinlib/mycoinlib.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:27:45.964370 mycoinlib-0.5/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-19 09:27:45.000000 mycoinlib-0.5/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-19 09:27:45.000000 mycoinlib-0.5/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:27:45.000000 mycoinlib-0.5/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-19 09:27:45.000000 mycoinlib-0.5/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-19 09:27:45.000000 mycoinlib-0.5/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:27:46.005096 mycoinlib-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-19 09:25:28.000000 mycoinlib-0.5/setup.py
```

