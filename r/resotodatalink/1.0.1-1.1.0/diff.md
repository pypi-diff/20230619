# Comparing `tmp/resotodatalink-1.0.1.tar.gz` & `tmp/resotodatalink-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotodatalink-1.0.1.tar", last modified: Thu Jun 15 06:49:02 2023, max compression
+gzip compressed data, was "resotodatalink-1.1.0.tar", last modified: Mon Jun 19 19:54:43 2023, max compression
```

## Comparing `resotodatalink-1.0.1.tar` & `resotodatalink-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/remote_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-06-15 06:43:43.000000 resotodatalink-1.0.1/resotodatalink/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/resotodatalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 06:49:02.000000 resotodatalink-1.0.1/resotodatalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 06:49:02.466517 resotodatalink-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/batch_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/remote_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-06-19 19:50:29.000000 resotodatalink-1.1.0/resotodatalink/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/resotodatalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 19:54:43.000000 resotodatalink-1.1.0/resotodatalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 19:54:43.565050 resotodatalink-1.1.0/setup.cfg
```

### Comparing `resotodatalink-1.0.1/LICENSE` & `resotodatalink-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/PKG-INFO` & `resotodatalink-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.0.1
+Version: 1.1.0
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotodatalink-1.0.1/pyproject.toml` & `resotodatalink-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotodatalink"
-version = "1.0.1"
+version = "1.1.0"
 authors = [{name="Some Engineering Inc."}]
 description = "Data Pipelines for Resoto infrastructure data."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
```

### Comparing `resotodatalink-1.0.1/requirements-all.txt` & `resotodatalink-1.1.0/requirements-all.txt`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/requirements.txt` & `resotodatalink-1.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/analytics.py` & `resotodatalink-1.1.0/resotodatalink/analytics.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/arrow/config.py` & `resotodatalink-1.1.0/resotodatalink/arrow/config.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/arrow/model.py` & `resotodatalink-1.1.0/resotodatalink/arrow/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,16 @@
         else:
             raise Exception(f"Unknown output format {output_format}")
 
     def create_schema(self, edges: List[Tuple[str, str]]) -> None:
         def table_schema(kind: Kind) -> None:
             table_name = get_table_name(kind.fqn, with_tmp_prefix=False)
             if table_name not in self.schemas:
-                properties, _ = kind_properties(kind, self.model)
-                schema = pa.schema(
-                    [
-                        pa.field("_id", pa.string()),
-                        *[pa.field(p.name, self.pyarrow_type(p.kind)) for p in properties],
-                    ]
-                )
+                properties, _ = kind_properties(kind, self.model, with_id=True)
+                schema = pa.schema([pa.field(p.name, self.pyarrow_type(p.kind)) for p in properties])
                 self.schemas[table_name] = schema
 
         def link_table_schema(from_kind: str, to_kind: str) -> None:
             from_table = get_table_name(from_kind, with_tmp_prefix=False)
             to_table = get_table_name(to_kind, with_tmp_prefix=False)
             link_table = get_link_table_name(from_kind, to_kind, with_tmp_prefix=False)
             if link_table not in self.schemas and from_table in self.schemas and to_table in self.schemas:
```

### Comparing `resotodatalink-1.0.1/resotodatalink/arrow/type_converter.py` & `resotodatalink-1.1.0/resotodatalink/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/arrow/writer.py` & `resotodatalink-1.1.0/resotodatalink/arrow/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import Dict, List, Any, NamedTuple, Optional, final, Union
-import pyarrow.csv as csv
-from dataclasses import dataclass
 import dataclasses
-from abc import ABC
-import pyarrow.parquet as pq
-import pyarrow as pa
+import hashlib
 import json
+from abc import ABC
+from dataclasses import dataclass
 from pathlib import Path
-from resotodatalink.arrow.model import ArrowModel
+from typing import Dict, List, Any, NamedTuple, Optional, final, Union, Tuple
+
+import boto3
+import pyarrow as pa
+import pyarrow.csv as csv
+import pyarrow.parquet as pq
+from google.cloud import storage
+from resotolib.json import value_in_path
+from resotolib.types import Json
+
 from resotodatalink.arrow.config import (
     ArrowOutputConfig,
     FileDestination,
     CloudBucketDestination,
     S3Bucket,
     GCSBucket,
     ArrowDestination,
 )
