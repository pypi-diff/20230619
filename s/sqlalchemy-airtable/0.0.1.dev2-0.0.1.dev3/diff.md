# Comparing `tmp/sqlalchemy-airtable-0.0.1.dev2.tar.gz` & `tmp/sqlalchemy-airtable-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-airtable-0.0.1.dev2.tar", last modified: Mon Apr  4 22:08:09 2022, max compression
+gzip compressed data, was "sqlalchemy-airtable-0.0.1.dev3.tar", last modified: Mon Jun 19 21:35:44 2023, max compression
```

## Comparing `sqlalchemy-airtable-0.0.1.dev2.tar` & `sqlalchemy-airtable-0.0.1.dev3.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-04 22:08:09.837526 sqlalchemy-airtable-0.0.1.dev2/
--rw-r--r--   0 alex       (501) staff       (20)     1070 2022-03-21 21:16:35.000000 sqlalchemy-airtable-0.0.1.dev2/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     4138 2022-04-04 22:08:09.836734 sqlalchemy-airtable-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3356 2022-04-04 21:20:30.000000 sqlalchemy-airtable-0.0.1.dev2/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-04 22:08:09.831871 sqlalchemy-airtable-0.0.1.dev2/airtabledb/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-03-22 21:23:38.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5994 2022-04-04 17:40:42.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/adapter.py
--rw-r--r--   0 alex       (501) staff       (20)      574 2022-03-30 01:25:28.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/db_engine_specs.py
--rw-r--r--   0 alex       (501) staff       (20)     3533 2022-03-31 18:50:57.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/dialect.py
--rw-r--r--   0 alex       (501) staff       (20)     5380 2022-04-04 17:40:42.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/fields.py
--rw-r--r--   0 alex       (501) staff       (20)     2709 2022-03-28 23:15:06.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/formulas.py
--rw-r--r--   0 alex       (501) staff       (20)     1521 2022-04-04 17:40:42.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/lib.py
--rw-r--r--   0 alex       (501) staff       (20)      349 2022-03-22 21:23:38.000000 sqlalchemy-airtable-0.0.1.dev2/airtabledb/types.py
--rw-r--r--   0 alex       (501) staff       (20)      107 2022-03-30 01:18:39.000000 sqlalchemy-airtable-0.0.1.dev2/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-04-04 22:08:09.837915 sqlalchemy-airtable-0.0.1.dev2/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     4233 2022-04-04 21:34:12.000000 sqlalchemy-airtable-0.0.1.dev2/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-04-04 22:08:09.835618 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     4138 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      480 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      225 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       65 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2022-04-04 22:08:09.000000 sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:35:44.261804 sqlalchemy-airtable-0.0.1.dev3/
+-rw-r--r--   0 alex       (501) staff       (20)     1070 2022-03-21 21:16:35.000000 sqlalchemy-airtable-0.0.1.dev3/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     3618 2023-06-19 21:35:44.261412 sqlalchemy-airtable-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2805 2022-08-17 20:12:15.000000 sqlalchemy-airtable-0.0.1.dev3/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:35:44.253259 sqlalchemy-airtable-0.0.1.dev3/airtabledb/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-03-22 21:23:38.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     7004 2022-08-17 20:12:15.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/adapter.py
+-rw-r--r--   0 alex       (501) staff       (20)      574 2022-04-05 05:03:46.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/db_engine_specs.py
+-rw-r--r--   0 alex       (501) staff       (20)     3692 2023-06-19 21:30:46.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/dialect.py
+-rw-r--r--   0 alex       (501) staff       (20)     5380 2022-04-05 05:03:46.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/fields.py
+-rw-r--r--   0 alex       (501) staff       (20)     3521 2022-04-06 05:38:56.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/formulas.py
+-rw-r--r--   0 alex       (501) staff       (20)     1521 2022-04-05 05:03:46.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/lib.py
+-rw-r--r--   0 alex       (501) staff       (20)      349 2022-03-22 21:23:38.000000 sqlalchemy-airtable-0.0.1.dev3/airtabledb/types.py
+-rw-r--r--   0 alex       (501) staff       (20)      107 2022-03-30 01:18:39.000000 sqlalchemy-airtable-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-06-19 21:35:44.261893 sqlalchemy-airtable-0.0.1.dev3/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     4252 2023-06-19 21:32:32.000000 sqlalchemy-airtable-0.0.1.dev3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:35:44.257076 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3618 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      585 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      225 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       47 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-06-19 21:35:44.000000 sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-06-19 21:35:44.260590 sqlalchemy-airtable-0.0.1.dev3/tests/
+-rw-r--r--   0 alex       (501) staff       (20)      659 2023-06-19 21:30:46.000000 sqlalchemy-airtable-0.0.1.dev3/tests/test_adapter.py
+-rw-r--r--   0 alex       (501) staff       (20)     4616 2023-06-19 21:30:46.000000 sqlalchemy-airtable-0.0.1.dev3/tests/test_dialect.py
+-rw-r--r--   0 alex       (501) staff       (20)     2895 2022-04-05 05:03:46.000000 sqlalchemy-airtable-0.0.1.dev3/tests/test_fields.py
+-rw-r--r--   0 alex       (501) staff       (20)     2245 2022-04-06 05:38:56.000000 sqlalchemy-airtable-0.0.1.dev3/tests/test_formula.py
+-rw-r--r--   0 alex       (501) staff       (20)      955 2022-04-05 05:03:46.000000 sqlalchemy-airtable-0.0.1.dev3/tests/test_lib.py
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/LICENSE` & `sqlalchemy-airtable-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-airtable-0.0.1.dev2/PKG-INFO` & `sqlalchemy-airtable-0.0.1.dev3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-airtable
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Python DB-API and SQLAlchemy interface for Airtable.
 Home-page: https://github.com/cancan101/airtable-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
