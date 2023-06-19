# Comparing `tmp/pystorz-0.3.5.tar.gz` & `tmp/pystorz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.3.5.tar", last modified: Sun Jun 18 01:32:12 2023, max compression
+gzip compressed data, was "pystorz-0.4.0.tar", last modified: Mon Jun 19 17:35:10 2023, max compression
```

## Comparing `pystorz-0.3.5.tar` & `pystorz-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.353195 pystorz-0.3.5/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.5/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-18 01:32:12.352971 pystorz-0.3.5/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.5/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.342860 pystorz-0.3.5/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.5/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.344077 pystorz-0.3.5/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.5/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.344532 pystorz-0.3.5/pystorz/meta/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.5/pystorz/meta/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.5/pystorz/meta/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.346067 pystorz-0.3.5/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.5/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.5/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.5/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.347985 pystorz-0.3.5/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.5/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.5/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.5/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.5/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.5/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.349151 pystorz-0.3.5/pystorz/rest/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.5/pystorz/rest/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/rest/client.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.5/pystorz/rest/headers.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/rest/internals.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.5/pystorz/rest/server.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.349608 pystorz-0.3.5/pystorz/router/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.5/pystorz/router/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2336 2023-06-18 00:52:08.000000 pystorz-0.3.5/pystorz/router/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.351100 pystorz-0.3.5/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.5/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2544 2023-06-18 01:30:20.000000 pystorz-0.3.5/pystorz/sql/adapter.py
--rw-r--r--   0 wazofski   (501) staff       (20)      876 2023-06-18 01:24:36.000000 pystorz-0.3.5/pystorz/sql/mysql.py
--rw-r--r--   0 wazofski   (501) staff       (20)      470 2023-06-18 01:24:50.000000 pystorz-0.3.5/pystorz/sql/sqlite.py
--rw-r--r--   0 wazofski   (501) staff       (20)    15152 2023-06-18 01:17:02.000000 pystorz-0.3.5/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.352399 pystorz-0.3.5/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.5/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.5/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.5/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.343752 pystorz-0.3.5/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1104 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-18 01:32:12.353261 pystorz-0.3.5/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-18 00:43:38.000000 pystorz-0.3.5/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.777354 pystorz-0.4.0/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.4.0/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-19 17:35:10.777188 pystorz-0.4.0/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.4.0/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.768400 pystorz-0.4.0/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.4.0/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.769366 pystorz-0.4.0/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.4.0/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.4.0/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.769769 pystorz-0.4.0/pystorz/meta/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.4.0/pystorz/meta/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.4.0/pystorz/meta/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.770815 pystorz-0.4.0/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.4.0/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     5586 2023-06-19 02:28:25.000000 pystorz-0.4.0/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7560 2023-06-19 01:54:15.000000 pystorz-0.4.0/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.772779 pystorz-0.4.0/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.4.0/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       75 2023-06-19 01:22:47.000000 pystorz-0.4.0/pystorz/mgen/templates/clone.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      111 2023-06-19 01:22:29.000000 pystorz-0.4.0/pystorz/mgen/templates/cloneimp.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.4.0/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      462 2023-06-19 00:35:26.000000 pystorz-0.4.0/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.4.0/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      540 2023-06-19 01:46:45.000000 pystorz-0.4.0/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1022 2023-06-19 00:31:14.000000 pystorz-0.4.0/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1875 2023-06-19 01:23:56.000000 pystorz-0.4.0/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.4.0/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.4.0/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.773850 pystorz-0.4.0/pystorz/rest/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.4.0/pystorz/rest/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     8303 2023-06-19 17:32:50.000000 pystorz-0.4.0/pystorz/rest/client.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.4.0/pystorz/rest/headers.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2451 2023-06-19 17:24:42.000000 pystorz-0.4.0/pystorz/rest/internals.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9642 2023-06-19 17:28:16.000000 pystorz-0.4.0/pystorz/rest/server.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.774224 pystorz-0.4.0/pystorz/router/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.4.0/pystorz/router/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2336 2023-06-18 00:52:08.000000 pystorz-0.4.0/pystorz/router/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.776056 pystorz-0.4.0/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.4.0/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2671 2023-06-19 02:47:21.000000 pystorz-0.4.0/pystorz/sql/adapter.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      876 2023-06-18 01:24:36.000000 pystorz-0.4.0/pystorz/sql/mysql.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      470 2023-06-18 01:24:50.000000 pystorz-0.4.0/pystorz/sql/sqlite.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15173 2023-06-19 17:32:42.000000 pystorz-0.4.0/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.776906 pystorz-0.4.0/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.4.0/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    10736 2023-06-19 01:10:48.000000 pystorz-0.4.0/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     6078 2023-06-19 17:24:38.000000 pystorz-0.4.0/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3311 2023-06-19 17:32:31.000000 pystorz-0.4.0/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-19 17:35:10.769087 pystorz-0.4.0/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-19 17:35:10.000000 pystorz-0.4.0/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1110 2023-06-19 17:35:10.000000 pystorz-0.4.0/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-19 17:35:10.000000 pystorz-0.4.0/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-19 17:35:10.000000 pystorz-0.4.0/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-19 17:35:10.000000 pystorz-0.4.0/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-19 17:35:10.777393 pystorz-0.4.0/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-19 02:26:36.000000 pystorz-0.4.0/setup.py
```

### Comparing `pystorz-0.3.5/LICENSE` & `pystorz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/PKG-INFO` & `pystorz-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.5
+Version: 0.4.0
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-        </p>
-        
-        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-        
-        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-        
-        Original storz was written in go. You can check it out here:
-        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-        
-        This is a python port of the original storz.
-        Still in development.
-        
-        ## Quick Start Guide
-        
-        ### Installation
-        ```
-        pip install pystorz
-        ```
-        
-        ## Model example
-        
-        You can find a saomple model in the tests folder.
-        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-        
-        You can define simple structures and reference them as fields in other structures.
-        
-        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-        
-        Only a SQLite store is implemented at the moment.
-        
-        More to come.
-        Check out the go version (link above) for more information.
-        
-        ## Usage
-        ```
-            from pystorz.mgen import builder
-        
-            # run the code gen to 
-            builder.Generate("path/to/model.yml")
-            # this will make a generated folder in the project home directory
-        
-            # you can then import the generated model
-            from generated import model
-        
-            # initialize a store
-            stor = SqliteStore(
-                Schema(),
-                SqliteConnector("path/to/your/sqlite3.db"))
-        
-            world = model.WorldFactory()
-            world.External().SetName("hello")
-        
-            created_world = stor.Create(world)
-            world.External().SetDescription("hello world")
-            updated_world = stor.Update(world.Metadata().Identity(), world)
-            
-            # ...
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+</p>
+
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+
+Original storz was written in go. You can check it out here:
+[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+
+This is a python port of the original storz.
+Still in development.
+
+## Quick Start Guide
+
+### Installation
+```
+pip install pystorz
+```
+
+## Model example
+
+You can find a saomple model in the tests folder.
+[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+
+You can define simple structures and reference them as fields in other structures.
+
+You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+
+Only a SQLite store is implemented at the moment.
+
+More to come.
+Check out the go version (link above) for more information.
+
+## Usage
+```
+    from pystorz.mgen import builder
+
+    # run the code gen to 
+    builder.Generate("path/to/model.yml")
+    # this will make a generated folder in the project home directory
+
+    # you can then import the generated model
+    from generated import model
+
+    # initialize a store
+    stor = SqliteStore(
+        Schema(),
+        SqliteConnector("path/to/your/sqlite3.db"))
+
+    world = model.WorldFactory()
+    world.External().SetName("hello")
+
+    created_world = stor.Create(world)
+    world.External().SetDescription("hello world")
+    updated_world = stor.Update(world.Metadata().Identity(), world)
+    
+    # ...
+
+```
```

