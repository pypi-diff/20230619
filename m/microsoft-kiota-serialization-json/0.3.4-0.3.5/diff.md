# Comparing `tmp/microsoft_kiota_serialization_json-0.3.4.tar.gz` & `tmp/microsoft_kiota_serialization_json-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_serialization_json-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_serialization_json-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_serialization_json-0.3.4.tar` & `microsoft_kiota_serialization_json-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,41 @@
--rw-r--r--   0        0        0       82 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1870 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.gitignore
--rw-r--r--   0        0        0    15976 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/.pylintrc
--rw-r--r--   0        0        0      978 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/LICENSE
--rw-r--r--   0        0        0      350 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/Pipfile
--rw-r--r--   0        0        0    35819 2023-05-17 11:25:41.033948 microsoft_kiota_serialization_json-0.3.4/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/README.md
--rw-r--r--   0        0        0     2757 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    10696 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1445 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    17554 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1456 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0       94 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1710 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/entity.py
--rw-r--r--   0        0        0      105 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/office_location.py
--rw-r--r--   0        0        0     5687 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/helpers/user.py
--rw-r--r--   0        0        0        0 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/__init__.py
--rw-r--r--   0        0        0     5930 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1747 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     6947 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1101 2023-05-17 11:25:41.037948 microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1874 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.gitignore
+-rw-r--r--   0        0        0    15976 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/.pylintrc
+-rw-r--r--   0        0        0     1126 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1146 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/Pipfile
+-rw-r--r--   0        0        0    71082 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/README.md
+-rw-r--r--   0        0        0     2757 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    11570 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1445 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    16605 2023-06-19 11:00:08.644644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      909 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0      119 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1569 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/entity.py
+-rw-r--r--   0        0        0     2692 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/intersection_type.py
+-rw-r--r--   0        0        0       94 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     3077 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/union_type.py
+-rw-r--r--   0        0        0     3133 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/user.py
+-rw-r--r--   0        0        0     2151 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/helpers/user2.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1554 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/conftest.py
+-rw-r--r--   0        0        0     5236 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_intersection_wrapper.py
+-rw-r--r--   0        0        0     4123 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1686 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     7188 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1018 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     5873 2023-06-19 11:00:08.648644 microsoft_kiota_serialization_json-0.3.5/tests/unit/test_union_wrapper.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft_kiota_serialization_json-0.3.5/PKG-INFO
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_serialization_json-0.3.5/.github/workflows/auto-merge-dependabot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.4.0
+        uses: dependabot/fetch-metadata@v1.5.1
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/.github/workflows/build_publish.yml` & `microsoft_kiota_serialization_json-0.3.5/.github/workflows/build_publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 name: Python Serialization JSON
 
 on:
   workflow_dispatch:
   push:
-    branches: [ main ]
+    branches: [main]
   pull_request:
-    branches: [ main, dev ]
+    branches: [main, dev]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
-          pipenv install --dev --skip-lock
+          pipenv install -r requirements-dev.txt
       - name: Check code format
         run: |
           pipenv run yapf -dr kiota_serialization_json
       - name: Check import order
         run: |
           pipenv run isort kiota_serialization_json
       - name: Lint with Pylint
@@ -58,8 +58,8 @@
         run: |
           pip install flit
       - name: Publish the distibution to PyPI
         run: flit publish
         env:
           FLIT_INDEX_URL: https://upload.pypi.org/legacy/
           FLIT_USERNAME: __token__
-          FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
+          FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_serialization_json-0.3.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_serialization_json-0.3.5/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/.gitignore` & `microsoft_kiota_serialization_json-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/.pylintrc` & `microsoft_kiota_serialization_json-0.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/CHANGELOG.md` & `microsoft_kiota_serialization_json-0.3.5/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.3.5] - 2023-06-14
+
+### Added
+
+- Added support for composed types (de)serialization.
+
+### Changed
+
+- Fixed a bug with assigning field values.
+
 ## [0.3.4] - 2023-05-17
 
 ### Added
 
 ### Changed
 
 - Fixed a bug with assigning field values.
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/LICENSE` & `microsoft_kiota_serialization_json-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/README.md` & `microsoft_kiota_serialization_json-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/SECURITY.md` & `microsoft_kiota_serialization_json-0.3.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/SUPPORT.md` & `microsoft_kiota_serialization_json-0.3.5/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node.py` & `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from __future__ import annotations
 
-import base64
 import json
-import re
 import warnings
 from datetime import date, datetime, time, timedelta
 from enum import Enum
-from typing import Any, Callable, Dict, Generic, List, Optional, Type, TypeVar
+from typing import Any, Callable, Dict, Generic, List, Optional, TypeVar, Union
 from uuid import UUID
 
 from dateutil import parser
-from kiota_abstractions.serialization import (
-    AdditionalDataHolder,
-    Parsable,
-    ParsableFactory,
-    ParseNode,
-)
+from kiota_abstractions.serialization import Parsable, ParsableFactory, ParseNode
 
 T = TypeVar("T")
 
 U = TypeVar("U", bound=Parsable)
 
 K = TypeVar("K", bound=Enum)
 
