# Comparing `tmp/color_latam-0.0.1.tar.gz` & `tmp/color_latam-0.0.2.tar.gz`

## Comparing `color_latam-0.0.1.tar` & `color_latam-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 color_latam-0.0.1/src/color_es/__init__.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 color_latam-0.0.1/src/color_es/color.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 color_latam-0.0.1/LICENSE
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 color_latam-0.0.1/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 color_latam-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 color_latam-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 color_latam-0.0.2/src/color_latam/__init__.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 color_latam-0.0.2/src/color_latam/color_latam.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 color_latam-0.0.2/LICENSE
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 color_latam-0.0.2/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 color_latam-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 color_latam-0.0.2/PKG-INFO
```

### Comparing `color_latam-0.0.1/src/color_es/color.py` & `color_latam-0.0.2/src/color_latam/color_latam.py`

 * *Files identical despite different names*

### Comparing `color_latam-0.0.1/LICENSE` & `color_latam-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `color_latam-0.0.1/pyproject.toml` & `color_latam-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "color_latam"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Israel Ubeda", email="israel.ubedabravo@gmail.com" },
 ]
 description = "Libreria que cambia el color del texto en español"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `color_latam-0.0.1/PKG-INFO` & `color_latam-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_latam
-Version: 0.0.1
+Version: 0.0.2
 Summary: Libreria que cambia el color del texto en español
 Project-URL: Homepage, https://github.com/israelubeda/color_es
 Project-URL: Bug Tracker, https://github.com/israelubeda/color_es
 Author-email: Israel Ubeda <israel.ubedabravo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

