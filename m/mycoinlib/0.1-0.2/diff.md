# Comparing `tmp/mycoinlib-0.1.tar.gz` & `tmp/mycoinlib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-0.1.tar", last modified: Mon Jun 19 04:47:55 2023, max compression
+gzip compressed data, was "mycoinlib-0.2.tar", last modified: Mon Jun 19 05:14:09 2023, max compression
```

## Comparing `mycoinlib-0.1.tar` & `mycoinlib-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 04:47:55.303811 mycoinlib-0.1/
--rw-rw-rw-   0        0        0       54 2023-06-19 04:47:55.301824 mycoinlib-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 04:47:55.298844 mycoinlib-0.1/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-19 04:47:54.000000 mycoinlib-0.1/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-06-19 04:47:55.000000 mycoinlib-0.1/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 04:47:54.000000 mycoinlib-0.1/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 04:47:54.000000 mycoinlib-0.1/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 04:47:55.304805 mycoinlib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      132 2023-06-19 04:45:20.000000 mycoinlib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 05:14:09.085509 mycoinlib-0.2/
+-rw-rw-rw-   0        0        0       54 2023-06-19 05:14:09.083356 mycoinlib-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 05:14:09.075409 mycoinlib-0.2/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-19 05:14:08.000000 mycoinlib-0.2/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-06-19 05:14:08.000000 mycoinlib-0.2/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:14:08.000000 mycoinlib-0.2/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 05:14:08.000000 mycoinlib-0.2/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 05:14:09.086336 mycoinlib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      132 2023-06-19 05:14:01.000000 mycoinlib-0.2/setup.py
```

