# Comparing `tmp/trytond-factories-6.6.4.tar.gz` & `tmp/trytond-factories-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-factories-6.6.4.tar", last modified: Mon May 22 08:24:57 2023, max compression
+gzip compressed data, was "trytond-factories-6.8.1.tar", last modified: Mon Jun 19 07:37:23 2023, max compression
```

## Comparing `trytond-factories-6.6.4.tar` & `trytond-factories-6.8.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:24:57.789091 trytond-factories-6.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-22 08:24:57.789091 trytond-factories-6.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-22 08:24:57.793091 trytond-factories-6.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:24:57.785091 trytond-factories-6.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:24:57.789091 trytond-factories-6.6.4/src/trytond_factories/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/company.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/party.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/sale_amendment.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 08:24:43.000000 trytond-factories-6.6.4/src/trytond_factories/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:24:57.789091 trytond-factories-6.6.4/src/trytond_factories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-22 08:24:57.000000 trytond-factories-6.6.4/src/trytond_factories.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-22 08:24:57.000000 trytond-factories-6.6.4/src/trytond_factories.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:24:57.000000 trytond-factories-6.6.4/src/trytond_factories.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 08:24:57.000000 trytond-factories-6.6.4/src/trytond_factories.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 08:24:57.000000 trytond-factories-6.6.4/src/trytond_factories.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:37:23.260348 trytond-factories-6.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-19 07:37:23.260348 trytond-factories-6.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-19 07:37:23.260348 trytond-factories-6.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:37:23.256348 trytond-factories-6.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:37:23.260348 trytond-factories-6.8.1/src/trytond_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/party.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/sale_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-19 07:37:14.000000 trytond-factories-6.8.1/src/trytond_factories/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:37:23.260348 trytond-factories-6.8.1/src/trytond_factories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-19 07:37:23.000000 trytond-factories-6.8.1/src/trytond_factories.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-19 07:37:23.000000 trytond-factories-6.8.1/src/trytond_factories.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:37:23.000000 trytond-factories-6.8.1/src/trytond_factories.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 07:37:23.000000 trytond-factories-6.8.1/src/trytond_factories.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 07:37:23.000000 trytond-factories-6.8.1/src/trytond_factories.egg-info/top_level.txt
```

### Comparing `trytond-factories-6.6.4/LICENSE` & `trytond-factories-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/PKG-INFO` & `trytond-factories-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-factories
-Version: 6.6.4
+Version: 6.8.1
 Summary: A collection of opinionated factories for common Tryton modules
 Home-page: https://github.com/calidae/trytond-factories
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPLv3+
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trytond-factories-6.6.4/README.md` & `trytond-factories-6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/setup.cfg` & `trytond-factories-6.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 [options]
 python_requires = >=3.8
 packages = trytond_factories
 package_dir = 
 	=src
 install_requires = 
 	factory_trytond
-	trytond ~= 6.6.0
+	trytond ~= 6.8.0
 
 [options.extras_require]
 tests = 
 	pytest-trytond
-	trytond-account_invoice ~= 6.6.0
+	trytond-account_invoice ~= 6.8.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trytond-factories-6.6.4/src/trytond_factories/__init__.py` & `trytond-factories-6.8.1/src/trytond_factories/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '6.6.4'
+__version__ = '6.8.1'
 
 from .tools import *  # NOQA: 401
 from .account import *  # NOQA: 401
 from .action import *  # NOQA: 401
 from .attachment import *  # NOQA: 401
 from .company import *  # NOQA: 401
 from .currency import *  # NOQA: 401
```

### Comparing `trytond-factories-6.6.4/src/trytond_factories/account.py` & `trytond-factories-6.8.1/src/trytond_factories/account.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/action.py` & `trytond-factories-6.8.1/src/trytond_factories/action.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 
 
 class Action(factory_trytond.TrytonFactory):
     class Meta:
         model = 'ir.action'
 
     name = factory.Faker('word')
-    type = factory.Faker('word', ext_word_list=['tree', 'form'])
+    type = factory.Faker('word', ext_word_list=[
+        'ir.action.url',
+        'ir.action.act_window',
+        'ir.action.wizard',
+        'ir.action.report',
+    ])
     records = 'selected'
     usage = factory.Faker('word')
     keywords = factory.RelatedFactoryList(
         'trytond_factories.action.Keyword',
         factory_related_name='action',
         size=1,
     )
```

### Comparing `trytond-factories-6.6.4/src/trytond_factories/attachment.py` & `trytond-factories-6.8.1/src/trytond_factories/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/company.py` & `trytond-factories-6.8.1/src/trytond_factories/company.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/currency.py` & `trytond-factories-6.8.1/src/trytond_factories/currency.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/invoice.py` & `trytond-factories-6.8.1/src/trytond_factories/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/party.py` & `trytond-factories-6.8.1/src/trytond_factories/party.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/product.py` & `trytond-factories-6.8.1/src/trytond_factories/product.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/purchase.py` & `trytond-factories-6.8.1/src/trytond_factories/purchase.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/sale.py` & `trytond-factories-6.8.1/src/trytond_factories/sale.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/sale_amendment.py` & `trytond-factories-6.8.1/src/trytond_factories/sale_amendment.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/stock.py` & `trytond-factories-6.8.1/src/trytond_factories/stock.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/tools.py` & `trytond-factories-6.8.1/src/trytond_factories/tools.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/user.py` & `trytond-factories-6.8.1/src/trytond_factories/user.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories/wizards.py` & `trytond-factories-6.8.1/src/trytond_factories/wizards.py`

 * *Files identical despite different names*

### Comparing `trytond-factories-6.6.4/src/trytond_factories.egg-info/PKG-INFO` & `trytond-factories-6.8.1/src/trytond_factories.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-factories
-Version: 6.6.4
+Version: 6.8.1
 Summary: A collection of opinionated factories for common Tryton modules
 Home-page: https://github.com/calidae/trytond-factories
 Author: Calidae
 Author-email: dev@calidae.com
 License: GPLv3+
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `trytond-factories-6.6.4/src/trytond_factories.egg-info/SOURCES.txt` & `trytond-factories-6.8.1/src/trytond_factories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