### Comparing `pystorz-0.3.5/README.md` & `pystorz-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/meta/store.py` & `pystorz-0.4.0/pystorz/meta/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/mgen/builder.py` & `pystorz-0.4.0/pystorz/mgen/builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,22 +23,25 @@
         s, r = load_model(model)
         
         structs.extend(s)
         resources.extend(r)
 
     imports = [
         "import json",
+        "from pystorz.internal import constants",
         "from pystorz.store import utils",
         "from pystorz.store import store",
-        "from pystorz.store import meta",
+        "from datetime import datetime",
+        "from typing import Type",
     ]
 
     b = StringIO()
 
     b.write(render("mgen/templates/imports.py", {"imports": imports}))
+
     b.write(compileStructs(structs))
     b.write(compileResources(resources))
 
     res = b.getvalue().replace("&#34;", "\"")
 
     # refactor and format python code
     res = reformat_python_code(res)
@@ -59,15 +62,15 @@
         log.debug(f"Compiling resource {r.name}...")
 
         props = [
             Prop(
                 "Meta",
                 "store.Meta",
                 "metadata",
-                f'meta.MetaFactory("{r.name}")')
+                f'store.MetaFactory("{r.name}")')
         ]
 
         if r.external:
             props.append(Prop(
                 "External",
                 r.external,
                 "external"))
@@ -76,73 +79,120 @@
             props.append(Prop(
                 "Internal",
                 r.internal,
                 "internal"))
 
         s = Struct(
             r.name,
-            r.name,
+            "store.Object",
             props,
         )
 
         b.write(compileStruct(s))
         b.write(render("mgen/templates/meta.py", r))
 
     b.write(render("mgen/templates/schema.py", {"resources": resources}))
 
     return b.getvalue()
 
 
 def compileStructs(structs: list[Struct]) -> str:
     b = StringIO()
 
-    for s in structs:
-        b.write(compileStruct(s))
+    dep, nodep = checkDependencies(structs)
 
+    for s in nodep:
+        b.write(compileStruct(s))
+    
+    for s in dep:
+        b.write(compileStruct(s))
+    
     return b.getvalue()
 
 
+def checkDependencies(structs: list[Struct]) -> tuple[list[Struct], list[Struct]]:
+    dep = []
+    nodep = []
+
+    known_types = ["string", "int", "float", "bool", "datetime"]
+
+    for s in structs:
+        for p in s.properties:
+            if p.IsArray():
+                elem_type = p.SubType()
+                if elem_type not in known_types:
+                    dep.append(s)
+                    break
+                continue
+
+            if p.IsMap():
+                # map[int]string
+                elem_type = p.SubType()
+                key_type = p.type[4:].split("]")[0]
+                val_type = p.type[4:].split("]")[1]
+                if key_type not in known_types:
+                    dep.append(s)
+                    break
+
+                if val_type not in known_types:
+                    dep.append(s)
+                    break
+                continue
+
+            if p.type not in known_types:
+                dep.append(s)
+                break
+    
+    for s in structs:
+        if s not in dep:
+            nodep.append(s)
+
+    return (dep, nodep)
+
+
 def compileStruct(s: Struct) -> str:
     log.debug(f"Compiling struct {s.name}...")
 
     b = StringIO()
     methods = []
 
     s.properties = addDefaultPropValues(s.properties)
 
-    parent = "" # s.implements
+    parent = s.implements
 
     for p in s.properties:
         if p.name != "Meta":
             # methods.append(f"{p.name}(self) -> {p.StrippedType()}")
-            methods.append(f"{p.name}(self)")
+            methods.append((f"{p.name}(self)", p.StrippedType()))
 
         if p.name != "Meta" and p.name != "External" and p.name != "Internal":
             # methods.append(f"Set{p.name}(self, val: {p.StrippedType()})")
