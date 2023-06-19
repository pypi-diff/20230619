# Comparing `tmp/sqlalchemy-graphqlapi-0.0.1.dev3.tar.gz` & `tmp/sqlalchemy-graphqlapi-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-graphqlapi-0.0.1.dev3.tar", last modified: Fri Nov  4 17:52:15 2022, max compression
+gzip compressed data, was "sqlalchemy-graphqlapi-0.0.1.dev4.tar", last modified: Mon Jun 19 21:51:48 2023, max compression
```

## Comparing `sqlalchemy-graphqlapi-0.0.1.dev3.tar` & `sqlalchemy-graphqlapi-0.0.1.dev4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:52:15.885641 sqlalchemy-graphqlapi-0.0.1.dev3/
--rw-r--r--   0 alex       (501) staff       (20)     1070 2022-02-23 17:37:39.000000 sqlalchemy-graphqlapi-0.0.1.dev3/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     2894 2022-11-04 17:52:15.885347 sqlalchemy-graphqlapi-0.0.1.dev3/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2127 2022-04-07 18:16:49.000000 sqlalchemy-graphqlapi-0.0.1.dev3/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:52:15.883310 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-02-23 18:27:34.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    12271 2022-11-04 17:52:05.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/adapter.py
--rw-r--r--   0 alex       (501) staff       (20)      573 2022-04-04 21:39:46.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/db_engine_specs.py
--rw-r--r--   0 alex       (501) staff       (20)     2848 2022-04-07 18:16:50.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/dialect.py
--rw-r--r--   0 alex       (501) staff       (20)     1679 2022-04-07 18:16:50.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/lib.py
--rw-r--r--   0 alex       (501) staff       (20)      160 2022-04-04 22:06:50.000000 sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/types.py
--rw-r--r--   0 alex       (501) staff       (20)      133 2022-11-04 17:52:05.000000 sqlalchemy-graphqlapi-0.0.1.dev3/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-11-04 17:52:15.885737 sqlalchemy-graphqlapi-0.0.1.dev3/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     4112 2022-11-04 17:52:05.000000 sqlalchemy-graphqlapi-0.0.1.dev3/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:52:15.884852 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     2894 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      442 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      134 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       71 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       10 2022-11-04 17:52:15.000000 sqlalchemy-graphqlapi-0.0.1.dev3/sqlalchemy_graphqlapi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:51:48.800430 sqlalchemy-graphqlapi-0.0.1.dev4/
+-rw-r--r--   0 alex       (501) staff       (20)     1070 2022-02-23 17:37:39.000000 sqlalchemy-graphqlapi-0.0.1.dev4/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     3053 2023-06-19 21:51:48.799706 sqlalchemy-graphqlapi-0.0.1.dev4/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2235 2023-03-12 23:36:14.000000 sqlalchemy-graphqlapi-0.0.1.dev4/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:51:48.791456 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-02-23 18:27:34.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    16138 2023-03-12 23:29:04.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/adapter.py
+-rw-r--r--   0 alex       (501) staff       (20)      573 2022-04-04 21:39:46.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/db_engine_specs.py
+-rw-r--r--   0 alex       (501) staff       (20)     2946 2023-05-30 20:11:45.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/dialect.py
+-rw-r--r--   0 alex       (501) staff       (20)     1844 2023-05-30 20:11:45.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/lib.py
+-rw-r--r--   0 alex       (501) staff       (20)      160 2022-04-04 22:06:50.000000 sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/types.py
+-rw-r--r--   0 alex       (501) staff       (20)      133 2022-11-04 17:52:05.000000 sqlalchemy-graphqlapi-0.0.1.dev4/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-19 21:51:48.800674 sqlalchemy-graphqlapi-0.0.1.dev4/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     4131 2023-06-19 21:51:35.000000 sqlalchemy-graphqlapi-0.0.1.dev4/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:51:48.795895 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3053 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      504 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      134 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       53 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       10 2023-06-19 21:51:48.000000 sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:51:48.798207 sqlalchemy-graphqlapi-0.0.1.dev4/tests/
+-rw-r--r--   0 alex       (501) staff       (20)     2740 2022-04-07 18:16:50.000000 sqlalchemy-graphqlapi-0.0.1.dev4/tests/test_adapter.py
+-rw-r--r--   0 alex       (501) staff       (20)     2566 2023-05-23 21:48:58.000000 sqlalchemy-graphqlapi-0.0.1.dev4/tests/test_dialect.py
+-rw-r--r--   0 alex       (501) staff       (20)      981 2022-04-07 18:16:50.000000 sqlalchemy-graphqlapi-0.0.1.dev4/tests/test_lib.py
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/LICENSE` & `sqlalchemy-graphqlapi-0.0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/PKG-INFO` & `sqlalchemy-graphqlapi-0.0.1.dev4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-graphqlapi
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # graphql-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-graphqlapi.svg)](https://badge.fury.io/py/sqlalchemy-graphqlapi) ![main workflow](https://github.com/cancan101/graphql-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/graphql-db-api/branch/main/graph/badge.svg?token=TOI17GOA2O)](https://codecov.io/gh/cancan101/graphql-db-api)
 