@@ -28,217 +21,205 @@
 
     on_before_assign_field_values: Optional[Callable[[Parsable], None]] = None
     on_after_assign_field_values: Optional[Callable[[Parsable], None]] = None
 
     def __init__(self, node: Any) -> None:
         """
         Args:
-            node (Any):The JsonElement to initialize the node with
+            node (Any): The JsonElement\
+                to initialize the node with
         """
         self._json_node = node
 
-    def get_str_value(self) -> Optional[str]:
-        """Gets the string value from the json node
-        Returns:
-            str: The string value of the node
-        """
-        if self._json_node or self._json_node == '':
-            return str(self._json_node)
-        return None
-
     def get_child_node(self, identifier: str) -> Optional[ParseNode]:
         """Gets a new parse node for the given identifier
         Args:
             identifier (str): The identifier of the current node property
         Returns:
             Optional[ParseNode]: A new parse node for the given identifier
         """
-        if self._json_node and self._json_node.get(identifier):
-            return JsonParseNode(self._json_node[identifier])
+        if not identifier:
+            raise ValueError("identifier cannot be None or empty.")
+
+        if isinstance(node := self._json_node, dict) and identifier in node:
+            return JsonParseNode(node[identifier])
         return None
 
+    def get_str_value(self) -> Optional[str]:
+        """Gets the string value from the json node
+        Returns:
+            str: The string value of the node
+        """
+        return self._json_node if isinstance(self._json_node, str) else None
+
     def get_bool_value(self) -> Optional[bool]:
         """Gets the boolean value of the json node
         Returns:
             bool: The boolean value of the node
         """
-        if self._json_node or self._json_node is False:
-            return bool(self._json_node)
-        return None
+        return self._json_node if isinstance(self._json_node, bool) else None
 
     def get_int_value(self) -> Optional[int]:
         """Gets the integer value of the json node
         Returns:
             int: The integer value of the node
         """
-        if self._json_node:
-            return int(self._json_node)
-        return None
+        return self._json_node if isinstance(self._json_node, int) else None
 
     def get_float_value(self) -> Optional[float]:
         """Gets the float value of the json node
         Returns:
             float: The integer value of the node
         """
-        if self._json_node:
-            return float(self._json_node)
-        return None
+        return self._json_node if isinstance(self._json_node, float) else None
 
     def get_uuid_value(self) -> Optional[UUID]:
         """Gets the UUID value of the json node
         Returns:
             UUID: The GUID value of the node
         """
-        if self._json_node:
+        if isinstance(self._json_node, UUID):
+            return self._json_node
+        if isinstance(self._json_node, str):
             return UUID(self._json_node)
         return None
 
     def get_datetime_value(self) -> Optional[datetime]:
         """Gets the datetime value of the json node
         Returns:
             datetime: The datetime value of the node
         """
-        datetime_str = self.get_str_value()
-        if datetime_str:
-            datetime_obj = parser.parse(datetime_str)
-            return datetime_obj
+        if isinstance(self._json_node, datetime):
+            return self._json_node
+        if isinstance(self._json_node, str):
+            return parser.parse(self._json_node)
         return None
 
     def get_timedelta_value(self) -> Optional[timedelta]:
         """Gets the timedelta value of the node
         Returns:
             timedelta: The timedelta value of the node
         """
-        datetime_str = self.get_str_value()
-        if datetime_str:
-            datetime_obj = parser.parse(datetime_str)
+        if isinstance(self._json_node, timedelta):
+            return self._json_node
+        if isinstance(self._json_node, str):
+            datetime_obj = parser.parse(self._json_node)
             return timedelta(
                 hours=datetime_obj.hour, minutes=datetime_obj.minute, seconds=datetime_obj.second
             )
         return None
 
     def get_date_value(self) -> Optional[date]:
         """Gets the date value of the node
         Returns:
             date: The datevalue of the node in terms on year, month, and day.
         """
-        datetime_str = self.get_str_value()
-        if datetime_str:
-            datetime_obj = parser.parse(datetime_str)
+        if isinstance(self._json_node, date):
+            return self._json_node
+        if isinstance(self._json_node, str):
+            datetime_obj = parser.parse(self._json_node)
             return datetime_obj.date()
         return None
 
     def get_time_value(self) -> Optional[time]:
         """Gets the time value of the node
         Returns:
             time: The time value of the node in terms of hour, minute, and second.
         """
-        datetime_str = self.get_str_value()
-        if datetime_str:
-            datetime_obj = parser.parse(datetime_str)
+        if isinstance(self._json_node, time):
+            return self._json_node
+        if isinstance(self._json_node, str):
+            datetime_obj = parser.parse(self._json_node)
             return datetime_obj.time()
         return None
 
-    def get_collection_of_primitive_values(self, primitive_type) -> Optional[List[T]]:
+    def get_collection_of_primitive_values(self, primitive_type: Any) -> Optional[List[T]]:
         """Gets the collection of primitive values of the node
         Returns:
             List[T]: The collection of primitive values
         """
 
+        primitive_types = {bool, str, int, float, UUID, datetime, timedelta, date, time, bytes}
+
         def func(item):
-            generic_type = type(item)
+            generic_type = primitive_type if primitive_type else type(item)
             current_parse_node = JsonParseNode(item)