-from resotodatalink.schema_utils import insert_node
-from resotoclient.models import JsObject
-
-import boto3
-from google.cloud import storage
-import hashlib
+from resotodatalink.arrow.model import ArrowModel
+from resotodatalink.schema_utils import get_table_name, get_link_table_name, carz_access
 
 
 class WriteResult(NamedTuple):
     table_name: str
 
 
 @final
@@ -50,15 +52,14 @@
     format: FileWriterFormat
 
 
 @final
 @dataclass(frozen=True)
 class ArrowBatch:
     table_name: str
-    rows: List[Dict[str, Any]]
     schema: pa.Schema
     writer: FileWriter
     destination: ArrowDestination
 
 
 class ConversionTarget(ABC):
     pass
@@ -163,35 +164,28 @@
             # consume the current element of the path
             new_npath = dataclasses.replace(npath, path=path[1:])
             return [normalize(new_npath, v) for v in obj]
         else:
             raise Exception(f"Unexpected object type {type(obj)}, path: {npath}")
 
 
-def write_batch_to_file(batch: ArrowBatch) -> ArrowBatch:
+def write_batch_to_file(batch: ArrowBatch, rows: List[Json]) -> None:
     to_normalize = collect_normalization_paths(batch.schema)
 
-    for row in batch.rows:
+    for row in rows:
         for path in to_normalize:
             normalize(path, row)
 
-    pa_table = pa.Table.from_pylist(batch.rows, batch.schema)
+    pa_table = pa.Table.from_pylist(rows, batch.schema)
     if isinstance(batch.writer.format, Parquet):
         batch.writer.format.parquet_writer.write_table(pa_table)
     elif isinstance(batch.writer.format, CSV):
         batch.writer.format.csv_writer.write_table(pa_table)
     else:
         raise ValueError(f"Unknown format {batch.writer}")
-    return ArrowBatch(
-        table_name=batch.table_name,
-        rows=[],
-        schema=batch.schema,
-        writer=batch.writer,
-        destination=batch.destination,
-    )
 
 
 def close_writer(batch: ArrowBatch) -> None:
     def upload_to_s3(path: Path, bucket_name: str, region: str) -> None:
         s3_client = boto3.client("s3", region_name=region)
         s3_client.upload_file(str(path), bucket_name, path.name)
 
@@ -262,43 +256,54 @@
 class ArrowWriter:
     def __init__(self, model: ArrowModel, output_config: ArrowOutputConfig):
         self.model = model
         self.kind_by_id: Dict[str, str] = {}
         self.batches: Dict[str, ArrowBatch] = {}
         self.output_config: ArrowOutputConfig = output_config
 
-    def insert_value(self, table_name: str, values: Any) -> Optional[WriteResult]:
-        if self.model.schemas.get(table_name):
+    def batch_for(self, table_name: str) -> Optional[ArrowBatch]:
+        if table_name in self.batches:
+            return self.batches[table_name]
+        elif table_name in self.model.schemas:
             schema = self.model.schemas[table_name]
-            if table_name in self.batches:
-                batch = self.batches[table_name]
-            else:
-                batch = ArrowBatch(
-                    table_name,
-                    [],
-                    schema,
-                    new_writer(table_name, schema, self.output_config),
-                    self.output_config.destination,
-                )
-
-            batch.rows.append(values)
+            batch = ArrowBatch(
+                table_name,
+                schema,
+                new_writer(table_name, schema, self.output_config),
+                self.output_config.destination,
+            )
             self.batches[table_name] = batch
+            return batch
+        else:
+            return None
+
+    def insert_nodes(self, kind: str, nodes: List[Json]) -> Optional[WriteResult]:
+        def to_node(node: Json) -> Json:
+            reported: Json = node.get("reported", {})
+            reported["_id"] = node["id"]
+            reported["cloud"] = value_in_path(node, carz_access["cloud"])
+            reported["account"] = value_in_path(node, carz_access["account"])
+            reported["region"] = value_in_path(node, carz_access["region"])
+            reported["zone"] = value_in_path(node, carz_access["zone"])
+            reported.pop("kind")
+            return reported
+
+        table_name = get_table_name(kind, with_tmp_prefix=False)
+        if batch := self.batch_for(table_name):
+            write_batch_to_file(batch, [to_node(node) for node in nodes])
             return WriteResult(table_name)
         return None
 
