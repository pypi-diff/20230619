# Comparing `tmp/georef-ar-py-0.0.2.tar.gz` & `tmp/georef-ar-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georef-ar-py-0.0.2.tar", last modified: Sun Jun 18 22:53:36 2023, max compression
+gzip compressed data, was "georef-ar-py-0.0.3.tar", last modified: Mon Jun 19 19:54:40 2023, max compression
```

## Comparing `georef-ar-py-0.0.2.tar` & `georef-ar-py-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1065 2023-04-27 22:52:08.000000 georef-ar-py-0.0.2/LICENSE
--rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1942 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/README.md
--rw-r--r--   0 pablo     (1000) pablo     (1000)      852 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/pyproject.toml
--rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/setup.cfg
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/
--rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/__init__.py
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/georef_ar_py/
--rw-r--r--   0 pablo     (1000) pablo     (1000)      138 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/__init__.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)      339 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/__main__.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     3123 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/commands.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1113 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/constants.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     6941 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/diff.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     2245 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/georequests.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     5570 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/src/georef_ar_py/info.py
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.598030 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/PKG-INFO
--rw-r--r--   0 pablo     (1000) pablo     (1000)      553 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/SOURCES.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/dependency_links.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       54 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/entry_points.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       67 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/requires.txt
--rw-r--r--   0 pablo     (1000) pablo     (1000)       22 2023-06-18 22:53:36.000000 georef-ar-py-0.0.2/src/georef_ar_py.egg-info/top_level.txt
-drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:53:36.602030 georef-ar-py-0.0.2/tests/
--rw-r--r--   0 pablo     (1000) pablo     (1000)     4886 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_diff.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1536 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_georequests.py
--rw-r--r--   0 pablo     (1000) pablo     (1000)     1309 2023-06-18 22:48:04.000000 georef-ar-py-0.0.2/tests/test_info.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1065 2023-04-27 22:52:08.000000 georef-ar-py-0.0.3/LICENSE
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1942 2023-06-18 22:48:04.000000 georef-ar-py-0.0.3/README.md
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      852 2023-06-19 19:46:10.000000 georef-ar-py-0.0.3/pyproject.toml
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/setup.cfg
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-19 19:54:40.721904 georef-ar-py-0.0.3/src/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-06-18 22:48:04.000000 georef-ar-py-0.0.3/src/__init__.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/src/georef_ar_py/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      138 2023-06-18 22:48:04.000000 georef-ar-py-0.0.3/src/georef_ar_py/__init__.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      339 2023-06-18 22:48:04.000000 georef-ar-py-0.0.3/src/georef_ar_py/__main__.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     3421 2023-06-19 15:26:45.000000 georef-ar-py-0.0.3/src/georef_ar_py/commands.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1113 2023-06-18 22:48:04.000000 georef-ar-py-0.0.3/src/georef_ar_py/constants.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     6928 2023-06-19 16:18:55.000000 georef-ar-py-0.0.3/src/georef_ar_py/diff.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1221 2023-06-19 19:02:48.000000 georef-ar-py-0.0.3/src/georef_ar_py/georequests.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     5107 2023-06-19 17:47:02.000000 georef-ar-py-0.0.3/src/georef_ar_py/info.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      911 2023-06-19 19:08:50.000000 georef-ar-py-0.0.3/src/georef_ar_py/similar.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      746 2023-06-19 19:29:15.000000 georef-ar-py-0.0.3/src/georef_ar_py/territorial.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2533 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      661 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/SOURCES.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/dependency_links.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       54 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/entry_points.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       67 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/requires.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       22 2023-06-19 19:54:40.000000 georef-ar-py-0.0.3/src/georef_ar_py.egg-info/top_level.txt
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-06-19 19:54:40.725904 georef-ar-py-0.0.3/tests/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     5950 2023-06-19 18:20:03.000000 georef-ar-py-0.0.3/tests/test_diff.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      424 2023-06-19 19:11:34.000000 georef-ar-py-0.0.3/tests/test_georequests.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1295 2023-06-19 18:24:22.000000 georef-ar-py-0.0.3/tests/test_info.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1531 2023-06-19 19:15:42.000000 georef-ar-py-0.0.3/tests/test_similar.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1103 2023-06-19 19:29:06.000000 georef-ar-py-0.0.3/tests/test_territorial.py
```

### Comparing `georef-ar-py-0.0.2/LICENSE` & `georef-ar-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `georef-ar-py-0.0.2/PKG-INFO` & `georef-ar-py-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georef-ar-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar
 Author-email: "Pablo E. Andino" <pabloe.andino@gmail.com>
 Project-URL: Homepage, https://github.com/pavloae/georef-ar-py
 Project-URL: Bug Tracker, https://github.com/pavloae/georef-ar-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `georef-ar-py-0.0.2/README.md` & `georef-ar-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `georef-ar-py-0.0.2/pyproject.toml` & `georef-ar-py-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "georef-ar-py"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Pablo E. Andino", email="pabloe.andino@gmail.com" },
 ]
 description = "Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py/commands.py` & `georef-ar-py-0.0.3/src/georef_ar_py/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import os
 
 import click
 from requests import RequestException
 
+from . import georequests
 from .constants import ENTITIES
 from .diff import get_diff_object
 from .georequests import API_BASE_URL
 from .info import get_resume
 
 
 def get_logger(level):
@@ -21,15 +22,16 @@
 def cli():
     pass
 
 
 @cli.command()
 @click.argument('url', type=str)
 @click.option('--origin_url', required=False, type=str, show_default=True, default=API_BASE_URL)
-@click.option('--layer', required=False, type=click.Choice(ENTITIES, case_sensitive=True), show_default=True, default="all")
+@click.option('--token', required=False, type=str, show_default=True, default=None)
+@click.option('--layer', required=False, type=click.Choice(ENTITIES, case_sensitive=True), show_default=True, default=None)
 @click.option('--extension', required=False, type=click.Choice(['json', 'csv', 'both'], case_sensitive=True), show_default=True, default="both")
 @click.option('--debug', is_flag=True, show_default=False)
 def diff(*args, **kwargs):
     """
     geoarpy diff Commandline
 
     Calcula las diferencias de registros entre dos API's.
@@ -38,24 +40,25 @@
     url es el path a la API destino que se quiere comparar.
     """
     debug = kwargs.pop('debug')
     log = get_logger(logging.DEBUG if debug else logging.INFO)
     log.info("Comenzando la generación de diferencias...")
 
     src_url = kwargs.pop('origin_url')
-    target_url = kwargs.pop('t')
+    target_url = kwargs.pop('url')
     ext = kwargs.pop('extension')
     layer = kwargs.pop('layer')
+    georequests.__dict__['TOKEN'] = kwargs.pop('token')
 
     path_dir = os.getcwd()
 
     if ext and ext not in ['json', 'csv', 'both']:
         raise NotImplemented(f'La extensión {ext} no está implementada.')
 
-    entities = layer if layer != 'all' else ENTITIES
+    entities = layer if layer else ENTITIES
 
     if isinstance(entities, str):
         entities = [layer]
 
     for layer in entities:
         log.info(f'Procesando la capa "{layer}"')
 
@@ -70,27 +73,29 @@
                 diff_entity.diff_as_csv(os.path.join(path_dir, f'diff_{layer}.csv'))
         except RequestException as rqe:
             log.error(f'No se pudo procesar la petición {rqe.request}')
 
 
 @cli.command()
 @click.option('--url', required=False, type=str, show_default=True, default=API_BASE_URL)
+@click.option('--token', required=False, type=str, show_default=True, default=None)
 @click.option('--debug', is_flag=True, show_default=False)
 def info(*args, **kwargs):
     """
     geoarpy info Commandline
 
     Obtienen un resumen de los registros en la API especificada
 
     url es el path a la API destino que se quiere consultar.
     """
     debug = kwargs.pop('debug')
     log = get_logger(logging.DEBUG if debug else logging.INFO)
     log.info("Comenzando la generación del resumen...")
 
     target_url = kwargs.pop('url')
+    georequests.__dict__['TOKEN'] = kwargs.pop('token')
 
     resume = get_resume(target_url)
 
     filename = os.path.join(os.getcwd(), 'info.json')
     with open(filename, '+w') as f:
         json.dump(resume, f)
```

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py/constants.py` & `georef-ar-py-0.0.3/src/georef_ar_py/constants.py`

 * *Files identical despite different names*

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py/diff.py` & `georef-ar-py-0.0.3/src/georef_ar_py/diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,85 +11,94 @@
 
 log = logging.getLogger(__name__)
 
 
 class DiffEntity:
     def __init__(
             self, entity, src_url, target_url, entity_key=None, max_registries=None,
-            ignore_order=True, significant_digits=1, exclude_paths=None, exclude_regex_paths=None
+            ignore_order=True, significant_digits=1, exclude_paths=None, exclude_regex_paths=None, **kwargs
     ) -> None:
         super().__init__()
         self._entity = entity
         self._src_url = src_url
         self._target_url = target_url
         self._entity_key = entity_key or entity
         self._max_registries = max_registries
         self._ignore_order = ignore_order
         self._significant_digits = significant_digits
         self._exclude_paths = exclude_paths
         self._exclude_regex_paths = exclude_regex_paths
         self._src_registers = None
         self._target_registers = None
         self._diff_dict = None
+        self._limit = kwargs.get('limit', 5000)
+        self._max_src = None
+        self._max_target = None
 
-    def _get_max_entity_number(self):
-        return max(
-            get_entity_number(self._src_url, self._entity),
-            get_entity_number(self._target_url, self._entity)
-        )
+    def _get_response(self, url, **kwargs):
+        return get_json(url, self._entity, **kwargs)
 
     @property
-    def max_registries(self):
-        if not self._max_registries:
-            self._max_registries = self._get_max_entity_number()
-        return self._max_registries
+    def max_src(self):
+        if not self._max_src:
+            self._max_src = get_entity_number(self._src_url, self._entity)
+        return self._max_src
+
+    @property
+    def max_target(self):
+        if not self._max_target:
+            self._max_target = get_entity_number(self._target_url, self._entity)
+        return self._max_target
+
+    def _get_max_entity_number(self):
+        return max(self.max_src, self.max_target)
+
+    def _get_registers(self, url, **kwargs):
+        log.debug(f"Obteniendo registros de {url}")
+        return {entity['id']: entity for entity in self._get_response(url, **kwargs)[self._entity_key]}
 
     def _get_registers_by_region(self, url, **kwargs):
         log.debug(f"Obteniendo registros de {url}")
-        self._max_registries = 5000
-        sum_dict = {}
+        limit = kwargs.get('max', self._limit)
+
+        params = {'campos': 'completo', 'orden': 'id', 'max': limit}
+
+        item_dict = {}
         for state_id in constants.PROVINCES_DICT.keys():
-            max_streets_province = get_entity_number(url, self._entity, provincia=state_id)
-            if max_streets_province <= 5000:
-                part_dict = self._get_response(
-                    url, campos='completo', orden='id', max=self.max_registries,
-                    provincia=state_id, **kwargs
-                )
-                sum_dict.update({entity['id']: entity for entity in part_dict[self._entity_key]})
+            max_items_province = get_entity_number(url, self._entity, provincia=state_id)
+            if max_items_province <= limit:
+                log.info(f"Consultando {self._entity}:provincia[{state_id}]")
+                params.pop('departamento', None)
+                params.update({'provincia': state_id})
+                item_dict.update(self._get_registers(url, **params))
             else:
                 for dep_id in get_departments_ids(url, state_id):
-                    part_dict = self._get_response(
-                        url, campos='completo', orden='id', max=self.max_registries,
-                        departamento=dep_id, **kwargs
-                    )
-                    sum_dict.update({entity['id']: entity for entity in part_dict[self._entity_key]})
-
-        return sum_dict
+                    log.info(f"Consultando {self._entity}:departamento[{dep_id}]")
+                    params.pop('provincia', None)
+                    params.update({'departamento': dep_id})
+                    item_dict.update(self._get_registers(url, **params))
 
-    def _get_response(self, url, **kwargs):
-        return get_json(url, self._entity, **kwargs)
-
-    def _get_registers(self, url, **kwargs):
-        log.debug(f"Obteniendo registros de {url}")
-        return {entity['id']: entity for entity in self._get_response(url, **kwargs)[self._entity_key]}
+        return item_dict
 
     @property
     def src_registers(self):
         if not self._src_registers:
-            self._src_registers = self._get_registers(
-                self._src_url, campos="completo", orden="id", max=self.max_registries
-            )
+            if self.max_src < self._limit:
+                self._src_registers = self._get_registers(self._src_url, campos="completo", orden="id", max=self._limit)
+            else:
+                self._src_registers = self._get_registers_by_region(self._src_url)
         return self._src_registers
 
     @property
     def target_registers(self):
         if not self._target_registers:
-            self._target_registers = self._get_registers(
-                self._target_url, campos="completo", orden="id", max=self.max_registries
-            )
+            if self.max_target < self._limit:
+                self._target_registers = self._get_registers(self._target_url, campos="completo", orden="id", max=self._limit)
+            else:
+                self._target_registers = self._get_registers_by_region(self._target_url)
         return self._target_registers
 
     def _get_diff_as_dict(self):
         return DeepDiff(
             self.src_registers, self.target_registers,
             ignore_order=self._ignore_order, significant_digits=self._significant_digits,
             exclude_paths=self._exclude_paths, exclude_regex_paths=self._exclude_regex_paths
@@ -149,32 +158,16 @@
         diff_df = pd.DataFrame.from_dict(diff_dict, orient='index')
 
         diff_df.to_csv(filename, index_label='id')
 
         log.debug(f"Archivo generado: {filename}")
 
 
-class DiffSettlement(DiffEntity):
-
-    def _get_registers(self, url, **kwargs):
-        return self._get_registers_by_region(url, **kwargs)
-
-
-class DiffStreet(DiffEntity):
-
-    def _get_registers(self, url, **kwargs):
-        return self._get_registers_by_region(url, **kwargs)
-
-
 def get_diff_object(src_url, target_url, entity):
-    if entity in ['provincias', 'departamentos', 'municipios', 'localidades']:
+    if entity in ['provincias', 'departamentos', 'municipios', 'asentamientos', 'localidades', 'calles']:
         return DiffEntity(entity, src_url, target_url)
     elif entity == 'localidades-censales':
         return DiffEntity(
             entity, src_url, target_url, entity_key='localidades_censales',
-            exclude_regex_paths=r"root\['\d+']\['centroide'\]"
+            exclude_regex_paths=None  # r"root\['\d+']\['centroide'\]"
         )
-    elif entity == 'asentamientos':
-        return DiffSettlement(entity, src_url, target_url)
-    elif entity == 'calles':
-        return DiffStreet(entity, src_url, target_url)
     raise NotImplemented(f'La capa {entity} no se encuentra implementada')
```

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py/info.py` & `georef-ar-py-0.0.3/src/georef_ar_py/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,125 @@
 import logging
 from requests import RequestException
 