-            if generic_type == bool:
-                return current_parse_node.get_bool_value()
-            if generic_type == str:
-                return current_parse_node.get_str_value()
-            if generic_type == int:
-                return current_parse_node.get_int_value()
-            if generic_type == float:
-                return current_parse_node.get_float_value()
-            if generic_type == UUID:
-                return current_parse_node.get_uuid_value()
-            if generic_type == datetime:
-                return current_parse_node.get_datetime_value()
-            if generic_type == timedelta:
-                return current_parse_node.get_timedelta_value()
-            if generic_type == date:
-                return current_parse_node.get_time_value()
-            if generic_type == time:
-                return current_parse_node.get_time_value()
+            if generic_type in primitive_types:
+                method = getattr(current_parse_node, f'get_{generic_type.__name__.lower()}_value')
+                return method()
             raise Exception(f"Encountered an unknown type during deserialization {generic_type}")
 
         if isinstance(self._json_node, str):
             return list(map(func, json.loads(self._json_node)))
         return list(map(func, list(self._json_node)))
 
     def get_collection_of_object_values(self, factory: ParsableFactory) -> List[U]:
         """Gets the collection of type U values from the json node
         Returns:
             List[U]: The collection of model object values of the node
         """
-        object_collection = self._json_node
-        if not object_collection:
-            return []
-        return list(
-            map(
-                lambda x: JsonParseNode(x).get_object_value(factory),  # type: ignore
-                object_collection
+        if isinstance(self._json_node, list):
+            return list(
+                map(
+                    lambda x: JsonParseNode(x).get_object_value(factory),  # type: ignore
+                    self._json_node,
+                )
             )
-        )
+        return []
 
     def get_collection_of_enum_values(self, enum_class: K) -> List[Optional[K]]:
         """Gets the collection of enum values of the json node
         Returns:
             List[K]: The collection of enum values
         """
-        enum_collection = self._json_node
-        if not enum_collection:
-            return []
-        return list(map(lambda x: JsonParseNode(x).get_enum_value(enum_class), enum_collection))
+        if isinstance(self._json_node, list):
+            return list(map(lambda x: JsonParseNode(x).get_enum_value(enum_class), self._json_node))
+        return []
 
     def get_enum_value(self, enum_class: K) -> Optional[K]:
         """Gets the enum value of the node
         Returns:
             Optional[K]: The enum value of the node
         """
-        raw_key = self.get_str_value()
+        raw_key = str(self._json_node)
+        if not raw_key:
+            return None
+
         camel_case_key = None
-        if raw_key:
-            if raw_key.lower() == "none":
-                # None is a reserved keyword in python
-                camel_case_key = "None_"
-            else:
-                camel_case_key = raw_key[0].upper() + raw_key[1:]
-        if camel_case_key:
-            try:
-                return enum_class[camel_case_key]  # type: ignore
-            except KeyError:
-                raise Exception(f'Invalid key: {camel_case_key} for enum {enum_class}.')
-        return None
+        if raw_key.lower() == "none":
+            # None is a reserved keyword in python
+            camel_case_key = "None_"
+        else:
+            camel_case_key = raw_key[0].upper() + raw_key[1:]
+
+        try:
+            return enum_class[camel_case_key]  # type: ignore
+        except KeyError:
+            raise Exception(f'Invalid key: {camel_case_key} for enum {enum_class}.')
 
     def get_object_value(self, factory: ParsableFactory) -> U:
         """Gets the model object value of the node
         Returns:
             Parsable: The model object value of the node
         """
+
         result = factory.create_from_discriminator_value(self)
         if self.on_before_assign_field_values:
             self.on_before_assign_field_values(result)
         self._assign_field_values(result)
         if self.on_after_assign_field_values:
             self.on_after_assign_field_values(result)
         return result
 
     def get_bytes_value(self) -> Optional[bytes]:
         """Get a bytearray value from the nodes
         Returns:
             bytearray: The bytearray value from the nodes
         """
-        base64_string = self.get_str_value()
+        base64_string = str(self._json_node)
         if not base64_string:
             return None
         return base64_string.encode("utf-8")
 
     def get_on_before_assign_field_values(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called before the node is deserialized.
         Returns:
@@ -266,35 +247,62 @@
         Args:
             value (Callable[[Parsable], None]): the callback called after the node is
             deserialized.
         """
         self.on_after_assign_field_values = value
 
     def _assign_field_values(self, item: U) -> None:
-
-        object_dict = self._json_node
-
-        item_additional_data = None
+        """Assigns the field values to the model object"""
 
         # if object is null
-        if not object_dict:
+        if not isinstance(self._json_node, dict):
             return
 
-        if isinstance(object_dict, str):
-            object_dict = json.loads(object_dict)
-
-        if isinstance(item, AdditionalDataHolder):
+        item_additional_data = None
+        if not hasattr(item, "additional_data") or item.additional_data is None:
+            item_additional_data = {}
+        else:
             item_additional_data = item.additional_data
 
         field_deserializers = item.get_field_deserializers()
 
-        for key, val in object_dict.items():
-            deserializer = field_deserializers.get(key)
-            if deserializer:
-                deserializer(JsonParseNode(val))
+        for field_name, field_value in self._json_node.items():
+            if field_name in field_deserializers:
+                if field_value is None:
+                    continue
+                field_deserializer = field_deserializers[field_name]
+                field_deserializer(JsonParseNode(field_value))
             elif item_additional_data is not None:
-                item_additional_data[key] = val
+                item_additional_data[field_name] = self.try_get_anything(field_value)
             else:
                 warnings.warn(
-                    f"Found additional property {key} to \
+                    f"Found additional property {field_name} to \
                     deserialize but the model doesn't support additional data"
                 )
+
+    def try_get_anything(self, value: Any) -> Any:
+        if isinstance(value, (int, float, bool)) or value is None:
+            return value
+        if isinstance(value, list):
+            return list(map(self.try_get_anything, value))
+        if isinstance(value, dict):
+            return dict(map(lambda x: (x[0], self.try_get_anything(x[1])), value.items()))
+        if isinstance(value, str):
+            try:
+                datetime_obj = parser.parse(value)
+                return timedelta(
+                    hours=datetime_obj.hour,
+                    minutes=datetime_obj.minute,
+                    seconds=datetime_obj.second
+                )
+            except ValueError:
+                pass
+            try:
+                return parser.parse(value)
+            except ValueError:
+                pass
+            try:
+                return UUID(value)
+            except ValueError:
+                pass
+            return value
+        raise ValueError(f"Unexpected additional value type {type(value)} during deserialization.")
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import base64
 import json
 from datetime import date, datetime, time, timedelta
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 from uuid import UUID
 
@@ -17,258 +19,281 @@
 
     _on_start_object_serialization: Optional[Callable[[Parsable, SerializationWriter], None]] = None
 
     _on_before_object_serialization: Optional[Callable[[Parsable], None]] = None
 
     _on_after_object_serialization: Optional[Callable[[Parsable], None]] = None
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.writer: Dict = {}
+        self.value: Any = None
 
-    def write_str_value(self, key: Optional[str], value: Optional[str]) -> Optional[str]:
+    def write_str_value(self, key: Optional[str], value: Optional[str]) -> None:
         """Writes the specified string value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[str]): The string value to be written.
         """
-        if key and (value or value == ''):  #keeps empty strings as valid values
-            self.writer[key] = value
-        elif (value or value == '') and not key:
-            return value
-        return None
+        if isinstance(value, str):
+            if key:
+                self.writer[key] = value
+            else:
+                self.value = value
 
-    def write_bool_value(self, key: Optional[str], value: Optional[bool]) -> Optional[bool]:
+    def write_bool_value(self, key: Optional[str], value: Optional[bool]) -> None:
         """Writes the specified boolean value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[bool]): The boolean value to be written.
         """
-        if key and (value or value is False):  # Escape False value from null check
-            self.writer[key] = value
-        elif (value or value is False) and not key:
-            return value
-        return None
+        if isinstance(value, bool):
+            if key:
+                self.writer[key] = value
+            else:
+                self.value = value
 
-    def write_int_value(self, key: Optional[str], value: Optional[int]) -> Optional[int]:
+    def write_int_value(self, key: Optional[str], value: Optional[int]) -> None:
         """Writes the specified integer value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[int]): The integer value to be written.
         """
-        if key and value:
-            self.writer[key] = value
-        elif value and not key:
-            return value
-        return None
+        if isinstance(value, int):
+            if key:
+                self.writer[key] = value
+            else:
+                self.value = value
 
-    def write_float_value(self, key: Optional[str], value: Optional[float]) -> Optional[float]:
+    def write_float_value(self, key: Optional[str], value: Optional[float]) -> None:
         """Writes the specified float value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[float]): The float value to be written.
         """
-        if key and value:
-            self.writer[key] = value
-        elif value and not key:
-            return value
-        return None
+        if isinstance(value, float):
+            if key:
+                self.writer[key] = value
+            else:
+                self.value = value
 
-    def write_uuid_value(self, key: Optional[str], value: Optional[UUID]) -> Optional[str]:
+    def write_uuid_value(self, key: Optional[str], value: Optional[UUID]) -> None:
         """Writes the specified uuid value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[UUId]): The uuid value to be written.
         """
-        if key and value:
-            self.writer[key] = str(value)
-        elif value and not key:
-            return str(value)
-        return None
+        if isinstance(value, UUID):
+            if key:
+                self.writer[key] = str(value)
+            else:
+                self.value = str(value)
 
-    def write_datetime_value(self, key: Optional[str], value: Optional[datetime]) -> Optional[str]:
+    def write_datetime_value(self, key: Optional[str], value: Optional[datetime]) -> None:
         """Writes the specified datetime offset value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[datetime]): The datetime offset value to be written.
         """
-        if key and value:
-            self.writer[key] = str(value.isoformat())
-        elif value and not key:
-            return str(value.isoformat())
-        return None
+        if isinstance(value, datetime):
+            if key:
+                self.writer[key] = str(value.isoformat())
+            else:
+                self.value = str(value.isoformat())
 
-    def write_timedelta_value(self, key: Optional[str],
-                              value: Optional[timedelta]) -> Optional[str]:
+    def write_timedelta_value(self, key: Optional[str], value: Optional[timedelta]) -> None:
         """Writes the specified timedelta value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[timedelta]): The timedelta value to be written.
         """
-        if key and value:
-            self.writer[key] = str(value)
-        elif value and not key:
-            return str(value)
-        return None
+        if isinstance(value, timedelta):
+            if key:
+                self.writer[key] = str(value)
+            else:
+                self.value = str(value)
 
-    def write_date_value(self, key: Optional[str], value: Optional[date]) -> Optional[str]:
+    def write_date_value(self, key: Optional[str], value: Optional[date]) -> None:
         """Writes the specified date value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[date]): The date value to be written.
         """
-        if key and value:
-            self.writer[key] = str(value)
-        elif value and not key:
-            return str(value)
-        return None
+        if isinstance(value, date):
+            if key:
+                self.writer[key] = str(value)
+            else:
+                self.value = str(value)
 
-    def write_time_value(self, key: Optional[str], value: Optional[time]) -> Optional[str]:
+    def write_time_value(self, key: Optional[str], value: Optional[time]) -> None:
         """Writes the specified time value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[time]): The time value to be written.
         """
-        if key and value:
-            self.writer[key] = str(value)
-        elif value and not key:
-            return str(value)
-        return None
+        if isinstance(value, time):
+            if key:
+                self.writer[key] = str(value)
+            else:
+                self.value = str(value)
 
-    def write_collection_of_primitive_values(self, key: Optional[str],
-                                             values: Optional[List[T]]) -> Optional[List[T]]:
+    def write_collection_of_primitive_values(
+        self, key: Optional[str], values: Optional[List[T]]
+    ) -> None:
         """Writes the specified collection of primitive values to the stream with an optional
         given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values (Optional[List[T]]): The collection of primitive values to be written.
         """
-        if key and (values or values == []):  # Empty list is meaningful
-            self.writer[key] = list(map(lambda x: self.write_any_value(None, x), values))
-        elif (values or values == []) and not key:
-            return list(map(lambda x: self.write_any_value(None, x), values))
-        return None
+        if isinstance(values, list):
+            result = []
+            for val in values:
+                temp_writer = JsonSerializationWriter()
+                temp_writer.write_any_value(None, val)
+                result.append(temp_writer.value)
+
+            if key:
+                self.writer[key] = result
+            else:
+                self.value = result
 
     def write_collection_of_object_values(
         self, key: Optional[str], values: Optional[List[U]]
-    ) -> Optional[List[Optional[Dict]]]:
+    ) -> None:
         """Writes the specified collection of model objects to the stream with an optional
         given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values (Optional[List[U]]): The collection of model objects to be written.
         """
-        if key and (values or values == []):
-            obj_list = list(map(lambda x: self.write_object_value(None, x), values))  # type: ignore
-            if obj_list != [None]:
+        if isinstance(values, list):
+            obj_list = []
+            for val in values:
+                temp_writer = JsonSerializationWriter()
+                temp_writer.write_object_value(None, val)
+                obj_list.append(temp_writer.value)
+
+            if key:
                 self.writer[key] = obj_list
-        elif (values or values == []) and not key:
-            obj_list = list(map(lambda x: self.write_object_value(None, x), values))  # type: ignore
-            if obj_list != [None]:
-                return obj_list
-        return None
+            else:
+                self.value = obj_list
 
-    def write_collection_of_enum_values(self, key: Optional[str],
-                                        values: Optional[List[Enum]]) -> Optional[str]:
+    def write_collection_of_enum_values(
+        self, key: Optional[str], values: Optional[List[Enum]]
+    ) -> None:
         """Writes the specified collection of enum values to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             values Optional[List[Enum]): The enum values to be written.
         """
-        if key and (values or values == []):
-            self.writer[key] = ','.join(
-                list(map(lambda x: self.write_enum_value(None, x), values))  # type: ignore
-            )
-        elif (values or values == []) and key:
-            return ','.join(
-                list(map(lambda x: self.write_enum_value(None, x), values))  # type: ignore
-            )
-        return None
+        if isinstance(values, list):
+            result = []
+            for val in values:
+                temp_writer = JsonSerializationWriter()
+                temp_writer.write_enum_value(None, val)
+                result.append(temp_writer.value)
+
+            if key:
+                self.writer[key] = result
+            else:
+                self.value = result
 
-    def write_bytes_value(self, key: Optional[str], value: bytes) -> Optional[str]:
+    def write_bytes_value(self, key: Optional[str], value: bytes) -> None:
         """Writes the specified byte array as a base64 string to the stream with an optional
         given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (bytes): The byte array to be written.
         """
-        if key and value:
+        if isinstance(value, bytes):
             base64_bytes = base64.b64encode(value)
             base64_string = base64_bytes.decode('utf-8')
-            self.writer['key'] = base64_string
-        elif value and not key:
-            base64_bytes = base64.b64encode(value)
-            base64_string = base64_bytes.decode('utf-8')
-            return base64_string
-        return None
+            if key:
+                self.writer['key'] = base64_string
+            else:
+                self.value = base64_string
 
-    def write_object_value(self, key: Optional[str],
-                           value: Optional[U]) -> Optional[Dict[Any, Any]]:
+    def write_object_value(
+        self, key: Optional[str], value: Optional[U], *additional_values_to_merge: U
+    ) -> None:
         """Writes the specified model object to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Parsable): The model object to be written.