-            methods.append(f"Set{p.name}(self, val)")
+            methods.append((f"Set{p.name}(self, val: {p.StrippedType()})", ""))
 
         if p.name == "External":
             parent = "store.ExternalHolder"
     
     b.write(
         render(
             "mgen/templates/interface.py",
             {
                 'name': s.name,
                 'methods': methods,
                 'implements': parent
             }))
 
-    for p in s.properties:
-        if p.name == "External":
-            b.write(render("mgen/templates/specinternal.py", None))
+    if parent in ["store.Object", "store.ExternalHolder"]:
+        b.write(render("mgen/templates/clone.py", s))
 
     b.write(render("mgen/templates/structure.py", s))
     b.write(render("mgen/templates/unmarshall.py", s))
 
+    if parent in ["store.Object", "store.ExternalHolder"]:
+        b.write(render("mgen/templates/cloneimp.py", s))
+
     return b.getvalue()
 
 
 def render(rpath: str, data) -> str:
     path = os.path.join(utils.runtime_dir(), rpath)
 
     with open(path, 'r') as f:
```

### Comparing `pystorz-0.3.5/pystorz/mgen/loader.py` & `pystorz-0.4.0/pystorz/mgen/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 
     def IsArray(self):
         if len(self.type) < 2:
             return False
 
         return self.type[:2] == "[]"
 
+    def SubType(self):
+        if self.IsMap() or self.IsArray():
+            return self.type.split("]")[1]
+
+        return self.type
+
+    def IsComplexType(self):
+        res = self.SubType() not in ["string", "int", "float", "bool", "datetime"]
+        log.debug("IsComplexType: {} {} -> {}".format(self.name, self.SubType(), res))
+        return res
+
     def StrippedType(self):
         if self.IsMap():
             return "dict"
         if self.IsArray():
             return "list"
         if self.type == "string":
             return "str"
@@ -89,15 +100,16 @@
 
         for m in model["types"]:
             if m["kind"].lower() == "struct":
                 if m["name"] in struct_cache:
                     raise Exception("duplicate struct: {}".format(m["name"]))
                 struct_cache.add(m["name"])
 
-                structs.append(Struct(m["name"], "", capitalize_props(m["properties"])))
+                structs.append(
+                    Struct(m["name"], "", capitalize_props(m["properties"])))
                 continue
             if m["kind"].lower() == "object":
                 if m["name"] in resource_cache:
                     raise Exception("duplicate object: {}".format(m["name"]))
                 resource_cache.add(m["name"])
 
                 pkey = "metadata.identity"
@@ -138,25 +150,26 @@
 
     for s in structs:
         known_types.append(s.name)
 
     for s in structs:
         for p in s.properties:
             if p.IsArray():
-                elem_type = p.type[2:]
+                elem_type = p.SubType()
                 if elem_type not in known_types:
                     errors.append(
                         "struct {} property {}: unknown type: {}".format(
                             s.name, p.name, elem_type
                         )
                     )
                 continue
 
             if p.IsMap():
                 # map[int]string
+                elem_type = p.SubType()
                 key_type = p.type[4:].split("]")[0]
                 val_type = p.type[4:].split("]")[1]
                 if key_type not in known_types:
                     errors.append(
                         "struct {} property {}: unknown type: {}".format(
                             s.name, p.name, elem_type
                         )
@@ -174,27 +187,30 @@
                     "struct {} property {}: unknown type: {}".format(
                         s.name, p.name, p.type
                     )
                 )
 
     for r in resources:
         if r.external is None and r.internal is None:
-            errors.append("resource {} has no internal and external".format(r.name))
+            errors.append(
+                "resource {} has no internal and external".format(r.name))
             continue
 
         if r.external is not None:
             if r.external not in known_types:
                 errors.append(
-                    "resource {} external: unknown type: {}".format(r.name, r.external)
+                    "resource {} external: unknown type: {}".format(
+                        r.name, r.external)
                 )
 
         if r.internal is not None:
             if r.internal not in known_types:
                 errors.append(
-                    "resource {} internal: unknown type: {}".format(r.name, r.internal)
+                    "resource {} internal: unknown type: {}".format(
+                        r.name, r.internal)
                 )
 
     return errors
 
 
 def read_model(path: str):
     log.debug(f"reading model from {path}")
@@ -246,20 +262,18 @@
     if tp == "datetime":
         return '"0001-01-01T00:00:00.000000Z"'
 
     return f"{tp}Factory()"
 
 
 def complexTypeValueDefault(tp: str) -> str:
-    log.debug(f"typeValueDefault: {tp}")
-
     if tp.startswith("[]"):
         return typeDefault(tp[2:])
 
     if tp.startswith("map"):
         closing_bracket_index = tp.find("]")
         if closing_bracket_index == -1:
             raise Exception("invalid map type: {}".format(tp))
 
-        return typeDefault(tp[closing_bracket_index + 1 :])
+        return typeDefault(tp[closing_bracket_index + 1:])
 
     raise Exception("unknown type: {}".format(tp))
```

### Comparing `pystorz-0.3.5/pystorz/mgen/templates/structure.py` & `pystorz-0.4.0/pystorz/mgen/templates/structure.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
  
 
-def {{ data.name }}Factory():
+def {{ data.name }}Factory() -> {{ data.name }}:
 	ret = _{{ data.name }}()
 	{% for prop in data.properties %}
 	ret.{{ prop.name }}_ = {{ prop.default }}{% endfor %}
 	
 	return ret
 
 
-class _{{ data.name }}({{data.implements}}):
+class _{{ data.name }}({{data.name}}):
 
 	def __init__(self):
 		{% for prop in data.properties %}
 		self.{{ prop.name }}_ = {{prop.default}}{% endfor %}
 
 	{% for prop in data.properties %}
