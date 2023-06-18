# Comparing `tmp/georef-ar-py-0.0.1.tar.gz` & `tmp/georef-ar-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georef-ar-py-0.0.1.tar", last modified: Fri Apr 28 16:06:27 2023, max compression
+gzip compressed data, was "georef-ar-py-0.0.2.tar", last modified: Sun Jun 18 22:53:36 2023, max compression
```

## Comparing `georef-ar-py-0.0.1.tar` & `georef-ar-py-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 16:06:27.587351 georef-ar-py-0.0.1/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1065 2023-04-27 22:52:08.000000 georef-ar-py-0.0.1/LICENSE
--rw-r--r--   0 pablo     (1000) pablo     (1000)      664 2023-04-28 16:06:27.587351 georef-ar-py-0.0.1/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)       94 2023-04-27 22:52:08.000000 georef-ar-py-0.0.1/README.md
--rw-r--r--   0 pablo     (1000) pablo     (1000)      684 2023-04-28 16:04:16.000000 georef-ar-py-0.0.1/pyproject.toml
--rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-04-28 16:06:27.587351 georef-ar-py-0.0.1/setup.cfg
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 16:06:27.583351 georef-ar-py-0.0.1/src/
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 16:06:27.583351 georef-ar-py-0.0.1/src/georef_ar_py/
--rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-04-27 23:28:38.000000 georef-ar-py-0.0.1/src/georef_ar_py/__init__.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1745 2023-04-28 00:25:06.000000 georef-ar-py-0.0.1/src/georef_ar_py/georequests.py
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 16:06:27.583351 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/
--rw-r--r--   0 pablo     (1000) pablo     (1000)      664 2023-04-28 16:06:27.000000 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)      318 2023-04-28 16:06:27.000000 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/SOURCES.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-04-28 16:06:27.000000 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/dependency_links.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       17 2023-04-28 16:06:27.000000 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/requires.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       13 2023-04-28 16:06:27.000000 georef-ar-py-0.0.1/src/georef_ar_py.egg-info/top_level.txt
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-04-28 16:06:27.587351 georef-ar-py-0.0.1/tests/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1202 2023-04-28 00:23:53.000000 georef-ar-py-0.0.1/tests/test_georequests.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1065 2023-04-27 22:52:08.000000 georef-ar-py-0.0.2/LICENSE
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1942 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/README.md
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      852 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/pyproject.toml
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/setup.cfg
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/__init__.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/georef_ar_py/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      138 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/__init__.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      339 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/__main__.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     3123 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/commands.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1113 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/constants.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     6941 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/diff.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2245 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/georequests.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     5570 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/info.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      553 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/SOURCES.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/dependency_links.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       54 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/entry_points.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       67 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/requires.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       22 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/top_level.txt
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/tests/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     4886 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_diff.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1536 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_georequests.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1309 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_info.py
```

### Comparing `georef-ar-py-0.0.1/LICENSE` & `georef-ar-py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `georef-ar-py-0.0.1/PKG-INFO` & `georef-ar-py-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,35 @@
-Metadata-Version: 2.1
-Name: georef-ar-py
-Version: 0.0.1
-Summary: Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar
-Author-email: "Pablo E. Andino" <pabloe.andino@gmail.com>
-Project-URL: Homepage, https://github.com/pavloae/georef-ar-py
-Project-URL: Bug Tracker, https://github.com/pavloae/georef-ar-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-# georef-ar-py
-Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar
+[project]
+name = "georef-ar-py"
+version = "0.0.2"
+authors = [
+  { name="Pablo E. Andino", email="pabloe.andino@gmail.com" },
+]
+description = "Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    'requests ~= 2.29.0',
+    'deepdiff ~= 6.3.0',
+    'pandas == 2.0.2'
+]
+
+[project.optional-dependencies]
+cli = [
+    'click==8.1.3'
+]
+
+[project.urls]
+"Homepage" = "https://github.com/pavloae/georef-ar-py"
+"Bug Tracker" = "https://github.com/pavloae/georef-ar-py/issues"
+
+[project.scripts]
+geoarpy = "georef_ar_py.commands:cli"
```

### Comparing `georef-ar-py-0.0.1/src/georef_ar_py/georequests.py` & `georef-ar-py-0.0.2/src/georef_ar_py/georequests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 import urllib
 
 import requests as requests
 
 API_BASE_URL = "https://apis.datos.gob.ar/georef/api/"
 
 
+def get_json(url, endpoint, **kwargs):
+    """
+        Obtiene una respuesta como json para la entidad consultada.
+    :param url: URL de la API a consultar.
+    :param endpoint: nombre de una de las capas.
+    :param kwargs: parámetros de consulta.
+    :return: Un diccionario con la respuesta obtenida
+    """
+    with requests.get("{}{}".format(url, endpoint), params=kwargs) as req:
+        if req.status_code == 200:
+            return req.json()
+        raise requests.RequestException(req)
+
+
 def get_similar(endpoint, nombre, **kwargs):
     kwargs["nombre"] = nombre
     url = "{}{}?{}".format(API_BASE_URL, endpoint, urllib.parse.urlencode(kwargs))
     return requests.get(url).json()[endpoint]
 
 
 def get_similar_bulk(endpoint, nombres):
```

### Comparing `georef-ar-py-0.0.1/tests/test_georequests.py` & `georef-ar-py-0.0.2/tests/test_georequests.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+import logging
 import unittest
+from unittest import TestCase
+
+import pytest as pytest
+from requests import RequestException
 
 from src.georef_ar_py import georequests
+from src.georef_ar_py.georequests import get_json
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 class MyTestCase(unittest.TestCase):
+
     def test_get_similar(self):
         response = georequests.get_similar('provincias', 'San Juan')
         self.assertEqual(response[0]['id'], '70')
         self.assertEqual(response[0]['nombre'], 'San Juan')
 
     def test_similar_bulk(self):
         response = georequests.get_similar_bulk("provincias", ["pxa", "sant fe"])
@@ -24,9 +34,11 @@
         self.assertEqual('Santa Fe', location1['provincia_nombre'])
         self.assertEqual('Rosario', location1['departamento_nombre'])
 
         self.assertEqual(location2['provincia_nombre'], 'Ciudad Autónoma de Buenos Aires')
         self.assertEqual(location2['departamento_nombre'], 'Comuna 1')
 
 
-if __name__ == '__main__':
-    unittest.main()
+class Test(TestCase):
+    def test_get_json(self):
+        with pytest.raises(RequestException):
+            get_json(georequests.API_BASE_URL, 'paises')
```

