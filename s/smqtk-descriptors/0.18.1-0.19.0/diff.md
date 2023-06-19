# Comparing `tmp/smqtk_descriptors-0.18.1.tar.gz` & `tmp/smqtk_descriptors-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smqtk_descriptors-0.18.1.tar", max compression
+gzip compressed data, was "smqtk_descriptors-0.19.0.tar", max compression
```

## Comparing `smqtk_descriptors-0.18.1.tar` & `smqtk_descriptors-0.19.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1481 2021-11-03 15:57:09.289611 smqtk_descriptors-0.18.1/LICENSE.txt
--rw-r--r--   0        0        0      759 2021-11-03 15:57:09.293611 smqtk_descriptors-0.18.1/README.md
--rw-r--r--   0        0        0     3227 2021-11-04 19:42:29.882057 smqtk_descriptors-0.18.1/pyproject.toml
--rw-r--r--   0        0        0      300 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/__init__.py
--rw-r--r--   0        0        0     3549 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/descriptor_element_factory.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/__init__.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/__init__.py
--rw-r--r--   0        0        0     4757 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/file.py
--rw-r--r--   0        0        0     3318 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/memory.py
--rw-r--r--   0        0        0    18701 2021-11-04 19:12:08.305440 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/postgres.py
--rw-r--r--   0        0        0     5760 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/solr.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_generator/__init__.py
--rw-r--r--   0        0        0    19348 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_generator/caffe1.py
--rw-r--r--   0        0        0     4030 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_generator/image_descriptor_generator_wrapper.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/__init__.py
--rw-r--r--   0        0        0    10346 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/memory.py
--rw-r--r--   0        0        0    19108 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/postgres.py
--rw-r--r--   0        0        0    12982 2021-11-03 15:57:09.297612 smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/solr.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/__init__.py
--rw-r--r--   0        0        0     8382 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_element.py
--rw-r--r--   0        0        0    14859 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_generator.py
--rw-r--r--   0        0        0     6377 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_set.py
--rw-r--r--   0        0        0      831 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/image_descriptor_generator.py
--rw-r--r--   0        0        0        0 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/py.typed
--rw-r--r--   0        0        0       49 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/utils/__init__.py
--rw-r--r--   0        0        0    30493 2021-11-03 15:57:09.301612 smqtk_descriptors-0.18.1/smqtk_descriptors/utils/parallel.py
--rw-r--r--   0        0        0     3038 2021-11-04 19:45:32.990282 smqtk_descriptors-0.18.1/setup.py
--rw-r--r--   0        0        0     2015 2021-11-04 19:45:32.990617 smqtk_descriptors-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-06-19 03:34:07.614958 smqtk_descriptors-0.19.0/LICENSE.txt
+-rw-r--r--   0        0        0      759 2023-06-19 03:34:07.614958 smqtk_descriptors-0.19.0/README.md
+-rw-r--r--   0        0        0     4016 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/__init__.py
+-rw-r--r--   0        0        0     3549 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/descriptor_element_factory.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/__init__.py
+-rw-r--r--   0        0        0     4757 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/file.py
+-rw-r--r--   0        0        0     3400 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/memory.py
+-rw-r--r--   0        0        0    18701 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/postgres.py
+-rw-r--r--   0        0        0     5760 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/solr.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/__init__.py
+-rw-r--r--   0        0        0    19348 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/caffe1.py
+-rw-r--r--   0        0        0     4030 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/image_descriptor_generator_wrapper.py
+-rw-r--r--   0        0        0    19781 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/pytorch.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/__init__.py
+-rw-r--r--   0        0        0    10346 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/memory.py
+-rw-r--r--   0        0        0    19410 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/postgres.py
+-rw-r--r--   0        0        0    13002 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/solr.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/__init__.py
+-rw-r--r--   0        0        0     8447 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_element.py
+-rw-r--r--   0        0        0    14859 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_generator.py
+-rw-r--r--   0        0        0     6377 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_set.py
+-rw-r--r--   0        0        0      851 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/image_descriptor_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/py.typed
+-rw-r--r--   0        0        0       49 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/utils/__init__.py
+-rw-r--r--   0        0        0    30493 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/utils/parallel.py
+-rw-r--r--   0        0        0     4802 2023-06-19 03:34:07.618958 smqtk_descriptors-0.19.0/smqtk_descriptors/utils/pytorch_utils.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 smqtk_descriptors-0.19.0/PKG-INFO
```

### Comparing `smqtk_descriptors-0.18.1/LICENSE.txt` & `smqtk_descriptors-0.19.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/README.md` & `smqtk_descriptors-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/pyproject.toml` & `smqtk_descriptors-0.19.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ###############################################################################
 [tool.poetry]
 name = "smqtk_descriptors"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # SMQTK prefers to use the strict numbering standard when possible.
