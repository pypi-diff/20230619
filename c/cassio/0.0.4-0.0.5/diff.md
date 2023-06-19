# Comparing `tmp/cassio-0.0.4.tar.gz` & `tmp/cassio-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cassio-0.0.4.tar", last modified: Tue Jun  6 14:15:01 2023, max compression
+gzip compressed data, was "cassio-0.0.5.tar", last modified: Mon Jun 19 12:49:54 2023, max compression
```

## Comparing `cassio-0.0.4.tar` & `cassio-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-06 14:15:01.412580 cassio-0.0.4/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1084 2023-06-06 13:38:56.000000 cassio-0.0.4/README.md
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-06 14:15:01.412580 cassio-0.0.4/setup.cfg
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     1606 2023-06-06 13:40:21.000000 cassio-0.0.4/setup.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.408580 cassio-0.0.4/src/
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      128 2023-06-06 13:59:08.000000 cassio-0.0.4/src/cassio/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/db_extractor/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.4/src/cassio/db_extractor/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2825 2023-06-06 13:59:13.000000 cassio-0.0.4/src/cassio/db_extractor/cassandra_extractor.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/globals/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       43 2023-05-23 20:27:43.000000 cassio-0.0.4/src/cassio/globals/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      601 2023-06-06 13:51:23.000000 cassio-0.0.4/src/cassio/globals/globals.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/history/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.4/src/cassio/history/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2386 2023-05-23 21:39:10.000000 cassio-0.0.4/src/cassio/history/history_management.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/inspection/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       73 2023-05-19 16:24:06.000000 cassio-0.0.4/src/cassio/inspection/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      323 2023-05-30 22:40:16.000000 cassio-0.0.4/src/cassio/inspection/schema.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/keyvalue/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.4/src/cassio/keyvalue/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     3326 2023-05-25 15:21:39.000000 cassio-0.0.4/src/cassio/keyvalue/kv_cache.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/utils/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       50 2023-05-23 21:35:34.000000 cassio-0.0.4/src/cassio/utils/__init__.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/utils/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       67 2023-05-23 21:35:29.000000 cassio-0.0.4/src/cassio/utils/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2531 2023-05-24 14:14:55.000000 cassio-0.0.4/src/cassio/utils/vector/distance_metrics.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio/vector/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       57 2023-05-23 20:58:39.000000 cassio-0.0.4/src/cassio/vector/__init__.py
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     7926 2023-06-06 13:57:00.000000 cassio-0.0.4/src/cassio/vector/vector_db_driver.py
-drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-06 14:15:01.412580 cassio-0.0.4/src/cassio.egg-info/
--rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/PKG-INFO
--rw-rw-r--   0 stefano   (1000) stefano   (1000)      743 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/SOURCES.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/dependency_links.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/requires.txt
--rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-06 14:15:01.000000 cassio-0.0.4/src/cassio.egg-info/top_level.txt
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-19 12:49:54.204303 cassio-0.0.5/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1084 2023-06-16 14:11:44.000000 cassio-0.0.5/README.md
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       78 2023-06-19 12:49:54.204303 cassio-0.0.5/setup.cfg
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1606 2023-06-19 10:36:08.000000 cassio-0.0.5/setup.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.200303 cassio-0.0.5/src/
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.200303 cassio-0.0.5/src/cassio/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       93 2023-06-16 15:56:04.000000 cassio-0.0.5/src/cassio/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/cql/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2384 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/cql/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/db_extractor/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       71 2023-05-30 22:40:16.000000 cassio-0.0.5/src/cassio/db_extractor/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     3001 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/db_extractor/cassandra_extractor.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/history/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       64 2023-05-23 00:11:06.000000 cassio-0.0.5/src/cassio/history/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     1622 2023-06-19 12:49:19.000000 cassio-0.0.5/src/cassio/history/history_management.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/keyvalue/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       45 2023-05-23 14:40:40.000000 cassio-0.0.5/src/cassio/keyvalue/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2377 2023-06-16 14:33:36.000000 cassio-0.0.5/src/cassio/keyvalue/kv_cache.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/utils/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       48 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/__init__.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/utils/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       65 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2554 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/utils/vector/distance_metrics.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio/vector/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       55 2023-06-16 14:11:47.000000 cassio-0.0.5/src/cassio/vector/__init__.py
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     6235 2023-06-16 15:56:04.000000 cassio-0.0.5/src/cassio/vector/vector_db_driver.py
+drwxrwxr-x   0 stefano   (1000) stefano   (1000)        0 2023-06-19 12:49:54.204303 cassio-0.0.5/src/cassio.egg-info/
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)     2520 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/PKG-INFO
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)      643 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        1 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)       36 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/requires.txt
+-rw-rw-r--   0 stefano   (1000) stefano   (1000)        7 2023-06-19 12:49:54.000000 cassio-0.0.5/src/cassio.egg-info/top_level.txt
```

### Comparing `cassio-0.0.4/PKG-INFO` & `cassio-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.4/README.md` & `cassio-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cassio-0.0.4/setup.py` & `cassio-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='cassio',
-    version='0.0.4',
+    version='0.0.5',
     author='Stefano Lottini',
     author_email='stefano.lottini@datastax.com',
     package_dir={"": "src"},
     packages=find_packages(where='src'),
     # entry_points={
     #     "console_scripts": [
     #         # will we ever have a command-line cassio script?
