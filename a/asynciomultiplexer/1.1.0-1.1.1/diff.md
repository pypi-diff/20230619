# Comparing `tmp/asynciomultiplexer-1.1.0.tar.gz` & `tmp/asynciomultiplexer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynciomultiplexer-1.1.0.tar", last modified: Tue Jun  6 04:05:40 2023, max compression
+gzip compressed data, was "asynciomultiplexer-1.1.1.tar", last modified: Mon Jun 19 21:02:35 2023, max compression
```

## Comparing `asynciomultiplexer-1.1.0.tar` & `asynciomultiplexer-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.0/LICENSE
--rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.0/README.md
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/setup.cfg
--rw-rw-r--   0 pi        (1000) pi        (1000)      345 2023-06-06 04:05:06.000000 asynciomultiplexer-1.1.0/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.495728 asynciomultiplexer-1.1.0/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/src/asynciomultiplexer/
--rw-rw-r--   0 pi        (1000) pi        (1000)     5868 2023-06-06 04:00:41.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer/asynciomultiplexer.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      281 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       19 2023-06-06 04:05:40.000000 asynciomultiplexer-1.1.0/src/asynciomultiplexer.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-06 04:05:40.499729 asynciomultiplexer-1.1.0/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     1324 2023-06-06 04:03:49.000000 asynciomultiplexer-1.1.0/test/test_multiplexing.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1490 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.1/LICENSE
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      106 2023-05-29 22:44:19.000000 asynciomultiplexer-1.1.1/README.md
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      345 2023-06-19 21:01:35.000000 asynciomultiplexer-1.1.1/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/src/asynciomultiplexer/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6014 2023-06-19 21:01:19.000000 asynciomultiplexer-1.1.1/src/asynciomultiplexer/asynciomultiplexer.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/src/asynciomultiplexer.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      138 2023-06-19 21:02:35.000000 asynciomultiplexer-1.1.1/src/asynciomultiplexer.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      281 2023-06-19 21:02:35.000000 asynciomultiplexer-1.1.1/src/asynciomultiplexer.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-19 21:02:35.000000 asynciomultiplexer-1.1.1/src/asynciomultiplexer.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       19 2023-06-19 21:02:35.000000 asynciomultiplexer-1.1.1/src/asynciomultiplexer.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-19 21:02:35.836283 asynciomultiplexer-1.1.1/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1324 2023-06-06 04:03:49.000000 asynciomultiplexer-1.1.1/test/test_multiplexing.py
```

### Comparing `asynciomultiplexer-1.1.0/LICENSE` & `asynciomultiplexer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asynciomultiplexer-1.1.0/src/asynciomultiplexer/asynciomultiplexer.py` & `asynciomultiplexer-1.1.1/src/asynciomultiplexer/asynciomultiplexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 multiplexing utils for parallel (async) tasks
 """
 
 import asyncio
 import queue
 from contextlib import suppress
-from typing import AsyncIterator, TypeVar, Generic, Optional, Callable, AsyncGenerator
+from typing import AsyncIterator, TypeVar, Generic, Optional, Coroutine, Callable, Awaitable
 
 __all__ = ["AsyncMultiplexedIterator", "AsyncAdaptorQueue"]
 T = TypeVar('T')
 
 
 class AsyncMultiplexedIterator(Generic[T]):
     """
@@ -29,21 +29,21 @@
             self._iterator = iterator
 
         @property
         def iterator(self) -> AsyncIterator[T]:
             return self._iterator
 
     def __init__(self, *iterators: AsyncIterator[T], timeout=0,
-                 handle_orphan: Optional[Callable[[T], None]] = None):
+                 handle_orphan: Optional[Callable[[T], Awaitable[None]]] = None):
         """
         :param iterators: which iterators to iterate over in parallel
         :param timeout: timeout in seconds to wait on next item, or default/zero to wait indefinitely
         :param handle_orphan: optional callback to handle orphaned items.  An itme is orphaned when
             the multiplexer exits early but the client inserts an item into the multiplexing queue
-            AFTER the multiplexer stops processing the queue but BEFORE it has properly shutdown
+            AFTER the multiplexer stops processing the queue, but BEFORE it has properly shutdown
             all the workers.  Any exceptions from this handler will be ignored and not propagated.
         """
         self._iterators = list(iterators)
         self._multiplexing_q: asyncio.Queue[T] = asyncio.Queue()
         self._timeout = timeout
         self._handle_orphan = handle_orphan
         self._active = False
@@ -51,19 +51,21 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         self._active = False
         for task in [t for t in self._tasks if not t.done()]:
             await task
-        while self._handle_orphan is not None:  # always True or False
+        while self._handle_orphan is not None:  # always either True or False, should never change during lifetime
             try:
                 item = self._multiplexing_q.get_nowait()
+                if isinstance(item, self.Sentinel):
+                    break
                 with suppress(Exception):
-                    self._handle_orphan(item)
+                    await self._handle_orphan(item)
             except asyncio.queues.QueueEmpty:
                 break
 
     def __aiter__(self) -> "AsyncMultiplexedIterator[T]":
         async def worker(iterator: AsyncIterator[T]):
             try:
                 async for item in iterator:
```

### Comparing `asynciomultiplexer-1.1.0/test/test_multiplexing.py` & `asynciomultiplexer-1.1.1/test/test_multiplexing.py`

 * *Files identical despite different names*