-
 A Python DB API 2.0 for GraphQL APIs
 
 This module allows you to query GraphQL APIs using SQL.
 
 ## SQLAlchemy support
+
 This module provides a SQLAlchemy dialect.
 
 ```python
 from sqlalchemy.engine import create_engine
 
 engine = create_engine('graphql://host:port/path?is_https=0')
 ```
 
 ### Example Usage
+
+#### Querying Connections
+
 ```python
 from sqlalchemy import create_engine
 from sqlalchemy import text
 
 # We use GraphQL SWAPI (The Star Wars API) c/o Netlify:
 engine = create_engine('graphql://swapi-graphql.netlify.app/.netlify/functions/index')
 
 with engine.connect() as connection:
     # Demonstration of requesting nested resource of homeworld
     # and then selecting fields from it
     for row in connection.execute(text("select name, homeworld__name from 'allPeople?include=homeworld'")):
         print(row)
 ```
 
-## Installation
-I was having issues with `apsw-3.9.2.post1` (the newest version of `apsw` that would install for me from PyPI) and ended up needing to follow [the instructions here](https://shillelagh.readthedocs.io/en/latest/install.html) to build / install `apsw` from source. There is an [open ticket on the APSW project](https://github.com/rogerbinns/apsw/issues/310) to provide newer wheels. The issue might be triggered if the table name needs escaping and the error looked like:
-```
-SystemError: <method 'execute' of 'apsw.Cursor' objects> returned NULL without setting an exception
+#### Querying Lists
+
+```python
+from sqlalchemy import create_engine
+from sqlalchemy import text
+
+engine = create_engine('graphql://pet-library.moonhighway.com/')
+
+with engine.connect() as connection:
+    for row in connection.execute(text("select id, name from 'allPets?is_connection=0'")):
+        print(row)
 ```
 
+## Superset support
+
+In order to use with Superset, install this package and then use the `graphql` protocol in the SQLAlchemy URI like: `graphql://swapi-graphql.netlify.app/.netlify/functions/index`. We install a [`db_engine_spec`](https://github.com/cancan101/graphql-db-api/blob/main/graphqldb/db_engine_specs.py) so Superset should recognize the driver.
+
 ## Roadmap
-* [ ] Non-Connections top level
-* [x] Path traversal (basic)
-* [ ] Path traversal (basic + nested)
-* [ ] Path traversal (list / connection)
-* [x] Bearer Tokens in `Authorization` Header
-* [ ] Advanced Auth (e.g. with token refresh)
-* [ ] Passing Headers (e.g. Auth in other locations)
-* [ ] Filtering
-* [ ] Sorting
-* [x] Relay Pagination
+
+- [x] Non-Connections top level
+- [x] Path traversal (basic)
+- [ ] Path traversal (basic + nested)
+- [ ] Path traversal (list / connection)
+- [x] Bearer Tokens in `Authorization` Header
+- [ ] Advanced Auth (e.g. with token refresh)
+- [ ] Passing Headers (e.g. Auth in other locations)
+- [ ] Filtering
+- [ ] Sorting
+- [x] Relay Pagination
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/README.md` & `sqlalchemy-graphqlapi-0.0.1.dev4/sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,83 @@
-# graphql-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-graphqlapi.svg)](https://badge.fury.io/py/sqlalchemy-graphqlapi) ![main workflow](https://github.com/cancan101/graphql-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/graphql-db-api/branch/main/graph/badge.svg?token=TOI17GOA2O)](https://codecov.io/gh/cancan101/graphql-db-api)
+Metadata-Version: 2.1
+Name: sqlalchemy-graphqlapi
+Version: 0.0.1.dev4
+Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
+Home-page: https://github.com/cancan101/graphql-db-api
+Author: Alex Rothberg
+Author-email: agrothberg@gmail.com
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE
 
+# graphql-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-graphqlapi.svg)](https://badge.fury.io/py/sqlalchemy-graphqlapi) ![main workflow](https://github.com/cancan101/graphql-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/graphql-db-api/branch/main/graph/badge.svg?token=TOI17GOA2O)](https://codecov.io/gh/cancan101/graphql-db-api)
 
 A Python DB API 2.0 for GraphQL APIs
 
 This module allows you to query GraphQL APIs using SQL.
 
 ## SQLAlchemy support
+
 This module provides a SQLAlchemy dialect.
 
 ```python
 from sqlalchemy.engine import create_engine
 
 engine = create_engine('graphql://host:port/path?is_https=0')
 ```
 
 ### Example Usage
+
+#### Querying Connections
+
 ```python
 from sqlalchemy import create_engine
 from sqlalchemy import text
 
 # We use GraphQL SWAPI (The Star Wars API) c/o Netlify:
 engine = create_engine('graphql://swapi-graphql.netlify.app/.netlify/functions/index')
 
 with engine.connect() as connection:
     # Demonstration of requesting nested resource of homeworld
     # and then selecting fields from it
     for row in connection.execute(text("select name, homeworld__name from 'allPeople?include=homeworld'")):
         print(row)
 ```
 
-## Installation
-I was having issues with `apsw-3.9.2.post1` (the newest version of `apsw` that would install for me from PyPI) and ended up needing to follow [the instructions here](https://shillelagh.readthedocs.io/en/latest/install.html) to build / install `apsw` from source. There is an [open ticket on the APSW project](https://github.com/rogerbinns/apsw/issues/310) to provide newer wheels. The issue might be triggered if the table name needs escaping and the error looked like:
-```
-SystemError: <method 'execute' of 'apsw.Cursor' objects> returned NULL without setting an exception
+#### Querying Lists
+
+```python
+from sqlalchemy import create_engine
+from sqlalchemy import text
+
+engine = create_engine('graphql://pet-library.moonhighway.com/')
+
+with engine.connect() as connection:
+    for row in connection.execute(text("select id, name from 'allPets?is_connection=0'")):
+        print(row)
 ```
 
+## Superset support
+
+In order to use with Superset, install this package and then use the `graphql` protocol in the SQLAlchemy URI like: `graphql://swapi-graphql.netlify.app/.netlify/functions/index`. We install a [`db_engine_spec`](https://github.com/cancan101/graphql-db-api/blob/main/graphqldb/db_engine_specs.py) so Superset should recognize the driver.
+
 ## Roadmap
-* [ ] Non-Connections top level
-* [x] Path traversal (basic)
-* [ ] Path traversal (basic + nested)
-* [ ] Path traversal (list / connection)
-* [x] Bearer Tokens in `Authorization` Header
-* [ ] Advanced Auth (e.g. with token refresh)
-* [ ] Passing Headers (e.g. Auth in other locations)
-* [ ] Filtering
-* [ ] Sorting
-* [x] Relay Pagination
+
+- [x] Non-Connections top level
+- [x] Path traversal (basic)
+- [ ] Path traversal (basic + nested)
+- [ ] Path traversal (list / connection)
+- [x] Bearer Tokens in `Authorization` Header
+- [ ] Advanced Auth (e.g. with token refresh)
+- [ ] Passing Headers (e.g. Auth in other locations)
+- [ ] Filtering
+- [ ] Sorting
+- [x] Relay Pagination
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/adapter.py` & `sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from __future__ import annotations
+
 from collections import defaultdict
 from typing import (
     Any,
     Collection,
     Dict,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
+    cast,
 )
 from urllib.parse import parse_qs, urlparse
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.fields import (
     Boolean,
     Field,
@@ -22,26 +25,26 @@
     ISODate,
     ISODateTime,
     ISOTime,
     String,
 )
 from shillelagh.typing import RequestedOrder
 
-from .lib import run_query
+from .lib import get_last_query, run_query
 from .types import TypedDict
 
 # -----------------------------------------------------------------------------
 
 
 class MaybeNamed(TypedDict):
     name: Optional[str]
 
 
 class TypeInfo(MaybeNamed):
-    ofType: Optional[MaybeNamed]
+    ofType: Optional[Union[TypeInfo, MaybeNamed]]
     # technically an enum:
     kind: str
 
 
 class FieldInfo(TypedDict):
     name: str
     type: TypeInfo
@@ -87,15 +90,15 @@
 
 
 def get_type_entries(
     field_obj: FieldInfo,
     *,
     data_types: Dict[str, TypeInfoWithFields],
     include: Collection[str],
-    path: List[str] = None,
+    path: Optional[List[str]] = None,
 ) -> Dict[str, Field]:
     path = path or []
 
     field_name = field_obj["name"]
     new_path = path + [field_name]
 
     field_obj_type = field_obj["type"]
@@ -148,31 +151,42 @@
         return {}
 
 
 # -----------------------------------------------------------------------------
 
 
 # clean these up:
-def find_by_name(name: str, *, types: List[FieldInfo]) -> FieldInfo:
-    return [x for x in types if x["name"] == name][0]
+def find_by_name(name: str, *, types: List[FieldInfo]) -> Optional[FieldInfo]:
+    name_match = [x for x in types if x["name"] == name]
+    if len(name_match) == 0:
+        return None
+    return name_match[0]
 
 
-def find_type_by_name(name: str, *, types: List[FieldInfo]) -> TypeInfo:
-    return find_by_name(name, types=types)["type"]
+def find_type_by_name(name: str, *, types: List[FieldInfo]) -> Optional[TypeInfo]:
+    entry = find_by_name(name, types=types)
+    if entry is None:
+        return None
+    return entry["type"]
 
 
 def get_edges_type_name(fields: List[FieldInfo]) -> Optional[str]:
-    edges_info = find_type_by_name("edges", types=fields)["ofType"]
+    entry_type = find_type_by_name("edges", types=fields)
+    if entry_type is None:
+        return None
+    edges_info = entry_type["ofType"]
     if edges_info is None:
         return None
     return edges_info["name"]
 
 
 def get_node_type_name(fields: List[FieldInfo]) -> Optional[str]:
     node_info = find_type_by_name("node", types=fields)
+    if node_info is None:
+        return None
     return node_info["name"]
 
 
 # -----------------------------------------------------------------------------
 
 
 def extract_flattened_value(node: Dict[str, Any], field_name: str) -> Any:
@@ -184,15 +198,15 @@
             raise TypeError(f"{field_name} is not dict path")
         ret = ret.get(path)
     return ret
 
 
 def get_gql_fields(column_names: Sequence[str]) -> str:
     # TODO(cancan101): actually nest this
-    def get_field_str(fields: List[str], root: str = None) -> str:
+    def get_field_str(fields: List[str], root: Optional[str] = None) -> str:
         ret = " ".join(fields)
         if root is not None:
             ret = f"{root} {{{ret}}}"
         return ret
 
     mappings: Dict[Optional[str], List[str]] = defaultdict(list)
     for field in [x.split("__", 1) for x in column_names]:
@@ -250,33 +264,38 @@
     safe = True
 
     def __init__(
         self,
         table: str,
         include: Collection[str],
         query_args: Dict[str, QueryArg],
+        is_connection: bool,
         graphql_api: str,
-        bearer_token: str = None,
-        pagination_relay: bool = None,
+        bearer_token: Optional[str] = None,
+        pagination_relay: Optional[bool] = None,
     ):
         super().__init__()
 
         # The query field name
         self.table = table
 
         self.include = set(include)
         self.query_args = query_args
+        self.is_connection = is_connection
 
         self.graphql_api = graphql_api
         self.bearer_token = bearer_token
 
+        if pagination_relay is True and self.is_connection is False:
+            raise ValueError("pagination_relay True and is_connection False")
         # For now, default this to True. In the future, we can perhaps guess
         self.pagination_relay = True if pagination_relay is None else pagination_relay
 
-        query_type_and_types_query = """{
+        if self.is_connection:
+            query_type_and_types_query = """{
   __schema {
     queryType {
       fields {
         name
         type {
           name
         }
@@ -294,50 +313,118 @@
             name
           }
         }
       }
     }
   }
 }"""
+        else:
+            query_type_and_types_query = """{
+  __schema {
+    queryType {
+      fields {
+        name
+        type {
+          name
+          kind
+          ofType {
+            name
+            kind
+            ofType {
+              kind
+              name
+              ofType {
+                name
+              }
+            }
+          }
+        }
+      }
+    }
+    types {
+      name
+      kind
+      fields {
+        name
+        type {
+          name
+          kind
+          ofType {
+            name
+          }
+        }
+      }
+    }
+  }
+}"""
 
         query_type_and_types = self.run_query(query=query_type_and_types_query)
         query_type_and_types_schema = query_type_and_types["__schema"]
         queries_return_fields: List[FieldInfo] = query_type_and_types_schema[
             "queryType"
         ]["fields"]
 
         # find the matching query (a field on the query object)
         # TODO(cancan101): handle missing
-        query_return_type_name = find_type_by_name(
-            self.table, types=queries_return_fields
-        )["name"]
-        if query_return_type_name is None:
-            raise ValueError("Unable to resolve query_return_type_name")
+        type_entry = find_type_by_name(self.table, types=queries_return_fields)
+        if type_entry is None:
+            raise ValueError(f"Unable to resolve type_entry for {self.table}")
 
         data_types_list: List[TypeInfoWithFields] = query_type_and_types_schema["types"]
         data_types: Dict[str, TypeInfoWithFields] = {
             t["name"]: t for t in data_types_list if t["name"] is not None
         }
 
-        query_return_fields = data_types[query_return_type_name]["fields"]
-        if query_return_fields is None:
-            raise ValueError("No fields found on query")
-
-        # we are assuming a top level connection
-        edges_type_name = get_edges_type_name(query_return_fields)
-        if edges_type_name is None:
-            raise ValueError("Unable to resolve edges_type_name")
-
-        edges_fields = data_types[edges_type_name]["fields"]
-        if edges_fields is None:
-            raise ValueError("No fields found on edge")
-
-        node_type_name = get_node_type_name(edges_fields)
-        if node_type_name is None:
-            raise ValueError("Unable to resolve node_type_name")
+        if self.is_connection:
+            query_return_type_name = type_entry["name"]
+            if query_return_type_name is None:
+                raise ValueError(
+                    f"Unable to resolve query_return_type_name for {self.table}"
+                )
+
+            query_return_fields = data_types[query_return_type_name]["fields"]
+            if query_return_fields is None:
+                raise ValueError("No fields found on query")
+
+            # we are assuming a top level connection
+            edges_type_name = get_edges_type_name(query_return_fields)
+            if edges_type_name is None:
+                raise ValueError("Unable to resolve edges_type_name")
+
+            edges_fields = data_types[edges_type_name]["fields"]
+            if edges_fields is None:
+                raise ValueError("No fields found on edge")
+
+            node_type_name = get_node_type_name(edges_fields)
+            if node_type_name is None:
+                raise ValueError("Unable to resolve node_type_name")
+
+        else:
+            # We are assuming it is NonNull of List of NonNull of item
+            list_type = type_entry["ofType"]
+            if list_type is None:
+                raise ValueError("Unable to resolve list_type")
+
+            # TODO(cancan101): put this info into type system
+            list_type = cast(TypeInfo, list_type)
+
+            item_container_type = list_type["ofType"]
+            if item_container_type is None:
+                raise ValueError("Unable to resolve item_container_type")
+
+            # TODO(cancan101): put this info into type system
+            item_container_type = cast(TypeInfo, item_container_type)
+
+            node_type = item_container_type["ofType"]
+            if node_type is None:
+                raise ValueError("Unable to resolve node_type")
+
+            node_type_name = node_type["name"]
+            if node_type_name is None:
+                raise ValueError("Unable to resolve node_type_name")
 
         node_fields = data_types[node_type_name]["fields"]
         if node_fields is None:
             raise ValueError("No fields found on node")
 
         self.columns: Dict[str, Field] = {}
         for node_field in node_fields:
@@ -349,48 +436,51 @@
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         # TODO the slow path here could connect to the GQL Server
         return True
 
     @staticmethod
-    def parse_uri(table: str) -> Tuple[str, List[str], Dict[str, QueryArg]]:
+    def parse_uri(table: str) -> Tuple[str, List[str], Dict[str, QueryArg], bool]:
         """
         This will pass in the first n args of __init__ for the Adapter
         """
         parsed = urlparse(table)
         query_string = parse_qs(parsed.query)
 
         include_entry = query_string.get("include")
+        is_connection = get_last_query(query_string.get("is_connection", "1")) != "0"
+
         include: List[str] = []
         if include_entry:
             for i in include_entry:
                 include.extend(i.split(","))
 
         query_args = _parse_query_args(query_string)
 
-        return (parsed.path, include, query_args)
+        return (parsed.path, include, query_args, is_connection)
 
     def get_columns(self) -> Dict[str, Field]:
         return self.columns
 
     def run_query(self, query: str) -> Dict[str, Any]:
         return run_query(self.graphql_api, query=query, bearer_token=self.bearer_token)
 
-    def get_data(
+    def get_data_connection(
         self,
         bounds: Dict[str, Filter],
         order: List[Tuple[str, RequestedOrder]],
         **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
         fields_str = get_gql_fields(list(self.columns.keys()))
         query_args_user = dict(self.query_args)
 
         after = query_args_user.pop("after", None)
 
+        # We loop for each page in the pagination
         while True:
             args = dict(query_args_user)
             if after is not None:
                 args["after"] = after
 
             if args:
                 variable_str = f"({_get_variable_argument_str(args)})"
@@ -412,19 +502,58 @@
         }}
         {page_info_str}
     }}
     }}"""
             query_data = self.run_query(query=query)
             query_data_connection = query_data[self.table]
 