+            additional_values_to_merge (tuple[Parsable]): The additional values to merge to the
+            main value when serializing an intersection wrapper.
         """
-        if key and value:
-            if self._on_before_object_serialization:
-                self._on_before_object_serialization(value)
-            if self._on_start_object_serialization:
-                self._on_start_object_serialization(value, self)
+        if value or additional_values_to_merge:
             temp_writer = JsonSerializationWriter()
-            value.serialize(temp_writer)
-            if self._on_after_object_serialization:
-                self._on_after_object_serialization(value)
-            self.writer[key] = temp_writer.writer
-        elif value and not key:
-            if self._on_before_object_serialization:
-                self._on_before_object_serialization(value)
-            if self._on_start_object_serialization:
-                self._on_start_object_serialization(value, self)
-            temp_writer = JsonSerializationWriter()
-            value.serialize(temp_writer)
-            if self._on_after_object_serialization:
+
+            if value:
+                self._serialize_value(temp_writer, value)
+
+            if additional_values_to_merge:
+                for additional_value in filter(lambda x: x is not None, additional_values_to_merge):
+                    self._serialize_value(temp_writer, additional_value)
+                    if self._on_after_object_serialization:
+                        self._on_after_object_serialization(additional_value)
+
+            if value and self._on_after_object_serialization:
                 self._on_after_object_serialization(value)
-            return temp_writer.writer
-        return None
 
-    def write_enum_value(self, key: Optional[str], value: Optional[Enum]) -> Optional[str]:
+            if key:
+                self.writer[key] = temp_writer.writer
+            else:
+                self.value = temp_writer.writer
+
+    def write_enum_value(self, key: Optional[str], value: Optional[Enum]) -> None:
         """Writes the specified enum value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (Optional[Enum]): The enum value to be written.
         """
-        if key and value:
-            self.writer[key] = value.name
-        elif value and not key:
-            return value.name
-        return None
+        if isinstance(value, Enum):
+            if key:
+                self.writer[key] = value.value
+            else:
+                self.value = value.value
 
     def write_null_value(self, key: Optional[str]) -> None:
         """Writes a null value for the specified key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
         """
         if key:
             self.writer[key] = None
+        else:
+            self.value = "null"
 
     def write_additional_data_value(self, value: Dict[str, Any]) -> None:
         """Writes the specified additional data to the stream.
         Args:
             value (Dict[str, Any]): he additional data to be written.
         """
-        if value:
+        if isinstance(value, dict):
             for key, val in value.items():
                 self.writer[key] = val
 
     def get_serialized_content(self) -> bytes:
         """Gets the value of the serialized content.
         Returns:
             bytes: The value of the serialized content.
         """
-        json_string = json.dumps(self.writer)
-        self.writer.clear()
+        if self.writer and self.value is not None:
+            # Json output is invalid if it has a mix of values
+            # and key-value pairs.
+            raise ValueError("Invalid Json output")
+
+        if self.value:
+            json_string = json.dumps(self.value)
+            self.value = None
+        else:
+            json_string = json.dumps(self.writer)
+            self.writer.clear()
+
         stream = json_string.encode('utf-8')
         return stream
 
     def get_on_before_object_serialization(self) -> Optional[Callable[[Parsable], None]]:
         """Gets the callback called before the object gets serialized.
         Returns:
             Optional[Callable[[Parsable], None]]:the callback called before the object
