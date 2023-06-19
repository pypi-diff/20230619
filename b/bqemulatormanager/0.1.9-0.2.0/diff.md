# Comparing `tmp/bqemulatormanager-0.1.9.tar.gz` & `tmp/bqemulatormanager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqemulatormanager-0.1.9.tar", max compression
+gzip compressed data, was "bqemulatormanager-0.2.0.tar", max compression
```

## Comparing `bqemulatormanager-0.1.9.tar` & `bqemulatormanager-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1321 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/README.md
--rw-r--r--   0        0        0      145 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/__init__.py
--rw-r--r--   0        0        0      915 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/emulator.py
--rw-r--r--   0        0        0     3000 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/manager.py
--rw-r--r--   0        0        0     1883 2023-06-01 08:46:54.679991 bqemulatormanager-0.1.9/bqemulatormanager/schema.py
--rw-r--r--   0        0        0     1176 2023-06-01 08:47:11.107981 bqemulatormanager-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 bqemulatormanager-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1321 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/README.md
+-rw-r--r--   0        0        0      145 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/emulator.py
+-rw-r--r--   0        0        0     3484 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/manager.py
+-rw-r--r--   0        0        0     2878 2023-06-19 07:58:17.008013 bqemulatormanager-0.2.0/bqemulatormanager/schema.py
+-rw-r--r--   0        0        0     1178 2023-06-19 07:58:37.576342 bqemulatormanager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 bqemulatormanager-0.2.0/PKG-INFO
```

### Comparing `bqemulatormanager-0.1.9/README.md` & `bqemulatormanager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bqemulatormanager-0.1.9/bqemulatormanager/emulator.py` & `bqemulatormanager-0.2.0/bqemulatormanager/emulator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 import subprocess
+import time
 
 
 class PortOccupiedError(Exception):
     pass
 
 
-class Emulator:
-    running_flg = False
+class EmulatorError(Exception):
+    pass
 
-    def __init__(self, project_name: str, port: int, launch_emulator: bool = True, debug_mode: bool = False):
+
+class Emulator:
+    def __init__(self, project_name: str, port: int, grpc_port: int, launch_emulator: bool = True, debug_mode: bool = False):
         self.project_name = project_name
 
         if launch_emulator:
             log_level = "debug" if debug_mode else "info"
 
             if is_port_in_use(port):
                 raise PortOccupiedError(f"port {port} is occupied.")
-            self.running_flg = True
-            self.proc = subprocess.Popen(["bigquery-emulator", "--project", f"{project_name}", "--port", f"{port}", "--log-level", f"{log_level}"], shell=True)
+            if is_port_in_use(grpc_port):
+                raise PortOccupiedError(f"port {grpc_port} is occupied.")
+            self.proc = subprocess.Popen(
+                ["bigquery-emulator", "--project", project_name, "--port", f"{port}", "--grpc-port", f"{grpc_port}", "--log-level", log_level],
+            )
+            self._wait_for_emulator(port, timeout=10)
 
     def __del__(self):
-        if self.running_flg:
+        if self.proc is None:
+            return
+
+        if self.proc.poll() is None:
             self.proc.terminate()
+            self.proc.wait()
+
+    def _wait_for_emulator(self, port: int, timeout: int):
+        for _ in range(timeout):
+            if is_port_in_use(port):
+                return
+            time.sleep(1)
+        raise EmulatorError("emulator did not start.")
 
 
 def is_port_in_use(port: int) -> bool:
     import socket
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         return s.connect_ex(("localhost", port)) == 0
```

### Comparing `bqemulatormanager-0.1.9/bqemulatormanager/manager.py` & `bqemulatormanager-0.2.0/bqemulatormanager/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-from typing import Dict, List
+from typing import Dict, List, Union
 
 import pandas as pd
 from google.api_core.client_options import ClientOptions
 from google.auth.credentials import AnonymousCredentials
 from google.cloud import bigquery
 
 from bqemulatormanager.emulator import Emulator, PortOccupiedError
 from bqemulatormanager.schema import SchemaManager
 
 
+class ManagerError(Exception):
+    pass
+
+
 class Manager:
     def __init__(
         self,
         project: str = "test",
         port: int = 9050,
+        grpc_port: int = 9060,
         schema_path: str = "master_schema.yaml",
         launch_emulator: bool = True,
         debug_mode: bool = False,
         max_pool: int = 20,
     ):
         original_port = port
+        grpc_original_port = grpc_port
         for i in range(max_pool):
             port = original_port + i
+            grpc_port = grpc_original_port + i
             try:
