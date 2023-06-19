# Comparing `tmp/asynkit-0.9.1.tar.gz` & `tmp/asynkit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynkit-0.9.1.tar", max compression
+gzip compressed data, was "asynkit-0.9.2.tar", max compression
```

## Comparing `asynkit-0.9.1.tar` & `asynkit-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1081 2023-06-04 21:35:04.612865 asynkit-0.9.1/LICENSE
--rw-r--r--   0        0        0    22751 2023-06-04 21:35:04.612865 asynkit-0.9.1/README.md
--rw-r--r--   0        0        0     2078 2023-06-04 21:35:04.616865 asynkit-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/compat.py
--rw-r--r--   0        0        0    17639 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/coroutine.py
--rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/experimental/__init__.py
--rw-r--r--   0        0        0     4293 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/experimental/anyio.py
--rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/default.py
--rw-r--r--   0        0        0     4815 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/eventloop.py
--rw-r--r--   0        0        0     2981 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/extensions.py
--rw-r--r--   0        0        0     2922 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/schedulingloop.py
--rw-r--r--   0        0        0      281 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/loop/types.py
--rw-r--r--   0        0        0    10720 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/monitor.py
--rw-r--r--   0        0        0        0 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/py.typed
--rw-r--r--   0        0        0     5352 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/scheduling.py
--rw-r--r--   0        0        0     1209 2023-06-04 21:35:04.616865 asynkit-0.9.1/src/asynkit/tools.py
--rw-r--r--   0        0        0    23701 1970-01-01 00:00:00.000000 asynkit-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-19 14:37:49.787008 asynkit-0.9.2/LICENSE
+-rw-r--r--   0        0        0    22490 2023-06-19 14:37:49.787008 asynkit-0.9.2/README.md
+-rw-r--r--   0        0        0     2101 2023-06-19 14:37:49.787008 asynkit-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/compat.py
+-rw-r--r--   0        0        0    17148 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/coroutine.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/experimental/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/experimental/anyio.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/default.py
+-rw-r--r--   0        0        0     4815 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/eventloop.py
+-rw-r--r--   0        0        0     2981 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/extensions.py
+-rw-r--r--   0        0        0     2922 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/schedulingloop.py
+-rw-r--r--   0        0        0      281 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/loop/types.py
+-rw-r--r--   0        0        0    10720 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/monitor.py
+-rw-r--r--   0        0        0        0 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/py.typed
+-rw-r--r--   0        0        0     5352 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/scheduling.py
+-rw-r--r--   0        0        0     1209 2023-06-19 14:37:49.787008 asynkit-0.9.2/src/asynkit/tools.py
+-rw-r--r--   0        0        0    23440 1970-01-01 00:00:00.000000 asynkit-0.9.2/PKG-INFO
```

### Comparing `asynkit-0.9.1/LICENSE` & `asynkit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/README.md` & `asynkit-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -113,106 +113,91 @@
 
 If you are writing code which should work both synchronously and asynchronously,
 you can now write the code fully _async_ and then run it _synchronously_ in the absence
 of an event loop.  As long as the code doesn't _block_ (await unfinished _futures_) and doesn't try to access the event loop, it can successfully be executed.  This helps avoid writing duplicate code.
 
 ```python
 async def async_get_processed_data(datagetter):
-    data = datagetter()  # could be an async callback
+    data = datagetter()  # an optionally async callback
     data = await data if isawaitable(data) else data
     return process_data(data)
 
 
 # raises SynchronousError if datagetter blocks
 def sync_get_processed_data(datagetter):
     return asynkit.coro_sync(async_get_processed_data(datagetter))
 ```
 
 This sort of code might previously have been written thus:
 
 ```python
-# may return an awaitable
-def get_processed_data(datagetter):
+# A hybrid function, _may_ return an _awaitable_
+def hybrid_get_processed_data(datagetter):
     data = datagetter()
     if isawaitable(data):
-        # return an awaitable helper function
+        # return an awaitable helper closure
         async def helper():
             data = await data
             return process_data(data)
 
         return helper
     return process_data(data)  # duplication
 
 
 async def async_get_processed_data(datagetter):
-    r = get_processed_data(datagetter)
+    r = hybrid_get_processed_data(datagetter)
     return await r if isawaitable(r) else r
 
 
 def sync_get_processed_data(datagetter):
-    r = get_processed_data(datagetter)
+    r = hybrid_get_processed_data(datagetter)
     if isawaitable(r):
         raise RuntimeError("callbacks failed to run synchronously")
     return r
 ```
 
 The above pattern, writing async methods as sync and returning async helpers,
 is common in library code which needs to work both in synchronous and asynchronous
 context.  Needless to say, it is very convoluted, hard to debug and contains a lot
