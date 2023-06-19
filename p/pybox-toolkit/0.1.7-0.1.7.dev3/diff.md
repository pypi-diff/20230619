# Comparing `tmp/pybox-toolkit-0.1.7.tar.gz` & `tmp/pybox-toolkit-0.1.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.7.tar", last modified: Mon Jun 19 09:29:47 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.7.dev3.tar", last modified: Thu Jun 15 14:02:40 2023, max compression
```

## Comparing `pybox-toolkit-0.1.7.tar` & `pybox-toolkit-0.1.7.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.864714 pybox-toolkit-0.1.7/
--rw-r--r--   0 root         (0) root         (0)      474 2023-06-19 09:29:47.864714 pybox-toolkit-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 09:29:47.864714 pybox-toolkit-0.1.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.856713 pybox-toolkit-0.1.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.860714 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      474 2023-06-19 09:29:47.000000 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-19 09:29:47.000000 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 09:29:47.000000 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-19 09:29:47.000000 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 09:29:47.000000 pybox-toolkit-0.1.7/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.860714 pybox-toolkit-0.1.7/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15087 2023-06-15 11:07:27.000000 pybox-toolkit-0.1.7/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.860714 pybox-toolkit-0.1.7/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.7/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.864714 pybox-toolkit-0.1.7/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:28:37.000000 pybox-toolkit-0.1.7/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 09:29:47.864714 pybox-toolkit-0.1.7/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:15:14.000000 pybox-toolkit-0.1.7/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-11 12:19:14.000000 pybox-toolkit-0.1.7/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:15:14.000000 pybox-toolkit-0.1.7/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-30 13:22:09.000000 pybox-toolkit-0.1.7.dev3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.7.dev3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.640549 pybox-toolkit-0.1.7.dev3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-15 14:02:40.000000 pybox-toolkit-0.1.7.dev3/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15087 2023-06-15 14:02:16.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-05-30 15:20:01.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 14:02:40.644549 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.7.dev3/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.7/pyproject.toml` & `pybox-toolkit-0.1.7.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.7/src/toolkit/utils.py` & `pybox-toolkit-0.1.7.dev3/src/toolkit/utils.py`

 * *Files identical despite different names*