@@ -320,82 +345,60 @@
         """Sets the callback called right after the serialization process starts.
         Args:
             value (Optional[Callable[[Parsable, SerializationWriter], None]]): the callback
             called right after the serialization process starts.
         """
         self._on_start_object_serialization = value
 
-    def write_non_parsable_object_value(self, key: Optional[str], value: T) -> Optional[dict]:
+    def write_non_parsable_object_value(self, key: Optional[str], value: T) -> None:
         """Writes the specified value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value (object): The value to be written.
         """
-        if key and value:
-            self.writer[key] = value.__dict__
-        elif value and not key:
-            return value.__dict__
-        return None
+        if hasattr(value, '__dict__'):
+            if key:
+                self.writer[key] = value.__dict__
+            else:
+                self.value = value.__dict__
 
     def write_any_value(self, key: Optional[str], value: Any) -> Any:
         """Writes the specified value to the stream with an optional given key.
         Args:
             key (Optional[str]): The key to be used for the written value. May be null.
             value Any): The value to be written.
         """
-        if key and value:
+        primitive_types = [bool, str, int, float, UUID, datetime, timedelta, date, time, Enum]
+        if value:
             value_type = type(value)
-            if value_type == bool:
-                self.write_bool_value(key, value)
-            elif value_type == str:
-                self.write_str_value(key, value)
-            elif value_type == int:
-                self.write_int_value(key, value)
-            elif value_type == float:
-                self.write_float_value(key, value)
-            elif value_type == UUID:
-                self.write_uuid_value(key, value)
-            elif value_type == datetime:
-                self.write_datetime_value(key, value)
-            elif value_type == timedelta:
-                self.write_timedelta_value(key, value)
-            elif value_type == date:
-                self.write_date_value(key, value)
-            elif value_type == time:
-                self.write_time_value(key, value)
-            elif isinstance(value, Enum):
-                self.write_enum_value(key, value)
-            elif isinstance(value, Parsable):
-                self.write_object_value(key, value)
-            elif hasattr(value, '__dict__'):
-                self.write_non_parsable_object_value(key, value)
+            if key:
+                if value_type in primitive_types:
+                    method = getattr(self, f'write_{value_type.__name__.lower()}_value')
+                    method(key, value)
+                elif isinstance(value, Parsable):
+                    self.write_object_value(key, value)
+                elif hasattr(value, '__dict__'):
+                    self.write_non_parsable_object_value(key, value)
+                else:
+                    raise TypeError(
+                        f"Encountered an unknown type during serialization {value_type} \
+                            with key {key}"
+                    )
             else:
-                raise Exception(f"Encountered an unknown type during serialization {value_type}")
-
-        elif value and not key:
-            value_type = type(value)
-            if value_type == bool:
-                return self.write_bool_value(None, value)
-            if value_type == str:
-                return self.write_str_value(None, value)
-            if value_type == int:
-                return self.write_int_value(None, value)
-            if value_type == float:
-                return self.write_float_value(None, value)
-            if value_type == UUID:
-                return self.write_uuid_value(None, value)
-            if value_type == datetime:
-                return self.write_datetime_value(None, value)
-            if value_type == timedelta:
-                return self.write_timedelta_value(None, value)
-            if value_type == date:
-                return self.write_date_value(None, value)
-            if value_type == time:
-                return self.write_time_value(None, value)
-            if isinstance(value, Enum):
-                return self.write_enum_value(None, value)
-            if isinstance(value, Parsable):
-                return self.write_object_value(None, value)
-            if hasattr(value, '__dict__'):
-                return self.write_non_parsable_object_value(None, value)
-            raise Exception(f"Encountered an unknown type during serialization {value_type}")
-        return None
+                if value_type in primitive_types:
+                    method = getattr(self, f'write_{value_type.__name__.lower()}_value')
+                    method(None, value)
+                elif isinstance(value, Parsable):
+                    self.write_object_value(None, value)
+                elif hasattr(value, '__dict__'):
+                    self.write_non_parsable_object_value(None, value)
+                else:
+                    raise TypeError(
+                        f"Encountered an unknown type during serialization {value_type}"
+                    )
+
+    def _serialize_value(self, temp_writer: JsonSerializationWriter, value: U):
+        if self._on_before_object_serialization:
+            self._on_before_object_serialization(value)
+        if self._on_start_object_serialization:
+            self._on_start_object_serialization(value, self)
+        value.serialize(temp_writer)
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.5/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/pyproject.toml` & `microsoft_kiota_serialization_json-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_serialization_json-0.3.4/tests/helpers/entity.py` & `microsoft_kiota_serialization_json-0.3.5/tests/helpers/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,20 @@
 from __future__ import annotations