-version = "0.18.1"
+version = "0.19.0"
 description = """\
     Algorithms, data structures and utilities around computing\
     descriptor vectors from data."""
 license = "BSD-3-Clause"
 authors = ["Kitware, Inc. <smqtk-developers@kitware.com>"]
 readme = "README.md"
 repository = "https://github.com/Kitware/SMQTK-Descriptors"
@@ -21,68 +21,82 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.19.5"
+python = "^3.8"
+numpy = ">=1.19.5"
 smqtk-core = ">=0.18.0"
 smqtk-dataprovider = ">=0.16.0"
-smqtk-image-io = "^0.16.2"
+smqtk-image-io = [
+    { version = ">=0.16.2", python = "<3.11" },
+    { version = ">=0.17.0", python=">=3.11"}
+]
+torch = {version = ">=1.10.0,!=2.0.1", optional = true}
+torchvision = {version = ">=0.11.1", optional = true}
 
 [tool.poetry.extras]
+pytorch = ["torch", "torchvision"]
 
 [tool.poetry.dev-dependencies]
 # CI
-flake8 = "^3.9.0"
-flake8-mutable = "^1.2.0"
-mypy = "^0.812"
+flake8 = [
+    # Hinge because 6.0 minimum supported python version is 3.8.1
+    { version = ">=5", python = "<3.8.1" },
+    { version = ">=6", python = ">=3.8.1" }
+]
+flake8-mutable = ">=1.2.0"
+mypy = ">=0.812"
 # Docs
 # - Also see: `docs/readthedocs-reqs.txt` for use by RTD
-Sphinx = "^3.5.3"
-sphinx-rtd-theme = "^0.5.1"
-sphinx-argparse = "^0.2.5"
-sphinx-prompt = "^1.4.0"
-livereload = "^2.6.3"
+Sphinx = ">=3.5.3"
+sphinx-rtd-theme = ">=0.5.1"
+sphinx-argparse = ">=0.2.5"
+sphinx-prompt = ">=1.4.0"
+livereload = ">=2.6.3"
 # Testing
-coverage = "^5.5"
-pytest = "^6.2.2"
-pytest-cov = "^2.11.1"
+coverage = ">=5.5"
+pytest = ">=6.2.2"
+pytest-cov = ">=2.11.1"
 # Development
-ipython = "^7.16.1"
-jedi = "^0.17.2"
+ipython = ">=7.16.3"
 
 [tool.poetry.plugins."smqtk_plugins"]
 # DescriptorElement
 "smqtk_descriptors.impls.descriptor_element.file" = "smqtk_descriptors.impls.descriptor_element.file"
 "smqtk_descriptors.impls.descriptor_element.memory" = "smqtk_descriptors.impls.descriptor_element.memory"
 "smqtk_descriptors.impls.descriptor_element.postgres" = "smqtk_descriptors.impls.descriptor_element.postgres"
 "smqtk_descriptors.impls.descriptor_element.solr" = "smqtk_descriptors.impls.descriptor_element.solr"
 # DescriptorGenerator
 "smqtk_descriptors.impls.descriptor_generator.caffe1" = "smqtk_descriptors.impls.descriptor_generator.caffe1"