-    def insert_node(self, node: JsObject) -> None:
-        result = insert_node(
-            node,
-            self.kind_by_id,
-            self.insert_value,
-            with_tmp_prefix=False,
-        )
-        should_write_batch = result and len(self.batches[result.table_name].rows) > self.output_config.batch_size
-        if result and should_write_batch:
-            batch = self.batches[result.table_name]
-            self.batches[result.table_name] = write_batch_to_file(batch)
+    def insert_edges(self, from_to: Tuple[str, str], nodes: List[Json]) -> Optional[WriteResult]:
+        def to_node(node: Json) -> Json:
+            return {"from_id": node["from"], "to_id": node["to"]}
+
+        from_kind, to_kind = from_to
+        table_name = get_link_table_name(from_kind, to_kind, with_tmp_prefix=False)
+        if batch := self.batch_for(table_name):
+            write_batch_to_file(batch, [to_node(node) for node in nodes])
+            return WriteResult(table_name)
+        return None
 
     def close(self) -> None:
         for table_name, batch in self.batches.items():
-            batch = write_batch_to_file(batch)
-            self.batches[table_name] = batch
             close_writer(batch)
```

### Comparing `resotodatalink-1.0.1/resotodatalink/remote_graph.py` & `resotodatalink-1.1.0/resotodatalink/remote_graph.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/schema_utils.py` & `resotodatalink-1.1.0/resotodatalink/schema_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from resotolib.baseresources import BaseResource
-from resotolib import baseresources
 import inspect
-from resotoclient.models import Property, Kind, JsObject, Model
+from typing import List, Dict, Tuple
+
+from resotoclient.models import Property, Kind, Model
+from resotolib import baseresources
+from resotolib.baseplugin import BaseCollectorPlugin
+from resotolib.baseresources import BaseResource, EdgeType
+from resotolib.core.model_export import node_to_dict
 from resotolib.types import Json
-from typing import List, Dict, Tuple, Optional, Any, Callable, TypeVar
-from resotolib.json import value_in_path
 
 # This set will hold the names of all "base" resources
 # Since that are abstract classes, there will be no instances of them - hence we do not need a table for them.
 base_kinds = {
     clazz.kind for _, clazz in inspect.getmembers(baseresources, inspect.isclass) if issubclass(clazz, BaseResource)
 }
 
@@ -30,15 +32,15 @@
 
 def get_link_table_name(from_kind: str, to_kind: str, with_tmp_prefix: bool = True) -> str:
     # postgres table names are not allowed to be longer than 63 characters
     replaced = f"link_{get_table_name(from_kind, False)[0:25]}_{get_table_name(to_kind, False)[0:25]}"
     return temp_prefix + replaced if with_tmp_prefix else replaced
 
 
-def kind_properties(kind: Kind, model: Model) -> Tuple[List[Property], List[str]]:
+def kind_properties(kind: Kind, model: Model, with_id: bool = False) -> Tuple[List[Property], List[str]]:
     visited = set()
 
     def base_props_not_visited(kd: Kind) -> Tuple[List[Property], List[str]]:
         if kd.fqn in visited:
             return [], []
         visited.add(kd.fqn)
         # take all properties that are not synthetic
@@ -53,37 +55,31 @@
                 props, succs = base_props_not_visited(ck)
                 for prop in props:
                     properties[prop.name] = prop
                 successors.extend(succs)
         return list(properties.values()), successors
 
     prs, scs = base_props_not_visited(kind)
