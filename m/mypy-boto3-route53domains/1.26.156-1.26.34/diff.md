# Comparing `tmp/mypy-boto3-route53domains-1.26.156.tar.gz` & `tmp/mypy-boto3-route53domains-1.26.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.26.156.tar", last modified: Mon Jun 19 19:33:27 2023, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.26.34.tar", last modified: Tue Dec 20 20:26:41 2022, max compression
```

## Comparing `mypy-boto3-route53domains-1.26.156.tar` & `mypy-boto3-route53domains-1.26.34.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.188819 mypy-boto3-route53domains-1.26.156/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-06-19 19:33:27.184819 mypy-boto3-route53domains-1.26.156/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.184819 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-19 19:32:54.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-06-19 19:32:54.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-06-19 19:32:54.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:33:27.184819 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 19:33:27.000000 mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:33:27.188819 mypy-boto3-route53domains-1.26.156/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-19 19:32:53.000000 mypy-boto3-route53domains-1.26.156/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15761 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28925 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28880 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27512 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27491 2022-12-20 20:26:10.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-20 20:26:40.000000 mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 20:26:41.046595 mypy-boto3-route53domains-1.26.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-20 20:26:09.000000 mypy-boto3-route53domains-1.26.34/setup.py
```

### Comparing `mypy-boto3-route53domains-1.26.156/LICENSE` & `mypy-boto3-route53domains-1.26.34/LICENSE`

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

### Comparing `mypy-boto3-route53domains-1.26.156/PKG-INFO` & `mypy-boto3-route53domains-1.26.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.26.156
-Summary: Type annotations for boto3.Route53Domains 1.26.156 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.34
+Summary: Type annotations for boto3.Route53Domains 1.26.34 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -443,42 +443,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.156/README.md` & `mypy-boto3-route53domains-1.26.34/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -411,42 +411,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/__main__.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Domains 1.26.156\nVersion:         1.26.156\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53Domains 1.26.34\nVersion:         1.26.34\nBuilder"
+        " version: 7.12.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.156")
+    print("1.26.34")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,17 +338,17 @@
         """
 
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
-        specified TLD: * Registration * Transfer * Owner change * Domain renewal *
-        Domain restoration See also: `AWS API Documentation
-        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
+        specified TLD * Registration * Transfer * Owner change * Domain renewal * Domain
+        restoration See also: `AWS API Documentation
+        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-1...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
 
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
```

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -312,17 +312,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_operations)
         """
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
-        specified TLD: * Registration * Transfer * Owner change * Domain renewal *
-        Domain restoration See also: `AWS API Documentation
-        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
+        specified TLD * Registration * Transfer * Owner change * Domain renewal * Domain
+        restoration See also: `AWS API Documentation
+        <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-1...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
         This operation returns all of the tags that are associated with the specified
```

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContactTypeType",
     "CountryCodeType",
     "DomainAvailabilityType",
     "ExtraParamNameType",
     "ListDomainsAttributeNameType",
     "ListDomainsPaginatorName",
@@ -40,15 +39,14 @@
     "Route53DomainsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContactTypeType = Literal["ASSOCIATION", "COMPANY", "PERSON", "PUBLIC_BODY", "RESELLER"]
 CountryCodeType = Literal[
     "AC",
     "AD",
     "AE",
     "AF",
     "AG",
@@ -427,34 +425,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
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
@@ -533,15 +528,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -552,20 +546,18 @@
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
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -575,15 +567,14 @@
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -596,15 +587,14 @@
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
@@ -623,19 +613,16 @@
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
@@ -715,21 +702,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ContactTypeType",
     "CountryCodeType",
     "DomainAvailabilityType",
     "ExtraParamNameType",
     "ListDomainsAttributeNameType",
     "ListDomainsPaginatorName",
@@ -39,14 +40,15 @@
     "Route53DomainsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ContactTypeType = Literal["ASSOCIATION", "COMPANY", "PERSON", "PUBLIC_BODY", "RESELLER"]
 CountryCodeType = Literal[
     "AC",
     "AD",
     "AE",
     "AF",
     "AG",
@@ -425,34 +427,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
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
@@ -531,15 +530,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -550,20 +548,18 @@
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
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
@@ -573,15 +569,14 @@
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -594,15 +589,14 @@
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
@@ -621,19 +615,16 @@
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
@@ -713,21 +704,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.26.156
-Summary: Type annotations for boto3.Route53Domains 1.26.156 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.34
+Summary: Type annotations for boto3.Route53Domains 1.26.34 service generated with mypy-boto3-builder 7.12.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.26.156](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.26.34](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -443,42 +443,42 @@
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

### Comparing `mypy-boto3-route53domains-1.26.156/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.26.34/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.26.156/setup.py` & `mypy-boto3-route53domains-1.26.34/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-route53domains.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.26.156",
+    version="1.26.34",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Domains 1.26.156 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53Domains 1.26.34 service generated with"
+        " mypy-boto3-builder 7.12.0"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/",
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

