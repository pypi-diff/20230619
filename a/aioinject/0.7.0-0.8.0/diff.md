# Comparing `tmp/aioinject-0.7.0.tar.gz` & `tmp/aioinject-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioinject-0.7.0.tar", last modified: Thu Jun 15 08:41:58 2023, max compression
+gzip compressed data, was "aioinject-0.8.0.tar", last modified: Mon Jun 19 06:31:31 2023, max compression
```

## Comparing `aioinject-0.7.0.tar` & `aioinject-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      429 2023-06-15 08:41:37.030861 aioinject-0.7.0/aioinject/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-09 04:28:13.918025 aioinject-0.7.0/aioinject/containers.py
--rw-r--r--   0        0        0     7191 2023-06-15 08:38:21.343298 aioinject-0.7.0/aioinject/context.py
--rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.7.0/aioinject/decorators.py
--rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.7.0/aioinject/ext/__init__.py
--rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.7.0/aioinject/ext/fastapi.py
--rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.7.0/aioinject/ext/strawberry.py
--rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.7.0/aioinject/markers.py
--rw-r--r--   0        0        0     6152 2023-06-15 08:40:09.657942 aioinject-0.7.0/aioinject/providers.py
--rw-r--r--   0        0        0     1078 2023-06-15 08:09:15.419129 aioinject-0.7.0/aioinject/utils.py
--rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.7.0/LICENSE
--rw-r--r--   0        0        0     1966 2023-06-15 08:41:37.095859 aioinject-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.7.0/readme.md
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/container/__init__.py
--rw-r--r--   0        0        0     3302 2023-06-15 07:30:36.661079 aioinject-0.7.0/tests/container/test_container.py
--rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.7.0/tests/container/test_override.py
--rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.7.0/tests/context/__init__.py
--rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.7.0/tests/context/conftest.py
--rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.7.0/tests/context/test_context.py
--rw-r--r--   0        0        0     4256 2023-06-15 08:37:09.906573 aioinject-0.7.0/tests/context/test_context_managers.py
--rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.7.0/tests/context/test_execute.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.7.0/tests/ext/strawberry/__init__.py
--rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.7.0/tests/ext/strawberry/test_inject_decorator.py
--rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.7.0/tests/providers/__init__.py
--rw-r--r--   0        0        0     4257 2023-06-15 08:40:10.535168 aioinject-0.7.0/tests/providers/test_callable.py
--rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.7.0/tests/providers/test_object.py
--rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.7.0/tests/providers/test_singleton.py
--rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.7.0/tests/test_inject.py
--rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.7.0/tests/utils/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.7.0/tests/utils/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.7.0/tests/utils/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.7.0/tests/utils/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.7.0/tests/utils/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.7.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1562 2023-06-15 08:40:10.557168 aioinject-0.7.0/tests/utils/test_guess_impl.py
--rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.7.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-06-19 06:31:17.724866 aioinject-0.8.0/aioinject/__init__.py
+-rw-r--r--   0        0        0     2675 2023-06-19 05:47:22.420243 aioinject-0.8.0/aioinject/containers.py
+-rw-r--r--   0        0        0     6161 2023-06-19 05:44:42.043586 aioinject-0.8.0/aioinject/context.py
+-rw-r--r--   0        0        0     3198 2023-02-19 10:45:20.646472 aioinject-0.8.0/aioinject/decorators.py
+-rw-r--r--   0        0        0        0 2022-06-21 12:45:09.224983 aioinject-0.8.0/aioinject/ext/__init__.py
+-rw-r--r--   0        0        0     1142 2023-02-19 10:46:32.417782 aioinject-0.8.0/aioinject/ext/fastapi.py
+-rw-r--r--   0        0        0      866 2023-03-25 23:51:07.879400 aioinject-0.8.0/aioinject/ext/strawberry.py
+-rw-r--r--   0        0        0      154 2022-02-14 23:34:38.786956 aioinject-0.8.0/aioinject/markers.py
+-rw-r--r--   0        0        0     6549 2023-06-19 05:47:07.031626 aioinject-0.8.0/aioinject/providers.py
+-rw-r--r--   0        0        0     1879 2023-06-19 05:44:42.060587 aioinject-0.8.0/aioinject/utils.py
+-rw-r--r--   0        0        0     1063 2022-02-10 14:33:31.888253 aioinject-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1966 2023-06-19 06:31:17.752865 aioinject-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5266 2022-05-25 14:51:11.254512 aioinject-0.8.0/readme.md
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.896255 aioinject-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.8.0/tests/container/__init__.py
+-rw-r--r--   0        0        0     3302 2023-06-15 07:30:36.661079 aioinject-0.8.0/tests/container/test_container.py
+-rw-r--r--   0        0        0      489 2023-02-18 10:15:01.863109 aioinject-0.8.0/tests/container/test_override.py
+-rw-r--r--   0        0        0        0 2022-02-14 23:35:15.649789 aioinject-0.8.0/tests/context/__init__.py
+-rw-r--r--   0        0        0      500 2023-02-18 10:10:22.057657 aioinject-0.8.0/tests/context/conftest.py
+-rw-r--r--   0        0        0     2022 2023-02-18 10:10:14.586441 aioinject-0.8.0/tests/context/test_context.py
+-rw-r--r--   0        0        0     4256 2023-06-17 18:05:12.793704 aioinject-0.8.0/tests/context/test_context_managers.py
+-rw-r--r--   0        0        0     2060 2023-02-18 11:02:03.522559 aioinject-0.8.0/tests/context/test_execute.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.8.0/tests/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524000 aioinject-0.8.0/tests/ext/strawberry/__init__.py
+-rw-r--r--   0        0        0      818 2023-02-18 11:06:42.742442 aioinject-0.8.0/tests/ext/strawberry/test_inject_decorator.py
+-rw-r--r--   0        0        0        0 2022-02-10 14:33:31.897254 aioinject-0.8.0/tests/providers/__init__.py
+-rw-r--r--   0        0        0     4257 2023-06-15 08:40:10.535168 aioinject-0.8.0/tests/providers/test_callable.py
+-rw-r--r--   0        0        0     1139 2023-02-18 11:02:25.628622 aioinject-0.8.0/tests/providers/test_object.py
+-rw-r--r--   0        0        0      686 2023-02-18 09:50:26.751944 aioinject-0.8.0/tests/providers/test_singleton.py
+-rw-r--r--   0        0        0     3845 2023-02-19 10:03:00.125198 aioinject-0.8.0/tests/test_inject.py
+-rw-r--r--   0        0        0       39 2022-08-16 11:16:21.152175 aioinject-0.8.0/tests/utils/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-16 11:16:21.153175 aioinject-0.8.0/tests/utils/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2022-08-16 11:16:21.152175 aioinject-0.8.0/tests/utils/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2022-08-16 11:16:21.153175 aioinject-0.8.0/tests/utils/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-16 11:16:21.154175 aioinject-0.8.0/tests/utils/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-02-19 10:38:23.524819 aioinject-0.8.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1562 2023-06-15 08:40:10.557168 aioinject-0.8.0/tests/utils/test_guess_impl.py
+-rw-r--r--   0        0        0      520 2023-02-18 11:01:50.087958 aioinject-0.8.0/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 aioinject-0.8.0/PKG-INFO
```

### Comparing `aioinject-0.7.0/aioinject/containers.py` & `aioinject-0.8.0/aioinject/containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import contextlib
 from collections import defaultdict
 from collections.abc import Generator
