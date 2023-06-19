# Comparing `tmp/energymon-0.1.1.tar.gz` & `tmp/energymon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energymon-0.1.1.tar", last modified: Fri Mar 25 17:54:43 2022, max compression
+gzip compressed data, was "energymon-0.1.2.tar", last modified: Mon Jun 19 19:36:30 2023, max compression
```

## Comparing `energymon-0.1.1.tar` & `energymon-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cimes      (501) staff       (20)        0 2022-03-25 17:54:43.002205 energymon-0.1.1/
--rw-r--r--   0 cimes      (501) staff       (20)    11357 2022-02-07 16:19:41.000000 energymon-0.1.1/LICENSE-APACHE
--rw-r--r--   0 cimes      (501) staff       (20)     1060 2022-03-01 17:43:51.000000 energymon-0.1.1/LICENSE-MIT
--rw-r--r--   0 cimes      (501) staff       (20)     5108 2022-03-25 17:54:43.002281 energymon-0.1.1/PKG-INFO
--rw-r--r--   0 cimes      (501) staff       (20)     4651 2022-03-01 17:40:27.000000 energymon-0.1.1/README.md
--rw-r--r--   0 cimes      (501) staff       (20)      107 2022-02-07 16:19:41.000000 energymon-0.1.1/pyproject.toml
--rw-r--r--   0 cimes      (501) staff       (20)      594 2022-03-25 17:54:43.002652 energymon-0.1.1/setup.cfg
-drwxr-xr-x   0 cimes      (501) staff       (20)        0 2022-03-25 17:54:42.997850 energymon-0.1.1/src/
-drwxr-xr-x   0 cimes      (501) staff       (20)        0 2022-03-25 17:54:42.999899 energymon-0.1.1/src/energymon/
--rw-r--r--   0 cimes      (501) staff       (20)     1136 2022-03-01 15:09:23.000000 energymon-0.1.1/src/energymon/__init__.py
--rw-r--r--   0 cimes      (501) staff       (20)     5806 2022-03-09 18:12:38.000000 energymon-0.1.1/src/energymon/context.py
--rw-r--r--   0 cimes      (501) staff       (20)     8312 2022-03-01 15:22:59.000000 energymon-0.1.1/src/energymon/util.py
-drwxr-xr-x   0 cimes      (501) staff       (20)        0 2022-03-25 17:54:43.000899 energymon-0.1.1/src/energymon.egg-info/
--rw-r--r--   0 cimes      (501) staff       (20)     5108 2022-03-25 17:54:42.000000 energymon-0.1.1/src/energymon.egg-info/PKG-INFO
--rw-r--r--   0 cimes      (501) staff       (20)      344 2022-03-25 17:54:42.000000 energymon-0.1.1/src/energymon.egg-info/SOURCES.txt
--rw-r--r--   0 cimes      (501) staff       (20)        1 2022-03-25 17:54:42.000000 energymon-0.1.1/src/energymon.egg-info/dependency_links.txt
--rw-r--r--   0 cimes      (501) staff       (20)       10 2022-03-25 17:54:42.000000 energymon-0.1.1/src/energymon.egg-info/top_level.txt
-drwxr-xr-x   0 cimes      (501) staff       (20)        0 2022-03-25 17:54:43.001737 energymon-0.1.1/test/
--rw-r--r--   0 cimes      (501) staff       (20)     3865 2022-03-01 17:40:27.000000 energymon-0.1.1/test/test_context.py
--rw-r--r--   0 cimes      (501) staff       (20)     2138 2022-02-07 16:19:41.000000 energymon-0.1.1/test/test_energymon.py
--rw-r--r--   0 cimes      (501) staff       (20)     3190 2022-03-01 15:23:48.000000 energymon-0.1.1/test/test_util.py
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-19 19:36:30.512527 energymon-0.1.2/
+-rw-r--r--   0 cimes      (501) staff       (20)    11357 2022-02-07 16:19:41.000000 energymon-0.1.2/LICENSE-APACHE
+-rw-r--r--   0 cimes      (501) staff       (20)     1060 2023-06-19 19:11:05.000000 energymon-0.1.2/LICENSE-MIT
+-rw-r--r--   0 cimes      (501) staff       (20)     5132 2023-06-19 19:36:30.512790 energymon-0.1.2/PKG-INFO
+-rw-r--r--   0 cimes      (501) staff       (20)     4712 2022-05-25 13:45:55.000000 energymon-0.1.2/README.md
+-rw-r--r--   0 cimes      (501) staff       (20)      107 2022-02-07 16:19:41.000000 energymon-0.1.2/pyproject.toml
+-rw-r--r--   0 cimes      (501) staff       (20)      594 2023-06-19 19:36:30.513116 energymon-0.1.2/setup.cfg
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-19 19:36:30.509451 energymon-0.1.2/src/
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-19 19:36:30.510890 energymon-0.1.2/src/energymon/
+-rw-r--r--   0 cimes      (501) staff       (20)     1136 2022-03-01 15:09:23.000000 energymon-0.1.2/src/energymon/__init__.py
+-rw-r--r--   0 cimes      (501) staff       (20)     5822 2022-06-30 20:43:38.000000 energymon-0.1.2/src/energymon/context.py
+-rw-r--r--   0 cimes      (501) staff       (20)     8333 2022-06-30 20:43:04.000000 energymon-0.1.2/src/energymon/util.py
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-19 19:36:30.511510 energymon-0.1.2/src/energymon.egg-info/
+-rw-r--r--   0 cimes      (501) staff       (20)     5132 2023-06-19 19:36:30.000000 energymon-0.1.2/src/energymon.egg-info/PKG-INFO
+-rw-r--r--   0 cimes      (501) staff       (20)      344 2023-06-19 19:36:30.000000 energymon-0.1.2/src/energymon.egg-info/SOURCES.txt
+-rw-r--r--   0 cimes      (501) staff       (20)        1 2023-06-19 19:36:30.000000 energymon-0.1.2/src/energymon.egg-info/dependency_links.txt
+-rw-r--r--   0 cimes      (501) staff       (20)       10 2023-06-19 19:36:30.000000 energymon-0.1.2/src/energymon.egg-info/top_level.txt
+drwxr-xr-x   0 cimes      (501) staff       (20)        0 2023-06-19 19:36:30.512349 energymon-0.1.2/test/
+-rw-r--r--   0 cimes      (501) staff       (20)     4051 2022-05-23 20:45:41.000000 energymon-0.1.2/test/test_context.py
+-rw-r--r--   0 cimes      (501) staff       (20)     2138 2022-02-07 16:19:41.000000 energymon-0.1.2/test/test_energymon.py
+-rw-r--r--   0 cimes      (501) staff       (20)     3190 2022-03-01 15:23:48.000000 energymon-0.1.2/test/test_util.py
```

### Comparing `energymon-0.1.1/LICENSE-APACHE` & `energymon-0.1.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `energymon-0.1.1/LICENSE-MIT` & `energymon-0.1.2/LICENSE-MIT`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2022 Connor Imes
+Copyright (c) 2021-2023 Connor Imes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `energymon-0.1.1/PKG-INFO` & `energymon-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: energymon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings to native energymon libraries
 Home-page: https://github.com/energymon/energymon-py
 Author: Connor Imes
-License: UNKNOWN
 Keywords: energymon,energy,monitoring,bindings
-Platform: UNKNOWN
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE-MIT
 License-File: LICENSE-APACHE
 
@@ -57,14 +55,20 @@
 
 Versioned releases of the `energymon` package are published in the Python Package Index and installable with pip:
 
 ```sh
 pip install energymon
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
 
 
@@ -155,9 +159,7 @@
 
 ## Project Source
 
 Find this and related project sources at the [energymon organization on GitHub](https://github.com/energymon).  
 This project originates at: https://github.com/energymon/energymon-py
 
 Bug reports and pull requests for bug fixes and enhancements are welcome.
-
-
```

### Comparing `energymon-0.1.1/README.md` & `energymon-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
 Versioned releases of the `energymon` package are published in the Python Package Index and installable with pip:
 
 ```sh
 pip install energymon
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
```

### Comparing `energymon-0.1.1/setup.cfg` & `energymon-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energymon
-version = 0.1.1
+version = 0.1.2
 url = https://github.com/energymon/energymon-py
 license_files = 
 	LICENSE-MIT
 	LICENSE-APACHE
 description = Python bindings to native energymon libraries
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `energymon-0.1.1/src/energymon/__init__.py` & `energymon-0.1.2/src/energymon/__init__.py`

 * *Files identical despite different names*

### Comparing `energymon-0.1.1/src/energymon/context.py` & `energymon-0.1.2/src/energymon/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         self._ctx = util.get_energymon(lib, func_get)
 
     @property
     def initialized(self) -> bool:
         """bool: True if the ``energymon`` is initialized, False otherwise."""
         return self._refcount > 0
 
-    def init(self):
+    def init(self) -> None:
         """
         Initialize the underlying ``energymon``.
 
         Only call this method if not using the pattern: ``with EnergyMon(...) as context:``.
         """
         if self._refcount > 0:
             raise ValueError('energymon is already initialized')
         util.init(self._ctx)
         self._refcount += 1
 
-    def finish(self):
+    def finish(self) -> None:
         """
         Finish the underlying ``energymon``.
         If not already initialized, this is a no-op.
 
         Only call this method if not using the pattern: ``with EnergyMon(...) as context:``.
         """
         if self._refcount > 0:
```

### Comparing `energymon-0.1.1/src/energymon/util.py` & `energymon-0.1.2/src/energymon/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             suffix = '.dll'
         else:
             suffix = '.so'
         path = 'lib' + name + suffix
         raise FileNotFoundError('Failed to find library by name: ' + name + ' (' + path + ')')
     return CDLL(path, use_errno=True, use_last_error=True)
 
-def get_energymon(lib, func_get='energymon_get_default') -> energymon:
+def get_energymon(lib, func_get: str='energymon_get_default') -> energymon:
     """
     Create an ``energymon`` and "get" it (populate its function pointers), but do not initialize it.
 
     Parameters
     ----------
     lib : ctypes library
         An ``energymon`` library loaded by ``ctypes`` (e.g., a ``CDLL``).
@@ -88,15 +88,15 @@
     assert em.ffinish
     assert em.fsource
     assert em.finterval
     assert em.fprecision
     assert em.fexclusive
     return em
 
-def init(em: energymon):
+def init(em: energymon) -> None:
     """
     Initialize the ``energymon`` (initialize private state).
 
     Parameters
     ----------
     em : energymon
         The ``energymon`` must not be initialized.
@@ -111,15 +111,15 @@
     if not em.finit:
         raise ValueError('\'finit\' not set - did you \'get\' the energymon?')
     set_errno(0)
     if em.finit(byref(em)) != 0:
         errno = get_errno()
         raise OSError(errno, os.strerror(errno))
 
-def finish(em: energymon):
+def finish(em: energymon) -> None:
     """
     Finish the ``energymon`` (clean up private state).
 
     Parameters
     ----------
     em : energymon
         The ``energymon`` must be initialized.
```

### Comparing `energymon-0.1.1/src/energymon.egg-info/PKG-INFO` & `energymon-0.1.2/src/energymon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: energymon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python bindings to native energymon libraries
 Home-page: https://github.com/energymon/energymon-py
 Author: Connor Imes
-License: UNKNOWN
 Keywords: energymon,energy,monitoring,bindings
-Platform: UNKNOWN
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE-MIT
 License-File: LICENSE-APACHE
 
@@ -57,14 +55,20 @@
 
 Versioned releases of the `energymon` package are published in the Python Package Index and installable with pip:
 
 ```sh
 pip install energymon
 ```
 
+and through Conda Forge:
+
+```sh
+conda install energymon
+```
+
 To install from source:
 
 ```sh
 pip install .
 ```
 
 
@@ -155,9 +159,7 @@
 
 ## Project Source
 
 Find this and related project sources at the [energymon organization on GitHub](https://github.com/energymon).  
 This project originates at: https://github.com/energymon/energymon-py
 
 Bug reports and pull requests for bug fixes and enhancements are welcome.
-
-
```

### Comparing `energymon-0.1.1/test/test_context.py` & `energymon-0.1.2/test/test_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pylint: disable=C0114, C0116
+import gc
 import pickle
 import unittest
 from energymon import util
 from energymon.context import EnergyMon
 
 class TestEnergyMon(unittest.TestCase):
     """Test EnergyMon."""
@@ -65,14 +66,17 @@
         self.assertIsInstance(enm.is_exclusive(), bool)
 
     def test_del_warning(self):
         enm = EnergyMon()
         enm.init()
         with self.assertWarns(ResourceWarning):
             del enm
+            # CPython runs `__del__` synchronously when `del` is invoked
+            # PyPy doesn't use reference counting though, so we must force gc
+            gc.collect()
 
     def test_context(self):
         with EnergyMon() as enm:
             self.assertIsInstance(enm, EnergyMon)
             self.assertTrue(enm.initialized)
 
     def test_context_predefined(self):
```

### Comparing `energymon-0.1.1/test/test_energymon.py` & `energymon-0.1.2/test/test_energymon.py`

 * *Files identical despite different names*

### Comparing `energymon-0.1.1/test/test_util.py` & `energymon-0.1.2/test/test_util.py`

 * *Files identical despite different names*

