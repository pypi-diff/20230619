# Comparing `tmp/bc-acc-dup-1.1.tar.gz` & `tmp/bc-acc-dup-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc-acc-dup-1.1.tar", last modified: Mon Jun 19 02:48:51 2023, max compression
+gzip compressed data, was "bc-acc-dup-1.2.tar", last modified: Mon Jun 19 02:52:07 2023, max compression
```

## Comparing `bc-acc-dup-1.1.tar` & `bc-acc-dup-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 02:48:51.964693 bc-acc-dup-1.1/
--rw-rw-rw-   0        0        0      189 2023-06-19 02:48:51.958575 bc-acc-dup-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 02:48:51.965693 bc-acc-dup-1.1/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-06-19 02:48:40.000000 bc-acc-dup-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 02:48:51.905452 bc-acc-dup-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 02:48:51.952115 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/
--rw-rw-rw-   0        0        0      189 2023-06-19 02:48:51.000000 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-06-19 02:48:51.000000 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:48:51.000000 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-19 02:48:51.000000 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:48:51.000000 bc-acc-dup-1.1/src/bc_acc_dup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 02:52:07.811128 bc-acc-dup-1.2/
+-rw-rw-rw-   0        0        0      189 2023-06-19 02:52:07.807918 bc-acc-dup-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:52:07.811568 bc-acc-dup-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      633 2023-06-19 02:51:48.000000 bc-acc-dup-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:52:07.762636 bc-acc-dup-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 02:52:07.801679 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/
+-rw-rw-rw-   0        0        0      189 2023-06-19 02:52:07.000000 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-19 02:52:07.000000 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:52:07.000000 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-19 02:52:07.000000 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:52:07.000000 bc-acc-dup-1.2/src/bc_acc_dup.egg-info/top_level.txt
```

