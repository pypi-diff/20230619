# Comparing `tmp/smpgpt-4.0.tar.gz` & `tmp/smpgpt-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpgpt-4.0.tar", last modified: Fri Jun 16 21:06:57 2023, max compression
+gzip compressed data, was "smpgpt-8.0.tar", last modified: Mon Jun 19 06:39:34 2023, max compression
```

## Comparing `smpgpt-4.0.tar` & `smpgpt-8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976959 smpgpt-4.0/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.976758 smpgpt-4.0/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-4.0/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-16 21:06:57.977017 smpgpt-4.0/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-16 21:06:53.000000 smpgpt-4.0/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.974766 smpgpt-4.0/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.975622 smpgpt-4.0/src/smpgpt/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-4.0/src/smpgpt/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     1570 2023-06-16 21:06:48.000000 smpgpt-4.0/src/smpgpt/smpgpt.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-16 21:06:57.976529 smpgpt-4.0/src/smpgpt.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-4.0/src/smpgpt.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-16 21:06:57.000000 smpgpt-4.0/src/smpgpt.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.293228 smpgpt-8.0/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:39:34.293060 smpgpt-8.0/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smpgpt-8.0/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-19 06:39:34.293291 smpgpt-8.0/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-19 06:39:31.000000 smpgpt-8.0/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.291422 smpgpt-8.0/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.292114 smpgpt-8.0/src/smpgpt/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smpgpt-8.0/src/smpgpt/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     2478 2023-06-19 06:39:25.000000 smpgpt-8.0/src/smpgpt/smpgpt.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-19 06:39:34.292854 smpgpt-8.0/src/smpgpt.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      231 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-16 20:45:08.000000 smpgpt-8.0/src/smpgpt.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        7 2023-06-19 06:39:34.000000 smpgpt-8.0/src/smpgpt.egg-info/top_level.txt
```

