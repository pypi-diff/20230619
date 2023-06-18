# Comparing `tmp/mappie-0.0.2.tar.gz` & `tmp/mappie-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappie-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mappie-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mappie-0.0.2.tar` & `mappie-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      672 2023-06-13 00:57:44.504070 mappie-0.0.2/.builds/main.yml
--rw-r--r--   0        0        0      615 2023-06-13 00:40:41.885378 mappie-0.0.2/.builds/mockbuild-epel9.yml
--rw-r--r--   0        0        0      620 2023-06-13 00:40:41.883378 mappie-0.0.2/.builds/mockbuild.yml
--rw-r--r--   0        0        0      252 2023-06-13 00:00:05.424119 mappie-0.0.2/.copr/Makefile
--rw-r--r--   0        0        0      147 2023-06-13 00:00:05.424119 mappie-0.0.2/.gitignore
--rw-r--r--   0        0        0     1676 2023-06-13 00:00:05.424119 mappie-0.0.2/CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-06-13 00:40:41.892378 mappie-0.0.2/LICENSE -> LICENSES/MIT.txt
--rw-r--r--   0        0        0     1078 2023-06-13 00:00:05.424119 mappie-0.0.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0      304 2023-06-15 20:09:00.413993 mappie-0.0.2/NEWS.md
--rw-r--r--   0        0        0     1348 2023-06-13 00:00:05.424119 mappie-0.0.2/README.md
--rwxr-xr-x   0        0        0      912 2023-06-13 00:00:05.424119 mappie-0.0.2/contrib/fedoraify.py
--rw-r--r--   0        0        0     4395 2023-06-13 00:25:05.463160 mappie-0.0.2/noxfile.py
--rw-r--r--   0        0        0     1992 2023-06-13 00:00:05.425119 mappie-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1245 2023-06-15 20:09:00.008994 mappie-0.0.2/python-mappie.spec
--rw-r--r--   0        0        0      694 2023-06-13 00:00:05.425119 mappie-0.0.2/ruff.toml
--rw-r--r--   0        0        0     5865 2023-06-15 20:08:54.661005 mappie-0.0.2/src/mappie/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 19:54:33.674885 mappie-0.0.2/src/mappie/py.typed
--rw-r--r--   0        0        0       80 2023-06-13 00:00:05.425119 mappie-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3242 2023-06-13 00:00:05.548118 mappie-0.0.2/tests/test_mappie.py
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 mappie-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-06-16 15:25:20.907467 mappie-0.1.0/.builds/main.yml
+-rw-r--r--   0        0        0      615 2023-06-13 00:40:41.885378 mappie-0.1.0/.builds/mockbuild-epel9.yml
+-rw-r--r--   0        0        0      620 2023-06-13 00:40:41.883378 mappie-0.1.0/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      252 2023-06-13 00:00:05.424119 mappie-0.1.0/.copr/Makefile
+-rw-r--r--   0        0        0      147 2023-06-13 00:00:05.424119 mappie-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1676 2023-06-13 00:00:05.424119 mappie-0.1.0/CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-06-13 00:40:41.892378 mappie-0.1.0/LICENSE -> LICENSES/MIT.txt
+-rw-r--r--   0        0        0     1078 2023-06-13 00:00:05.424119 mappie-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      618 2023-06-18 22:27:59.152362 mappie-0.1.0/NEWS.md
+-rw-r--r--   0        0        0     1348 2023-06-13 00:00:05.424119 mappie-0.1.0/README.md
+-rwxr-xr-x   0        0        0      912 2023-06-13 00:00:05.424119 mappie-0.1.0/contrib/fedoraify.py
+-rw-r--r--   0        0        0     4396 2023-06-16 15:24:06.403605 mappie-0.1.0/noxfile.py
+-rw-r--r--   0        0        0     1993 2023-06-16 15:23:50.719634 mappie-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2023-06-18 22:27:58.716362 mappie-0.1.0/python-mappie.spec
+-rw-r--r--   0        0        0      694 2023-06-13 00:00:05.425119 mappie-0.1.0/ruff.toml
+-rw-r--r--   0        0        0     6138 2023-06-18 22:27:53.040363 mappie-0.1.0/src/mappie/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 19:54:33.674885 mappie-0.1.0/src/mappie/py.typed
+-rw-r--r--   0        0        0       80 2023-06-13 00:00:05.425119 mappie-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3476 2023-06-16 00:34:47.500860 mappie-0.1.0/tests/test_mappie.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 mappie-0.1.0/PKG-INFO
```

### Comparing `mappie-0.0.2/.builds/main.yml` & `mappie-0.1.0/.builds/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 ---
 
 image: fedora/rawhide
 packages:
   - pipx