+"smqtk_descriptors.impls.descriptor_generator.pytorch" = "smqtk_descriptors.impls.descriptor_generator.pytorch"
 # DescriptorSet
 "smqtk_descriptors.impls.descriptor_set.memory" = "smqtk_descriptors.impls.descriptor_set.memory"
 "smqtk_descriptors.impls.descriptor_set.postgres" = "smqtk_descriptors.impls.descriptor_set.postgres"
 "smqtk_descriptors.impls.descriptor_set.solr" = "smqtk_descriptors.impls.descriptor_set.solr"
 
 ###############################################################################
 [tool.pytest.ini_options]
 addopts = [
-    "-lv",                  # Show local in trace-backs.
-    "--doctest-modules",    # Increased verbosity.
-    "--tb=long",            # Trace-back print mode.
+    "-lv",                          # Show local in trace-backs.
+    "--doctest-modules",            # Increased verbosity.
+    "--tb=long",                    # Trace-back print mode.
+    "--cov=./smqtk_descriptors",    # Cover our package specifically
+    "--cov=./tests",                # Also cover our tests for dead spots
+    "--cov-report=term",            # Coverage report to terminal
+    "--cov-report=xml:coverage.xml" # for external tool reporting
 ]
 testpaths = [
     "tests",
     "smqtk_descriptors",
 ]
 norecursedirs = [
     "tests/data"
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/descriptor_element_factory.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/descriptor_element_factory.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/file.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/file.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/memory.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     @classmethod
     def is_usable(cls) -> bool:
         return True
 
     def __init__(self, uuid: Hashable):
         super(DescriptorMemoryElement, self).__init__(uuid)
-        self.__v = None
+        self.__v = None  # type: Optional[numpy.ndarray[Any, numpy.dtype[Any]]]
 
     @classmethod
     def _get_many_vectors(
         cls,
         descriptors: Iterable["DescriptorElement"]
     ) -> Generator[Tuple[Hashable, Optional[numpy.ndarray]], None, None]:
         # Memory elements are super simple.
@@ -34,15 +34,15 @@
             yield d.uuid(), d.vector()
 
     def __getstate__(self) -> Dict[str, Any]:
         state = super(DescriptorMemoryElement, self).__getstate__()
         # save vector as binary string
         b = BytesIO()
         # noinspection PyTypeChecker
-        numpy.save(b, self.vector())
+        numpy.save(b, self.vector())  # type: ignore
         state['v'] = b.getvalue()
         return state
 
     def __setstate__(self, state: Union[Sequence, Mapping[str, Any]]) -> None:
         # Handle the previous state format:
         if isinstance(state, Sequence):
             # Could state ever be a str/bytes instance? That would cause a problem if so.
@@ -76,15 +76,15 @@
             None of there is no vector stored in this container.
         """
         # Copy if storing an array, otherwise return the None value
         if self.__v is not None:
             return numpy.copy(self.__v)
         return None
 
-    def set_vector(self, new_vec: numpy.ndarray) -> "DescriptorMemoryElement":
+    def set_vector(self, new_vec: Optional[numpy.ndarray]) -> "DescriptorMemoryElement":
         """
         Set the contained vector.
 
         If this container already stores a descriptor vector, this will
         overwrite it.
 
         ``new_vec`` may be None, which clears this descriptor's vector from the
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/postgres.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/postgres.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_element/solr.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_element/solr.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_generator/caffe1.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/caffe1.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_generator/image_descriptor_generator_wrapper.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_generator/image_descriptor_generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/memory.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/memory.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/postgres.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,28 +175,33 @@
         self.element_col = element_col
 
         self.multiquery_batch_size = multiquery_batch_size
         self.pickle_protocol = pickle_protocol
         self.read_only = bool(read_only)
         self.create_table = create_table
 
+        assert -1 <= self.pickle_protocol <= 2, \
+            ("Given pickle protocol is not in the known valid range. Given: %s"
+             % self.pickle_protocol)
         # Checking parameters where necessary
         if self.multiquery_batch_size is not None:
             self.multiquery_batch_size = int(self.multiquery_batch_size)
             assert self.multiquery_batch_size > 0, \
                 "A given batch size must be greater than 0 in size " \
                 "(given: %d)." % self.multiquery_batch_size
-        assert -1 <= self.pickle_protocol <= 2, \
-            ("Given pickle protocol is not in the known valid range. Given: %s"
-             % self.pickle_protocol)
 
-        self.psql_helper = PsqlConnectionHelper(db_name, db_host, db_port,
-                                                db_user, db_pass,
-                                                self.multiquery_batch_size,
-                                                PSQL_TABLE_CREATE_RLOCK)
+            self.psql_helper = PsqlConnectionHelper(db_name, db_host, db_port,
+                                                    db_user, db_pass,
+                                                    itersize=self.multiquery_batch_size,
+                                                    table_upsert_lock=PSQL_TABLE_CREATE_RLOCK)
+        else:
+            self.psql_helper = PsqlConnectionHelper(db_name, db_host, db_port,
+                                                    db_user, db_pass,
+                                                    table_upsert_lock=PSQL_TABLE_CREATE_RLOCK)
+
         if not self.read_only and self.create_table:
             self.psql_helper.set_table_upsert_sql(
                 self.UPSERT_TABLE_TMPL.format(
                     table_name=self.table_name,
                     uuid_col=self.uuid_col,
                     element_col=self.element_col,
                 )
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/impls/descriptor_set/solr.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/impls/descriptor_set/solr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 import pickle
 import time
-from typing import Any, Deque, Dict, Generator, Hashable, Iterable, Mapping, Sequence, Tuple
+from typing import Any, Deque, Dict, Generator, Hashable, Iterable, Mapping, Optional, Sequence, Tuple
 
 from smqtk_descriptors import DescriptorElement, DescriptorSet
 
 # Try to import required module
 try:
     import solr  # type: ignore
 except ImportError:
@@ -34,15 +34,15 @@
         self,
         solr_conn_addr: str,
         set_uuid: str,
         set_uuid_field: str,
         d_uid_field: str,
         descriptor_field: str,
         timestamp_field: str,
-        solr_params: Dict[str, Any] = None,
+        solr_params: Optional[Dict[str, Any]] = None,
         commit_on_add: bool = True,
         max_boolean_clauses: int = 1024,
         pickle_protocol: int = -1
     ):
         """
         Construct a descriptor set pointing to a Solr instance.
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_element.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 T = TypeVar("T", bound="DescriptorElement")
 
 
 def _uuid_and_vector_from_descriptor(
     descriptor: "DescriptorElement"
-) -> Tuple[Hashable, numpy.ndarray]:
+) -> Tuple[Hashable, Optional[numpy.ndarray]]:
     """
     Given a descriptor, return a tuple containing the UUID and associated
     vector for that descriptor
 
     :param descriptor: The descriptor to process.
     :return: Tuple containing the UUID and associated vector for the given
         descriptor
@@ -54,15 +54,15 @@
         self._uuid = uuid
 
     def __hash__(self) -> int:
         return hash(self.uuid())
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, DescriptorElement):
-            return numpy.array_equal(self.vector(), other.vector())
+            return numpy.array_equal(self.vector(), other.vector())  # type: ignore
         return False
 
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}{{uuid: {self.uuid()}}}"
@@ -184,15 +184,15 @@
             batch_dictionary[type(descriptor_)].append(descriptor_)
             # Keep track of the order of descriptors to ensure that we return
             # vectors in the requested order after batching them out.
             uuid_indices[descriptor_.uuid()] = index
 
         # Default to None, since _get_many_vectors implementations can ignore
         # any descriptors that cannot be retrieved