-	{% if prop.name != "External" %}
 
 	def Set{{ prop.name }}(self, val):
 		{% if prop.type == "datetime" %}
 		self.{{ prop.name }}_ = utils.datetime_string(val)
 		{% elif prop.type == "string" %}
 		self.{{ prop.name }}_ = str(val)
 		{% elif prop.type == "int" %}
@@ -35,13 +34,9 @@
 	def {{ prop.name }}(self):
 		{% if prop.type == "datetime" %}
 		return utils.datetime_parse(self.{{ prop.name }}_)
 		{% else %}
 		return self.{{ prop.name }}_
 		{% endif %}
 
-	{% endif %}
 	{% endfor %}
 
-	def Clone(entity):
-		return utils.clone_object(entity, Schema())
-
```

### Comparing `pystorz-0.3.5/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.4.0/pystorz/mgen/templates/unmarshall.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,35 +10,39 @@
 
 	def ToDict(self):
 		data = {}
 		{% for prop in data.properties %}
 		{% if prop.IsArray() %}
 		rawList = []
 		for v in self.{{prop.name}}_:
-			if hasattr(v, "ToDict"):
-				rawList.append(v.ToDict())
-			else:
-				rawList.append(v)
+			{% if prop.IsComplexType() %}
+			rawList.append(v.ToDict())
+			{% else %}
+			rawList.append(v)
+			{% endif %}
 
 		data["{{prop.json}}"] = rawList
 		{% elif prop.IsMap() %}
 		rawSubmap = {}
 		for k, v in self.{{prop.name}}_.items():
-			if hasattr(v, "ToDict"):
-				rawSubmap[k] = v.ToDict()
-			else:
-				rawSubmap[k] = v
+			{% if prop.IsComplexType() %}
+			rawSubmap[k] = v.ToDict()
+			{% else %}
+			rawSubmap[k] = v
+			{% endif %}
 
 		data["{{prop.json}}"] = rawSubmap
 		{% else %}
-	
-		if self.{{prop.name}}_ is not None and hasattr(self.{{prop.name}}_, "ToDict"):
-			data["{{prop.json}}"] = self.{{prop.name}}_.ToDict()
-		else:
-			data["{{prop.json}}"] = self.{{prop.name}}_
+		
+		{% if prop.IsComplexType() %}
+		# if self.{{prop.name}}_ is not None:
+		data["{{prop.json}}"] = self.{{prop.name}}_.ToDict()
+		{% else %}
+		data["{{prop.json}}"] = self.{{prop.name}}_
+		{% endif %}
 	
 		{% endif %}
 		{% endfor %}
 		return data
 	
 
 	def FromDict(self, data):
@@ -49,36 +53,39 @@
 			{% for prop in data.properties %}
 			if key == "{{prop.json}}":
 				{% if prop.IsArray() %}
 				res = {{ prop.default }}
 
 				for rw in rawValue:
 					ud = {{ prop.ComplexTypeValueDefault() }}
-					if hasattr(ud, "FromDict"):
-						ud.FromDict(rw)
-					else:
-						ud = rw
+					{% if prop.IsComplexType() %}
+					ud.FromDict(rw)
+					{% else %}
+					ud = rw
+					{% endif %}
 					res.append(ud)
 
 				self.{{prop.name}}_ = res
 				{% elif prop.IsMap() %}
 				res = {{ prop.default }}
 				
 				for rk, rw in rawValue.items():
 					ud = {{prop.ComplexTypeValueDefault()}}
-					if hasattr(ud, "FromDict"):
-						ud.FromDict(rw)
-					else:
-						ud = rw
+					{% if prop.IsComplexType() %}
+					ud.FromDict(rw)
+					{% else %}
+					ud = rw
+					{% endif %}
 					res[rk] = ud
 
 				self.{{prop.name}}_ = res
 				{% else %}
-				if hasattr(self.{{prop.name}}_, "FromDict"):
-					self.{{prop.name}}_.FromDict(rawValue)
-				else:
-					self.{{prop.name}}_ = rawValue
+				{% if prop.IsComplexType() %}
+				self.{{prop.name}}_.FromDict(rawValue)
+				{% else %}
+				self.{{prop.name}}_ = rawValue
+				{% endif %}
 				
 				{% endif %}
 			{% endfor %}
```

### Comparing `pystorz-0.3.5/pystorz/mgen/test.py` & `pystorz-0.4.0/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/mgen/utils.py` & `pystorz-0.4.0/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/rest/client.py` & `pystorz-0.4.0/pystorz/rest/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # from urllib.parse import urljoin, urlunparse, urlencode
 from urllib.parse import quote, urlparse
 
 
 log = logging.getLogger(__name__)
 
 
-class RestOptions:
+class RestOptions(options.CommonOptionHolder):
     def __init__(self):
-        self.common_option_holder = options.CommonOptionHolderFactory()
+        super().__init__()
         self.headers = {}
 
-    def common_options(self):
-        return self.common_option_holder
+    def common_options(self) -> options.CommonOptionHolder:
+        return self
 
 
 def new_rest_options(d):
     res = RestOptions()
     res.headers = {}
 
     for h in d.headers:
@@ -250,15 +250,16 @@
 
         parsed = json.loads(res)
 
         marshalledResult = store.ObjectList()
         if len(parsed) == 0:
             return marshalledResult
 
-        resource = self.schema.ObjectForKind(utils.object_kind(parsed[0]))
+        resource = self.schema.ObjectForKind(
+            utils.object_kind(parsed[0]))
 
         for r in parsed:
             clone = resource.Clone()
             clone.FromDict(r)
 
             marshalledResult.append(clone)
 
