# Comparing `tmp/ler-0.1.3.tar.gz` & `tmp/ler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ler-0.1.3.tar", last modified: Tue Apr 25 11:28:15 2023, max compression
+gzip compressed data, was "ler-0.1.6.tar", last modified: Mon Jun 19 08:51:53 2023, max compression
```

## Comparing `ler-0.1.3.tar` & `ler-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 11:28:15.393433 ler-0.1.3/
--rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-25 11:28:15.393126 ler-0.1.3/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)       50 2023-04-12 04:14:44.000000 ler-0.1.3/README.md
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 11:28:15.390780 ler-0.1.3/ler/
--rw-r--r--   0 hemantaph   (501) staff       (20)      314 2023-04-18 09:53:24.000000 ler-0.1.3/ler/__init__.py
--rw-r--r--   0 hemantaph   (501) staff       (20)     7651 2023-04-25 09:26:09.000000 ler-0.1.3/ler/helperroutines.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    29203 2023-04-25 09:45:40.000000 ler-0.1.3/ler/lens_galaxy_population.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    36380 2023-04-25 11:26:41.000000 ler-0.1.3/ler/ler.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    12762 2023-04-25 09:41:30.000000 ler-0.1.3/ler/multiprocessing_routine.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    11815 2023-04-25 09:41:41.000000 ler-0.1.3/ler/source_population.py
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 11:28:15.392758 ler-0.1.3/ler.egg-info/
--rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-04-25 11:28:15.000000 ler-0.1.3/ler.egg-info/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      287 2023-04-25 11:28:15.000000 ler-0.1.3/ler.egg-info/SOURCES.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-25 11:28:15.000000 ler-0.1.3/ler.egg-info/dependency_links.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)      131 2023-04-25 11:28:15.000000 ler-0.1.3/ler.egg-info/requires.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-04-25 11:28:15.000000 ler-0.1.3/ler.egg-info/top_level.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-25 11:28:15.393520 ler-0.1.3/setup.cfg
--rw-r--r--   0 hemantaph   (501) staff       (20)      592 2023-04-25 11:28:06.000000 ler-0.1.3/setup.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-06-19 08:51:53.924350 ler-0.1.6/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-06-19 08:51:53.924076 ler-0.1.6/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)       50 2023-04-12 04:14:44.000000 ler-0.1.6/README.md
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-06-19 08:51:53.921523 ler-0.1.6/ler/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      315 2023-06-07 19:37:25.000000 ler-0.1.6/ler/__init__.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)     5504 2023-06-18 19:46:11.000000 ler-0.1.6/ler/helperroutines.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    44200 2023-06-18 19:51:40.000000 ler-0.1.6/ler/lens_galaxy_population.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    62458 2023-06-18 19:31:52.000000 ler-0.1.6/ler/ler.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    16064 2023-06-18 19:43:27.000000 ler-0.1.6/ler/multiprocessing_routine.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    32971 2023-06-18 19:31:00.000000 ler-0.1.6/ler/source_population.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-06-19 08:51:53.923701 ler-0.1.6/ler.egg-info/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      192 2023-06-19 08:51:53.000000 ler-0.1.6/ler.egg-info/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)      287 2023-06-19 08:51:53.000000 ler-0.1.6/ler.egg-info/SOURCES.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-06-19 08:51:53.000000 ler-0.1.6/ler.egg-info/dependency_links.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)      171 2023-06-19 08:51:53.000000 ler-0.1.6/ler.egg-info/requires.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        4 2023-06-19 08:51:53.000000 ler-0.1.6/ler.egg-info/top_level.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-06-19 08:51:53.924436 ler-0.1.6/setup.cfg
+-rw-r--r--   0 hemantaph   (501) staff       (20)      649 2023-06-19 08:51:00.000000 ler-0.1.6/setup.py
```

