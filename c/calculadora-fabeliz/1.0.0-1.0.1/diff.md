# Comparing `tmp/calculadora-fabeliz-1.0.0.tar.gz` & `tmp/calculadora-fabeliz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculadora-fabeliz-1.0.0.tar", last modified: Mon Jun 19 19:45:27 2023, max compression
+gzip compressed data, was "calculadora-fabeliz-1.0.1.tar", last modified: Mon Jun 19 19:57:02 2023, max compression
```

## Comparing `calculadora-fabeliz-1.0.0.tar` & `calculadora-fabeliz-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 19:45:27.527567 calculadora-fabeliz-1.0.0/
--rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      337 2023-06-19 19:45:27.526551 calculadora-fabeliz-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-19 19:07:30.000000 calculadora-fabeliz-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 19:45:27.518341 calculadora-fabeliz-1.0.0/calculadora_fabeliz.egg-info/
--rw-rw-rw-   0        0        0      337 2023-06-19 19:45:27.000000 calculadora-fabeliz-1.0.0/calculadora_fabeliz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-06-19 19:45:27.000000 calculadora-fabeliz-1.0.0/calculadora_fabeliz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 19:45:27.000000 calculadora-fabeliz-1.0.0/calculadora_fabeliz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 19:45:27.000000 calculadora-fabeliz-1.0.0/calculadora_fabeliz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 19:45:27.524440 calculadora-fabeliz-1.0.0/calculadorafabeliz/
--rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.0.0/calculadorafabeliz/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.0.0/calculadorafabeliz/basicOperations.py
--rw-rw-rw-   0        0        0     1263 2023-06-19 19:42:22.000000 calculadora-fabeliz-1.0.0/calculadorafabeliz/mathOperations.py
--rw-rw-rw-   0        0        0       42 2023-06-19 19:45:27.527567 calculadora-fabeliz-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-06-19 19:45:22.000000 calculadora-fabeliz-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 19:57:02.734874 calculadora-fabeliz-1.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-19 15:54:55.000000 calculadora-fabeliz-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      337 2023-06-19 19:57:02.734874 calculadora-fabeliz-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-19 19:07:30.000000 calculadora-fabeliz-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 19:57:02.728309 calculadora-fabeliz-1.0.1/calculadora_fabeliz.egg-info/
+-rw-rw-rw-   0        0        0      337 2023-06-19 19:57:02.000000 calculadora-fabeliz-1.0.1/calculadora_fabeliz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-06-19 19:57:02.000000 calculadora-fabeliz-1.0.1/calculadora_fabeliz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 19:57:02.000000 calculadora-fabeliz-1.0.1/calculadora_fabeliz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-19 19:57:02.000000 calculadora-fabeliz-1.0.1/calculadora_fabeliz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 19:57:02.732114 calculadora-fabeliz-1.0.1/calculadorafabeliz/
+-rw-rw-rw-   0        0        0      227 2023-06-19 18:17:32.000000 calculadora-fabeliz-1.0.1/calculadorafabeliz/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-06-19 19:30:53.000000 calculadora-fabeliz-1.0.1/calculadorafabeliz/basicOperations.py
+-rw-rw-rw-   0        0        0     1401 2023-06-19 19:53:38.000000 calculadora-fabeliz-1.0.1/calculadorafabeliz/mathOperations.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 19:57:02.735872 calculadora-fabeliz-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-06-19 19:52:18.000000 calculadora-fabeliz-1.0.1/setup.py
```

### Comparing `calculadora-fabeliz-1.0.0/LICENSE` & `calculadora-fabeliz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.0.0/calculadorafabeliz/basicOperations.py` & `calculadora-fabeliz-1.0.1/calculadorafabeliz/basicOperations.py`

 * *Files identical despite different names*

### Comparing `calculadora-fabeliz-1.0.0/calculadorafabeliz/mathOperations.py` & `calculadora-fabeliz-1.0.1/calculadorafabeliz/mathOperations.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,7 +52,13 @@
         return 1/math.tan(num1)
 
     def hipotenusa(self, num1, num2):
         """
         Metodo para calcular la hipotenusa
         """
         return math.hypot(num1, num2)
+    
+    def radian(self, num1):
+        """
+        Metodo para calcular el radiante
+        """
+        return math.radians(num1)
```