-of code duplication where the same logic is repeated inside async helper methods.
+of code duplication where the same logic is repeated inside async helper closures.
 
 Using `coro_sync()` it is possible to write the entire logic as `async` methods and
 then simply fail if the code tries to invoke any truly async operations.
 If the invoked coroutine blocks, a `SynchronousError` is raised _from_ a `SynchronousAbort` exception which
 contains a traceback.  This makes it easy to pinpoint the location in the code where the
 async code blocked.  If the code tries to access the event loop, e.g. by creating a `Task`, a `RuntimeError` will be raised.  
 
-
-`coro_sync()` can also be applied as a decorator:
+The `syncfunction()` decorator can be used to automatically wrap an async function
+so that it is executed using `coro_sync()`:
 
 ```pycon
->>> @asynkit.coro_sync
+>>> @asynkit.syncfunction
 ... async def sync_function():
 ...     async def async_function():
 ...         return "look, no async!"
 ...     return await async_function()
 ...
 >>> sync_function()
 'look, no async!'
 >>>
 ```
 
-the `ensure_corofunc()` utility can be used when passing callbacks to async
-code, to ensure that the callbacks are async.  This, with `coro_sync()`, can help integrate
-synchronous code with async middleware:
+the `asyncfunction()` utility can be used when passing synchronous callbacks to async
+code, to make them async.  This, along with `syncfunction()` and `coro_sync()`,
+can be used to integrate synchronous code with async middleware:
 
 ```python
-def sync_client(sync_callback):
-    middleware = AsyncMiddleware(asynkit.ensure_corofunc(sync_callback))
-    return asynkit.coro_sync(middleware.run())
+@asynkit.syncfunction
+async def sync_client(sync_callback):
+    middleware = AsyncMiddleware(asynkit.asyncfunction(sync_callback))
+    return await middleware.run()
 ```
 
-Using this pattern, one can avoid writing special synchronous versions of middleware, or having
-_hybrid_ methods which _optionally_ return awaitables:
-
-```python
-# the hybrid method antipattern
-def hybrid_method(callable):
-    """A hybrid method, possibly returning awaitable"""
-    data = callable()
-    if isawaitable(data):
-        # inner async method with duplicate code
-        async def async_helper(data):
-            data2 = await data
-            return process_data(data2)
-
-        return async_helper
-    else:
-        return process_data(data)  # duplicate code
-```
+Using this pattern, one can write the middleware completely async, make it also work
+for synchronous code, while avoiding the hybrid function _antipattern._
 
 ## `CoroStart`
 
 This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
 an exception.  It can subsequently be _awaited_ to retreive the result.
