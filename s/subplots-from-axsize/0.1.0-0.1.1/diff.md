# Comparing `tmp/subplots_from_axsize-0.1.0.tar.gz` & `tmp/subplots_from_axsize-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subplots_from_axsize-0.1.0.tar", max compression
+gzip compressed data, was "subplots_from_axsize-0.1.1.tar", max compression
```

## Comparing `subplots_from_axsize-0.1.0.tar` & `subplots_from_axsize-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-15 13:53:46.767142 subplots_from_axsize-0.1.0/README.md
--rw-r--r--   0        0        0      378 2023-06-17 17:10:18.089802 subplots_from_axsize-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.0/src/subplots_from_axsize/__init__.py
--rw-r--r--   0        0        0     2563 2023-06-15 14:16:56.937304 subplots_from_axsize-0.1.0/src/subplots_from_axsize/_subplots_from_axsize.py
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-06-15 13:41:52.549659 subplots_from_axsize-0.1.1/LICENSE
+-rw-r--r--   0        0        0       77 2023-06-17 17:56:09.932773 subplots_from_axsize-0.1.1/README.md
+-rw-r--r--   0        0        0      396 2023-06-19 09:07:28.921701 subplots_from_axsize-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-06-15 14:07:27.491712 subplots_from_axsize-0.1.1/src/subplots_from_axsize/__init__.py
+-rw-r--r--   0        0        0     2954 2023-06-17 17:53:53.828390 subplots_from_axsize-0.1.1/src/subplots_from_axsize/_subplots_from_axsize.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 subplots_from_axsize-0.1.1/PKG-INFO
```

### Comparing `subplots_from_axsize-0.1.0/LICENSE` & `subplots_from_axsize-0.1.1/LICENSE`

 * *Files identical despite different names*

