# Comparing `tmp/calculadora-fabeliz-1.4.3.tar.gz` & `tmp/calculadora-fabeliz-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-1.4.3.tar", last modified: Mon Jun 19 21:18:33 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-1.5.3.tar", last modified: Mon Jun 19 21:20:15 2023, max compression
```

## Comparing `calculadora-fabeliz-1.4.3.tar` & `calculadora-fabeliz-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:33.067668 calculadora-fabeliz-1.4.3/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     1570 2023-06-19 21:18:33.067142 calculadora-fabeliz-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-06-19 21:18:04.000000 calculadora-fabeliz-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:33.059262 calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0     1570 2023-06-19 21:18:32.000000 calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-19 21:18:33.000000 calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:18:32.000000 calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 21:18:32.000000 calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 21:18:33.065147 calculadora-fabeliz-1.4.3/calculadorafabeliz/
--rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.4.3/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.4.3/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.4.3/calculadorafabeliz/mathOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 21:18:33.067668 calculadora-fabeliz-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-06-19 21:18:29.000000 calculadora-fabeliz-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:20:15.458343 calculadora-fabeliz-1.5.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1570 2023-06-19 21:20:15.456554 calculadora-fabeliz-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1310 2023-06-19 21:19:48.000000 calculadora-fabeliz-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 21:20:15.432733 calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0     1570 2023-06-19 21:20:15.000000 calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-19 21:20:15.000000 calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 21:20:15.000000 calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 21:20:15.000000 calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 21:20:15.438628 calculadora-fabeliz-1.5.3/calculadorafabeliz/
+-rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.5.3/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.5.3/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.5.3/calculadorafabeliz/mathOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 21:20:15.458343 calculadora-fabeliz-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-06-19 21:20:10.000000 calculadora-fabeliz-1.5.3/setup.py
```

### Comparing `calculadora-fabeliz-1.4.3/LICENSE` & `calculadora-fabeliz-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.4.3/PKG-INFO` & `calculadora-fabeliz-1.5.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculadora-fabeliz
-Version: 1.4.3
+Version: 1.5.3
 Summary: Calculadora Matematica / Math Calculator
 Author: Fabeliz Irene Alvarez Salazar
 Author-email: irenex2018@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Calculadora-Fabeliz
@@ -17,16 +17,16 @@
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
 FIAS Tecnologia
 
 ## Instalation/Instalacion:
 
 ```bash
-pip install calculadora-fabeliz==1.0.4
-pipenv install calculadora-fabeliz==1.0.4
+pip install calculadora-fabeliz==1.5.3
+pipenv install calculadora-fabeliz==1.5.3
 ```
 
 ## Use/Uso:
 
 Para su uso se debe importar la libreria y crear un objeto como se muestra
 a continuacion:
```

### Comparing `calculadora-fabeliz-1.4.3/README.md` & `calculadora-fabeliz-1.5.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
 FIAS Tecnologia
 
 ## Instalation/Instalacion:
 
 ```bash
-pip install calculadora-fabeliz==1.0.4
-pipenv install calculadora-fabeliz==1.0.4
+pip install calculadora-fabeliz==1.5.3
+pipenv install calculadora-fabeliz==1.5.3
 ```
 
 ## Use/Uso:
 
 Para su uso se debe importar la libreria y crear un objeto como se muestra
 a continuacion:
```

### Comparing `calculadora-fabeliz-1.4.3/calculadora_fabeliz.egg-info/PKG-INFO` & `calculadora-fabeliz-1.5.3/calculadora_fabeliz.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calculadora-fabeliz
-Version: 1.4.3
+Version: 1.5.3
 Summary: Calculadora Matematica / Math Calculator
 Author: Fabeliz Irene Alvarez Salazar
 Author-email: irenex2018@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Calculadora-Fabeliz
@@ -17,16 +17,16 @@
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
 FIAS Tecnologia
 
 ## Instalation/Instalacion:
 
 ```bash
-pip install calculadora-fabeliz==1.0.4
-pipenv install calculadora-fabeliz==1.0.4
+pip install calculadora-fabeliz==1.5.3
+pipenv install calculadora-fabeliz==1.5.3
 ```
 
 ## Use/Uso:
 
 Para su uso se debe importar la libreria y crear un objeto como se muestra
 a continuacion:
```

### Comparing `calculadora-fabeliz-1.4.3/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-1.5.3/calculadorafabeliz/basicOperations.py`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.4.3/calculadorafabeliz/mathOperations.py` & `calculadora-fabeliz-1.5.3/calculadorafabeliz/mathOperations.py`

 * *Files identical despite different names*