-from . import georequests, constants
+from .georequests import get_json
+from .constants import ENTITIES, PROVINCES_DICT
 
 log = logging.getLogger(__name__)
 
 
-def get_departments_ids(url, state=None):
-    kwargs = {'campos': 'basico', 'orden': 'id', 'max': 5000}
-    if state:
-        kwargs.update({'provincia': state})
-
-    response = {'reason': 'Unknown'}
-    try:
-        response = georequests.get_json(url, 'departamentos', **kwargs)
-        return [department['id'] for department in response['departamentos']]
-    except KeyError:
-        raise RequestException(response)
-
-
 def _get_response(url, entity, **kwargs):
-    return georequests.get_json(url, entity, **kwargs)
+    return get_json(url, entity, **kwargs)
 
 
 def get_entity_number(url, entity, **kwargs):
     log.debug(f"Consultando cantidad de registros en {entity}")
-    kwargs.pop('campos', None)
-    kwargs.pop('max', None)
-    if entity not in constants.ENTITIES:
+    if entity not in ENTITIES:
         raise NotImplemented(f"La entidad \"{entity}\" no se encuentra implementada.")
-    return _get_response(url, entity, campos='basico', max=1)['total']
+    kwargs.update({'campos': 'basico', 'max': 1})
+    return _get_response(url, entity, **kwargs)['total']
 
 
-def get_entities_number(url):
+def get_entities_number(url, **kwargs):
     entities = {}