-                self.emulator = Emulator(project, port, launch_emulator=launch_emulator, debug_mode=debug_mode)
+                self.emulator = Emulator(project, port, grpc_port, launch_emulator=launch_emulator, debug_mode=debug_mode)
             except PortOccupiedError as e:
                 print(e)
             else:
                 break
         else:
             raise RuntimeError(f"there is no empty port from {original_port} to {port}")
 
         self.client = self._make_client(project, port)
 
-        prod_client = bigquery.Client(project)
+        prod_client = bigquery.Client(project, credentials=AnonymousCredentials())
 
-        self.schema_manager = SchemaManager(client=prod_client, master_path=schema_path)
+        self.schema_manager = SchemaManager(client=prod_client, schema_file_path=schema_path)
         self.structure: Dict[str, Dict[str, bool]] = {}
         self.project_name = project
 
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -52,33 +59,35 @@
         client = bigquery.Client(
             project_name,
             client_options=client_options,
             credentials=AnonymousCredentials(),
         )
         return client
 
-    def load(self, data, path):
-        dataset, table = path.split(".")
+    def load(self, data: pd.DataFrame, path: str):
+        dataset, table_id = path.split(".")
         if dataset not in self.structure:
             self.create_dataset(dataset)
 
-        if table not in self.structure[dataset]:
-            self.create_table(dataset, table, [])
+        if table_id not in self.structure[dataset]:
+            self.create_table(dataset, table_id, [])
 
         table = self.client.get_table(f"{self.project_name}.{path}")
         self.client.insert_rows_from_dataframe(table, data)
 
-    def create_dataset(self, dataset_name: str, exists_ok=True):
+    def create_dataset(self, dataset_name: str, exists_ok=True, timeout: Union[float, None] = None):
         dataset = bigquery.Dataset(f"{self.project_name}.{dataset_name}")
-        self.client.create_dataset(dataset, exists_ok=exists_ok)
+        self.client.create_dataset(dataset, exists_ok=exists_ok, timeout=timeout)
         self.structure[dataset_name] = {}
 
-    def create_table(self, dataset_name: str, table_name: str, schema: List[bigquery.SchemaField]):
+    def create_table(self, dataset_name: str, table_name: str, schema: List[bigquery.SchemaField], timeout: Union[float, None] = None):
         if schema == []:
-            schema = self.schema_manager.get_schema(f"{self.project_name}.{dataset_name}.{table_name}")
+            schema = self.schema_manager.get_schema(self.project_name, dataset_name, table_name)
+            if schema is None:
+                raise ManagerError(f"schema for {dataset_name}.{table_name} is not found in master schema")
 
         table = bigquery.Table(f"{self.project_name}.{dataset_name}.{table_name}", schema=schema)
-        self.client.create_table(table)
+        self.client.create_table(table, timeout=timeout)
         self.structure[dataset_name][table_name] = True
 
     def query(self, sql: str) -> pd.DataFrame:
         return self.client.query(sql).to_dataframe(create_bqstorage_client=False)
```

### Comparing `bqemulatormanager-0.1.9/pyproject.toml` & `bqemulatormanager-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "bqemulatormanager"
-version = "0.1.9"  # using poetry-dynamic-versioning
+version = "0.2.0"  # using poetry-dynamic-versioning
 description = "bqemulatormanager is a wrapper of bigquery-emulator which provides us BigQuery mock working in local machine."
 authors = ["gyuta <kuroshiba0408@gmail.com>", "M3, Inc."]
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pyyaml = "*"
-google-cloud-bigquery = "^3.0.0"
+google-cloud-bigquery = ">=2.34.4"
 db-dtypes = "^1.0.0"
 psutil = "^5.0.0"
 google-auth = "^2.17.2"
 
 [tool.poetry.group.dev.dependencies]
 pyproject-flake8 = "*"
 tox = "*"
```

### Comparing `bqemulatormanager-0.1.9/PKG-INFO` & `bqemulatormanager-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: bqemulatormanager
-Version: 0.1.9
+Version: 0.2.0
 Summary: bqemulatormanager is a wrapper of bigquery-emulator which provides us BigQuery mock working in local machine.
 Author: gyuta
 Author-email: kuroshiba0408@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: db-dtypes (>=1.0.0,<2.0.0)
 Requires-Dist: google-auth (>=2.17.2,<3.0.0)
-Requires-Dist: google-cloud-bigquery (>=3.0.0,<4.0.0)
+Requires-Dist: google-cloud-bigquery (>=2.34.4)
 Requires-Dist: psutil (>=5.0.0,<6.0.0)
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # BiqQueryEmulator Manager
```

