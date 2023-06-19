# Comparing `tmp/pypoolstation-0.5.2.tar.gz` & `tmp/pypoolstation-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypoolstation-0.5.2.tar", max compression
+gzip compressed data, was "pypoolstation-0.5.3.tar", max compression
```

## Comparing `pypoolstation-0.5.2.tar` & `pypoolstation-0.5.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 pypoolstation-0.5.2/LICENSE
--rw-r--r--   0        0        0     8693 2023-06-18 20:03:44.452041 pypoolstation-0.5.2/pypoolstation/__init__.py
--rw-r--r--   0        0        0      444 2023-06-18 20:04:10.359437 pypoolstation-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pypoolstation-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 pypoolstation-0.5.3/LICENSE
+-rw-r--r--   0        0        0     8702 2023-06-19 10:02:38.336386 pypoolstation-0.5.3/pypoolstation/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-19 10:03:14.288197 pypoolstation-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pypoolstation-0.5.3/PKG-INFO
```

### Comparing `pypoolstation-0.5.2/LICENSE` & `pypoolstation-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypoolstation-0.5.2/pypoolstation/__init__.py` & `pypoolstation-0.5.3/pypoolstation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         self.binary_input_1_name = None
         self.binary_input_2 = None
         self.binary_input_2_name = None
         self.binary_input_3 = None
         self.binary_input_3_name = None
         self.binary_input_4 = None
         self.binary_input_4_name = None
-        self.waterflow_sensor = None
+        self.waterflow_problem = None
         self.logger = logger
 
     async def post(self, url, data=""):
         try:
             resp = await self._session.post(
                 url,
                 data=f"Authorization=Bearer {self._token}" + data,
@@ -126,15 +126,15 @@
             self.salt_concentration = float(info["vars"][API_SIGNS["salt_concentration"]][0:-1])  # in gr/l
             self.current_ph = float(info["vars"][API_SIGNS["current_ph"]])
             self.target_ph = float(info["vars"][API_SIGNS["target_ph"]])
             self.binary_input_1 = info["vars"][API_SIGNS["binary_input_1"]] == "1"
             self.binary_input_2 = info["vars"][API_SIGNS["binary_input_2"]] == "1"
             self.binary_input_3 = info["vars"][API_SIGNS["binary_input_3"]] == "1"
             self.binary_input_4 = info["vars"][API_SIGNS["binary_input_4"]] == "1"
-            self.waterflow = info["vars"][API_SIGNS["waterflow"]] == "1"
+            self.waterflow_problem = info["vars"][API_SIGNS["waterflow"]] == "0"
             self.binary_input_1_name = info[API_SIGNS["binary_input_1_name"]]
             self.binary_input_2_name = info[API_SIGNS["binary_input_2_name"]]
             self.binary_input_3_name = info[API_SIGNS["binary_input_3_name"]]
             self.binary_input_4_name = info[API_SIGNS["binary_input_4_name"]]
         except ValueError:
             pass
         try:
```

### Comparing `pypoolstation-0.5.2/PKG-INFO` & `pypoolstation-0.5.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypoolstation
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python library to interact with the API of the Poolstation (https://poolstation.net) domotic platform for pool equipment
 License: MIT
 Author: cibernox
 Author-email: miguel.camba@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

