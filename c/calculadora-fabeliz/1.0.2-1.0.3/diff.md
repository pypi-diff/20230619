# Comparing `tmp/calculadora-fabeliz-1.0.2.tar.gz` & `tmp/calculadora-fabeliz-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-1.0.2.tar", last modified: Mon Jun 19 20:06:47 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-1.0.3.tar", last modified: Mon Jun 19 20:23:40 2023, max compression
```

## Comparing `calculadora-fabeliz-1.0.2.tar` & `calculadora-fabeliz-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:06:47.215230 calculadora-fabeliz-1.0.2/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      190 2023-06-19 20:06:47.214812 calculadora-fabeliz-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-19 19:07:30.000000 calculadora-fabeliz-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 20:06:47.203050 calculadora-fabeliz-1.0.2/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0      190 2023-06-19 20:06:47.000000 calculadora-fabeliz-1.0.2/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-19 20:06:47.000000 calculadora-fabeliz-1.0.2/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:06:47.000000 calculadora-fabeliz-1.0.2/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 20:06:47.000000 calculadora-fabeliz-1.0.2/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 20:06:47.211325 calculadora-fabeliz-1.0.2/calculadorafabeliz/
--rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.0.2/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.0.2/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.0.2/calculadorafabeliz/mathOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 20:06:47.216228 calculadora-fabeliz-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-06-19 20:04:47.000000 calculadora-fabeliz-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:23:40.271839 calculadora-fabeliz-1.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-06-19 20:23:40.271839 calculadora-fabeliz-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-19 20:22:36.000000 calculadora-fabeliz-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 20:23:40.266485 calculadora-fabeliz-1.0.3/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-06-19 20:23:40.000000 calculadora-fabeliz-1.0.3/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-19 20:23:40.000000 calculadora-fabeliz-1.0.3/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:23:40.000000 calculadora-fabeliz-1.0.3/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 20:23:40.000000 calculadora-fabeliz-1.0.3/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 20:23:40.269667 calculadora-fabeliz-1.0.3/calculadorafabeliz/
+-rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.0.3/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.0.3/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.0.3/calculadorafabeliz/mathOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:23:40.271839 calculadora-fabeliz-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-19 20:21:20.000000 calculadora-fabeliz-1.0.3/setup.py
```

### Comparing `calculadora-fabeliz-1.0.2/LICENSE` & `calculadora-fabeliz-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.0.2/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-1.0.3/calculadorafabeliz/basicOperations.py`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.0.2/calculadorafabeliz/mathOperations.py` & `calculadora-fabeliz-1.0.3/calculadorafabeliz/mathOperations.py`

 * *Files identical despite different names*

