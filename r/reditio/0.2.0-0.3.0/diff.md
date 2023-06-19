# Comparing `tmp/reditio-0.2.0.tar.gz` & `tmp/reditio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reditio-0.2.0.tar", last modified: Wed May 24 07:06:06 2023, max compression
+gzip compressed data, was "reditio-0.3.0.tar", last modified: Mon Jun 19 05:57:35 2023, max compression
```

## Comparing `reditio-0.2.0.tar` & `reditio-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-24 07:06:06.802451 reditio-0.2.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-05-07 04:13:06.000000 reditio-0.2.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-24 07:06:06.802451 reditio-0.2.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1688 2023-05-07 06:13:23.000000 reditio-0.2.0/README.md
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-24 07:06:06.802451 reditio-0.2.0/reditio.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      191 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       29 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        8 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3604 2023-05-24 07:04:37.000000 reditio-0.2.0/reditio.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-24 07:06:06.802451 reditio-0.2.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      741 2023-05-24 07:05:40.000000 reditio-0.2.0/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-19 05:57:35.901038 reditio-0.3.0/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-05-07 04:13:06.000000 reditio-0.3.0/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      617 2023-06-19 05:57:35.901038 reditio-0.3.0/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1688 2023-05-07 06:13:23.000000 reditio-0.3.0/README.md
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-06-19 05:57:35.901038 reditio-0.3.0/reditio.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      617 2023-06-19 05:57:35.000000 reditio-0.3.0/reditio.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      191 2023-06-19 05:57:35.000000 reditio-0.3.0/reditio.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-06-19 05:57:35.000000 reditio-0.3.0/reditio.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       29 2023-06-19 05:57:35.000000 reditio-0.3.0/reditio.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        8 2023-06-19 05:57:35.000000 reditio-0.3.0/reditio.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     4509 2023-06-19 05:55:46.000000 reditio-0.3.0/reditio.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-06-19 05:57:35.901038 reditio-0.3.0/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      741 2023-06-19 05:57:12.000000 reditio-0.3.0/setup.py
```

### Comparing `reditio-0.2.0/LICENSE` & `reditio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reditio-0.2.0/PKG-INFO` & `reditio-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: reditio
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple typed Python interface to Redis
 Home-page: https://github.com/MatthewScholefield/reditio
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: reditio
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `reditio-0.2.0/README.md` & `reditio-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `reditio-0.2.0/reditio.egg-info/PKG-INFO` & `reditio-0.3.0/reditio.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: reditio
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple typed Python interface to Redis
 Home-page: https://github.com/MatthewScholefield/reditio
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
+License: UNKNOWN
 Keywords: reditio
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: dev
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `reditio-0.2.0/reditio.py` & `reditio-0.3.0/reditio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from redis import Redis
 from pydantic import BaseModel, StrBytes
-from typing import Optional, Type, List, Dict, TypeVar, Generic
+from typing import Any, Optional, Type, List, Dict, TypeVar, Generic
 
 T = TypeVar('T', BaseModel, str)
+ContainerSubtype = TypeVar('ContainerSubtype', bound='RedisContainer')
 
 
 class RedisContainer(Generic[T]):
     def __init__(
         self,
         key: str,
         model: Type[T] = str,
         redis: Redis = Redis(),
     ):
         self.key = key
         self.model = model
         self.red = redis
 
+    def to_template(self: ContainerSubtype) -> 'RedisContainerTemplate[ContainerSubtype]':
+        return RedisContainerTemplate(self.key, self.model, self.red, self.__class__)
+
     def _parse_key(self, value: StrBytes) -> str:
         if isinstance(value, bytes):
             return value.decode()
         return value
 
     def _parse_value(self, value: StrBytes) -> Optional[T]:
         if not value:
             return None
         if issubclass(self.model, BaseModel):
             return self.model.parse_raw(value)
         if not issubclass(self.model, (str, bytes)):
             raise RuntimeError(f'Invalid model type: {self.model}')
+        if isinstance(value, bytes):
+            return value.decode()
         return value
 
     def _serialize_value(self, value: T) -> StrBytes:
         if self.model is not str:
             return value.json()
         return value
 
@@ -41,26 +47,45 @@
         return self._parse_value(self.red.get(self.key))
 
     def set(self, value: T):
         serialized_value = self._serialize_value(value)
         self.red.set(self.key, serialized_value)
 
 
+class RedisContainerTemplate(Generic[ContainerSubtype]):
+    def __init__(
+        self,
+        key_template: str,
+        model: Type[T],
+        redis: Redis,
+        container_type: Type[ContainerSubtype]
+    ):
+        super().__init__()
+        self.key_template = key_template
+        self.model = model
+        self.redis = redis
+        self.container_type = container_type
+
+    def __call__(self, *args: Any, **kwargs: Any) -> ContainerSubtype:
+        key = self.key_template.format(*args, **kwargs)
+        return self.container_type(key, self.model, self.redis)
+
+
 class RList(Generic[T], RedisContainer[T]):
     def getrange(self, start: int, end: int) -> List[T]:
         return [
             self._parse_value(v) for v in self.red.lrange(self.key, start, end)
         ]
 
     def append(self, value: T):
         serialized_value = self._serialize_value(value)
         self.red.rpush(self.key, serialized_value)
 
     def bpop(self, timeout=0) -> Optional[T]:
-        return self._parse_value(self.red.blpop(self.key, timeout))
+        return self._parse_value(self.red.blpop(self.key, timeout)[1])
 
 
 class RSet(Generic[T], RedisContainer[T]):
     def members(self) -> list[T]:
         return [self._parse_value(v) for v in self.red.smembers(self.key)]
 
     def add(self, value: T):
```

### Comparing `reditio-0.2.0/setup.py` & `reditio-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='reditio',
-    version='0.2.0',
+    version='0.3.0',
     description='Simple typed Python interface to Redis',
     url='https://github.com/MatthewScholefield/reditio',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