-    for entity in constants.ENTITIES:
+    for entity in ENTITIES:
         try:
-            entities.update({entity: get_entity_number(url, entity)})
+            entities.update({entity: get_entity_number(url, entity, **kwargs)})
         except RequestException:
             entities.update({entity: None})
     return entities
 
 
-def _get_response_by_region(url, entity, entity_key=None, **kwargs):
-    if not entity_key:
-        entity_key = entity
-
-    max_registries = 5000
-    sum_dict = None
-    for state_id in constants.PROVINCES_DICT.keys():
-        max_streets_province = get_entity_number(url, entity, provincia=state_id)
-        if max_streets_province <= max_registries:
+def get_departments_ids(url, state=None):
+    params = {'campos': 'basico', 'orden': 'id', 'max': 5000}
+    if state:
+        params.update({'provincia': state})
+    response = _get_response(url, 'departamentos', **params)
+    return [department['id'] for department in response['departamentos']]
+
+
+def _get_items(url, entity, entity_key=None, **kwargs):
+    entity_key = entity_key or entity
+    params = {'campos': 'completo', 'orden': 'id', 'max': kwargs.get('max', 5000)}
+    response = _get_response(url, entity, **params)
+    return response[entity_key]
+
+
+def _get_items_by_region(url, entity, entity_key=None, **kwargs):
+
+    entity_key = entity_key or entity
+    limit = kwargs.get('max', 5000)
+
+    params = {'campos': 'completo', 'orden': 'id', 'max': limit}
+
+    item_list = []
+    for state_id in PROVINCES_DICT.keys():
+        max_items_province = get_entity_number(url, entity, provincia=state_id)
+        if max_items_province <= limit:
             log.info(f"Consultando {entity}:provincia[{state_id}]")
