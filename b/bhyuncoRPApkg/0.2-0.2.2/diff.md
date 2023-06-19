# Comparing `tmp/bhyuncoRPApkg-0.2.tar.gz` & `tmp/bhyuncoRPApkg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhyuncoRPApkg-0.2.tar", last modified: Mon Jun 19 07:16:49 2023, max compression
+gzip compressed data, was "bhyuncoRPApkg-0.2.2.tar", last modified: Mon Jun 19 07:20:37 2023, max compression
```

## Comparing `bhyuncoRPApkg-0.2.tar` & `bhyuncoRPApkg-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:16:49.162842 bhyuncoRPApkg-0.2/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-19 07:16:49.162842 bhyuncoRPApkg-0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:16:49.162842 bhyuncoRPApkg-0.2/bhyuncoRPApkg.egg-info/
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-19 07:16:48.000000 bhyuncoRPApkg-0.2/bhyuncoRPApkg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-19 07:16:48.000000 bhyuncoRPApkg-0.2/bhyuncoRPApkg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:16:48.000000 bhyuncoRPApkg-0.2/bhyuncoRPApkg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:16:48.000000 bhyuncoRPApkg-0.2/bhyuncoRPApkg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 07:16:49.162842 bhyuncoRPApkg-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-19 07:08:38.000000 bhyuncoRPApkg-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:20:37.864874 bhyuncoRPApkg-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-19 07:20:37.864874 bhyuncoRPApkg-0.2.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 07:20:37.863874 bhyuncoRPApkg-0.2.2/bhyuncoRPApkg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-19 07:20:37.000000 bhyuncoRPApkg-0.2.2/bhyuncoRPApkg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-19 07:20:37.000000 bhyuncoRPApkg-0.2.2/bhyuncoRPApkg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:20:37.000000 bhyuncoRPApkg-0.2.2/bhyuncoRPApkg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 07:20:37.000000 bhyuncoRPApkg-0.2.2/bhyuncoRPApkg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 07:20:37.864874 bhyuncoRPApkg-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-19 07:08:38.000000 bhyuncoRPApkg-0.2.2/setup.py
```