+
+from dataclasses import dataclass
 from typing import Callable, Dict, Optional
+from uuid import UUID
 
-from kiota_abstractions.serialization import (
-    Parsable,
-    ParseNode,
-    SerializationWriter,
-)
-        
-class Entity(Parsable):
+from kiota_abstractions.serialization import Parsable, ParseNode, SerializationWriter
 
-    def __init__(self) -> None:
-        self._id: Optional[str] = None
 
-    @property
-    def id(self):
-        return self._id
-
-    @id.setter
-    def id(self, new_id):
-        self._id = new_id
+@dataclass
+class Entity(Parsable):
 
-    
+    id: Optional[UUID] = None
 
     @staticmethod
     def create_from_discriminator_value(parse_node: Optional[ParseNode] = None) -> Entity:
         """
         Creates a new instance of the appropriate class based on discriminator value
         Args:
             parseNode: The parse node to use to read the discriminator value and create the object
@@ -38,21 +28,19 @@
         """Gets the deserialization information for this object.
 
         Returns:
             Dict[str, Callable[[ParseNode], None]]: The deserialization information for this
             object where each entry is a property key with its deserialization callback.
         """
         return {
-            "id":
-            lambda n: setattr(self, 'id', n.get_uuid_value()),
+            "id": lambda n: setattr(self, 'id', n.get_uuid_value()),
         }
 
     def serialize(self, writer: SerializationWriter) -> None:
         """Writes the objects properties to the current writer.
 
         Args:
             writer (SerializationWriter): The writer to write to.
         """
         if not writer:
             raise ValueError("Writer cannot be undefined")
         writer.write_uuid_value("id", self.id)
-
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_parse_node_factory.py` & `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_parse_node_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 
 import pytest
-from kiota_abstractions.serialization import ParseNodeFactory
 
 from kiota_serialization_json.json_parse_node import JsonParseNode
 from kiota_serialization_json.json_parse_node_factory import JsonParseNodeFactory
 
 
 @pytest.fixture
 def sample_json_string():
@@ -15,14 +14,15 @@
 def test_get_root_parse_node(sample_json_string):
     factory = JsonParseNodeFactory()
     sample_json_string_bytes = sample_json_string.encode('utf-8')
     root = factory.get_root_parse_node('application/json', sample_json_string_bytes)
     assert isinstance(root, JsonParseNode)
     assert str(root.get_bytes_value(), "utf-8") == sample_json_string
 
+
 def test_get_root_parse_node_no_content_type(sample_json_string):
     with pytest.raises(Exception) as e_info:
         factory = JsonParseNodeFactory()
         sample_json_string_bytes = sample_json_string.encode('utf-8')
         root = factory.get_root_parse_node('', sample_json_string_bytes)
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer.py` & `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from uuid import UUID
 
 import pytest
 from dateutil import parser
-from kiota_abstractions.serialization import Parsable, SerializationWriter
 
 from kiota_serialization_json.json_serialization_writer import JsonSerializationWriter
 
-from ..helpers import OfficeLocation, User
+from ..helpers import OfficeLocation, User, User2
 
 
 @pytest.fixture
 def user_1():
     user = User()
-    user.age = 31
+    user.updated_at = parser.parse("2022-01-27T12:59:45.596117")
     user.is_active = True
-    user.display_name = "Jane Doe"
+    user.id = UUID("8f841f30-e6e3-439a-a812-ebd369559c36")
     return user
 
 
 @pytest.fixture
 def user_2():
-    user = User()
+    user = User2()
     user.age = 32
-    user.is_active = False
     user.display_name = "John Doe"
     return user
 
 
 def test_write_str_value():
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_str_value("displayName", "Adele Vance")
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
     assert content_string == '{"displayName": "Adele Vance"}'
 
 
 def test_write_string_value_no_key():
     json_serialization_writer = JsonSerializationWriter()
-    value = json_serialization_writer.write_str_value(None, "Adele Vance")
-    assert value == "Adele Vance"
+    json_serialization_writer.write_str_value(None, "Adele Vance")
+    content = json_serialization_writer.get_serialized_content()
+    content_string = content.decode('utf-8')
+    assert content_string == '"Adele Vance"'
 
 
 def test_write_bool_value():
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_bool_value("isActive", True)
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
@@ -124,41 +124,44 @@
 
 
 def test_write_collection_of_object_values(user_1, user_2):
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_collection_of_object_values("users", [user_1, user_2])
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
-    assert content_string == '{"users": [{"display_name": "Jane Doe", "is_active": true, "age": 31}, {"display_name": "John Doe", "is_active": false, "age": 32}]}'
+    assert content_string == '{"users": [{"id": "8f841f30-e6e3-439a-a812-ebd369559c36", '\
+        '"updated_at": "2022-01-27T12:59:45.596117", "is_active": true}, '\
+        '{"display_name": "John Doe", "age": 32}]}'
 
 
 def test_write_collection_of_enum_values():
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_collection_of_enum_values(
         "officeLocation", [OfficeLocation.Dunhill, OfficeLocation.Oval]
     )
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
-    assert content_string == '{"officeLocation": "Dunhill,Oval"}'
+    assert content_string == '{"officeLocation": ["dunhill", "oval"]}'
 
 
 def test_write_object_value(user_1):
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_object_value("user1", user_1)
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
-    assert content_string == '{"user1": {"display_name": "Jane Doe", "is_active": true, "age": 31}}'
+    assert content_string == '{"user1": {"id": "8f841f30-e6e3-439a-a812-ebd369559c36", '\
+        '"updated_at": "2022-01-27T12:59:45.596117", "is_active": true}}'
 
 
 def test_write_enum_value():
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_enum_value("officeLocation", OfficeLocation.Dunhill)
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
-    assert content_string == '{"officeLocation": "Dunhill"}'
+    assert content_string == '{"officeLocation": "dunhill"}'
 
 
 def test_write_null_value():
     json_serialization_writer = JsonSerializationWriter()
     json_serialization_writer.write_null_value("mobilePhone")
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
@@ -171,8 +174,10 @@
         {
             "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
             "businessPhones": ["+1 205 555 0108"],
         }
     )
     content = json_serialization_writer.get_serialized_content()
     content_string = content.decode('utf-8')
-    assert content_string == '{"@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity", "businessPhones": ["+1 205 555 0108"]}'
+    assert content_string == '{"@odata.context": '\
+        '"https://graph.microsoft.com/v1.0/$metadata#users/$entity", '\
+            '"businessPhones": ["+1 205 555 0108"]}'
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/tests/unit/test_json_serialization_writer_factory.py` & `microsoft_kiota_serialization_json-0.3.5/tests/unit/test_json_serialization_writer_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from kiota_abstractions.serialization import SerializationWriterFactory
 
 from kiota_serialization_json.json_serialization_writer import JsonSerializationWriter
 from kiota_serialization_json.json_serialization_writer_factory import (
     JsonSerializationWriterFactory,
 )
 
 
@@ -12,20 +11,20 @@
     writer = factory.get_serialization_writer('application/json')
     assert isinstance(writer, JsonSerializationWriter)
 
 
 def test_get_serialization_writer_no_content_type():
     with pytest.raises(TypeError) as e_info:
         factory = JsonSerializationWriterFactory()
-        writer = factory.get_serialization_writer('')
+        factory.get_serialization_writer('')
 
 
 def test_get_serialization_writer_unsupported_content_type():
     with pytest.raises(Exception) as e_info:
-        factory = JsonSerializationWriterFactory
-        writer = factory.get_root_parse_node('application/xml')
+        factory = JsonSerializationWriterFactory()
+        factory.get_serialization_writer('application/xml')
 
 
 def test_get_valid_content_type():
     factory = JsonSerializationWriterFactory()
     content_type = factory.get_valid_content_type()
     assert content_type == 'application/json'
```

### Comparing `microsoft_kiota_serialization_json-0.3.4/PKG-INFO` & `microsoft_kiota_serialization_json-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.4
+Version: 0.3.5
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