```

### Comparing `asynkit-0.9.1/pyproject.toml` & `asynkit-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asynkit"
-version = "0.9.1"
+version = "0.9.2"
 description = "Async toolkit for advanced scheduling"
 authors = ["Kristján Valur Jónsson <sweskman@gmail.com>"]
 repository = "https://github.com/kristjanvalur/py-asynkit"
 readme = "README.md"
 keywords = ["asyncio", "eventloop"]
 license = "MIT"
 classifiers = [
@@ -71,14 +71,15 @@
 allow_untyped_calls = true
 
 [[tool.mypy.overrides]]
 module = [
     "asynkit.loop.eventloop",
     "asynkit.compat",
     "asynkit.tools",
+    "tests.test_coro",
 ]
 warn_unused_ignores=false
 
 [[tool.mypy.overrides]]
 module = "asynkit.compat"
 disable_error_code="call-arg"
```

### Comparing `asynkit-0.9.1/src/asynkit/compat.py` & `asynkit-0.9.2/src/asynkit/compat.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/coroutine.py` & `asynkit-0.9.2/src/asynkit/coroutine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import functools
 import inspect
 import sys
 import types
 from contextvars import Context, copy_context
-from inspect import iscoroutinefunction
 from types import FrameType
 from typing import (
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Coroutine,
@@ -30,23 +29,24 @@
 __all__ = [
     "CoroStart",
     "awaitmethod",
     "coro_await",
     "coro_eager",
     "func_eager",
     "eager",
-    "ensure_corofunc",
     "coro_get_frame",
     "coro_is_new",
     "coro_is_suspended",
     "coro_is_finished",
     "coro_iter",
     "coro_sync",
     "SynchronousError",
     "SynchronousAbort",
+    "asyncfunction",
+    "syncfunction",
 ]
 
 PYTHON_37 = sys.version_info.major == 3 and sys.version_info.minor == 7
 
 T = TypeVar("T")
 S = TypeVar("S")
 P = ParamSpec("P")
@@ -501,44 +501,18 @@
     @functools.wraps(func)
     def wrapper(self: S) -> Iterator[T]:
         return coro_iter(func(self))
 
     return wrapper
 
 
-@overload
 def coro_sync(coro: Coroutine[Any, Any, T]) -> T:
-    ...
-
-
-@overload
-def coro_sync(coro: Callable[P, Coroutine[Any, Any, T]]) -> Callable[P, T]:
-    ...
-
-
-def coro_sync(
-    coro: Union[Coroutine[Any, Any, T], Callable[P, Coroutine[Any, Any, T]]]
-) -> Union[T, Callable[P, T]]:
-
     """Runs a corouting synchronlously.  If the coroutine blocks, a
     SynchronousError is raised.
-
-    Can also be used as a decorator for an async function.
     """
-    if iscoroutinefunction(coro):
-        # we are a decorator
-        coro2 = cast(Callable[..., Coroutine[Any, Any, T]], coro)
-
-        @functools.wraps(coro)
-        def helper(*args: Any, **kwargs: Any) -> T:
-            return coro_sync(coro2(*args, **kwargs))
-
-        return helper
-    coro = cast(Coroutine[Any, Any, T], coro)
-    # We are running a coroutine synchronously
     start = CoroStart[T](coro)
     if start.done():
         return start.result()
     # kill the coroutine
     try:
         # we can't use GeneratorExit because that gets special handling and
         # a traceback is not collected.
@@ -552,21 +526,29 @@
     finally:
         try:
             start.close()
         except RuntimeError:
             pass
 
 
-def ensure_corofunc(
-    callable: Union[Callable[P, T], Callable[P, Coroutine[Any, Any, T]]]
-) -> Callable[P, Coroutine[Any, Any, T]]:
-    """Make a callable async, so that the result needs to be awaited.
-    Useful for adding synchronous callbacs to async code.
+def syncfunction(func: Callable[P, Coroutine[Any, Any, T]]) -> Callable[P, T]:
+    """Make an async function synchronous, by invoking
+    `coro_sync()` on its coroutine.  Useful as a decorator.
     """
-    if inspect.iscoroutinefunction(callable):
-        return callable
 
+    @functools.wraps(func)
+    def helper(*args: P.args, **kwargs: P.kwargs) -> T:
+        return coro_sync(func(*args, **kwargs))
+
+    return helper
+
+
+def asyncfunction(func: Callable[P, T]) -> Callable[P, Coroutine[Any, Any, T]]:
+    """Make a regular function async, so that its result needs to be awaited.
+    Useful when providing synchronous callbacks to async code.
+    """
+
+    @functools.wraps(func)
     async def helper(*args: P.args, **kwargs: P.kwargs) -> T:
-        callable2 = cast(Callable[P, T], callable)
-        return callable2(*args, **kwargs)
+        return func(*args, **kwargs)
 
     return helper
```

### Comparing `asynkit-0.9.1/src/asynkit/experimental/anyio.py` & `asynkit-0.9.2/src/asynkit/experimental/anyio.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/loop/default.py` & `asynkit-0.9.2/src/asynkit/loop/default.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/loop/eventloop.py` & `asynkit-0.9.2/src/asynkit/loop/eventloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/loop/extensions.py` & `asynkit-0.9.2/src/asynkit/loop/extensions.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/loop/schedulingloop.py` & `asynkit-0.9.2/src/asynkit/loop/schedulingloop.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/monitor.py` & `asynkit-0.9.2/src/asynkit/monitor.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/scheduling.py` & `asynkit-0.9.2/src/asynkit/scheduling.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/src/asynkit/tools.py` & `asynkit-0.9.2/src/asynkit/tools.py`

 * *Files identical despite different names*

### Comparing `asynkit-0.9.1/PKG-INFO` & `asynkit-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Async toolkit for advanced scheduling
 Home-page: https://github.com/kristjanvalur/py-asynkit
 License: MIT
 Keywords: asyncio,eventloop
 Author: Kristján Valur Jónsson
 Author-email: sweskman@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -137,106 +137,91 @@
 
 If you are writing code which should work both synchronously and asynchronously,
 you can now write the code fully _async_ and then run it _synchronously_ in the absence
 of an event loop.  As long as the code doesn't _block_ (await unfinished _futures_) and doesn't try to access the event loop, it can successfully be executed.  This helps avoid writing duplicate code.
 
 ```python
 async def async_get_processed_data(datagetter):
-    data = datagetter()  # could be an async callback
+    data = datagetter()  # an optionally async callback
     data = await data if isawaitable(data) else data
     return process_data(data)
 
 
 # raises SynchronousError if datagetter blocks
 def sync_get_processed_data(datagetter):
     return asynkit.coro_sync(async_get_processed_data(datagetter))
 ```
 
 This sort of code might previously have been written thus:
 
 ```python
-# may return an awaitable
-def get_processed_data(datagetter):
+# A hybrid function, _may_ return an _awaitable_
+def hybrid_get_processed_data(datagetter):
     data = datagetter()
     if isawaitable(data):
-        # return an awaitable helper function
+        # return an awaitable helper closure
         async def helper():
             data = await data
             return process_data(data)
 
         return helper
     return process_data(data)  # duplication
 
 
 async def async_get_processed_data(datagetter):
-    r = get_processed_data(datagetter)
+    r = hybrid_get_processed_data(datagetter)
     return await r if isawaitable(r) else r
 
 
 def sync_get_processed_data(datagetter):
-    r = get_processed_data(datagetter)
+    r = hybrid_get_processed_data(datagetter)
     if isawaitable(r):
         raise RuntimeError("callbacks failed to run synchronously")
     return r
 ```
 
 The above pattern, writing async methods as sync and returning async helpers,
 is common in library code which needs to work both in synchronous and asynchronous
 context.  Needless to say, it is very convoluted, hard to debug and contains a lot
-of code duplication where the same logic is repeated inside async helper methods.
+of code duplication where the same logic is repeated inside async helper closures.
 
 Using `coro_sync()` it is possible to write the entire logic as `async` methods and
 then simply fail if the code tries to invoke any truly async operations.
 If the invoked coroutine blocks, a `SynchronousError` is raised _from_ a `SynchronousAbort` exception which
 contains a traceback.  This makes it easy to pinpoint the location in the code where the
 async code blocked.  If the code tries to access the event loop, e.g. by creating a `Task`, a `RuntimeError` will be raised.  
 
-
-`coro_sync()` can also be applied as a decorator:
+The `syncfunction()` decorator can be used to automatically wrap an async function
+so that it is executed using `coro_sync()`:
 
 ```pycon
->>> @asynkit.coro_sync
+>>> @asynkit.syncfunction
 ... async def sync_function():
 ...     async def async_function():
 ...         return "look, no async!"
 ...     return await async_function()
 ...
 >>> sync_function()
 'look, no async!'
 >>>
 ```
 
-the `ensure_corofunc()` utility can be used when passing callbacks to async
-code, to ensure that the callbacks are async.  This, with `coro_sync()`, can help integrate
-synchronous code with async middleware:
+the `asyncfunction()` utility can be used when passing synchronous callbacks to async
+code, to make them async.  This, along with `syncfunction()` and `coro_sync()`,
+can be used to integrate synchronous code with async middleware:
 
 ```python
-def sync_client(sync_callback):
-    middleware = AsyncMiddleware(asynkit.ensure_corofunc(sync_callback))
-    return asynkit.coro_sync(middleware.run())
+@asynkit.syncfunction
+async def sync_client(sync_callback):
+    middleware = AsyncMiddleware(asynkit.asyncfunction(sync_callback))
+    return await middleware.run()
 ```
 
-Using this pattern, one can avoid writing special synchronous versions of middleware, or having
-_hybrid_ methods which _optionally_ return awaitables:
-
-```python
-# the hybrid method antipattern
-def hybrid_method(callable):
-    """A hybrid method, possibly returning awaitable"""
-    data = callable()
-    if isawaitable(data):
-        # inner async method with duplicate code
-        async def async_helper(data):
-            data2 = await data
-            return process_data(data2)
-
-        return async_helper
-    else:
-        return process_data(data)  # duplicate code
-```
+Using this pattern, one can write the middleware completely async, make it also work
+for synchronous code, while avoiding the hybrid function _antipattern._
 
 ## `CoroStart`
 
 This class manages the state of a partially run coroutine and is what what powers the `coro_eager()` and `coro_sync()` functions. 
 When initialized, it will _start_ the coroutine, running it until it either suspends, returns, or raises
 an exception.  It can subsequently be _awaited_ to retreive the result.
```