-  - python3.7
   - python3.8
   - python3.9
   - python3.10-devel
   - python3.11-devel
+  - python3.12-devel
 sources:
   - https://git.sr.ht/~gotmax23/mappie
 secrets:
   # gotmax23/mappie-dev webhook
   - 742238e7-444a-4ec8-bf95-e95cb8b86f1d
 tasks:
   - setup: |
```

### Comparing `mappie-0.0.2/.builds/mockbuild-epel9.yml` & `mappie-0.1.0/.builds/mockbuild-epel9.yml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/.builds/mockbuild.yml` & `mappie-0.1.0/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/CONTRIBUTING.md` & `mappie-0.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/LICENSES/MIT.txt` & `mappie-0.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/README.md` & `mappie-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/contrib/fedoraify.py` & `mappie-0.1.0/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/noxfile.py` & `mappie-0.1.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def git(session: nox.Session, *args, **kwargs):
     return session.run("git", *args, **kwargs, external=True)
 
 
 # General
 
 
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+@nox.session(python=["3.8", "3.9", "3.10", "3.11", "3.12"])
 def test(session: nox.Session):
     install(session, ".[test]", editable=True)
     session.run("pytest", *session.posargs)
 
 
 @nox.session(venv_backend="none")
 def lint(session: nox.Session):
