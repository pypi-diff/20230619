# Comparing `tmp/alpha_dom-0.1.0.tar.gz` & `tmp/alpha_dom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_dom-0.1.0.tar", max compression
+gzip compressed data, was "alpha_dom-0.1.1.tar", max compression
```

## Comparing `alpha_dom-0.1.0.tar` & `alpha_dom-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-06-18 05:35:59.810759 alpha_dom-0.1.0/LICENSE
--rw-r--r--   0        0        0       20 2023-06-18 05:35:59.810759 alpha_dom-0.1.0/README.md
--rw-r--r--   0        0        0      572 2023-06-18 05:35:59.810759 alpha_dom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-18 05:35:59.810759 alpha_dom-0.1.0/python/alpha_dom/__init__.py
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 alpha_dom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/LICENSE
+-rw-r--r--   0        0        0       72 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/README.md
+-rw-r--r--   0        0        0      640 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/python/alpha_dom/__init__.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 alpha_dom-0.1.1/PKG-INFO
```