@@ -271,14 +272,15 @@
         response = requests.request(
             request_type, path, data=content, headers=headers
         )
 
         # response.raise_for_status()
 
         return response.content
+        # return str(response.content)
 
     def _process_request(self, request_url, content, method, headers):
         req_id = str(uuid.uuid4())
 
         request_url = request_url.lower()
         url = urlparse(request_url)
         path = url.path
```

### Comparing `pystorz-0.3.5/pystorz/rest/headers.py` & `pystorz-0.4.0/pystorz/rest/headers.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/rest/internals.py` & `pystorz-0.4.0/pystorz/rest/internals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
             obj.Metadata().Kind(),
             obj.PrimaryKey()))
 
         original = self.Schema.ObjectForKind(obj.Metadata().Kind())
         if original is None:
             raise Exception(constants.ErrInvalidPath)
 
-        if isinstance(obj, store.ExternalHolder):
-            original.ExternalInternalSet(obj.External())
+        if isinstance(original, store.ExternalHolder):
+            original.SetExternal(obj.External())
 
         return self.Store.Create(original, *opt)
 
     def Update(
         self,
         identity: store.ObjectIdentity,
         obj: store.Object,
@@ -41,15 +41,15 @@
         if obj is None:
             raise Exception(constants.ErrObjectNil)
 
         log.info("update {}".format(identity.Path()))
 
         original = self.Store.Get(identity)
         if isinstance(obj, store.ExternalHolder):
-            original.ExternalInternalSet(obj.External())
+            original.SetExternal(obj.External())
 
         if original.Metadata().Kind() != obj.Metadata().Kind():
             raise Exception(constants.ErrObjectIdentityMismatch)
 
         return self.Store.Update(identity, original, *opt)
 
     def Delete(self, identity: store.ObjectIdentity, *opt: options.DeleteOption):
```

### Comparing `pystorz-0.3.5/pystorz/rest/server.py` & `pystorz-0.4.0/pystorz/rest/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,15 @@
         error_code = 404
     if msg == constants.ErrInvalidMethod:
         error_code = 405
 
     return _error_response(error_code, msg)
 
 
-def _json_response(code: int, data: dict):
-    log.debug(data)
-
+def _json_response(code: int, data):
     try:
         ret = json.dumps(data)
         log.debug("""json response: 
     {}""".format(utils.pp(data)))
 
         return ret, code, {"Content-Type": "application/json"}
     except Exception as e:
@@ -86,16 +84,15 @@
 
         return _handle_path(stor, iddentifier, robject)
 
     return handler
 
 
 def _handle_path(
-    stor: store.Store, identity: store.ObjectIdentity, object: store.Object
-):
+    stor: store.Store, identity: store.ObjectIdentity, object):
     log.info("handle path {}".format(identity.Path()))
     log.info("method {}".format(request.method))
 
     ret = None
     if request.method == ActionGet:
         try:
             ret = stor.Get(identity)
@@ -213,21 +210,21 @@
 
         return _error_response(405, constants.ErrInvalidMethod)
 
     return handler
 
 
 class Expose:
-    def __init__(self, kind: str, *actions: list):
+    def __init__(self, kind: str, *actions: str):
         self.Kind = kind
         self.Actions = actions
 
 
 class Server:
-    def __init__(self, schema, thestore, *to_expose: list[Expose]):
+    def __init__(self, schema, thestore, *to_expose: Expose):
         self.Schema = schema
         self.Store = InternalStore(schema, thestore)
 
         accepted_actions = set([ActionGet, ActionCreate, ActionUpdate, ActionDelete])
 
         exposed = {}
         for e in to_expose:
```

### Comparing `pystorz-0.3.5/pystorz/router/store.py` & `pystorz-0.4.0/pystorz/router/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/sql/adapter.py` & `pystorz-0.4.0/pystorz/sql/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
         self._cursor = None
 
     def connect(self):
         raise NotImplementedError()
 
     def connection(self):
         if not self._connection:
-            self._connection = self.connect()
             self._cursor = None
-        
+            self._connection = self.connect()
+
         return self._connection
 
     def cursor(self, retry=True):
         try:
             if not self._cursor:
                 connection = self.connection()
                 self._cursor = connection.cursor()
@@ -52,51 +52,55 @@
                 return cursor.execute(query, params)
             else:
                 return cursor.execute(query)
         except Exception as err:
             if not retry:
                 raise err
 
+        self._cursor = None
         self._connection = None
         return self.execute(query, params, False)
 
     def fetchall(self, retry=True):
         try:
             return self.cursor().fetchall()
         except Exception as err:
             if not retry:
                 raise err
 
+        self._cursor = None
         self._connection = None
         return self.fetchall(False)
-    
 
     def fetchone(self, retry=True):
         try:
             return self.cursor().fetchone()
         except Exception as err:
             if not retry:
                 raise err
 
+        self._cursor = None
         self._connection = None
         return self.fetchone(False)
 
     def commit(self, retry=True):
         try:
             return self.connection().commit()
         except Exception as err:
             log.info(f"exception: {retry}")
             if not retry:
                 raise err
 
+        self._cursor = None
         self._connection = None
         return self.commit(False)
 
     def rollback(self, retry=True):
         try:
             return self.connection().rollback()
         except Exception as err:
             if not retry:
                 raise err
 
+        self._cursor = None
         self._connection = None
         return self.rollback(False)
```

### Comparing `pystorz-0.3.5/pystorz/sql/mysql.py` & `pystorz-0.4.0/pystorz/sql/mysql.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.5/pystorz/sql/store.py` & `pystorz-0.4.0/pystorz/sql/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,16 @@
                 existing.Metadata().Identity().Path()
                 != obj.Metadata().Identity().Path()
             ):
                 raise Exception(constants.ErrObjectIdentityMismatch)
 
             # see if there is an object with the new primary key value
             target_identity = store.ObjectIdentity(
-                "{}/{}".format(existing.Metadata().Kind().lower(), obj.PrimaryKey())
+                "{}/{}".format(existing.Metadata().Kind().lower(),
+                               obj.PrimaryKey())
             )
 
             target = None
             try:
                 target = self.Get(target_identity)
             except Exception as e:
                 pass