-Platform: UNKNOWN
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
 
 # airtable-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-airtable.svg)](https://badge.fury.io/py/sqlalchemy-airtable) ![main workflow](https://github.com/cancan101/airtable-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/airtable-db-api/branch/main/graph/badge.svg?token=S8XR68NZCU)](https://codecov.io/gh/cancan101/airtable-db-api)
+
 A Python DB API 2.0 for Airtable
 
 This module allows you to query Airtable using SQL. It exposes:
+
 - a [Python DB API 2.0](https://peps.python.org/pep-0249/) (per PEP 249)
 - a [SQLAlchemy Dialect](https://docs.sqlalchemy.org/en/14/dialects/) (see also ["Developing new Dialects"](https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst))
 - a [Superset Engine Spec](https://preset.io/blog/building-database-connector/)
 
 ## SQLAlchemy support
+
 This module provides a SQLAlchemy dialect.
 
 ```python
 from sqlalchemy.engine import create_engine
 
 engine = create_engine(
     'airtable://:keyXXXX@appYYY?peek_rows=10&tables=tableA&tables=tableB',
     date_columns={"tableA": ["My Date Field"]},
 )
 ```
 
 ## Metadata
+
 At various points we need to know:
-1) The list of Tables supported in the Base
-2) The list of columns (Fields) supported on a given Table
-3) The type information for each Field
+
+1. The list of Tables supported in the Base
+2. The list of columns (Fields) supported on a given Table
+3. The type information for each Field
 
 As of now we solve 1) by passing in a list of Tables using the `tables` query parameter on the URL.
 We solve 2) and 3) using some combination of the `peek_rows` query parameter specifying the number of rows to fetch from Airtable to guess Field types and a `date_columns` engine parameter to specify which columns should be parsed as `Date`s.
 
 Alternatively, 1-3 could all be solved with a comprehensive `base_metadata` engine parameter that specifies the Tables and Fields. There are a number of ways to generate this, but one approach is scraping the Base's API docs page using [a technique like this](https://github.com/aivantg/airtable-schema-generator/issues/47#issue-1165801153).
 
 Further options are [documented here](https://github.com/cancan101/airtable-db-api/wiki/Metadata)
 
-## Installation
-I was having issues with `apsw-3.9.2.post1` (the newest version of `apsw` that would install for me from PyPI) and ended up needing to follow [the instructions here](https://shillelagh.readthedocs.io/en/latest/install.html) to build / install `apsw` from source. There is an [open ticket on the APSW project](https://github.com/rogerbinns/apsw/issues/310) to provide newer wheels. The issue might be triggered if the table name needs escaping and the error looked like:
-```
-SystemError: <method 'execute' of 'apsw.Cursor' objects> returned NULL without setting an exception
-```
-
 ## Development
+
 ### Python
+
 ```bash
 $ pip install -r requirements-dev.txt
 ```
 
 ### `pre-commit`
+
 ```bash
 $ pre-commit install
 ```
 
 ### `black`
+
 Can be run manually as:
+
 ```bash
 black --target-version py37
 ```
 
 ## Roadmap
-* [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
-* [ ] Support passed in Airtable Metadata (w/ types)
-* [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
-* [ ] Built in Metadata scraper (not using Metadata API)
-* [ ] Caching of field type "peeking"
-* [ ] Datetime support
-
 
+- [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
+- [ ] Support passed in Airtable Metadata (w/ types)
+- [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
+- [ ] Built in Metadata scraper (not using Metadata API)
+- [ ] Caching of field type "peeking"
+- [ ] Datetime support
+- [ ] More comprehensive testing
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/README.md` & `sqlalchemy-airtable-0.0.1.dev3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 # airtable-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-airtable.svg)](https://badge.fury.io/py/sqlalchemy-airtable) ![main workflow](https://github.com/cancan101/airtable-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/airtable-db-api/branch/main/graph/badge.svg?token=S8XR68NZCU)](https://codecov.io/gh/cancan101/airtable-db-api)
+
 A Python DB API 2.0 for Airtable
 
 This module allows you to query Airtable using SQL. It exposes:
+
 - a [Python DB API 2.0](https://peps.python.org/pep-0249/) (per PEP 249)
 - a [SQLAlchemy Dialect](https://docs.sqlalchemy.org/en/14/dialects/) (see also ["Developing new Dialects"](https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst))
 - a [Superset Engine Spec](https://preset.io/blog/building-database-connector/)
 
 ## SQLAlchemy support
+
 This module provides a SQLAlchemy dialect.
 
 ```python
 from sqlalchemy.engine import create_engine
 
 engine = create_engine(
     'airtable://:keyXXXX@appYYY?peek_rows=10&tables=tableA&tables=tableB',
     date_columns={"tableA": ["My Date Field"]},
 )
 ```
 
 ## Metadata
+
 At various points we need to know:
-1) The list of Tables supported in the Base
-2) The list of columns (Fields) supported on a given Table
-3) The type information for each Field
+
+1. The list of Tables supported in the Base
+2. The list of columns (Fields) supported on a given Table
+3. The type information for each Field
 
 As of now we solve 1) by passing in a list of Tables using the `tables` query parameter on the URL.
 We solve 2) and 3) using some combination of the `peek_rows` query parameter specifying the number of rows to fetch from Airtable to guess Field types and a `date_columns` engine parameter to specify which columns should be parsed as `Date`s.
 
 Alternatively, 1-3 could all be solved with a comprehensive `base_metadata` engine parameter that specifies the Tables and Fields. There are a number of ways to generate this, but one approach is scraping the Base's API docs page using [a technique like this](https://github.com/aivantg/airtable-schema-generator/issues/47#issue-1165801153).
 
 Further options are [documented here](https://github.com/cancan101/airtable-db-api/wiki/Metadata)
 
-## Installation
-I was having issues with `apsw-3.9.2.post1` (the newest version of `apsw` that would install for me from PyPI) and ended up needing to follow [the instructions here](https://shillelagh.readthedocs.io/en/latest/install.html) to build / install `apsw` from source. There is an [open ticket on the APSW project](https://github.com/rogerbinns/apsw/issues/310) to provide newer wheels. The issue might be triggered if the table name needs escaping and the error looked like:
-```
-SystemError: <method 'execute' of 'apsw.Cursor' objects> returned NULL without setting an exception
-```
-
 ## Development
+
 ### Python
+
 ```bash
 $ pip install -r requirements-dev.txt
 ```
 
 ### `pre-commit`
+
 ```bash
 $ pre-commit install
 ```
 
 ### `black`
+
 Can be run manually as:
+
 ```bash
 black --target-version py37
 ```
 
 ## Roadmap
-* [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
-* [ ] Support passed in Airtable Metadata (w/ types)
-* [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
-* [ ] Built in Metadata scraper (not using Metadata API)
-* [ ] Caching of field type "peeking"
-* [ ] Datetime support
+
+- [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
+- [ ] Support passed in Airtable Metadata (w/ types)
+- [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
+- [ ] Built in Metadata scraper (not using Metadata API)
+- [ ] Caching of field type "peeking"
+- [ ] Datetime support
+- [ ] More comprehensive testing
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/adapter.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,23 @@
     Tuple,
     Type,
 )
 
 from pyairtable import Table
 from shillelagh.adapters.base import Adapter
 from shillelagh.fields import Field, ISODate, ISODateTime, Order, String
-from shillelagh.filters import Equal, Filter, IsNotNull, IsNull, NotEqual, Range
+from shillelagh.filters import (
+    Equal,
+    Filter,
+    IsNotNull,
+    IsNull,
+    NotEqual,
+    Operator,
+    Range,
+)
 from shillelagh.typing import RequestedOrder
 
 from .fields import MaybeList, MaybeListString
 from .formulas import get_airtable_formula
 from .lib import FieldInfo, guess_field
 from .types import BaseMetadata, TableMetadata, TypedDict
 
@@ -29,15 +37,15 @@
     order: Order
     exact: bool
     filters: List[Type[Filter]]
 
 
 FIELD_KWARGS: FieldKwargs = {
     "order": Order.ANY,
-    "filters": [IsNull, IsNotNull, Range, Equal, NotEqual],
+    "filters": [IsNull, IsNotNull, Equal, NotEqual, Range],
     "exact": True,
 }
 
 
 def get_airtable_sort(order: List[Tuple[str, RequestedOrder]]) -> List[str]:
     return [(s if o is Order.ASCENDING else f"-{s}") for s, o in order]
 
@@ -54,14 +62,15 @@
         for table_value in base_metadata.values()
         if table_value["name"] == table_name
     ][0]
 
 
 class AirtableAdapter(Adapter):
     safe = True
+    supports_limit = True
 
     def __init__(
         self,
         table: str,
         base_id: str,
         api_key: str,
         base_metadata: Optional[BaseMetadata],
@@ -137,15 +146,17 @@
         # Right now I don't know how to sort on the backend:
         # https://community.airtable.com/t/sort-on-rest-api-by-createdtime-without-adding-new-column/
         # TODO(cancan101): implement filtering for id + createdTime
         # using special formula.
         # See:
         # https://support.airtable.com/hc/en-us/articles/360051564873-Record-ID
         # https://support.airtable.com/hc/en-us/articles/203255215-Formula-field-reference#record_functions
-        self.columns = dict(columns, id=String(), createdTime=ISODateTime())
+        self.columns = dict(
+            columns, id=String(filters=[Equal], exact=True), createdTime=ISODateTime()
+        )
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         # TODO the slow path here could connect to the Airtable API
         return True
 
     @staticmethod
@@ -155,27 +166,52 @@
     def get_columns(self) -> Dict[str, Field]:
         return self.columns
 
     def get_data(
         self,
         bounds: Dict[str, Filter],
         order: List[Tuple[str, RequestedOrder]],
+        limit: Optional[int] = None,
+        **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
         sort = get_airtable_sort(order)
 
         if bounds:
             formula = get_airtable_formula(bounds)
         else:
             formula = None
 
+        options = {}
+        if limit is not None:
+            options["max_records"] = limit
+
         # Pass fields here
-        for page in self._table_api.iterate(sort=sort, formula=formula):
+        for page in self._table_api.iterate(sort=sort, formula=formula, **options):
             for result in page:
                 yield dict(
                     {
                         k: v
                         for k, v in result["fields"].items()
                         if self.strict_col or k in self.columns
                     },
                     id=result["id"],
                     createdTime=result["createdTime"],
                 )
+
+    def get_cost(
+        self,
+        filtered_columns: List[Tuple[str, Operator]],
+        order: List[Tuple[str, RequestedOrder]],
+    ) -> float:
+        # Most of the cost here will come from network fetching / overhead
+
+        if ("id", Operator.EQ) in filtered_columns:
+            # We assume if it's = id, then there will be 0/1 result
+            return 100
+        elif any(operator is Operator.EQ for field_name, operator in filtered_columns):
+            # We assume if it's = something else, it might be 0/1 or it might be more
+            return 110
+        elif len(filtered_columns) > 0:
+            # Give some benefit for reduced data to fetch
+            return 150
+        else:
+            return 200
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/db_engine_specs.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/dialect.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/dialect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,30 @@
+from __future__ import annotations
+
 import urllib.parse
-from typing import Any, Collection, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Collection,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from shillelagh.backends.apsw.dialects.base import APSWDialect
-from sqlalchemy.engine import Connection
-from sqlalchemy.engine.url import URL
 
 from .types import BaseMetadata
 
+if TYPE_CHECKING:
+    from sqlalchemy.engine import Connection
+    from sqlalchemy.engine.url import URL
+
 # -----------------------------------------------------------------------------
 
 ADAPTER_NAME = "airtable"
 
 # -----------------------------------------------------------------------------
 
 
@@ -36,29 +50,29 @@
 
 
 class APSWAirtableDialect(APSWDialect):
     supports_statement_cache = True
 
     def __init__(
         self,
-        airtable_api_key: str = None,
-        base_metadata: BaseMetadata = None,
+        airtable_api_key: Optional[str] = None,
+        base_metadata: Optional[BaseMetadata] = None,
         # Ick:
-        date_columns: Dict[str, Collection[str]] = None,
+        date_columns: Optional[Dict[str, Collection[str]]] = None,
         **kwargs: Any,
     ):
         # We tell Shillelagh that this dialect supports just one adapter
         super().__init__(safe=True, adapters=[ADAPTER_NAME], **kwargs)
 
         self.airtable_api_key = airtable_api_key
         self.base_metadata = base_metadata
         self.date_columns = date_columns
 
     def get_table_names(
-        self, connection: Connection, schema: str = None, **kwargs: Any
+        self, connection: Connection, schema: Optional[str] = None, **kwargs: Any
     ) -> List[str]:
         url_query, _ = extract_query_host(connection.engine.url)
         tables = url_query.get("tables")
 
         if tables is not None:
             if isinstance(tables, str):
                 tables = [tables]
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/fields.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/fields.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/formulas.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/formulas.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 from pyairtable import formulas as base_formulas
 from shillelagh.filters import Equal, Filter, IsNotNull, IsNull, NotEqual, Range
 
 BLANK = "BLANK()"
 TRUE = "TRUE()"
 FALSE = "FALSE()"
+RECORD_ID = "RECORD_ID()"
+
+ID_FIELD = "id"
 
 
 def AND_BETTER(*args):
     if len(args) == 1:
         return args[0]
     return base_formulas.AND(*args)
 
@@ -41,37 +44,59 @@
 
 
 def STR_CAST(left: Any) -> str:
     return '{} & ""'.format(left)
 
 
 def get_formula(field_name: str, filter: Filter) -> str:
-    if isinstance(filter, IsNull):
+    if field_name == ID_FIELD:
+        if not isinstance(filter, Equal):
+            raise NotImplementedError(field_name, filter)
+
+        return base_formulas.EQUAL(
+            RECORD_ID,
+            base_formulas.to_airtable_value(filter.value),
+        )
+    elif isinstance(filter, IsNull):
         # https://community.airtable.com/t/blank-zero-problem/5662/13
         return base_formulas.IF(STR_CAST(base_formulas.FIELD(field_name)), FALSE, TRUE)
     elif isinstance(filter, IsNotNull):
         # https://community.airtable.com/t/blank-zero-problem/5662/13
         return base_formulas.IF(STR_CAST(base_formulas.FIELD(field_name)), TRUE, FALSE)
     elif isinstance(filter, Range):
-        parts = []
-        if filter.start is not None:
-            start_airtable_value = base_formulas.to_airtable_value(filter.start)
-            if filter.include_start:
-                parts.append(GE(base_formulas.FIELD(field_name), start_airtable_value))
-            else:
-                parts.append(GT(base_formulas.FIELD(field_name), start_airtable_value))
-
-        if filter.end is not None:
-            end_airtable_value = base_formulas.to_airtable_value(filter.end)
-            if filter.include_end:
-                parts.append(LE(base_formulas.FIELD(field_name), end_airtable_value))
-            else:
-                parts.append(LT(base_formulas.FIELD(field_name), end_airtable_value))
+        if filter.start == filter.end and filter.include_start and filter.include_end:
+            return base_formulas.EQUAL(
+                base_formulas.FIELD(field_name),
+                base_formulas.to_airtable_value(filter.start),
+            )
+        else:
+            parts = []
+            if filter.start is not None:
+                start_airtable_value = base_formulas.to_airtable_value(filter.start)
+                if filter.include_start:
+                    parts.append(
+                        GE(base_formulas.FIELD(field_name), start_airtable_value)
+                    )
+                else:
+                    parts.append(
+                        GT(base_formulas.FIELD(field_name), start_airtable_value)
+                    )
+
+            if filter.end is not None:
+                end_airtable_value = base_formulas.to_airtable_value(filter.end)
+                if filter.include_end:
+                    parts.append(
+                        LE(base_formulas.FIELD(field_name), end_airtable_value)
+                    )
+                else:
+                    parts.append(
+                        LT(base_formulas.FIELD(field_name), end_airtable_value)
+                    )
 
-        return AND_BETTER(*parts)
+            return AND_BETTER(*parts)
     elif isinstance(filter, Equal):
         return base_formulas.EQUAL(
             base_formulas.FIELD(field_name),
             base_formulas.to_airtable_value(filter.value),
         )
     elif isinstance(filter, NotEqual):
         return NOT_EQUAL(
```

### Comparing `sqlalchemy-airtable-0.0.1.dev2/airtabledb/lib.py` & `sqlalchemy-airtable-0.0.1.dev3/airtabledb/lib.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-airtable-0.0.1.dev2/setup.py` & `sqlalchemy-airtable-0.0.1.dev3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for Airtable."
-VERSION = "0.0.1.dev2"
+VERSION = "0.0.1.dev3"
 
 # -----------------------------------------------------------------------------
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
@@ -25,15 +25,15 @@
 
 class BaseCommand(Command):
     user_options: List[Tuple[str, str, str]] = []
 
     @staticmethod
     def status(s: str) -> None:
         """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(s))  # noqa: T001
+        print("\033[1m{0}\033[0m".format(s))  # noqa: T201
 
     def system(self, command: str) -> None:
         os.system(command)  # noqa: S605
 
     def initialize_options(self):
         pass
 
@@ -111,28 +111,28 @@
         "superset.db_engine_specs": [
             "airtable = airtabledb.db_engine_specs:AirtableEngineSpec"
         ],
     },
     install_requires=(
         "pyairtable",
         "shillelagh >= 1.0.6",
-        "sqlalchemy >= 1.3.0",
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

### Comparing `sqlalchemy-airtable-0.0.1.dev2/sqlalchemy_airtable.egg-info/PKG-INFO` & `sqlalchemy-airtable-0.0.1.dev3/sqlalchemy_airtable.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-airtable
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Python DB-API and SQLAlchemy interface for Airtable.
 Home-page: https://github.com/cancan101/airtable-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
-Platform: UNKNOWN
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
 
 # airtable-db-api [![PyPI version](https://badge.fury.io/py/sqlalchemy-airtable.svg)](https://badge.fury.io/py/sqlalchemy-airtable) ![main workflow](https://github.com/cancan101/airtable-db-api/actions/workflows/main.yml/badge.svg) [![codecov](https://codecov.io/gh/cancan101/airtable-db-api/branch/main/graph/badge.svg?token=S8XR68NZCU)](https://codecov.io/gh/cancan101/airtable-db-api)
+
 A Python DB API 2.0 for Airtable
 
 This module allows you to query Airtable using SQL. It exposes:
+
 - a [Python DB API 2.0](https://peps.python.org/pep-0249/) (per PEP 249)
 - a [SQLAlchemy Dialect](https://docs.sqlalchemy.org/en/14/dialects/) (see also ["Developing new Dialects"](https://github.com/zzzeek/sqlalchemy/blob/master/README.dialects.rst))
 - a [Superset Engine Spec](https://preset.io/blog/building-database-connector/)
 
 ## SQLAlchemy support
+
 This module provides a SQLAlchemy dialect.
 
 ```python
 from sqlalchemy.engine import create_engine
 
 engine = create_engine(
     'airtable://:keyXXXX@appYYY?peek_rows=10&tables=tableA&tables=tableB',
     date_columns={"tableA": ["My Date Field"]},
 )
 ```
 
 ## Metadata
+
 At various points we need to know:
-1) The list of Tables supported in the Base
-2) The list of columns (Fields) supported on a given Table
-3) The type information for each Field
+
+1. The list of Tables supported in the Base
+2. The list of columns (Fields) supported on a given Table
+3. The type information for each Field
 
 As of now we solve 1) by passing in a list of Tables using the `tables` query parameter on the URL.
 We solve 2) and 3) using some combination of the `peek_rows` query parameter specifying the number of rows to fetch from Airtable to guess Field types and a `date_columns` engine parameter to specify which columns should be parsed as `Date`s.
 
 Alternatively, 1-3 could all be solved with a comprehensive `base_metadata` engine parameter that specifies the Tables and Fields. There are a number of ways to generate this, but one approach is scraping the Base's API docs page using [a technique like this](https://github.com/aivantg/airtable-schema-generator/issues/47#issue-1165801153).
 
 Further options are [documented here](https://github.com/cancan101/airtable-db-api/wiki/Metadata)
 
-## Installation
-I was having issues with `apsw-3.9.2.post1` (the newest version of `apsw` that would install for me from PyPI) and ended up needing to follow [the instructions here](https://shillelagh.readthedocs.io/en/latest/install.html) to build / install `apsw` from source. There is an [open ticket on the APSW project](https://github.com/rogerbinns/apsw/issues/310) to provide newer wheels. The issue might be triggered if the table name needs escaping and the error looked like:
-```
-SystemError: <method 'execute' of 'apsw.Cursor' objects> returned NULL without setting an exception
-```
-
 ## Development
+
 ### Python
+
 ```bash
 $ pip install -r requirements-dev.txt
 ```
 
 ### `pre-commit`
+
 ```bash
 $ pre-commit install
 ```
 
 ### `black`
+
 Can be run manually as:
+
 ```bash
 black --target-version py37
 ```
 
 ## Roadmap
-* [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
-* [ ] Support passed in Airtable Metadata (w/ types)
-* [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
-* [ ] Built in Metadata scraper (not using Metadata API)
-* [ ] Caching of field type "peeking"
-* [ ] Datetime support
-
 
+- [ ] Support for [Airtable's Metadata API](https://airtable.com/api/meta)
+- [ ] Support passed in Airtable Metadata (w/ types)
+- [ ] Cleanup configuration (passed as [query param on URL](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls) vs [engine parameters](https://docs.sqlalchemy.org/en/14/core/engines.html#sqlalchemy.create_engine))
+- [ ] Built in Metadata scraper (not using Metadata API)
+- [ ] Caching of field type "peeking"
+- [ ] Datetime support
+- [ ] More comprehensive testing
```