-    return prs + carz, scs
-
-
-T = TypeVar("T")
+    id_prop = [Property("_id", "string", True)] if with_id else []
+    return id_prop + prs + carz, scs
 
 
-def insert_node(
-    node: JsObject,
-    kind_by_id: Dict[str, str],
-    insert_value: Callable[[str, Any], Optional[T]],
-    with_tmp_prefix: bool = True,
-    flatten: bool = False,
-) -> Optional[T]:
-    if node.get("type") == "node" and "id" in node and "reported" in node:
-        reported: Json = node.get("reported", {})
-        reported["_id"] = node["id"]
-        reported["cloud"] = value_in_path(node, carz_access["cloud"])
-        reported["account"] = value_in_path(node, carz_access["account"])
-        reported["region"] = value_in_path(node, carz_access["region"])
-        reported["zone"] = value_in_path(node, carz_access["zone"])
-        kind = reported.pop("kind")
-        kind_by_id[node["id"]] = kind
-        return insert_value(get_table_name(kind, with_tmp_prefix), reported)
-    elif node.get("type") == "edge" and "from" in node and "to" in node:
-        from_id = node["from"]
-        to_id = node["to"]
-        if (from_kind := kind_by_id.get(from_id)) and (to_kind := kind_by_id.get(to_id)):
-            link_table = get_link_table_name(from_kind, to_kind, with_tmp_prefix)
-            return insert_value(link_table, {"from_id": from_id, "to_id": to_id})
-    raise ValueError(f"Unknown node: {node}")
+def prepare_node(node: BaseResource, collector: BaseCollectorPlugin) -> Json:
+    node._graph = collector.graph
+    exported = node_to_dict(node)
+    exported["type"] = "node"
+    exported["ancestors"] = {
+        "cloud": {"reported": {"id": node.cloud().name}},
+        "account": {"reported": {"id": node.account().name}},
+        "region": {"reported": {"id": node.region().name}},
+        "zone": {"reported": {"id": node.zone().name}},
+    }
+    return exported
+
+
+def prepare_edge(from_resource: BaseResource, to_resource: BaseResource, edge_type: EdgeType) -> Json:
+    return {
+        "type": "edge",
+        "from": from_resource.chksum,
+        "to": to_resource.chksum,
+        "edge_type": edge_type.name,
+    }
```

### Comparing `resotodatalink-1.0.1/resotodatalink/show_progress.py` & `resotodatalink-1.1.0/resotodatalink/show_progress.py`

 * *Files identical despite different names*

### Comparing `resotodatalink-1.0.1/resotodatalink/snowflake.py` & `resotodatalink-1.1.0/resotodatalink/snowflake.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import json
 import logging
 from typing import Any, List, Iterator
 
 from resotoclient import Model
-from resotoclient.models import Property
 from resotolib.types import Json
 from snowflake.sqlalchemy import ARRAY, OBJECT
 from sqlalchemy import Integer, Float, String, Boolean, column
 from sqlalchemy import select
 from sqlalchemy.sql import Values
 from sqlalchemy.sql.dml import ValuesBase
 
-from resotodatalink.sql import SqlDefaultUpdater, DialectUpdater
-
 from resotodatalink.schema_utils import kind_properties, get_table_name
+from resotodatalink.sql import SqlDefaultUpdater, DialectUpdater
 
 log = logging.getLogger("resoto.datalink")
 
 
 def kind_to_snowflake_type(kind_name: str, model: Model) -> Any:  # Type[TypeEngine[Any]]
     """
     Map internal kinds to snowflake types.
@@ -57,16 +55,15 @@
     """
 
     def __init__(self, model: Model, **args: Any) -> None:
         super().__init__(model, **args)
         self.column_types_fn = kind_to_snowflake_type
 
     def insert_nodes(self, kind: str, nodes: List[Json]) -> Iterator[ValuesBase]:
-        kp, _ = kind_properties(self.model.kinds[kind], self.model)
-        kind_props = [Property("_id", "string")] + kp
+        kind_props, _ = kind_properties(self.model.kinds[kind], self.model, with_id=True)
         select_array = []
         column_definitions = []
         prop_is_json = {}
 
         # Inserting structured data into Snowflake requires a bit of work. General scheme:
         # insert into TBL(col_string, col_json) SELECT column1, parse_json(column2) from values('a', '{"b":1}');
         # All json and array elements need to be json encoded and parsed on the server side again.
```

### Comparing `resotodatalink-1.0.1/resotodatalink/sql.py` & `resotodatalink-1.1.0/resotodatalink/sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from abc import ABC, abstractmethod
 from datetime import datetime, date
-from typing import List, Any, Type, Tuple, Dict, Iterator, Optional
+from typing import List, Any, Type, Tuple, Dict, Iterator, Optional, Union
 