```

### Comparing `cassio-0.0.4/src/cassio/db_extractor/cassandra_extractor.py` & `cassio-0.0.5/src/cassio/db_extractor/cassandra_extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,81 @@
 """
 An extractor able to resolve single-row lookups from Cassandra tables in
 a keyspace, with a fair amount of metadata inspection.
 """
 
 from functools import reduce
+from typing import List
 
 from cassandra.query import SimpleStatement
 
-from cassio.inspection import (
-    _table_primary_key_columns,
-)
+import cassio.cql
 
 
-class CassandraExtractor():
+def _table_primary_key_columns(session, keyspace, table) -> List[str]:
+    table = session.cluster.metadata.keyspaces[keyspace].tables[table]
+    return [
+        col.name for col in table.partition_key
+    ] + [
+        col.name for col in table.clustering_key
+    ]
+
+
+class CassandraExtractor:
 
     def __init__(self, session, keyspace, field_mapper, literal_nones):
         self.session = session
         self.keyspace = keyspace
         self.field_mapper = field_mapper
-        self.literal_nones = literal_nones # TODO: handle much better
+        self.literal_nones = literal_nones  # TODO: handle much better
         # derived fields
-        self.tablesNeeded = {fmv[0] for fmv in field_mapper.values()}
-        self.primaryKeyMap = {
-            tableName: _table_primary_key_columns(self.session, self.keyspace, tableName)
-            for tableName in self.tablesNeeded
+        self.tables_needed = {fmv[0] for fmv in field_mapper.values()}
+        self.primary_key_map = {
+            table: _table_primary_key_columns(self.session, self.keyspace, table)
+            for table in self.tables_needed
         }
         # all primary-key values needed across tables
-        self.requiredParameters = list(reduce(lambda accum, nw: accum | set(nw), self.primaryKeyMap.values(), set()))
+        self.requiredParameters = list(reduce(lambda accum, nw: accum | set(nw), self.primary_key_map.values(), set()))
+
         # TODOs:
         #   move this getter creation someplace else
-        #   query a table only once (grouping required variables by source table, selecting only those unless function passed)
+        #   query a table only once (grouping required variables by source table,
+        #   selecting only those unless function passed)
         def _getter(**kwargs):
-            def _retrieve_field(_tableName2, _keyColumns, _columnOrExtractor, _keyValueMap):
-                selector = SimpleStatement('SELECT * FROM {keyspace}.{tableName} WHERE {whereClause} LIMIT 1;'.format(
+            def _retrieve_field(_table2, _key_columns, _column_or_extractor, _key_value_map):
+                selector = SimpleStatement(cassio.cql.retrieve_one_row.format(
                     keyspace=keyspace,
-                    tableName=_tableName2,
+                    table=_table2,
                     whereClause=' AND '.join(
                         f'{kc} = %s'
-                        for kc in _keyColumns
+                        for kc in _key_columns
                     ),
                 ))
                 values = tuple([
-                    _keyValueMap[kc]
-                    for kc in _keyColumns
+                    _key_value_map[kc]
+                    for kc in _key_columns
                 ])
                 row = session.execute(selector, values).one()
                 if row:
-                    if callable(_columnOrExtractor):
-                        return _columnOrExtractor(row)
+                    if callable(_column_or_extractor):
+                        return _column_or_extractor(row)
                     else:
-                        return getattr(row, _columnOrExtractor)
+                        return getattr(row, _column_or_extractor)
                 else:
                     if literal_nones:
                         return None
                     else:
                         raise ValueError('No data found for %s from %s.%s' % (
-                            str(_columnOrExtractor),
+                            str(_column_or_extractor),
                             keyspace,
-                            _tableName2,
+                            _table2,
                         ))
-            
+
             return {
-                field: _retrieve_field(tableName, self.primaryKeyMap[tableName], columnOrExtractor, kwargs)
-                for field, (tableName, columnOrExtractor) in field_mapper.items()
+                field: _retrieve_field(table, self.primary_key_map[table], columnOrExtractor, kwargs)
+                for field, (table, columnOrExtractor) in field_mapper.items()
             }
+
         self.getter = _getter
 
-    def __call__(self, *pargs, **kwargs):
-        return self.getter(*pargs, **kwargs)
+    def __call__(self, **kwargs):
+        return self.getter(**kwargs)
```

### Comparing `cassio-0.0.4/src/cassio/keyvalue/kv_cache.py` & `cassio-0.0.5/src/cassio/keyvalue/kv_cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,125 +3,86 @@
 One row per partition, serializes a multiple partition key into a string
 """
 
 from typing import Union, List, Any
 
 from cassandra.cluster import Session
 
-# CQL templates
-_createTableCQLTemplate = """
-CREATE TABLE IF NOT EXISTS {keyspace}.{tableName} (
-    key_desc TEXT,
-    cache_key TEXT,
-    cache_value TEXT,
-    PRIMARY KEY (( key_desc, cache_key ))
-);
-"""
-_getCachedItemCQLTemplate = """
-SELECT cache_value
-    FROM {keyspace}.{tableName}
-WHERE key_desc=%s
-    AND cache_key=%s;
-"""
-_deleteCachedItemCQLTemplate = """
-DELETE FROM {keyspace}.{tableName}
-WHERE key_desc=%s
-    AND cache_key=%s;
-"""
-_storeCachedItemCQLTemplate = """
-INSERT INTO {keyspace}.{tableName} (
-    key_desc,
-    cache_key,
-    cache_value
-) VALUES (
-    %s,
-    %s,
-    %s
-){ttlSpec};
-"""
-_truncateTableCQLTemplate = """
-TRUNCATE TABLE {keyspace}.{tableName};
-"""
+import cassio.cql
 
 
-class KVCache():
+class KVCache:
 
-    def __init__(self, session: Session, keyspace: str, tableName: str, keys: List[Any]):
+    def __init__(self, session: Session, keyspace: str, table: str, keys: List[Any]):
         self.session = session
         self.keyspace = keyspace
-        self.tableName = tableName
+        self.table = table
         self.keys = keys
-        self.keyDesc = '/'.join(self.keys)
+        self.key_desc = '/'.join(self.keys)
         # Schema creation, if needed
-        createTableCQL = _createTableCQLTemplate.format(
+        st = cassio.cql.create_kv_table.format(
             keyspace=self.keyspace,
-            tableName=self.tableName,
+            table=self.table,
         )
-        session.execute(createTableCQL)
+        session.execute(st)
 
     def clear(self):
-        truncateTableCQL = _truncateTableCQLTemplate.format(
+        st = cassio.cql.truncate_table.format(
             keyspace=self.keyspace,
-            tableName=self.tableName,
-        )
-        self.session.execute(
-            truncateTableCQL
+            table=self.table,
         )
+        self.session.execute(st)
 
-    def put(self, keyDict, cacheValue, ttlSeconds):
-        if ttlSeconds:
-            ttlSpec = f' USING TTL {ttlSeconds}'
+    def put(self, key_dict, cache_value, ttl_seconds):
+        if ttl_seconds:
+            ttl_spec = f' USING TTL {ttl_seconds}'
         else:
-            ttlSpec = ''
-        cacheKey = self._serializeKey([
-            keyDict[k]
+            ttl_spec = ''
+        cache_key = self._serialize_key([
+            key_dict[k]
             for k in self.keys
         ])
-        storeCachedItemCQL = _storeCachedItemCQLTemplate.format(
+        st = cassio.cql.store_kv_item.format(
             keyspace=self.keyspace,
-            tableName=self.tableName,
-            ttlSpec=ttlSpec,
+            table=self.table,
+            ttlSpec=ttl_spec,
         )
         self.session.execute(
-            storeCachedItemCQL,
-            (
-                self.keyDesc,
-                cacheKey,
-                cacheValue,
-            ),
+            st,
+            (self.key_desc, cache_key, cache_value,),
         )
 
-    def get(self, keyDict) -> Union[None, str]:
-        cacheKey = self._serializeKey([
-            keyDict[k]
+    def get(self, key_dict) -> Union[None, str]:
+        cache_key = self._serialize_key([
+            key_dict[k]
             for k in self.keys
         ])
-        getCachedItemCQL = _getCachedItemCQLTemplate.format(
+        st = cassio.cql.get_kv_item.format(
             keyspace=self.keyspace,
-            tableName=self.tableName,
+            table=self.table,
         )
-        foundRow = self.session.execute(
-            getCachedItemCQL,
-            (self.keyDesc, cacheKey),
+        row = self.session.execute(
+            st,
+            (self.key_desc, cache_key),
         ).one()
-        if foundRow:
-            return foundRow.cache_value
+        if row:
+            return row.cache_value
         else:
             return None
 
-    def delete(self, keyDict) -> None:
+    def delete(self, key_dict) -> None:
         """ Will not complain if the row does not exist. """
-        cacheKey = self._serializeKey([
-            keyDict[k]
+        cache_key = self._serialize_key([
+            key_dict[k]
             for k in self.keys
         ])
-        deleteCachedItemCQL = _deleteCachedItemCQLTemplate.format(
+        st = cassio.cql.delete_kv_item.format(
             keyspace=self.keyspace,
-            tableName=self.tableName,
+            table=self.table,
         )
         self.session.execute(
-            deleteCachedItemCQL,
-            (self.keyDesc, cacheKey),
+            st,
+            (self.key_desc, cache_key),
         )
 
-    def _serializeKey(self, keys: List[str]):
+    def _serialize_key(self, keys: List[str]):
         return str(keys)
```

### Comparing `cassio-0.0.4/src/cassio.egg-info/PKG-INFO` & `cassio-0.0.5/src/cassio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cassio
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework-agnostic Python library to seamlessly integrate Apache Cassandra with ML/LLM/genAI workloads.
 Home-page: https://github.com/hemidactylus/cassio
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 License: LICENSE.txt
 Description: # cassIO
```

### Comparing `cassio-0.0.4/src/cassio.egg-info/SOURCES.txt` & `cassio-0.0.5/src/cassio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 setup.py
 src/cassio/__init__.py
 src/cassio.egg-info/PKG-INFO
 src/cassio.egg-info/SOURCES.txt
 src/cassio.egg-info/dependency_links.txt
 src/cassio.egg-info/requires.txt
 src/cassio.egg-info/top_level.txt
+src/cassio/cql/__init__.py
 src/cassio/db_extractor/__init__.py
 src/cassio/db_extractor/cassandra_extractor.py
-src/cassio/globals/__init__.py
-src/cassio/globals/globals.py
 src/cassio/history/__init__.py
 src/cassio/history/history_management.py
-src/cassio/inspection/__init__.py
-src/cassio/inspection/schema.py
 src/cassio/keyvalue/__init__.py
 src/cassio/keyvalue/kv_cache.py
 src/cassio/utils/__init__.py
 src/cassio/utils/vector/__init__.py
 src/cassio/utils/vector/distance_metrics.py
 src/cassio/vector/__init__.py
 src/cassio/vector/vector_db_driver.py
```