-        ordered_vectors = [None] * (index + 1)
+        ordered_vectors = [None] * (index + 1)  # type: List[Optional[numpy.ndarray]]
 
         # Retrieve all the vectors for a given type of descriptor in a single
         # batch
         for _cls, descriptor_batch in batch_dictionary.items():
             # noinspection PyProtectedMember
             for uuid, vector in _cls._get_many_vectors(descriptor_batch):
                 ordered_vectors[uuid_indices[uuid]] = vector
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_generator.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_generator.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/descriptor_set.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/descriptor_set.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/interfaces/image_descriptor_generator.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/interfaces/image_descriptor_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import abc
-from typing import Iterable
+from typing import Iterable, Optional
 import numpy as np
 
 from smqtk_core import Configurable, Pluggable
 
 
 class ImageDescriptorGenerator (Configurable, Pluggable):
     """
     Algorithm that generates feature descriptor arrays for input image matrices
     as ``numpy.ndarray`` type arrays.
     """
 
     @abc.abstractmethod
     def generate_arrays_from_images(
         self,
-        img_mat_iter: Iterable[np.ndarray]
+        img_mat_iter: Iterable[Optional[np.ndarray]]
     ) -> Iterable[np.ndarray]:
         """
         Generate descriptor vector elements for input image matrices.
 
         :param img_mat_iter:
             Iterable of numpy arrays representing input image matrices.
```

### Comparing `smqtk_descriptors-0.18.1/smqtk_descriptors/utils/parallel.py` & `smqtk_descriptors-0.19.0/smqtk_descriptors/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `smqtk_descriptors-0.18.1/PKG-INFO` & `smqtk_descriptors-0.19.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: smqtk-descriptors
-Version: 0.18.1
+Version: 0.19.0
 Summary: Algorithms, data structures and utilities around computingdescriptor vectors from data.
 Home-page: https://github.com/Kitware/SMQTK-Descriptors
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: smqtk-developers@kitware.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy (>=1.19.5,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: pytorch
+Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: smqtk-core (>=0.18.0)
 Requires-Dist: smqtk-dataprovider (>=0.16.0)
-Requires-Dist: smqtk-image-io (>=0.16.2,<0.17.0)
+Requires-Dist: smqtk-image-io (>=0.16.2) ; python_version < "3.11"
+Requires-Dist: smqtk-image-io (>=0.17.0) ; python_version >= "3.11"
+Requires-Dist: torch (>=1.10.0,!=2.0.1) ; extra == "pytorch"
+Requires-Dist: torchvision (>=0.11.1) ; extra == "pytorch"
 Project-URL: Documentation, https://smqtk-descriptors.readthedocs.io/
 Project-URL: Repository, https://github.com/Kitware/SMQTK-Descriptors
 Description-Content-Type: text/markdown
 
 # SMQTK - Descriptors
 
 ## Intent
```

