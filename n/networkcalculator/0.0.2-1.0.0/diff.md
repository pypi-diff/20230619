# Comparing `tmp/networkcalculator-0.0.2.tar.gz` & `tmp/networkcalculator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "networkcalculator-1.0.0.tar", last modified: Sun May 28 01:02:42 2023, max compression
```

## Comparing `networkcalculator-0.0.2.tar` & `networkcalculator-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/src/networkcalculator/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/src/networkcalculator/__init__.py
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/src/networkcalculator/bandwidth_calculator.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/src/networkcalculator/networkcalculator.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/tests/bandwidth_calculator_test.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/tests/networkcalculator_test.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/README.md
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 networkcalculator-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/
+-rw-rw-rw-   0        0        0      507 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7903 2023-05-28 00:44:56.000000 networkcalculator-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 01:02:42.455754 networkcalculator-1.0.0/networkcalculator.egg-info/
+-rw-rw-rw-   0        0        0      507 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-28 01:00:04.000000 networkcalculator-1.0.0/setup.py
```