-            part_dict = georequests.get_json(
-                url, entity, campos='completo', orden='id', max=max_registries,
-                provincia=state_id, **kwargs
-            )
-            if not sum_dict:
-                sum_dict = part_dict
-            else:
-                sum_dict[entity_key].extend(part_dict[entity_key])
+            params.pop('departamento', None)
+            params.update({'provincia': state_id})
+            response = _get_response(url, entity, **params)
+            item_list.extend(response[entity_key])
         else:
             for dep_id in get_departments_ids(url, state_id):
                 log.info(f"Consultando {entity}:departamento[{dep_id}]")
-                part_dict = georequests.get_json(
-                    url, entity, campos='completo', orden='id', max=max_registries,
-                    departamento=dep_id, **kwargs
-                )
-                if not sum_dict:
-                    sum_dict = part_dict
-                else:
-                    sum_dict[entity_key].extend(part_dict[entity_key])
-
-    sum_dict['cantidad'] = len(sum_dict[entity_key])
+                params.pop('provincia', None)
+                params.update({'departamento': dep_id})
+                response = _get_response(url, entity, **params)
+                item_list.extend(response[entity_key])
 
-    return sum_dict
+    return item_list
 
 
-def get_resume(url):
+def get_resume(url, **kwargs):
 
     resume = {}
 
     log.info(f"Consultando provincias")
