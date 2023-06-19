# Comparing `tmp/calculadora-fabeliz-0.0.3.tar.gz` & `tmp/calculadora-fabeliz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-0.0.3.tar", last modified: Mon Jun 19 19:11:09 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-0.1.3.tar", last modified: Mon Jun 19 19:33:35 2023, max compression
```

## Comparing `calculadora-fabeliz-0.0.3.tar` & `calculadora-fabeliz-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:11:09.462027 calculadora-fabeliz-0.0.3/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      337 2023-06-19 19:11:09.462027 calculadora-fabeliz-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-19 19:07:30.000000 calculadora-fabeliz-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 19:11:09.453827 calculadora-fabeliz-0.0.3/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0      337 2023-06-19 19:11:09.000000 calculadora-fabeliz-0.0.3/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-19 19:11:09.000000 calculadora-fabeliz-0.0.3/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:11:09.000000 calculadora-fabeliz-0.0.3/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 19:11:09.000000 calculadora-fabeliz-0.0.3/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 19:11:09.458039 calculadora-fabeliz-0.0.3/calculadorafabeliz/
--rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-0.0.3/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-06-19 16:13:13.000000 calculadora-fabeliz-0.0.3/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0     1113 2023-06-19 17:55:09.000000 calculadora-fabeliz-0.0.3/calculadorafabeliz/mathOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 19:11:09.462027 calculadora-fabeliz-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-06-19 19:11:04.000000 calculadora-fabeliz-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:33:35.891537 calculadora-fabeliz-0.1.3/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      337 2023-06-19 19:33:35.891217 calculadora-fabeliz-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-19 19:07:30.000000 calculadora-fabeliz-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 19:33:35.883762 calculadora-fabeliz-0.1.3/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0      337 2023-06-19 19:33:35.000000 calculadora-fabeliz-0.1.3/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-19 19:33:35.000000 calculadora-fabeliz-0.1.3/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:33:35.000000 calculadora-fabeliz-0.1.3/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 19:33:35.000000 calculadora-fabeliz-0.1.3/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 19:33:35.888661 calculadora-fabeliz-0.1.3/calculadorafabeliz/
+-rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-0.1.3/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-0.1.3/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0     1113 2023-06-19 17:55:09.000000 calculadora-fabeliz-0.1.3/calculadorafabeliz/mathOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 19:33:35.891537 calculadora-fabeliz-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-06-19 19:32:18.000000 calculadora-fabeliz-0.1.3/setup.py
```

### Comparing `calculadora-fabeliz-0.0.3/LICENSE` & `calculadora-fabeliz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-0.0.3/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-0.1.3/calculadorafabeliz/basicOperations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Esta es un modulo que contiene las operaciones basicas de la calculadora
 """
 
 
 class calculadora:
     """
-    Clase Calculadora
+    Clase Calculadora self, num1, num2
     """
 
-    def suma(self, num1, num2):
+    def suma(self, *numbers):
         """
         Metodo para retornar al suma
 
         Parametros: num1 Valor float o int
                     num2 Valor float o int
 
         Return: Valor de la sumatoria floar o int            
         """
-        return num1 + num2
+        total = 0
+        
+        for number in numbers:
+            total += number
+
+        return total
 
     def resta(self, num1, num2):
         """
         Metodo para retornar la resta
 
         Parametros: num1 Valor float o int
                     num2 Valor float o int
@@ -47,8 +52,7 @@
 
         Parametros: num1 Valor float o int
                     num2 Valor float o int
 
         Return: Valor de la sumatoria floar o int            
         """
         return num1 / num2
-
```

### Comparing `calculadora-fabeliz-0.0.3/calculadorafabeliz/mathOperations.py` & `calculadora-fabeliz-0.1.3/calculadorafabeliz/mathOperations.py`

 * *Files identical despite different names*

