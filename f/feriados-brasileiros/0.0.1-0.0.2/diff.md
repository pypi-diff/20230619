# Comparing `tmp/feriados_brasileiros-0.0.1.tar.gz` & `tmp/feriados_brasileiros-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feriados_brasileiros-0.0.1.tar", last modified: Fri Jun 16 05:02:10 2023, max compression
+gzip compressed data, was "feriados_brasileiros-0.0.2.tar", last modified: Mon Jun 19 02:42:59 2023, max compression
```

## Comparing `feriados_brasileiros-0.0.1.tar` & `feriados_brasileiros-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:02:10.402629 feriados_brasileiros-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-16 05:02:10.402629 feriados_brasileiros-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:02:10.402629 feriados_brasileiros-0.0.1/feriados_brasileiros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/feriados_brasileiros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/feriados_brasileiros/feriados.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/feriados_brasileiros/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:02:10.402629 feriados_brasileiros-0.0.1/feriados_brasileiros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-16 05:02:10.000000 feriados_brasileiros-0.0.1/feriados_brasileiros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-16 05:02:10.000000 feriados_brasileiros-0.0.1/feriados_brasileiros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:02:10.000000 feriados_brasileiros-0.0.1/feriados_brasileiros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 05:02:10.000000 feriados_brasileiros-0.0.1/feriados_brasileiros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:02:10.402629 feriados_brasileiros-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 05:01:59.000000 feriados_brasileiros-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/feriados_brasileiros/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/datas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/feriados_brasileiros/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 02:42:59.000000 feriados_brasileiros-0.0.2/feriados_brasileiros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 02:42:59.925416 feriados_brasileiros-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-19 02:42:50.000000 feriados_brasileiros-0.0.2/setup.py
```

### Comparing `feriados_brasileiros-0.0.1/LICENSE` & `feriados_brasileiros-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.1/MANIFEST.in` & `feriados_brasileiros-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.1/setup.py` & `feriados_brasileiros-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
-VERSION = (0, 0, 1)
+VERSION = (0, 0, 2)
 __version__ = '.'.join(map(str, VERSION))
 
 setup(
     name='feriados_brasileiros',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
```