-    provinces = _get_response(url, 'provincias', campos='completo', max=24)
-    resume.setdefault('provincias', {}).update({'total': len(provinces.get('provincias', None))})
-    resume['provincias'].update(
-        {row['id']: {} for row in provinces['provincias']}
-    )
+    provinces_list = _get_items(url, 'provincias')
+    resume.setdefault('provincias', {}).update({'total': len(provinces_list)})
+    resume['provincias'].update({row['id']: {} for row in provinces_list})
 
     log.info(f"Consultando departamentos")
-    departments = _get_response(url, 'departamentos', campos='completo', max=600)
-    resume.setdefault('departamentos', {}).update({'total': len(departments.get('departamentos', None))})
-    for row in departments['departamentos']:
+    departments_list = _get_items(url, 'departamentos')
+    resume.setdefault('departamentos', {}).update({'total': len(departments_list)})
+    for row in departments_list:
         resume['provincias'][row['provincia']['id']].setdefault('departamentos', 0)
         resume['provincias'][row['provincia']['id']]['departamentos'] += 1
 
     log.info(f"Consultando municipios")
-    municipalities = _get_response(url, 'municipios', campos='completo', max=5000)
-    resume.setdefault('municipios', {}).update({'total': len(municipalities.get('municipios', None))})
-    for row in municipalities['municipios']:
+    municipalities_list = _get_items(url, 'municipios')
+    resume.setdefault('municipios', {}).update({'total': len(municipalities_list)})
+    for row in municipalities_list:
         resume['provincias'][row['provincia']['id']].setdefault('municipios', 0)
         resume['provincias'][row['provincia']['id']]['municipios'] += 1
 
     log.info(f"Consultando localidades-censales")
-    census_localities = _get_response(url, 'localidades-censales', campos='completo', max=5000)
-    resume.setdefault('localidades-censales', {}).update({'total': len(census_localities.get('localidades_censales', None))})
-    for row in census_localities['localidades_censales']:
+    census_localities_list = _get_items(url, 'localidades-censales', entity_key='localidades_censales')
+    resume.setdefault('localidades-censales', {}).update({'total': len(census_localities_list)})
+    for row in census_localities_list:
         resume['provincias'][row['provincia']['id']].setdefault('localidades-censales', 0)
         resume['provincias'][row['provincia']['id']]['localidades-censales'] += 1
 
     log.info(f"Consultando asentamientos")