-from contextlib import AsyncExitStack
 from typing import Any, TypeVar
 
 from .context import InjectionContext, SyncInjectionContext
-from .providers import Provider
+from .providers import Provider, Singleton
 
 _T = TypeVar("_T")
 _Providers = dict[type[_T], list[Provider[_T]]]
 
 
 class Container:
     def __init__(self) -> None:
         self.providers: _Providers = defaultdict(list)
         self._overrides: _Providers = defaultdict(list)
-        self._exit_stack = AsyncExitStack()
 
     def register(
         self,
         provider: Provider[_T],
     ) -> None:
         if provider.type not in self.providers:
             self.providers[provider.type] = []
@@ -62,27 +60,28 @@
             err_msg = f"Provider for type {type_.__qualname__} not found"
             raise ValueError(err_msg)
         return provider
 
     def context(self) -> InjectionContext:
         return InjectionContext(
             container=self,
-            singleton_exit_stack=self._exit_stack,
         )
 
     def sync_context(self) -> SyncInjectionContext:
         return SyncInjectionContext(
             container=self,
-            singleton_exit_stack=self._exit_stack,
         )
 
     @contextlib.contextmanager
     def override(
         self,
         provider: Provider[_T],
     ) -> Generator[None, None, None]:
         self._overrides[provider.type].append(provider)
         yield
         self._overrides[provider.type].remove(provider)
 
     async def aclose(self) -> None:
-        await self._exit_stack.aclose()
+        for _, providers in self.providers.items():
+            for provider in providers:
+                if isinstance(provider, Singleton):
+                    await provider.aclose()
```

### Comparing `aioinject-0.7.0/aioinject/context.py` & `aioinject-0.8.0/aioinject/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import typing
 from collections.abc import Callable, Coroutine, Iterable
 from contextlib import AsyncExitStack, ExitStack
 from contextvars import ContextVar
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Generic, Protocol, TypeVar, Union
 
