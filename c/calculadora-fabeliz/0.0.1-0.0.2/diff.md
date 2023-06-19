# Comparing `tmp/calculadora-fabeliz-0.0.1.tar.gz` & `tmp/calculadora-fabeliz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-0.0.1.tar", last modified: Mon Jun 19 15:59:21 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-0.0.2.tar", last modified: Mon Jun 19 16:17:24 2023, max compression
```

## Comparing `calculadora-fabeliz-0.0.1.tar` & `calculadora-fabeliz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 15:59:21.005233 calculadora-fabeliz-0.0.1/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      143 2023-06-19 15:59:21.005233 calculadora-fabeliz-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-06-19 15:56:41.000000 calculadora-fabeliz-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 15:59:20.631665 calculadora-fabeliz-0.0.1/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0      143 2023-06-19 15:59:20.000000 calculadora-fabeliz-0.0.1/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-19 15:59:20.000000 calculadora-fabeliz-0.0.1/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 15:59:20.000000 calculadora-fabeliz-0.0.1/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 15:59:20.000000 calculadora-fabeliz-0.0.1/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 15:59:20.634654 calculadora-fabeliz-0.0.1/calculadorafabeliz/
--rw-rw-rw-   0        0        0       78 2023-06-19 15:42:34.000000 calculadora-fabeliz-0.0.1/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0      715 2023-06-19 15:50:27.000000 calculadora-fabeliz-0.0.1/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 15:59:21.020855 calculadora-fabeliz-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-06-19 15:58:34.000000 calculadora-fabeliz-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:17:24.329093 calculadora-fabeliz-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-06-19 16:17:24.328097 calculadora-fabeliz-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-06-19 15:56:41.000000 calculadora-fabeliz-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 16:17:24.318122 calculadora-fabeliz-0.0.2/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-06-19 16:17:24.000000 calculadora-fabeliz-0.0.2/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-19 16:17:24.000000 calculadora-fabeliz-0.0.2/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:17:24.000000 calculadora-fabeliz-0.0.2/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 16:17:24.000000 calculadora-fabeliz-0.0.2/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:17:24.322113 calculadora-fabeliz-0.0.2/calculadorafabeliz/
+-rw-rw-rw-   0        0        0       78 2023-06-19 15:42:34.000000 calculadora-fabeliz-0.0.2/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-06-19 16:13:13.000000 calculadora-fabeliz-0.0.2/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:17:24.329093 calculadora-fabeliz-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-06-19 16:13:32.000000 calculadora-fabeliz-0.0.2/setup.py
```

### Comparing `calculadora-fabeliz-0.0.1/LICENSE` & `calculadora-fabeliz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-0.0.1/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-0.0.2/calculadorafabeliz/basicOperations.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,7 +25,30 @@
 
         Parametros: num1 Valor float o int
                     num2 Valor float o int
 
         Return: Valor de la sumatoria floar o int            
         """
         return num1 - num2
+
+    def multiplicacion(self, num1, num2):
+        """
+        Metodo para retornar la multiplicacion
+
+        Parametros: num1 Valor float o int
+                    num2 Valor float o int
+
+        Return: Valor de la sumatoria floar o int            
+        """
+        return num1 * num2
+
+    def division(self, num1, num2):
+        """
+        Metodo para retornar la multiplicacion
+
+        Parametros: num1 Valor float o int
+                    num2 Valor float o int
+
+        Return: Valor de la sumatoria floar o int            
+        """
+        return num1 / num2
+
```