-    settlements = _get_response_by_region(url, 'asentamientos')
-    resume.setdefault('asentamientos', {}).update({'total': len(settlements.get('asentamientos', None))})
-    for row in settlements['asentamientos']:
+    settlements_list = _get_items_by_region(url, 'asentamientos')
+    resume.setdefault('asentamientos', {}).update({'total': len(settlements_list)})
+    for row in settlements_list:
         resume['provincias'][row['provincia']['id']].setdefault('asentamientos', 0)
         resume['provincias'][row['provincia']['id']]['asentamientos'] += 1
 
     log.info(f"Consultando localidades")
-    localities = _get_response(url, 'localidades', campos='completo', max=5000)
-    resume.setdefault('localidades', {}).update({'total': len(localities.get('localidades', None))})
-    for row in localities['localidades']:
+    localities_list = _get_items(url, 'localidades')
+    resume.setdefault('localidades', {}).update({'total': len(localities_list)})
+    for row in localities_list:
         resume['provincias'][row['provincia']['id']].setdefault('localidades', 0)
         resume['provincias'][row['provincia']['id']]['localidades'] += 1
 
     log.info(f"Consultando calles")
-    streets = _get_response_by_region(url, 'calles')
-    resume.setdefault('calles', {}).update({'total': len(streets.get('calles', None))})
-    for row in streets['calles']:
+    streets_list = _get_items_by_region(url, 'calles')
+    resume.setdefault('calles', {}).update({'total': len(streets_list)})
+    for row in streets_list:
         resume['provincias'][row['provincia']['id']].setdefault('calles', 0)
         resume['provincias'][row['provincia']['id']]['calles'] += 1
 
     return resume
```

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py.egg-info/PKG-INFO` & `georef-ar-py-0.0.3/src/georef_ar_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georef-ar-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Paquete para consultas y procesamiento de respuestas sobre la API de georef-ar
 Author-email: "Pablo E. Andino" <pabloe.andino@gmail.com>
 Project-URL: Homepage, https://github.com/pavloae/georef-ar-py
 Project-URL: Bug Tracker, https://github.com/pavloae/georef-ar-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `georef-ar-py-0.0.2/src/georef_ar_py.egg-info/SOURCES.txt` & `georef-ar-py-0.0.3/src/georef_ar_py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 src/georef_ar_py/__init__.py
 src/georef_ar_py/__main__.py
 src/georef_ar_py/commands.py
 src/georef_ar_py/constants.py
 src/georef_ar_py/diff.py
 src/georef_ar_py/georequests.py
 src/georef_ar_py/info.py
+src/georef_ar_py/similar.py
+src/georef_ar_py/territorial.py
 src/georef_ar_py.egg-info/PKG-INFO
 src/georef_ar_py.egg-info/SOURCES.txt
 src/georef_ar_py.egg-info/dependency_links.txt
 src/georef_ar_py.egg-info/entry_points.txt
 src/georef_ar_py.egg-info/requires.txt
 src/georef_ar_py.egg-info/top_level.txt
 tests/test_diff.py
 tests/test_georequests.py
-tests/test_info.py
+tests/test_info.py
+tests/test_similar.py
+tests/test_territorial.py
```

### Comparing `georef-ar-py-0.0.2/tests/test_info.py` & `georef-ar-py-0.0.3/tests/test_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tests.test_diff
 from src.georef_ar_py import info
 from src.georef_ar_py.georequests import API_BASE_URL
 
 
 class Test(TestCase):
 
-    @mock.patch('src.georef_ar_py.georequests.get_json')
+    @mock.patch('src.georef_ar_py.info.get_json')
     def test_get_entity_number(self, get_response_mock):
 
         get_response_mock.side_effect = tests.test_diff.get_mocked_response
 
         self.assertEqual(24, info.get_entity_number(API_BASE_URL, 'provincias'))
 
         self.assertEqual(529, info.get_entity_number(API_BASE_URL, 'departamentos'))
@@ -22,15 +22,15 @@
 
         self.assertEqual(14673, info.get_entity_number(API_BASE_URL, 'asentamientos'))
 
         self.assertEqual(4037, info.get_entity_number(API_BASE_URL, 'localidades'))
 
         self.assertEqual(150054, info.get_entity_number(API_BASE_URL, 'calles'))
 
-    @mock.patch('src.georef_ar_py.georequests.get_json')
+    @mock.patch('src.georef_ar_py.info.get_json')
     def test_get_resume(self, get_response_mock):
 
         get_response_mock.side_effect = tests.test_diff.get_mocked_response
 
         resume = info.get_resume(API_BASE_URL)
 
         self.assertTrue(all([key in resume.keys() for key in ['provincias', 'departamentos', 'municipios']]))
```

