# Comparing `tmp/calculadora-fabeliz-1.2.3.tar.gz` & `tmp/calculadora-fabeliz-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-1.2.3.tar", last modified: Mon Jun 19 21:14:13 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-1.3.3.tar", last modified: Mon Jun 19 21:16:54 2023, max compression
```

## Comparing `calculadora-fabeliz-1.2.3.tar` & `calculadora-fabeliz-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:14:13.615978 calculadora-fabeliz-1.2.3/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     1579 2023-06-19 21:14:13.613011 calculadora-fabeliz-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1313 2023-06-19 20:50:10.000000 calculadora-fabeliz-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 21:14:13.604389 calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0     1579 2023-06-19 21:14:13.000000 calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-19 21:14:13.000000 calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:14:13.000000 calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 21:14:13.000000 calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 21:14:13.610153 calculadora-fabeliz-1.2.3/calculadorafabeliz/
--rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.2.3/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.2.3/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.2.3/calculadorafabeliz/mathOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 21:14:13.615978 calculadora-fabeliz-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      408 2023-06-19 21:13:52.000000 calculadora-fabeliz-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:16:54.796096 calculadora-fabeliz-1.3.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1573 2023-06-19 21:16:54.794340 calculadora-fabeliz-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-06-19 21:16:08.000000 calculadora-fabeliz-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 21:16:54.788279 calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0     1573 2023-06-19 21:16:54.000000 calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-19 21:16:54.000000 calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 21:16:54.000000 calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 21:16:54.000000 calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 21:16:54.791914 calculadora-fabeliz-1.3.3/calculadorafabeliz/
+-rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.3.3/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.3.3/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.3.3/calculadorafabeliz/mathOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 21:16:54.796096 calculadora-fabeliz-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      408 2023-06-19 21:16:46.000000 calculadora-fabeliz-1.3.3/setup.py
```

### Comparing `calculadora-fabeliz-1.2.3/LICENSE` & `calculadora-fabeliz-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.2.3/PKG-INFO` & `calculadora-fabeliz-1.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: calculadora-fabeliz
-Version: 1.2.3
+Version: 1.3.3
 Summary: Calculadora Matematica / Math Calculator
 Author: Fabeliz Irene Alvarez Salazar
 Author-email: irenex2018@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Calculadora-Fabeliz
 
 Esta es una calculadora que permite hacer operaciones matematicas. 
 
-Operaciones bÃ¡sicas: Suma, Resta, Multiplicacion, Division. 
+Operaciones basicas: Suma, Resta, Multiplicacion, Division. 
 Otras Operaciones: Valor Absoluto, RaÃ­z cuadrada, Seno, Coseno Tangente, Cotangente, Logaritmo, Radian.
 
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
-FIAS TecnologÃ­a
+FIAS Tecnologia
 
 ## Instalation/InstalaciÃ³n:
 
 ```bash
 pip install calculadora-fabeliz==1.0.4
 pipenv install calculadora-fabeliz==1.0.4
 ```
```

### Comparing `calculadora-fabeliz-1.2.3/README.md` & `calculadora-fabeliz-1.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Calculadora-Fabeliz
 
 Esta es una calculadora que permite hacer operaciones matematicas. 
 
-Operaciones básicas: Suma, Resta, Multiplicacion, Division. 
+Operaciones basicas: Suma, Resta, Multiplicacion, Division. 
 Otras Operaciones: Valor Absoluto, Raíz cuadrada, Seno, Coseno Tangente, Cotangente, Logaritmo, Radian.
 
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
-FIAS Tecnología
+FIAS Tecnologia
 
 ## Instalation/Instalación:
 
 ```bash
 pip install calculadora-fabeliz==1.0.4
 pipenv install calculadora-fabeliz==1.0.4
 ```
```

### Comparing `calculadora-fabeliz-1.2.3/calculadora_fabeliz.egg-info/PKG-INFO` & `calculadora-fabeliz-1.3.3/calculadora_fabeliz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: calculadora-fabeliz
-Version: 1.2.3
+Version: 1.3.3
 Summary: Calculadora Matematica / Math Calculator
 Author: Fabeliz Irene Alvarez Salazar
 Author-email: irenex2018@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Calculadora-Fabeliz
 
 Esta es una calculadora que permite hacer operaciones matematicas. 
 
-Operaciones bÃ¡sicas: Suma, Resta, Multiplicacion, Division. 
+Operaciones basicas: Suma, Resta, Multiplicacion, Division. 
 Otras Operaciones: Valor Absoluto, RaÃ­z cuadrada, Seno, Coseno Tangente, Cotangente, Logaritmo, Radian.
 
 ## Autor/Author:
 Fabeliz Irene Alvarez Salazar
-FIAS TecnologÃ­a
+FIAS Tecnologia
 
 ## Instalation/InstalaciÃ³n:
 
 ```bash
 pip install calculadora-fabeliz==1.0.4
 pipenv install calculadora-fabeliz==1.0.4
 ```
```

### Comparing `calculadora-fabeliz-1.2.3/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-1.3.3/calculadorafabeliz/basicOperations.py`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.2.3/calculadorafabeliz/mathOperations.py` & `calculadora-fabeliz-1.3.3/calculadorafabeliz/mathOperations.py`

 * *Files identical despite different names*