-from .providers import Dependency, Provider, Singleton
+from . import utils
+from .providers import Dependency
 
 if TYPE_CHECKING:
     from .containers import Container
 
 _T = TypeVar("_T")
 
 _AnyCtx = Union["InjectionContext", "SyncInjectionContext"]
@@ -40,49 +41,30 @@
 class _BaseInjectionContext(Generic[TExitStack]):
     _token: contextvars.Token | None
     _exit_stack_type: type[TExitStack]
 
     def __init__(
         self,
         container: Container,
-        singleton_exit_stack: AsyncExitStack,
     ) -> None:
         self.container = container
-        self.singleton_exit_stack = singleton_exit_stack
         self.exit_stack = self._exit_stack_type()
         self.cache: DICache = {}
         self._token = None
 
     def __class_getitem__(
         cls,
         item: type[TExitStack],
     ) -> _BaseInjectionContext[TExitStack]:
         return type(  # type: ignore[return-value]
             f"_BaseInjectionContext[{item.__class__.__name__}]",
             (cls,),
             {"_exit_stack_type": item},
         )
 
-    def _get_exit_stack(
-        self,
-        provider: Provider,
-    ) -> TExitStack | AsyncExitStack:
-        if isinstance(provider, Singleton):
-            return self.singleton_exit_stack
-        return self.exit_stack
-
-    def _update_singleton_cache(
-        self,
-        provider: Provider,
-        resolved_value: Any,
-    ) -> None:
-        if not isinstance(provider, Singleton):
-            return
-        provider.cache = resolved_value
-
 
 class InjectionContext(_BaseInjectionContext[AsyncExitStack]):
     async def resolve(
         self,
         type_: type[_T],
         impl: Any | None = None,
         *,
@@ -97,28 +79,19 @@
                 type_=dep.type_,
                 impl=dep.implementation,
                 use_cache=dep.use_cache,
             )
             for dep in provider.dependencies
         }
 
-        resolved = await provider.provide(**dependencies)
-        stack = self._get_exit_stack(provider=provider)
-
-        if isinstance(resolved, contextlib.ContextDecorator):
-            resolved = stack.enter_context(resolved)  # type: ignore[arg-type]
-
-        if isinstance(resolved, contextlib.AsyncContextDecorator):
-            resolved = await stack.enter_async_context(
-                resolved,  # type: ignore[arg-type]
-            )
-        self._update_singleton_cache(
-            provider=provider,
-            resolved_value=resolved,
+        resolved = utils.enter_context_maybe(
+            resolved=await provider.provide(**dependencies),
+            stack=self.exit_stack,
         )
+        resolved = await utils.await_maybe(resolved)
         if use_cache:
             self.cache[type_, impl] = resolved
         return resolved
 
     @typing.overload
     async def execute(
         self,
@@ -193,18 +166,14 @@
             )
             for dep in provider.dependencies
         }
 
         resolved = provider.provide_sync(**dependencies)
         if isinstance(resolved, contextlib.ContextDecorator):
             resolved = self.exit_stack.enter_context(resolved)  # type: ignore[arg-type]
-        self._update_singleton_cache(
-            provider=provider,
-            resolved_value=resolved,
-        )
         if use_cache:
             self.cache[type_, impl] = resolved
         return resolved
 
     def execute(
         self,
         function: Callable[..., _T],
```

### Comparing `aioinject-0.7.0/aioinject/decorators.py` & `aioinject-0.8.0/aioinject/decorators.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/aioinject/ext/fastapi.py` & `aioinject-0.8.0/aioinject/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/aioinject/ext/strawberry.py` & `aioinject-0.8.0/aioinject/ext/strawberry.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/aioinject/providers.py` & `aioinject-0.8.0/aioinject/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import asyncio
 import collections.abc
 import dataclasses
 import functools
 import inspect
 import threading
 import typing
-import typing as t
 from collections.abc import Iterable, Sequence
+from contextlib import AsyncExitStack
 from inspect import isclass
 from typing import Annotated, Any, Generic, TypeAlias
 
 from aioinject.markers import Inject
 
-_T = t.TypeVar("_T")
+from . import utils
+
+_T = typing.TypeVar("_T")
 
 
 @dataclasses.dataclass
 class Dependency(Generic[_T]):
     name: str
     type_: type[_T]
     implementation: Any
@@ -46,15 +48,15 @@
 
         if isinstance(arg, Inject):
             return arg
     return None
 
 
 def collect_dependencies(
-    dependant: t.Callable | dict[str, Any],
+    dependant: typing.Callable | dict[str, Any],
 ) -> Iterable[Dependency]:
     if not isinstance(dependant, dict):
         type_hints = typing.get_type_hints(dependant, include_extras=True)
     else:
         type_hints = dependant
 
     for name, hint in type_hints.items():
@@ -94,15 +96,15 @@
 }
 _ASYNC_GENERATORS = {
     collections.abc.AsyncGenerator,
     collections.abc.AsyncIterator,
 }
 
 
