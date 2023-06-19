# Comparing `tmp/m1nx4s_calculator-1.0.0.tar.gz` & `tmp/m1nx4s_calculator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m1nx4s_calculator-1.0.0.tar", last modified: Thu Jun 15 08:16:33 2023, max compression
+gzip compressed data, was "m1nx4s_calculator-1.1.0.tar", last modified: Mon Jun 19 11:01:25 2023, max compression
```

## Comparing `m1nx4s_calculator-1.0.0.tar` & `m1nx4s_calculator-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:16:33.634439 m1nx4s_calculator-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-14 08:21:18.000000 m1nx4s_calculator-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      339 2023-06-15 08:16:33.634439 m1nx4s_calculator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-06-13 08:15:34.000000 m1nx4s_calculator-1.0.0/README.md
--rw-rw-rw-   0        0        0      121 2023-06-15 08:16:33.640368 m1nx4s_calculator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-06-15 08:15:16.000000 m1nx4s_calculator-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:16:33.189232 m1nx4s_calculator-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 08:16:33.414155 m1nx4s_calculator-1.0.0/src/calculator/
--rw-rw-rw-   0        0        0       50 2023-06-15 08:01:16.000000 m1nx4s_calculator-1.0.0/src/calculator/__init__.py
--rw-rw-rw-   0        0        0     1161 2023-06-14 18:51:52.000000 m1nx4s_calculator-1.0.0/src/calculator/calculator.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:16:33.631933 m1nx4s_calculator-1.0.0/src/m1nx4s_calculator.egg-info/
--rw-rw-rw-   0        0        0      339 2023-06-15 08:16:32.000000 m1nx4s_calculator-1.0.0/src/m1nx4s_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-15 08:16:33.000000 m1nx4s_calculator-1.0.0/src/m1nx4s_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:16:32.000000 m1nx4s_calculator-1.0.0/src/m1nx4s_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 08:16:32.000000 m1nx4s_calculator-1.0.0/src/m1nx4s_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.984609 m1nx4s_calculator-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 08:21:18.000000 m1nx4s_calculator-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      339 2023-06-19 11:01:25.985608 m1nx4s_calculator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2025 2023-06-19 10:46:20.000000 m1nx4s_calculator-1.1.0/README.md
+-rw-rw-rw-   0        0        0      121 2023-06-19 11:01:25.991061 m1nx4s_calculator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-06-15 08:15:16.000000 m1nx4s_calculator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.881019 m1nx4s_calculator-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.941225 m1nx4s_calculator-1.1.0/src/calculator/
+-rw-rw-rw-   0        0        0       50 2023-06-19 11:00:50.000000 m1nx4s_calculator-1.1.0/src/calculator/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-06-19 07:09:46.000000 m1nx4s_calculator-1.1.0/src/calculator/calculator.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.972775 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/top_level.txt
```

### Comparing `m1nx4s_calculator-1.0.0/LICENSE` & `m1nx4s_calculator-1.1.0/LICENSE`

 * *Files identical despite different names*

