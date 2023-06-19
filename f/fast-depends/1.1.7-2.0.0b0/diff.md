# Comparing `tmp/fast_depends-1.1.7.tar.gz` & `tmp/fast_depends-2.0.0b0.tar.gz`

## Comparing `fast_depends-1.1.7.tar` & `fast_depends-2.0.0b0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/__init__.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/construct.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/injector.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/model.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/provider.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/types.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/usage.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.7/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.7/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.7/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.7/README.md
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/_compat.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/types.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/use.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/build.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/README.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/PKG-INFO
```

### Comparing `fast_depends-1.1.7/CONTRIBUTING.md` & `fast_depends-2.0.0b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/.github/workflows/documentation.yml` & `fast_depends-2.0.0b0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.0b0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.0b0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/.github/workflows/tests.yml` & `fast_depends-2.0.0b0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/fast_depends/utils.py` & `fast_depends-2.0.0b0/fast_depends/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,97 @@
-import asyncio
 import functools
 import inspect
 from contextlib import AsyncExitStack, ExitStack, asynccontextmanager, contextmanager
 from typing import (
     Any,
     AsyncGenerator,
     Callable,
     ContextManager,
     Dict,
+    ForwardRef,
     Iterable,
-    TypeVar,
-    cast,
+    List,
+    Tuple,
 )
 
 import anyio
+from typing_extensions import ParamSpec, TypeVar
 
-from fast_depends.types import AnyCallable, AnyDict, P
+from fast_depends._compat import evaluate_forwardref
 
+P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def args_to_kwargs(
-    arguments: Iterable[str], *args: P.args, **kwargs: P.kwargs
-) -> AnyDict:
-    if not args:
-        return kwargs
-
-    unused = filter(lambda x: x not in kwargs, arguments)
-
-    return dict((*zip(unused, args), *kwargs.items()))
-
-
 async def run_async(func: Callable[P, T], *args: P.args, **kwargs: P.kwargs) -> T:
-    if asyncio.iscoroutinefunction(func):
-        r = await func(*args, **kwargs)
-        return cast(T, r)
+    if is_coroutine_callable(func):
+        return await func(*args, **kwargs)
     else:
         return await run_in_threadpool(func, *args, **kwargs)
 
 
 async def run_in_threadpool(
     func: Callable[P, T], *args: P.args, **kwargs: P.kwargs
 ) -> T:
     if kwargs:  # pragma: no cover
         func = functools.partial(func, **kwargs)
     return await anyio.to_thread.run_sync(func, *args)
 
 
-def is_async_gen_callable(call: AnyCallable) -> bool:
-    if inspect.isasyncgenfunction(call):
-        return True
-    dunder_call = getattr(call, "__call__", None)  # noqa: B004
-    return inspect.isasyncgenfunction(dunder_call)
-
-
-def is_gen_callable(call: AnyCallable) -> bool:
-    if inspect.isgeneratorfunction(call):
-        return True
-    dunder_call = getattr(call, "__call__", None)  # noqa: B004
-    return inspect.isgeneratorfunction(dunder_call)
-
-
-def is_coroutine_callable(call: AnyCallable) -> bool:
-    if inspect.isroutine(call):
-        return inspect.iscoroutinefunction(call)
-    if inspect.isclass(call):
-        return False
-    call_ = getattr(call, "__call__", None)  # noqa: B004
-    return inspect.iscoroutinefunction(call_)
-
-
 async def solve_generator_async(
-    *, call: AnyCallable, stack: AsyncExitStack, sub_values: Dict[str, Any]
+    *, call: Callable[..., Any], stack: AsyncExitStack, **sub_values: Any
 ) -> Any:
     if is_gen_callable(call):
         cm = contextmanager_in_threadpool(contextmanager(call)(**sub_values))
     elif is_async_gen_callable(call):  # pragma: no branch
         cm = asynccontextmanager(call)(**sub_values)
     return await stack.enter_async_context(cm)
 
 
 def solve_generator_sync(
-    *, call: AnyCallable, stack: ExitStack, sub_values: Dict[str, Any]
+    *, call: Callable[..., Any], stack: ExitStack, **sub_values: Any
 ) -> Any:
     cm = contextmanager(call)(**sub_values)
     return stack.enter_context(cm)
 
 
