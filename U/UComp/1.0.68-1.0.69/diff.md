# Comparing `tmp/UComp-1.0.68.tar.gz` & `tmp/UComp-1.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.68.tar", last modified: Fri Jun 16 11:37:51 2023, max compression
+gzip compressed data, was "UComp-1.0.69.tar", last modified: Mon Jun 19 10:18:58 2023, max compression
```

## Comparing `UComp-1.0.68.tar` & `UComp-1.0.69.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.142896 UComp-1.0.68/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.68/MANIFEST.in
--rw-rw-rw-   0        0        0      343 2023-06-16 11:37:51.142896 UComp-1.0.68/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.68/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.114137 UComp-1.0.68/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.68/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.68/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11378 2023-06-16 11:36:35.000000 UComp-1.0.68/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11787 2023-06-16 11:36:22.000000 UComp-1.0.68/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.68/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.68/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24515 2023-06-16 11:36:30.000000 UComp-1.0.68/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.68/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.68/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.68/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29804 2023-06-16 11:36:12.000000 UComp-1.0.68/UComp/tools.py
--rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.68/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:37:51.140859 UComp-1.0.68/UComp.egg-info/
--rw-rw-rw-   0        0        0      343 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 11:37:50.000000 UComp-1.0.68/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:37:51.145853 UComp-1.0.68/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-16 11:37:45.000000 UComp-1.0.68/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:18:58.163562 UComp-1.0.69/
+-rw-rw-rw-   0        0        0      403 2023-06-19 10:16:42.000000 UComp-1.0.69/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-19 10:18:58.163562 UComp-1.0.69/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.69/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 10:18:58.125618 UComp-1.0.69/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.69/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.69/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11378 2023-06-16 11:36:35.000000 UComp-1.0.69/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0     3378 2023-06-19 10:14:45.000000 UComp-1.0.69/UComp/Nile.bin
+-rw-rw-rw-   0        0        0    11787 2023-06-16 11:36:22.000000 UComp-1.0.69/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.69/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   897024 2023-06-16 11:32:46.000000 UComp-1.0.69/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-16 11:36:30.000000 UComp-1.0.69/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.69/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.69/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.69/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.69/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.69/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29839 2023-06-19 10:17:26.000000 UComp-1.0.69/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.69/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:18:58.160569 UComp-1.0.69/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-19 10:18:57.000000 UComp-1.0.69/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-19 10:18:57.000000 UComp-1.0.69/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:18:57.000000 UComp-1.0.69/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-19 10:18:57.000000 UComp-1.0.69/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 10:18:57.000000 UComp-1.0.69/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:18:58.166665 UComp-1.0.69/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-19 10:16:15.000000 UComp-1.0.69/setup.py
```

### Comparing `UComp-1.0.68/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.69/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/ETSmodule.py` & `UComp-1.0.69/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/PTSmodule.py` & `UComp-1.0.69/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.69/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/UCmodule.py` & `UComp-1.0.69/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/airpas.bin` & `UComp-1.0.69/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/gdp.bin` & `UComp-1.0.69/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/ipi.bin` & `UComp-1.0.69/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/libopenblas.dll` & `UComp-1.0.69/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/UComp/tools.py` & `UComp-1.0.69/UComp/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     import ETSmodule as ets
     import PTSmodule as pts
 
 
 ipi = pd.read_pickle("ipi.bin")
 gdp = pd.read_pickle("gdp.bin")
 airpas = pd.read_pickle("airpas.bin")
+Nile = pd.read_pickle("Nile.bin")
 
 
 def window(y, start='', end=''):
     if start == '':
         start = y.index[0]
     if end == '':
         end = y.index[-1]
```

### Comparing `UComp-1.0.68/UComp/tsfile.py` & `UComp-1.0.69/UComp/tsfile.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.68/setup.py` & `UComp-1.0.69/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.68',
+    version='1.0.69',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