@@ -110,15 +111,15 @@
                 raise Exception(constants.ErrObjectExists)
 
         db = self._connection()
 
         try:
             # Start a transaction
             db.execute("BEGIN")
-            
+
             self._removeIdentity(db, existing.Metadata().Identity().Path())
 
             obj.Metadata().SetIdentity(existing.Metadata().Identity())
 
             self._setIdentity(
                 db,
                 obj.Metadata().Identity().Path(),
@@ -143,40 +144,38 @@
             raise Exception(constants.ErrInvalidPath)
 
         log.info("delete {}".format(identity.Path()))
         copt = options.CommonOptionHolderFactory()
         for o in opt:
             o.ApplyFunction()(copt)
 
-        existing = None
-        if copt.filter is None:
-            existing = self.Get(identity)
-
         db = self._connection()
 
-        # try:
-        # Start a transaction
-        db.execute("BEGIN")
-        
-        if copt.filter is None:
-            self._removeIdentity(db, existing.Metadata().Identity().Path())
-            self._removeObject(
-                db, existing.PrimaryKey(), existing.Metadata().Kind()
-            )
-        else:
-            clause = self._buildFilterClause(copt, identity)
-            keys = self._getObjectKeys(db, identity.Type(), clause)
+        try:
+            # Start a transaction
+            db.execute("BEGIN")
 
-            self._removeObjects(db, identity.Type(), clause)
-            self._removeIdentities(db, identity.Type(), keys)
+            if copt.filter is None:
+                existing = self.Get(identity)
 
-        db.commit()
-        # except Exception as e:
-        #     db.rollback()
-        #     raise e
+                self._removeIdentity(db, existing.Metadata().Identity().Path())
+                self._removeObject(
+                    db, existing.PrimaryKey(), existing.Metadata().Kind()
+                )
+            else:
+                clause = self._buildFilterClause(copt, identity)
+                keys = self._getObjectKeys(db, identity.Type(), clause)
+
+                self._removeObjects(db, identity.Type(), clause)
+                self._removeIdentities(db, identity.Type(), keys)
+
+            db.commit()
+        except Exception as e:
+            db.rollback()
+            raise e
 
     def Get(self, identity, *opt):
         if identity is None:
             raise Exception(constants.ErrInvalidPath)
 
         log.info("get {}".format(identity.Path()))
 
@@ -188,34 +187,33 @@
 
         res = None
         if identity.IsId():
             pkey, typ = self._getIdentity(db, identity.Path())
             res = self._getObject(db, pkey, typ)
         else:
             res = self._getObject(db, identity.Key(), identity.Type())
-        
+
         db.commit()
         return res
 
-    def List(self, identity, *opt: list[options.ListOption]):
+    def List(self, identity, *opt: options.ListOption):
         if identity is None:
             raise Exception(constants.ErrInvalidPath)
 
         log.info("list {}".format(identity.Path()))
 
         if len(identity.Key()) > 0:
             raise Exception(constants.ErrInvalidPath)
 
         copt = options.CommonOptionHolderFactory()
-
         for o in opt:
             o.ApplyFunction()(copt)
 
         db = self._connection()
-        
+
         query = """SELECT Object FROM Objects 
         WHERE Type = '{}'""".format(
             identity.Type()
         )
 
         query += self._buildFilterClause(copt, identity)
 
@@ -257,15 +255,14 @@
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL,
             Object JSON,
             PRIMARY KEY (Pkey,Type));
         """
 
         db.execute(create)
-        
         db.commit()
 
     def _getIdentity(self, db, path):
         query = """SELECT Pkey, Type FROM IdIndex 
         WHERE Path='{}'""".format(
             path
         )
@@ -372,16 +369,17 @@
         for row in rows:
             res.append(row[0])
         return res
 
     def _removeIdentities(self, db, typ, keys):
         batch_size = 100
         for i in range(0, len(keys), batch_size):
-            batch = keys[i : i + batch_size]
-            clause = "Pkey IN ({})".format(",".join(["'{}'".format(k) for k in batch]))
+            batch = keys[i: i + batch_size]
+            clause = "Pkey IN ({})".format(
+                ",".join(["'{}'".format(k) for k in batch]))
 
             query = """DELETE FROM IdIndex
                 WHERE Type = '{}' AND {}""".format(
                 typ.lower(),
                 clause,
             )
 
@@ -434,22 +432,24 @@
             copt = options.CommonOptionHolderFactory()
             filterOption.ApplyFunction()(copt)
             filterOption = copt.filter
 
         if isinstance(filterOption, options.AndOption):
             return "( {} )".format(
                 " AND ".join(
-                    [self._convertFilter(f, sample) for f in filterOption.filters]
+                    [self._convertFilter(f, sample)
+                     for f in filterOption.filters]
                 )
             )
 
         if isinstance(filterOption, options.OrOption):
             return "( {} )".format(
                 " OR ".join(
-                    [self._convertFilter(f, sample) for f in filterOption.filters]
+                    [self._convertFilter(f, sample)
+                     for f in filterOption.filters]
                 )
             )
 
         if isinstance(filterOption, options.NotOption):
             return "( NOT {} )".format(
                 self._convertFilter(filterOption.filter, sample)
             )
@@ -461,15 +461,15 @@
             # return "'{}'".format(v)
             if isinstance(v, str):
                 return "'{}'".format(utils.encode_string(v))
             elif isinstance(v, bool):
                 return str(v).lower()
             else:
                 return str(v)
-        
+
         if isinstance(filterOption, options.InOption):
             values = ", ".join([convert_value(v) for v in filterOption.values])
 
             return " json_extract(Object, '$.{}') IN ({})".format(
                 filterOption.key, values
             )
```

### Comparing `pystorz-0.3.5/pystorz/store/options.py` & `pystorz-0.4.0/pystorz/store/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 import json
 import logging
 
 
 log = logging.getLogger(__name__)
 
 from pystorz.store import utils
+from typing import Callable
+
+
+class CommonOptionHolder:
+    def __init__(self):
+        self.filter = None
+        self.order_by = None
+        self.order_incremental = None
+        self.page_size = None
+        self.page_offset = None
+
+    def common_options(self):
+        return self
 
 
 class Option:
-    def ApplyFunction(self):
-        pass
+    def ApplyFunction(self) -> Callable[[CommonOptionHolder], None]:
+        raise NotImplementedError
+    
+    def ToJson(self) -> str:
+        raise NotImplementedError
+
+    def ToDict(self) -> dict:
+        raise NotImplementedError
 
 
 class CreateOption(Option):
     def get_create_option(self) -> Option:
         raise NotImplementedError
 
 
@@ -63,23 +82,25 @@
         elif data["type"] == "or":
             return Or(*[ListDeleteOption.FromJson(f) for f in data["filters"]])
         elif data["type"] == "not":
             return Not(ListDeleteOption.FromJson(data["filter"]))
         else:
             raise ValueError("Unknown type: {}".format(data["type"]))
 
-    def ToJson(self):
+    def ToJson(self) -> str:
         return json.dumps(self.ToDict())
 
-    def ToDict(self):
+    def ToDict(self) -> dict:
         copt = CommonOptionHolderFactory()
         self.ApplyFunction()(copt)
-        return copt.filter.ToDict()
+        if isinstance(copt.filter, Option):
+            return copt.filter.ToDict()
+        return {}
 
-    def __str__(self):
+    def __str__(self) -> str:
         copt = CommonOptionHolderFactory()
         self.ApplyFunction()(copt)
         return str(copt.filter)
     
 
 class OptionHolder:
     def common_options(self):
@@ -143,27 +164,27 @@
         return {"type": "gte", "key": self.key, "value": self.value}
 
     def __str__(self):
         return "{} >= {}".format(self.key, self.value)
 
 
 class AndOption(ListDeleteOption):
-    def __init__(self, *filters: list[ListDeleteOption]):
+    def __init__(self, *filters: ListDeleteOption):
         self.filters = filters
 
     def ToDict(self):
         return {"type": "and", "filters": [f.ToDict() for f in self.filters]}
 
     def __str__(self):
         return "( {} )".format(
             " AND ".join([str(f) for f in self.filters]))
 
 
 class OrOption(ListDeleteOption):
-    def __init__(self, *filters: list[ListDeleteOption]):
+    def __init__(self, *filters: ListDeleteOption):
         self.filters = filters
 
     def ToDict(self):
         return {"type": "or", "filters": [f.ToDict() for f in self.filters]}
 
     def __str__(self):
         return "( {} )".format(
@@ -190,26 +211,14 @@
         return {"type": "in", "key": self.key, "values": self.values}
 
     def __str__(self):
         return "({} IN ({}))".format(
             self.key, ", ".join([str(v) for v in self.values]))
 
 
-class CommonOptionHolder:
-    def __init__(self):
-        self.filter = None
-        self.order_by = None
-        self.order_incremental = None
-        self.page_size = None
-        self.page_offset = None
-
-    def common_options(self):
-        return self
-
-
 def CommonOptionHolderFactory() -> CommonOptionHolder:
     return CommonOptionHolder()
 
 
 class _ListDeleteOption(ListDeleteOption):
     def __init__(self, function):
         self.function = function
@@ -220,26 +229,26 @@
     def get_list_option(self):
         return self
 
     def ApplyFunction(self):
         return self.function
 
 
-def And(*filters: list[ListDeleteOption]) -> ListDeleteOption:
+def And(*filters: ListDeleteOption) -> ListDeleteOption:
     def option_function(options: OptionHolder):
         common_options = options.common_options()
         if common_options.filter is not None:
             raise Exception("prop filter option already set")
 
         common_options.filter = AndOption(*filters)
 
     return _ListDeleteOption(option_function)
 
 
-def Or(*filters: list[ListDeleteOption]) -> ListDeleteOption:
+def Or(*filters: ListDeleteOption) -> ListDeleteOption:
     def option_function(options: OptionHolder):
         common_options = options.common_options()
         if common_options.filter is not None:
             raise Exception("prop filter option already set")
 
         common_options.filter = OrOption(*filters)
```

### Comparing `pystorz-0.3.5/pystorz/store/utils.py` & `pystorz-0.4.0/pystorz/store/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,35 +21,28 @@
 # class _MetaHolder:
 #     def __init__(self):
 #         self.Metadata = None
 #         self.External = None
 #         self.Internal = None
 
 
-def clone_object(obj: store.Object, schema: store.SchemaHolder) -> store.Object:
-    ret = schema.ObjectForKind(obj.Metadata().Kind())
-    jsn = obj.ToJson()
-    ret.FromJson(jsn)
-    return ret
-
-
 def unmarshal_object(
-    body: str, schema: store.SchemaHolder, kind: str
+    body, schema: store.SchemaHolder, kind: str
 ) -> store.Object:
     resource = schema.ObjectForKind(kind)
     resource.FromJson(body)
     return resource
 
 
 def object_kind(data) -> str:
     if "metadata" not in data:
-        return None
+        return ""
     
     if "kind" not in data["metadata"]:
-        return None
+        return ""
     
     return data["metadata"]["kind"]
 
 
 def pps(string: str) -> str:
     return pp(json.loads(string))
 
@@ -60,19 +53,19 @@
 
 def timestamp() -> str:
     return time.strftime("%Y-%m-%dT%H:%M:%S.%fZ", time.gmtime())
 
 
 def serialize(mo: store.Object) -> str:
     if mo is None:
-        raise constants.ErrObjectNil
+        raise Exception(constants.ErrObjectNil)
     return json.dumps(mo, default=lambda x: x.to_dict())
 
 
-def object_path(obj: store.Object, path: str) -> str:
+def object_path(obj: store.Object, path: str) -> object:
     # print("object_path: {} {}".format(obj, path))
     data = obj.ToDict()
     # print(pp(data))
     ret = JSONPath("$.{}".format(path)).parse(data)
     if not ret or len(ret) == 0:
         # print("object_path: no result for {} in {}".format(path, data))
         return None
@@ -83,23 +76,22 @@
     pathlib.Path(target_dir).mkdir(parents=True, exist_ok=True)
     target_file = os.path.join(target_dir, name)
     with open(target_file, "w") as f:
         f.write(content)
 
 
 def runtime_dir() -> str:
-    rd = pathlib.Path(__file__).parent.parent.absolute()
-    return rd
+    return str(pathlib.Path(__file__).parent.parent.absolute())
 
 
 def datetime_current() -> str:
     return datetime_string(datetime.now())
 
 
-def datetime_parse(dtstr) -> str:
+def datetime_parse(dtstr) -> datetime:
     return datetime.strptime(dtstr, constants.DATETIME_FORMAT)
 
 
 def datetime_string(dt) -> str:
     return dt.strftime(constants.DATETIME_FORMAT)
```

### Comparing `pystorz-0.3.5/pystorz.egg-info/PKG-INFO` & `pystorz-0.4.0/pystorz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.5
+Version: 0.4.0
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-        </p>
-        
-        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-        
-        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-        
-        Original storz was written in go. You can check it out here:
-        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-        
-        This is a python port of the original storz.
-        Still in development.
-        
-        ## Quick Start Guide
-        
-        ### Installation
-        ```
-        pip install pystorz
-        ```
-        
-        ## Model example
-        
-        You can find a saomple model in the tests folder.
-        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-        
-        You can define simple structures and reference them as fields in other structures.
-        
-        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-        
-        Only a SQLite store is implemented at the moment.
-        
-        More to come.
-        Check out the go version (link above) for more information.
-        
-        ## Usage
-        ```
-            from pystorz.mgen import builder
-        
-            # run the code gen to 
-            builder.Generate("path/to/model.yml")
-            # this will make a generated folder in the project home directory
-        
-            # you can then import the generated model
-            from generated import model
-        
-            # initialize a store
-            stor = SqliteStore(
-                Schema(),
-                SqliteConnector("path/to/your/sqlite3.db"))
-        
-            world = model.WorldFactory()
-            world.External().SetName("hello")
-        
-            created_world = stor.Create(world)
-            world.External().SetDescription("hello world")
-            updated_world = stor.Update(world.Metadata().Identity(), world)
-            
-            # ...
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+</p>
+
+**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+
+**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+
+Original storz was written in go. You can check it out here:
+[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+
+This is a python port of the original storz.
+Still in development.
+
+## Quick Start Guide
+
+### Installation
+```
+pip install pystorz
+```
+
+## Model example
+
+You can find a saomple model in the tests folder.
+[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+
+You can define simple structures and reference them as fields in other structures.
+
+You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+
+Only a SQLite store is implemented at the moment.
+
+More to come.
+Check out the go version (link above) for more information.
+
+## Usage
+```
+    from pystorz.mgen import builder
+
+    # run the code gen to 
+    builder.Generate("path/to/model.yml")
+    # this will make a generated folder in the project home directory
+
+    # you can then import the generated model
+    from generated import model
+
+    # initialize a store
+    stor = SqliteStore(
+        Schema(),
+        SqliteConnector("path/to/your/sqlite3.db"))
+
+    world = model.WorldFactory()
+    world.External().SetName("hello")
+
+    created_world = stor.Create(world)
+    world.External().SetDescription("hello world")
+    updated_world = stor.Update(world.Metadata().Identity(), world)
+    
+    # ...
+
+```
```

### Comparing `pystorz-0.3.5/pystorz.egg-info/SOURCES.txt` & `pystorz-0.4.0/pystorz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 pystorz/meta/store.py
 pystorz/mgen/__init__.py
 pystorz/mgen/builder.py
 pystorz/mgen/loader.py
 pystorz/mgen/test.py
 pystorz/mgen/utils.py
 pystorz/mgen/templates/__init__.py
+pystorz/mgen/templates/clone.py
+pystorz/mgen/templates/cloneimp.py
 pystorz/mgen/templates/imports.py
 pystorz/mgen/templates/interface.py
 pystorz/mgen/templates/meta.py
 pystorz/mgen/templates/schema.py
-pystorz/mgen/templates/specinternal.py
 pystorz/mgen/templates/structure.py
 pystorz/mgen/templates/unmarshall.py
 pystorz/rest/__init__.py
 pystorz/rest/client.py
 pystorz/rest/headers.py
 pystorz/rest/internals.py
 pystorz/rest/server.py
@@ -33,11 +34,10 @@
 pystorz/router/store.py
 pystorz/sql/__init__.py
 pystorz/sql/adapter.py
 pystorz/sql/mysql.py
 pystorz/sql/sqlite.py
 pystorz/sql/store.py
 pystorz/store/__init__.py
-pystorz/store/meta.py
 pystorz/store/options.py
 pystorz/store/store.py
 pystorz/store/utils.py
```

### Comparing `pystorz-0.3.5/setup.py` & `pystorz-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.3.5',
+    version='0.4.0',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