+def args_to_kwargs(
+    arguments: Iterable[str], *args: P.args, **kwargs: P.kwargs
+) -> Dict[str, Any]:
+    if not args:
+        return kwargs
+
+    unused = filter(lambda x: x not in kwargs, arguments)
+
+    return dict((*zip(unused, args), *kwargs.items()))
+
+
+def get_typed_signature(
+    call: Callable[..., Any]
+) -> Tuple[List[inspect.Parameter], Any]:
+    signature = inspect.signature(call)
+    globalns = getattr(call, "__globals__", {})
+    return [
+        inspect.Parameter(
+            name=param.name,
+            kind=param.kind,
+            default=param.default,
+            annotation=get_typed_annotation(param.annotation, globalns),
+        )
+        for param in signature.parameters.values()
+    ], signature.return_annotation
+
+
+def get_typed_annotation(annotation: Any, globalns: Dict[str, Any]) -> Any:
+    if isinstance(annotation, str):
+        annotation = ForwardRef(annotation)
+        annotation = evaluate_forwardref(annotation, globalns, globalns)
+    return annotation
+
+
 @asynccontextmanager
 async def contextmanager_in_threadpool(
     cm: ContextManager[T],
 ) -> AsyncGenerator[T, None]:
     exit_limiter = anyio.CapacityLimiter(1)
     try:
         yield await run_in_threadpool(cm.__enter__)
@@ -102,7 +103,30 @@
         )
         if not ok:  # pragma: no branch
             raise e
     else:
         await anyio.to_thread.run_sync(
             cm.__exit__, None, None, None, limiter=exit_limiter
         )
+
+
+def is_gen_callable(call: Callable[..., Any]) -> bool:
+    if inspect.isgeneratorfunction(call):
+        return True
+    dunder_call = getattr(call, "__call__", None)  # noqa: B004
+    return inspect.isgeneratorfunction(dunder_call)
+
+
+def is_async_gen_callable(call: Callable[..., Any]) -> bool:
+    if inspect.isasyncgenfunction(call):
+        return True
+    dunder_call = getattr(call, "__call__", None)  # noqa: B004
+    return inspect.isasyncgenfunction(dunder_call)
+
+
+def is_coroutine_callable(call: Callable[..., Any]) -> bool:
+    if inspect.isroutine(call):
+        return inspect.iscoroutinefunction(call)
+    if inspect.isclass(call):
+        return False
+    call_ = getattr(call, "__call__", None)  # noqa: B004
+    return inspect.iscoroutinefunction(call_)
```

### Comparing `fast_depends-1.1.7/fast_depends/library/model.py` & `fast_depends-2.0.0b0/fast_depends/library/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from abc import ABC
-from typing import Optional, TypeVar
-
-from fast_depends.types import AnyDict
+from typing import Any, Dict, Optional, TypeVar
 
 Cls = TypeVar("Cls", bound="CustomField")
 
 
 class CustomField(ABC):
     param_name: Optional[str]
     cast: bool
@@ -16,10 +14,10 @@
         self.param_name = None
         self.required = required
 
     def set_param_name(self: Cls, name: str) -> Cls:
         self.param_name = name
         return self
 
-    def use(self, **kwargs: AnyDict) -> AnyDict:
+    def use(self, **kwargs: Dict[str, Any]) -> Dict[str, Any]:
         assert self.param_name, "You should specify `param_name` before using"
         return kwargs
```

### Comparing `fast_depends-1.1.7/LICENSE` & `fast_depends-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/README.md` & `fast_depends-2.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.7/pyproject.toml` & `fast_depends-2.0.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "pydantic>=1.8",
+    "pydantic==2.0b3",
     "anyio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://lancetnik.github.io/FastDepends/"
```

### Comparing `fast_depends-1.1.7/PKG-INFO` & `fast_depends-2.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.7
+Version: 2.0.0b0
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: anyio
-Requires-Dist: pydantic>=1.8
+Requires-Dist: pydantic==2.0b3
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: fast-depends[doc]; extra == 'dev'
 Requires-Dist: fast-depends[test]; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy>=1.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.260; extra == 'dev'
```

