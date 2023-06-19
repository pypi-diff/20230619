# Comparing `tmp/mypy-boto3-pricing-1.26.156.tar.gz` & `tmp/mypy-boto3-pricing-1.26.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pricing-1.26.156.tar", last modified: Mon Jun 19 19:33:27 2023, max compression
+gzip compressed data, was "mypy-boto3-pricing-1.26.82.tar", last modified: Wed Mar  1 20:27:29 2023, max compression
```

## Comparing `mypy-boto3-pricing-1.26.156.tar` & `mypy-boto3-pricing-1.26.82.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.184819 mypy-boto3-pricing-1.26.156/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-19 19:33:27.180819 mypy-boto3-pricing-1.26.156/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.172819 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.180819 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 19:33:27.000000 mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:33:27.184819 mypy-boto3-pricing-1.26.156/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-19 19:32:52.000000 mypy-boto3-pricing-1.26.156/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.574109 mypy-boto3-pricing-1.26.82/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-01 20:27:19.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:27:29.570109 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 20:27:29.000000 mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 20:27:29.574109 mypy-boto3-pricing-1.26.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-01 20:27:18.000000 mypy-boto3-pricing-1.26.82/setup.py
```

### Comparing `mypy-boto3-pricing-1.26.156/LICENSE` & `mypy-boto3-pricing-1.26.82/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-pricing-1.26.156/PKG-INFO` & `mypy-boto3-pricing-1.26.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.26.156
-Summary: Type annotations for boto3.Pricing 1.26.156 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.82
+Summary: Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,42 +366,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pricing-1.26.156/README.md` & `mypy-boto3-pricing-1.26.82/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,42 +334,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__init__.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__init__.pyi` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/__main__.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Pricing 1.26.156\nVersion:         1.26.156\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Pricing 1.26.82\nVersion:         1.26.82\nBuilder version:"
+        " 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.156")
+    print("1.26.82")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/client.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/client.pyi` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/literals.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeServicesPaginatorName",
     "FilterTypeType",
     "GetAttributeValuesPaginatorName",
     "GetProductsPaginatorName",
     "ListPriceListsPaginatorName",
     "PricingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeServicesPaginatorName = Literal["describe_services"]
 FilterTypeType = Literal["TERM_MATCH"]
 GetAttributeValuesPaginatorName = Literal["get_attribute_values"]
 GetProductsPaginatorName = Literal["get_products"]
 ListPriceListsPaginatorName = Literal["list_price_lists"]
 PricingServiceName = Literal["pricing"]
 ServiceName = Literal[
@@ -97,15 +95,14 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -203,15 +200,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -247,15 +243,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -274,19 +269,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -370,17 +362,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/literals.pyi` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeServicesPaginatorName",
     "FilterTypeType",
     "GetAttributeValuesPaginatorName",
     "GetProductsPaginatorName",
     "ListPriceListsPaginatorName",
     "PricingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeServicesPaginatorName = Literal["describe_services"]
 FilterTypeType = Literal["TERM_MATCH"]
 GetAttributeValuesPaginatorName = Literal["get_attribute_values"]
 GetProductsPaginatorName = Literal["get_products"]
 ListPriceListsPaginatorName = Literal["list_price_lists"]
 PricingServiceName = Literal["pricing"]
 ServiceName = Literal[
@@ -95,15 +97,14 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -201,15 +202,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -245,15 +245,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -272,19 +271,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -368,17 +364,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/paginator.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/paginator.pyi` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/type_defs.py` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing/type_defs.pyi` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/PKG-INFO` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pricing
-Version: 1.26.156
-Summary: Type annotations for boto3.Pricing 1.26.156 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.82
+Summary: Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-pricing"></a>
 
 # mypy-boto3-pricing
 
 [![PyPI - mypy-boto3-pricing](https://img.shields.io/pypi/v/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pricing.svg?color=blue)](https://pypi.org/project/mypy-boto3-pricing)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pricing?color=blue)](https://pypistats.org/packages/mypy-boto3-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Pricing 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[boto3.Pricing 1.26.82](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-pricing docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,42 +366,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-pricing-1.26.156/mypy_boto3_pricing.egg-info/SOURCES.txt` & `mypy-boto3-pricing-1.26.82/mypy_boto3_pricing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pricing-1.26.156/setup.py` & `mypy-boto3-pricing-1.26.82/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-pricing.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-pricing",
-    version="1.26.156",
+    version="1.26.82",
     packages=["mypy_boto3_pricing"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Pricing 1.26.156 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Pricing 1.26.82 service generated with mypy-boto3-builder"
+        " 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pricing/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