-from resotoclient.models import Kind, Model
+from resotoclient.models import Kind, Model, Property
 from resotolib.types import Json
 from resotolib.utils import UTC_Date_Format
 from sqlalchemy import (
     Boolean,
     Column,
     Float,
     Integer,
@@ -20,23 +20,25 @@
     Date,
     TypeDecorator,
 )
 from sqlalchemy.engine import Engine, Connection, Dialect
 from sqlalchemy.sql.ddl import DropTable, DropConstraint
 from sqlalchemy.sql.dml import ValuesBase
 
+from resotodatalink import EngineConfig
 from resotodatalink.schema_utils import (
     base_kinds,
     temp_prefix,
     carz_access,
     get_table_name,
     get_link_table_name,
     kind_properties,
 )
 from resotolib.json import value_in_path
+from sqlalchemy import create_engine
 
 log = logging.getLogger("resoto.datalink")
 
 
 class DateTimeString(TypeDecorator):  # type: ignore
     """
     This type decorator translates between string (python) and datetime (sqlalchemy) types.
@@ -94,67 +96,88 @@
     elif kind and kind.runtime_kind is not None:  # refined simple type like enum
         return sql_kind_to_column_type(kind.runtime_kind, model)
     else:
         raise ValueError(f"Not able to handle kind {kind_name}")
 
 
 class SqlUpdater(ABC):
+    @property
+    @abstractmethod
+    def batch_size(self) -> int:
+        pass
+
     @abstractmethod
     def insert_nodes(self, kind: str, nodes: List[Json]) -> Iterator[ValuesBase]:
         pass
 
     @abstractmethod
     def insert_edges(self, from_to: Tuple[str, str], nodes: List[Json]) -> Iterator[ValuesBase]:
         pass
 
     @abstractmethod
     def create_schema(self, connection: Connection, edges: List[Tuple[str, str]]) -> MetaData:
         pass
 
     @staticmethod
-    def swap_temp_tables(engine: Engine) -> None:
-        with engine.connect() as connection:
-            with connection.begin():
-                metadata = MetaData()
-                metadata.reflect(connection, resolve_fks=False)
-
-                def drop_table(tl: Table) -> None:
-                    for cs in tl.foreign_key_constraints:
-                        connection.execute(DropConstraint(cs))
-                    connection.execute(DropTable(tl))
-
-                for table in metadata.tables.values():
-                    if table.name.startswith(temp_prefix):
-                        prod_table = table.name[len(temp_prefix) :]  # noqa: E203
-                        if prod_table in metadata.tables:
-                            drop_table(metadata.tables[prod_table])
-                        connection.execute(DDL(f"ALTER TABLE {table.name} RENAME TO {prod_table}"))
-                # todo: create foreign key constraints on the final tables
+    def swap_temp_tables(db_access: Union[EngineConfig, Connection], drop_existing_tables: bool = False) -> None:
+        def swap(connection: Connection) -> None:
+            metadata = MetaData()
+            metadata.reflect(connection, resolve_fks=False)
+            dropped_tables = set()
+
+            def drop_table(tl: Table) -> None:
+                if tl.name in dropped_tables:
+                    return
+                dropped_tables.add(tl.name)
+                for cs in tl.foreign_key_constraints:
+                    connection.execute(DropConstraint(cs))
+                connection.execute(DropTable(tl))
+
+            for table in metadata.tables.values():
+                if table.name.startswith(temp_prefix):
+                    prod_table = table.name[len(temp_prefix) :]  # noqa: E203
+                    if prod_table in metadata.tables:
+                        drop_table(metadata.tables[prod_table])
+                    connection.execute(DDL(f"ALTER TABLE {table.name} RENAME TO {prod_table}"))
+                elif drop_existing_tables:
+                    drop_table(table)
+            # todo: create foreign key constraints on the final tables
+
+        if isinstance(db_access, EngineConfig):
+            engine = create_engine(db_access.connection_string)
+            with engine.begin() as connection:
+                swap(connection)
+        else:
+            swap(db_access)
 
 
 class SqlDefaultUpdater(SqlUpdater):
     def __init__(self, model: Model, **kwargs: Any) -> None:
         self.model = model
         self.metadata = MetaData()
         self.table_kinds = [
             kind
             for kind in model.kinds.values()
             if kind.aggregate_root and kind.runtime_kind is None and kind.fqn not in base_kinds
         ]
         self.kind_by_id: Dict[str, str] = {}
         self.column_types_fn = kwargs.get("kind_to_column_type", sql_kind_to_column_type)
-        self.insert_batch_size = kwargs.get("insert_batch_size", 5000)
+        self.insert_batch_size: int = int(kwargs.get("insert_batch_size", 5000))
+
+    @property
+    def batch_size(self) -> int:
+        return self.insert_batch_size
 
     def create_schema(self, connection: Connection, edges: List[Tuple[str, str]]) -> MetaData:
         log.info(f"Create schema for {len(self.table_kinds)} kinds and their relationships")
 
         def table_schema(kind: Kind) -> None:
             table_name = get_table_name(kind.fqn)
             if table_name not in self.metadata.tables:
-                properties, _ = kind_properties(kind, self.model)
+                properties, _ = kind_properties(kind, self.model, with_id=False)
                 Table(
                     get_table_name(kind.fqn),
                     self.metadata,
                     *[
                         Column("_id", String, primary_key=True),
                         *[Column(p.name, self.column_types_fn(p.kind, self.model)) for p in properties],
                     ],
@@ -193,36 +216,39 @@
         self.metadata.drop_all(connection)
 
         # create the tables
         self.metadata.create_all(connection)
 
         return self.metadata
 
-    def node_to_json(self, node: Json) -> Json:
+    def node_to_json(self, node: Json, known_props: Optional[List[Property]] = None) -> Json:
         if node.get("type") == "node" and "id" in node and "reported" in node:
             reported: Json = node.get("reported", {})
             reported["_id"] = node["id"]
             reported["cloud"] = value_in_path(node, carz_access["cloud"])
             reported["account"] = value_in_path(node, carz_access["account"])
             reported["region"] = value_in_path(node, carz_access["region"])
             reported["zone"] = value_in_path(node, carz_access["zone"])
-            reported.pop("kind", None)
-            return reported
+            # In case of known props, make sure to always return a dict with all known props
+            if known_props is not None:
+                return {p.name: reported.get(p.name) for p in known_props}
+            else:
+                reported.pop("kind", None)
+                return reported
         elif node.get("type") == "edge" and "from" in node and "to" in node:
             return {"from_id": node["from"], "to_id": node["to"]}
         raise ValueError(f"Unknown node: {node}")
 
     def insert_nodes(self, kind: str, nodes: List[Json]) -> Iterator[ValuesBase]:
         # create a defaults dict with all properties set to None
-        kp, _ = kind_properties(self.model.kinds[kind], self.model)
-        defaults = {p.name: None for p in kp}
+        kp, _ = kind_properties(self.model.kinds[kind], self.model, with_id=True)
 
         if (table := self.metadata.tables.get(get_table_name(kind))) is not None:
             for batch in (nodes[i : i + self.insert_batch_size] for i in range(0, len(nodes), self.insert_batch_size)):
-                converted = [defaults | self.node_to_json(node) for node in batch]
+                converted = [self.node_to_json(node, kp) for node in batch]
                 yield table.insert().values(converted)
 
     def insert_edges(self, from_to: Tuple[str, str], nodes: List[Json]) -> Iterator[ValuesBase]:
         from_kind, to_kind = from_to
         table = self.metadata.tables.get(get_link_table_name(from_kind, to_kind))
         maybe_insert = table.insert() if table is not None else None
         if maybe_insert is not None:
```

### Comparing `resotodatalink-1.0.1/resotodatalink.egg-info/PKG-INFO` & `resotodatalink-1.1.0/resotodatalink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodatalink
-Version: 1.0.1
+Version: 1.1.0
 Summary: Data Pipelines for Resoto infrastructure data.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotodatalink-1.0.1/resotodatalink.egg-info/SOURCES.txt` & `resotodatalink-1.1.0/resotodatalink.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 requirements-all.txt
 requirements.txt
 setup.cfg
 resotodatalink/__init__.py
 resotodatalink/analytics.py
+resotodatalink/batch_stream.py
 resotodatalink/collect_plugins.py
 resotodatalink/py.typed
 resotodatalink/remote_graph.py
 resotodatalink/schema_utils.py
 resotodatalink/show_progress.py
 resotodatalink/snowflake.py
 resotodatalink/sql.py
```