-            for edge in query_data_connection["edges"]:
+            edges = query_data_connection["edges"]
+
+            for edge in edges:
                 node: Dict[str, Any] = edge["node"]
 
                 yield {c: extract_flattened_value(node, c) for c in self.columns.keys()}
 
             if self.pagination_relay:
                 page_info = query_data_connection["pageInfo"]
                 if not page_info["hasNextPage"]:
                     break
                 after = page_info["endCursor"]
             else:
+                # If there is no pagination being used, break immediately
                 break
+
+    def get_data_list(
+        self,
+        bounds: Dict[str, Filter],
+        order: List[Tuple[str, RequestedOrder]],
+        **kwargs: Any,
+    ) -> Iterator[Dict[str, Any]]:
+        fields_str = get_gql_fields(list(self.columns.keys()))
+
+        if self.query_args:
+            variable_str = f"({_get_variable_argument_str(self.query_args)})"
+        else:
+            # Don't generate the () for empty list of query_args
+            variable_str = ""
+
+        query = f"""query {{
+{self.table}{variable_str}{{
+    {fields_str}
+}}
+}}"""
+        query_data = self.run_query(query=query)
+        nodes: List[Dict[str, Any]] = query_data[self.table]
+
+        for node in nodes:
+            yield {c: extract_flattened_value(node, c) for c in self.columns.keys()}
+
+    def get_data(
+        self,
+        bounds: Dict[str, Filter],
+        order: List[Tuple[str, RequestedOrder]],
+        **kwargs: Any,
+    ) -> Iterator[Dict[str, Any]]:
+        if self.is_connection:
+            return self.get_data_connection(bounds=bounds, order=order, **kwargs)
+        else:
+            return self.get_data_list(bounds=bounds, order=order, **kwargs)
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/db_engine_specs.py` & `sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/dialect.py` & `sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/dialect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from typing import Any, Dict, List, Tuple
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from shillelagh.backends.apsw.dialects.base import APSWDialect
-from sqlalchemy.engine import Connection
-from sqlalchemy.engine.url import URL
+
+if TYPE_CHECKING:
+    from sqlalchemy.engine import Connection
+    from sqlalchemy.engine.url import URL
 
 from .lib import extract_query, get_last_query, run_query
 
 # -----------------------------------------------------------------------------
 
 ADAPTER_NAME = "graphql"
 