-def _guess_impl(factory: t.Callable[..., Any]) -> type:
+def _guess_impl(factory: typing.Callable[..., Any]) -> type:
     if isclass(factory):
         return factory
     type_hints = typing.get_type_hints(factory)
     try:
         return_type = type_hints["return"]
     except KeyError as e:
         err_msg = (
@@ -125,15 +127,15 @@
         if origin in _GENERATORS and inspect.isgeneratorfunction(
             maybe_wrapped,
         ):
             return args[0]
     return return_type
 
 
-class Provider(t.Generic[_T], abc.ABC):
+class Provider(Generic[_T], abc.ABC):
     def __init__(self, type_: type[_T], impl: Any) -> None:
         self.type = type_
         self.impl = impl
 
     @abc.abstractmethod
     def provide_sync(self, **kwargs: Any) -> _T:
         raise NotImplementedError
@@ -154,15 +156,15 @@
     def dependencies(self) -> Sequence[Dependency]:
         return tuple(collect_dependencies(self.type_hints))
 
 
 class Callable(Provider[_T]):
     def __init__(
         self,
-        factory: t.Callable[..., _T] | type[_T],
+        factory: typing.Callable[..., _T] | type[_T],
         type_: type[_T] | None = None,
     ) -> None:
         super().__init__(
             type_=type_ or _guess_impl(factory),
             impl=factory,
         )
 
@@ -185,35 +187,43 @@
     def is_async(self) -> bool:
         return inspect.iscoroutinefunction(self.impl)
 
 
 class Singleton(Callable, Generic[_T]):
     def __init__(
         self,
-        factory: t.Callable[..., _T] | type[_T],
+        factory: typing.Callable[..., _T] | type[_T],
         type_: type[_T] | None = None,
     ) -> None:
         super().__init__(factory=factory, type_=type_)
         self.cache: _T | None = None
         self._lock = threading.Lock()
         self._async_lock = asyncio.Lock()
+        self._exit_stack = AsyncExitStack()
 
     def provide_sync(self, **kwargs: Any) -> _T:
         if self.cache is None:
             with self._lock:
                 if self.cache is None:
                     self.cache = super().provide_sync(**kwargs)
         return self.cache
 
     async def provide(self, **kwargs: Any) -> _T:
         if self.cache is None:
             async with self._async_lock:
                 if self.cache is None:
-                    self.cache = await super().provide(**kwargs)
-        return self.cache
+                    awaitable = utils.enter_context_maybe(
+                        await super().provide(**kwargs),
+                        self._exit_stack,
+                    )
+                    self.cache = await utils.await_maybe(awaitable)
+        return self.cache  # type: ignore[return-value]
+
+    async def aclose(self) -> None:
+        await self._exit_stack.aclose()
 
 
 class Object(Provider[_T]):
     is_async = False
     type_hints: dict[str, Any] = {}
 
     def __init__(
```

### Comparing `aioinject-0.7.0/LICENSE` & `aioinject-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/pyproject.toml` & `aioinject-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 composite = [
     "coverage run",
     "coverage report",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.8.0"
 version_files = [
     "aioinject/__init__.py",
     "pyproject.toml:version",
 ]
 
 [tool.coverage.run]
 source = [
@@ -108,15 +108,15 @@
 ]
 staticmethod-decorators = [
     "staticmethod",
 ]
 
 [project]
 name = "aioinject"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = [
     { name = "Doctor", email = "thirvondukr@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "readme.md"
```

### Comparing `aioinject-0.7.0/readme.md` & `aioinject-0.8.0/readme.md`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/container/test_container.py` & `aioinject-0.8.0/tests/container/test_container.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/context/test_context.py` & `aioinject-0.8.0/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/context/test_context_managers.py` & `aioinject-0.8.0/tests/context/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/context/test_execute.py` & `aioinject-0.8.0/tests/context/test_execute.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/ext/strawberry/test_inject_decorator.py` & `aioinject-0.8.0/tests/ext/strawberry/test_inject_decorator.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/providers/test_callable.py` & `aioinject-0.8.0/tests/providers/test_callable.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/providers/test_object.py` & `aioinject-0.8.0/tests/providers/test_object.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/providers/test_singleton.py` & `aioinject-0.8.0/tests/providers/test_singleton.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/test_inject.py` & `aioinject-0.8.0/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/utils/test_guess_impl.py` & `aioinject-0.8.0/tests/utils/test_guess_impl.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/tests/utils/test_utils.py` & `aioinject-0.8.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `aioinject-0.7.0/PKG-INFO` & `aioinject-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioinject
-Version: 0.7.0
+Version: 0.8.0
 License: MIT
 Author-email: Doctor <thirvondukr@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 Async-first dependency injection library based on python type hints
```