```

### Comparing `mappie-0.0.2/pyproject.toml` & `mappie-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 authors = [{ name = "Maxwell G", email = "maxwell@gtmx.me" }]
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
 ]
 dependencies = [
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 codeqa = [
     "ruff",
     "reuse",
 ]
 formatters = [
```

### Comparing `mappie-0.0.2/python-mappie.spec` & `mappie-0.1.0/python-mappie.spec`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT
 
 Name:           python-mappie
-Version:        0.0.2
+Version:        0.1.0
 Release:        1%{?dist}
 Summary:        Python library with collections, frozen mappings, and more
 
 License:        MIT
 URL:            https://sr.ht/~gotmax23/mappie
 %global furl    https://git.sr.ht/~gotmax23/mappie
 Source0:        %{furl}/refs/download/v%{version}/mappie-%{version}.tar.gz
@@ -51,12 +51,15 @@
 
 %files -n python3-mappie -f %{pyproject_files}
 %doc README.md
 %license LICENSES/*
 
 
 %changelog
+* Sun Jun 18 2023 Maxwell G <maxwell@gtmx.me> - 0.1.0-1
+- Release 0.1.0.
+
 * Thu Jun 15 2023 Maxwell G <maxwell@gtmx.me> - 0.0.2-1
 - Release 0.0.2.
 
 * Tue Jun 13 2023 Maxwell G <maxwell@gtmx.me> - 0.0.1-1
 - Release 0.0.1.
```

### Comparing `mappie-0.0.2/ruff.toml` & `mappie-0.1.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `mappie-0.0.2/src/mappie/__init__.py` & `mappie-0.1.0/src/mappie/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # We deliberately import Mapping from typing.
 # Older Pythons don't have __class_getitem__ at runtime.
 from typing import TYPE_CHECKING, Any, Generic, Mapping, TypeVar
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 
 _T = TypeVar("_T")
 _T2 = TypeVar("_T2")
 
 
 def _copy_dict(mapping: Mapping[_T, _T2] | _UnsafeDict) -> dict[_T, _T2]:
     if isinstance(mapping, _UnsafeDict):
@@ -59,15 +59,17 @@
     """
     Immutable Mapping class
     """
 
     __data: dict[_T, _T2]
     _strict_eq = False
 
-    def __new__(cls: type[_MappieT], data: Mapping[_T, _T2] | _UnsafeDict) -> _MappieT:
+    def __new__(
+        cls: type[_MappieT], data: Mapping[_T, _T2] | _UnsafeDict, /
+    ) -> _MappieT:
         self = super().__new__(cls)
         data = _copy_dict(data)
         self.__data = data
         return self
 
     def __getitem__(self, key: _T) -> _T2:
         return self.__data[key]
@@ -108,14 +110,22 @@
     def __or__(self: _MappieT, other: Mapping[_T, _T2]) -> _MappieT:
         return type(self)({**self, **other})
 
     @classmethod
     def from_mapping(cls, mapping: Mapping) -> Self:
         return Mappifier(cls).mappify(mapping)
 
+    def __copy__(self: _MappieT) -> _MappieT:
+        return type(self)(dict(self))
+
+    def __deepcopy__(self: _MappieT, memo: dict[int, Any] | None) -> _MappieT:
+        from copy import deepcopy
+
+        return type(self)(deepcopy(dict(self), memo))
+
 
 class StrictFrozenMappie(FrozenMappie[_T, _T2]):
     """
     FrozenMappie that enforces strict equality
     """
 
     _strict_eq = True
@@ -124,18 +134,18 @@
 class FactoryFrozenMappie(FrozenMappie[_T, _T2]):
     """
     Immutable Mapping class that accepts a `validator` factory to modify values
     """
 
     @classmethod
     @abstractmethod
-    def validator(self, data: dict) -> dict[_T, _T2]:
+    def validator(cls, data: dict) -> dict[_T, _T2]:
         ...
 
-    def __new__(cls, data: Mapping | _UnsafeDict):
+    def __new__(cls, data: Mapping | _UnsafeDict, /):
         validate: bool = True
         new: _UnsafeDict
         if isinstance(data, _UnsafeDict):
             validate = data.validate
             new = data
         if validate:
             new = _UnsafeDict(cls.validator(_copy_dict(data)))
```

### Comparing `mappie-0.0.2/tests/test_mappie.py` & `mappie-0.1.0/tests/test_mappie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 
 
 from __future__ import annotations
 
+import copy
 from typing import Any, TypeVar
 
 import pytest
 
 from mappie import (
     AttrFrozenMappie,
     FactoryFrozenMappie,
@@ -94,14 +95,20 @@
     else:
         assert mappie == FrozenMappie(mappie)
         assert mappie == dict(mappie)
     # __hash__
     assert len({mappie, subcls(mappie)}) == 1
     # __or__
     assert mappie | mappie == mappie
+    # __copy__
+    assert copy.copy(mappie) == mappie
+    assert hash(copy.copy(mappie)) == hash(mappie)
+    # __deepcopy__
+    assert copy.deepcopy(mappie) == mappie
+    assert hash(copy.deepcopy(mappie)) == hash(mappie)
 
 
 def test_factory_frozen_mappie():
     mappie: ExampleFactoryFrozenMappie2 = ExampleFactoryFrozenMappie2(TEST_DICT_1)
     assert list(mappie.keys()) == list(TEST_DICT_1.values())
```

### Comparing `mappie-0.0.2/PKG-INFO` & `mappie-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mappie
-Version: 0.0.2
+Version: 0.1.0
 Summary: Collections, frozen mappings, and more
 Author-email: Maxwell G <maxwell@gtmx.me>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Requires-Dist: ruff ; extra == "codeqa"
 Requires-Dist: reuse ; extra == "codeqa"
 Requires-Dist: mappie[formatters] ; extra == "dev"
 Requires-Dist: mappie[test] ; extra == "dev"
 Requires-Dist: mappie[typing] ; extra == "dev"
```