@@ -20,15 +24,15 @@
         self,
         **kwargs: Any,
     ):
         # We tell Shillelagh that this dialect supports just one adapter
         super().__init__(safe=True, adapters=[ADAPTER_NAME], **kwargs)
 
     def get_table_names(
-        self, connection: Connection, schema: str = None, **kwargs: Any
+        self, connection: Connection, schema: Optional[str] = None, **kwargs: Any
     ) -> List[str]:
         url = connection.engine.url
         graphql_api = self.db_url_to_graphql_api(url)
 
         query = """{
   __schema {
     queryType {
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/graphqldb/lib.py` & `sqlalchemy-graphqlapi-0.0.1.dev4/graphqldb/lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+
 import urllib.parse
-from typing import Any, Dict, Sequence, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Union
 
 import requests
-from sqlalchemy.engine.url import URL
+
+if TYPE_CHECKING:
+    from sqlalchemy.engine.url import URL
 
 # -----------------------------------------------------------------------------
 
 
 # Imported from: shillelagh.backends.apsw.dialects.gsheets
 def extract_query(url: URL) -> Dict[str, Union[str, Sequence[str]]]:
     """
@@ -32,21 +36,24 @@
 # -----------------------------------------------------------------------------
 
 
 def run_query(
     graphql_api: str,
     *,
     query: str,
-    bearer_token: str = None,
+    bearer_token: Optional[str] = None,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
     if bearer_token:
         headers["Authorization"] = f"Bearer {bearer_token}"
 
-    resp = requests.post(graphql_api, json={"query": query}, headers=headers)
+    # TODO(cancan101): figure out timeouts
+    resp = requests.post(  # noqa: S113
+        graphql_api, json={"query": query}, headers=headers
+    )
     try:
         resp.raise_for_status()
     except requests.HTTPError as ex:
         # For now let's assume 400 will have errors
         # https://github.com/graphql/graphql-over-http/blob/main/spec/GraphQLOverHTTP.md#status-codes
         if ex.response.status_code != 400:
             raise
```

### Comparing `sqlalchemy-graphqlapi-0.0.1.dev3/setup.py` & `sqlalchemy-graphqlapi-0.0.1.dev4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev3"
+VERSION = "0.0.1.dev4"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
@@ -106,30 +106,30 @@
             "graphql = graphqldb.dialect:APSWGraphQLDialect",
         ],
         "shillelagh.adapter": [
             "graphql = graphqldb.adapter:GraphQLAdapter",
         ],
     },
     install_requires=(
-        "shillelagh >= 1.0.6",
-        "sqlalchemy >= 1.3.0",
-        "requests >= 2.20.0",
+        "shillelagh >= 1.2.0",
+        "requests >= 2.31.0",
         "typing-extensions",
     ),
     license="MIT",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     # $ setup.py publish support.
     cmdclass={
         "buildit": BuildCommand,
         "uploadtest": UploadTestCommand,
         "upload": UploadCommand,
```

