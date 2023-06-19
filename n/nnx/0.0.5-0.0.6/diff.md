# Comparing `tmp/nnx-0.0.5.tar.gz` & `tmp/nnx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.5.tar", max compression
+gzip compressed data, was "nnx-0.0.6.tar", max compression
```

## Comparing `nnx-0.0.5.tar` & `nnx-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.5/LICENSE
--rw-r--r--   0        0        0    18330 2023-06-12 22:45:34.700995 nnx-0.0.5/README.md
--rw-r--r--   0        0        0     1200 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/__init__.py
--rw-r--r--   0        0        0     7443 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/containers.py
--rw-r--r--   0        0        0     5707 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/contextlib.py
--rw-r--r--   0        0        0     4495 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/dataclasses.py
--rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/errors.py
--rw-r--r--   0        0        0     3628 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/helpers.py
--rw-r--r--   0        0        0    23360 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/module.py
--rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.5/nnx/nn/__init__.py
--rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/activations.py
--rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.5/nnx/nn/initializers.py
--rw-r--r--   0        0        0    16022 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/nn/linear.py
--rw-r--r--   0        0        0    13530 2023-06-12 22:45:21.347880 nnx-0.0.5/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2282 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/nn/stochastic.py
--rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.5/nnx/nodes.py
--rw-r--r--   0        0        0     2224 2023-06-14 04:55:58.785571 nnx-0.0.5/nnx/partitioning.py
--rw-r--r--   0        0        0     8445 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/pytreelib.py
--rw-r--r--   0        0        0     2313 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/reprlib.py
--rw-r--r--   0        0        0     5276 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/state.py
--rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.5/nnx/tracers.py
--rw-r--r--   0        0        0     6784 2023-06-12 22:45:21.351881 nnx-0.0.5/nnx/transforms.py
--rw-r--r--   0        0        0      615 2023-06-13 22:07:35.044745 nnx-0.0.5/nnx/utils.py
--rw-r--r--   0        0        0      764 2023-06-16 17:16:52.104906 nnx-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    18863 1970-01-01 00:00:00.000000 nnx-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.6/LICENSE
+-rw-r--r--   0        0        0    19148 2023-06-19 14:04:51.402418 nnx-0.0.6/README.md
+-rw-r--r--   0        0        0     1223 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/__init__.py
+-rw-r--r--   0        0        0     7443 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/containers.py
+-rw-r--r--   0        0        0     6512 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/contextlib.py
+-rw-r--r--   0        0        0     4495 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/dataclasses.py
+-rw-r--r--   0        0        0       45 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/errors.py
+-rw-r--r--   0        0        0     3617 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/helpers.py
+-rw-r--r--   0        0        0    23324 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.6/nnx/nn/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2763 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-06-08 02:13:59.008365 nnx-0.0.6/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16022 2023-06-12 22:45:21.347880 nnx-0.0.6/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13530 2023-06-12 22:45:21.347880 nnx-0.0.6/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2282 2023-06-12 22:45:21.351881 nnx-0.0.6/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0      348 2023-06-08 02:13:59.012365 nnx-0.0.6/nnx/nodes.py
+-rw-r--r--   0        0        0     2240 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/partitioning.py
+-rw-r--r--   0        0        0     8445 2023-06-13 22:07:35.044745 nnx-0.0.6/nnx/pytreelib.py
+-rw-r--r--   0        0        0     2313 2023-06-12 22:45:21.351881 nnx-0.0.6/nnx/reprlib.py
+-rw-r--r--   0        0        0     5399 2023-06-19 13:43:48.877037 nnx-0.0.6/nnx/state.py
+-rw-r--r--   0        0        0     2412 2023-06-08 02:13:59.016365 nnx-0.0.6/nnx/tracers.py
+-rw-r--r--   0        0        0    17611 2023-06-19 13:43:48.881037 nnx-0.0.6/nnx/transforms.py
+-rw-r--r--   0        0        0     2037 2023-06-19 13:43:48.881037 nnx-0.0.6/nnx/utils.py
+-rw-r--r--   0        0        0      764 2023-06-19 14:18:43.435867 nnx-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    19681 1970-01-01 00:00:00.000000 nnx-0.0.6/PKG-INFO
```

### Comparing `nnx-0.0.5/LICENSE` & `nnx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/README.md` & `nnx-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,48 +59,17 @@
 y = model(x)
 assert model.count == 1
 ```
 
 In this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`
 inside `__init__` to generate a random key to initialize the parameters.
 
-### Training
+### Training with the Functional API
 
-Here we show case two different approaches to training the model defined in the previous secition. The first one uses lifted transforms and the second one uses the functional API. Both approaches are equivalent and produce the same results.
-
-<details><summary>Lifted Transforms</summary>
-
-In this example, we uset the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD) and `train_step` doesn't require a return statement in this case as the model's state is automatically updated.
-
-```python
-@nnx.jit
-def train_step(model, x, y):
-    def loss_fn(model):
-        y_pred = model(x)
-        return jax.numpy.mean((y_pred - y) ** 2)
-    
-    # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
-    # SGD update
-    model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
-    )
-
-# execute the training step
-train_step(model, x, y)
-assert model.count == 2
-```
-
-**Note**: Using `nnx.jit` can introduce some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes and getting started quickly. For more advanced use cases, use the functional API.
-
-</details>
-
-<details><summary>Functional API </summary>
-
-In this example, we utilize the functional API for training. This approach provides more control over the state and allows you to use regular JAX transformations. The model is also trained using Stochastic Gradient Descent (SGD).
+The [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).
 
 ```python
 (params, counts), moduledef = model.partition("params", "counts")
 
 @jax.jit
 def train_step(params, counts, x, y):
     def loss_fn(params):
@@ -117,15 +86,38 @@
 
 # execute the training step
 params, counts = train_step(params, counts, x, y)
 model = moduledef.merge(params, counts)
 assert model.count == 2
 ```
 
-</details>
+### Training with Lifted Transforms
+
+[Lifted Transforms](#lifted-transforms) provide a convenient way interact with NNX Modules. In this example, we use the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD). Because lifted transforms automatically update the Module's state, `train_step` doesn't require a return statement.
+
+```python
+@nnx.jit
+def train_step(model, x, y):
+    def loss_fn(model):
+        y_pred = model(x)
+        return jax.numpy.mean((y_pred - y) ** 2)
+    
+    # compute gradient
+    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model.update_state(
+        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
+    )
+
+# execute the training step
+train_step(model, x, y)
+assert model.count == 2
+```
+
+**Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.
 
 ## Examples
 
 * [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/01_jit_transform.py): Shows how to train a simple model using lifted transforms.
 * [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/02_functional_api.py): Shows how to train a simple model using the functional API.
 * [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.
 * [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.
@@ -173,15 +165,15 @@
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
 model = Foo(din=12, dout=2, ctx=nnx.context(0))
 ```
-As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Map` Modules.
+As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Dict` Modules.
 
 ### Functional API
 
 NNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.
 
 ```python
 state, moduledef = model.partition()
@@ -261,14 +253,36 @@
 ```python
 # only get params
 params = state.filter("params")
 # get params and batch_stats
 params, batch_stats = state.filter("params", "batch_stats")
 ```
 
+### Filters
+
+Filters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:
+
+* `str`: matches all `Variable` nodes (e.g. `nnx.param` or `nnx.var`) with the given `collection` name.
+* `type`: matches all node instances of the given type.
+* `...`: matches all nodes.
+* `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.
+* `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.
+
+NNX also provides the following custom filters:
+
+* `nnx.Not(filter)`: matches all nodes that do not match the given filter
+* `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes
+
+Here is an example of how to use `Not` and `buffers`:
+```python
+rest = module.filter(nnx.Not("params"))
+buffers = module.filter(nnx.buffers)
+```
+
+
 ### Capturing Intermediate Values
 In NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.
 
 Here is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:
 
 ```python
 class Linear(nnx.Module):
@@ -310,15 +324,15 @@
 intermediates, state = state.partition("intermediates", ...)
 ```
 
 Alternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.
 
 
 
-### Stateful Transforms
+### Lifted Transforms
 
 Stateful transforms take a Module as their first argument, track changes in the state that occur within the transformation, and automatically propagate those changes to the input Module outside the transformation. In general, they behave as stateful functions with respect to the first argument.
 
 Here's a diagram illustrating how stateful transformations work:
 
 ![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
```

### Comparing `nnx-0.0.5/nnx/__init__.py` & `nnx-0.0.6/nnx/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     field,
     node_field,
     param_field,
     static_field,
     var_field,
 )
 from .errors import TraceContextError
-from .helpers import Map, Sequence, TrainState
-from .module import Module, ModuleDef, PureModule
+from .helpers import Dict, Sequence, TrainState
+from .module import Module, ModuleDef, Pure, PureModule
 from .nn import initializers
 from .nn.activations import (
     celu,
     elu,
     gelu,
     glu,
     hard_sigmoid,
@@ -54,11 +54,11 @@
     swish,
     tanh,
 )
 from .nn.linear import Conv, Embed, Linear
 from .nn.normalization import BatchNorm, LayerNorm
 from .nn.stochastic import Dropout
 from .nodes import is_node, register_node_type
-from .partitioning import buffers
+from .partitioning import All, Not, buffers
 from .pytreelib import Pytree
 from .state import State
-from .transforms import grad, jit
+from .transforms import grad, jit, scan
```

### Comparing `nnx-0.0.5/nnx/containers.py` & `nnx-0.0.6/nnx/containers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/contextlib.py` & `nnx-0.0.6/nnx/contextlib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import builtins
 import hashlib
 import typing as tp
 from types import MappingProxyType
 
 import jax
 import jax.tree_util as jtu
 
@@ -197,7 +198,33 @@
         else RngStream(value)
         if isinstance(value, jax.Array)
         else value
         for name, value in rngs.items()
     }
 
     return Context(rngs=_rngs, flags=_flags)
+
+
+if tp.TYPE_CHECKING:
+    ellipsis = builtins.ellipsis
+else:
+    ellipsis = tp.Any
+
+RngPredicate = tp.Callable[[str], bool]
+RngFilterLiteral = tp.Union[str, RngPredicate, ellipsis, None]
+RngFilter = tp.Union[RngFilterLiteral, tp.Sequence[RngFilterLiteral]]
+
+
+def to_rng_predicate(filter: RngFilter) -> RngPredicate:
+    if filter is None:
+        return lambda _: False
+    elif filter is ...:
+        return lambda _: True
+    elif callable(filter):
+        return filter
+    elif isinstance(filter, str):
+        return lambda name: name == filter
+    elif isinstance(filter, tuple):
+        predicates = tuple(map(to_rng_predicate, filter))
+        return lambda name: any(predicate(name) for predicate in predicates)
+    else:
+        raise TypeError(f"Invalid rng filter: {filter}")
```

### Comparing `nnx-0.0.5/nnx/dataclasses.py` & `nnx-0.0.6/nnx/dataclasses.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/helpers.py` & `nnx-0.0.6/nnx/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing as tp
 
 import optax
 
 from nnx import containers, pytreelib, utils
 from nnx.contextlib import Context
-from nnx.module import ApplyCaller, Module, PureModule
+from nnx.module import ApplyCaller, Module, Pure
 from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound=Module)
 
 
-class Map(Module, tp.Mapping[str, A]):
+class Dict(Module, tp.Mapping[str, A]):
     @tp.overload
     def __init__(self, __iterable: tp.Iterable[tp.Tuple[str, A]]):
         ...
 
     @tp.overload
     def __init__(self, __mapping: tp.Optional[tp.Mapping[str, A]] = None, **kwargs: A):
         ...
@@ -83,15 +83,15 @@
 
             output = f(*args, **kwargs)
 
         return output
 
 
 class ModuleDefApply(tp.Protocol, tp.Generic[M]):
-    def __call__(self, state: State, *states: State) -> ApplyCaller["PureModule[M]"]:
+    def __call__(self, state: State, *states: State) -> ApplyCaller["Pure[M]"]:
         ...
 
 
 class TrainState(pytreelib.Pytree, tp.Generic[M]):
     def __init__(
         self,
         *,
```

### Comparing `nnx-0.0.5/nnx/module.py` & `nnx-0.0.6/nnx/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import dataclasses
 import typing as tp
 from abc import ABCMeta
 from typing import Any
 
 import jax.tree_util as jtu
 
-from nnx import errors, nodes, partitioning, reprlib, tracers
+from nnx import errors, nodes, partitioning, reprlib, tracers, utils
 from nnx.containers import Container, Sharding, Variable
 from nnx.state import State
 
 A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound="Module")
+S = tp.TypeVar("S", bound=tp.Union[State, tp.Tuple[State, ...]])
 
 Path = tp.Tuple[str, ...]
 StateDict = tp.Dict[Path, tp.Any]
 StateMapping = tp.Mapping[Path, tp.Any]
 
 
 class ApplyCaller(tp.Protocol, tp.Generic[A]):
@@ -88,36 +89,33 @@
     ) -> tp.Tuple[tp.Tuple[str, tp.Union["ModuleDef[Module]", int]], ...]:
         return self._submodules
 
     @property
     def static_fields(self) -> tp.Tuple[tp.Tuple[str, tp.Any], ...]:
         return self._static_fields
 
-    @tp.overload
     def merge(self, state: State, *states: State) -> M:
-        ...
-
-    def merge(self, *states: State) -> M:
+        states = (state, *states)
         module = _build_module(self)
         current_state = State({})
 
         _update_module(module, current_state, states)
 
         return module
 
-    def apply(self, state: State, *states: State) -> ApplyCaller["PureModule[M]"]:
-        accessesor = DelayedAccessor()
+    def apply(self, state: State, *states: State) -> ApplyCaller["Pure[State, M]"]:
+        accessesor = utils.DelayedAccessor()
 
-        def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, PureModule[M]]:
+        def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, Pure[State, M]]:
             module = self.merge(state, *states)
             fn = accessesor(module)
             out = fn(*args, **kwargs)
             return out, module.partition()
 
-        return CallableProxy(_context, accessesor)  # type: ignore
+        return utils.CallableProxy(_context, accessesor)  # type: ignore
 
 
 def _moddef_flatten(moduledef: ModuleDef[M]):
     return (), (
         moduledef._type,
         moduledef._index,
         moduledef._submodules,
@@ -136,195 +134,197 @@
 ) -> ModuleDef[M]:
     return ModuleDef(*metadata)
 
 
 jtu.register_pytree_node(ModuleDef, _moddef_flatten, _moddef_unflatten)
 
 
-class PureModule(tp.Tuple[State, ModuleDef[M]]):
+class Pure(tp.Tuple[S, ModuleDef[M]]):
     @classmethod
-    def new(cls, state: State, moduledef: ModuleDef[M]) -> "PureModule[M]":
-        return cls((state, moduledef))
+    def new(cls, states: S, moduledef: ModuleDef[M]) -> "Pure[S, M]":
+        return cls((states, moduledef))
 
     @property
-    def state(self) -> State:
+    def states(self) -> S:
         return self[0]
 
     @property
     def moduledef(self) -> ModuleDef[M]:
         return self[1]
 
     def merge(self) -> M:
-        return self.moduledef.merge(self.state)
+        if isinstance(self.states, tuple):
+            return self.moduledef.merge(*self.states)
+        else:
+            return self.moduledef.merge(self.states)
 
     @property
-    def apply(self) -> ApplyCaller["PureModule[M]"]:
-        return self.moduledef.apply(self.state)
+    def apply(self) -> ApplyCaller["Pure[State, M]"]:
+        if isinstance(self.states, tuple):
+            return self.moduledef.apply(*self.states)
+        else:
+            return self.moduledef.apply(self.states)
 
     @property
     def call(self) -> M:
-        accessesor = DelayedAccessor()
+        accessesor = utils.DelayedAccessor()
 
         def _context(accessesor, *args, **kwargs):
             module = self.merge()
             fn = accessesor(module)
             return fn(*args, **kwargs)
 
-        return CallableProxy(_context, accessesor)  # type: ignore
+        return utils.CallableProxy(_context, accessesor)  # type: ignore
 
     def get_state(self) -> State:
-        return self.state
+        if isinstance(self.states, tuple):
+            return State.merge(*self.states)
+        return self.states
 
     @tp.overload
     def filter(
         self,
-        filter: partitioning.CollectionFilter,
+        filter: partitioning.Filter,
         /,
     ) -> State:
         ...
 
     @tp.overload
     def filter(
         self,
-        filter: partitioning.CollectionFilter,
-        filter2: partitioning.CollectionFilter,
+        filter: partitioning.Filter,
+        filter2: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Tuple[State, ...]:
         ...
 
     def filter(
-        self, *filters: partitioning.CollectionFilter
+        self, filter: partitioning.Filter, *filters: partitioning.Filter
     ) -> tp.Union[State, tp.Tuple[State, ...]]:
-        return self.state.filter(*filters)
+        filters = (filter, *filters)
+        state = self.get_state()
+
+        if len(filters) == 1:
+            return state.filter(filters[0])
+        else:
+            return state.filter(filters[0], filters[1], *filters[2:])
+
+    @tp.overload
+    def partition(self) -> "Pure[State, M]":
+        ...
 
     @tp.overload
-    def partition(self, first: partitioning.CollectionFilter, /) -> "PureModule[M]":
+    def partition(self, first: partitioning.Filter, /) -> "Pure[State, M]":
         ...
 
     @tp.overload
     def partition(
         self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
+        first: partitioning.Filter,
+        second: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]:
+        *filters: partitioning.Filter,
+    ) -> "Pure[tp.Tuple[State, ...], M]":
         ...
 
     def partition(
-        self,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Union["PureModule[M]", tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]],]:
-        states = self.state.partition(*filters)
+        self, *filters: partitioning.Filter
+    ) -> tp.Union["Pure[State, M]", "Pure[tp.Tuple[State, ...], M]"]:
+        state = self.get_state()
+
+        if len(filters) == 0:
+            states = state
+        elif len(filters) == 1:
+            states = state.partition(filters[0])
+        else:
+            states = state.partition(filters[0], filters[1], *filters[2:])
+
         if isinstance(states, State):
-            return PureModule.new(states, self.moduledef)
+            return Pure.new(states, self.moduledef)
         else:
-            return states, self.moduledef
+            return Pure.new(states, self.moduledef)
 
     @tp.overload
     def pop_state(
-        self, filter: partitioning.CollectionFilter, /
-    ) -> tp.Tuple[State, "PureModule[M]"]:
+        self, filter: partitioning.Filter, /
+    ) -> tp.Tuple[State, "Pure[State, M]"]:
         ...
 
     @tp.overload
     def pop_state(
         self,
-        filter: partitioning.CollectionFilter,
-        filter2: partitioning.CollectionFilter,
+        filter: partitioning.Filter,
+        filter2: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Tuple[tp.Tuple[State, ...], "PureModule[M]"]:
+        *filters: partitioning.Filter,
+    ) -> tp.Tuple[tp.Tuple[State, ...], "Pure[State, M]"]:
         ...
 
     def pop_state(
-        self, *filters: partitioning.CollectionFilter
-    ) -> tp.Tuple[tp.Union[State, tp.Tuple[State, ...]], "PureModule[M]"]:
-        if len(filters) == 0:
-            raise ValueError("At least one filter must be provided")
-        else:
-            *states, rest = self.state.partition(*filters, ...)
+        self, filter: partitioning.Filter, *filters: partitioning.Filter
+    ) -> tp.Tuple[tp.Union[State, tp.Tuple[State, ...]], "Pure[State, M]"]:
+        filters = (filter, *filters)
+
+        state = self.get_state()
+        *states, rest = state.partition(*filters, ...)
 
         if len(states) == 1:
             states = states[0]
         else:
             states = tuple(states)
 
-        return states, PureModule.new(rest, self.moduledef)
+        return states, Pure.new(rest, self.moduledef)
 
     def update_state(
         self,
-        updates: tp.Union[M, "PureModule[M]", State, tp.Tuple[State, ...]],
-    ) -> "PureModule[M]":
+        updates: tp.Union[M, "Pure[S, M]", State, tp.Tuple[State, ...]],
+    ) -> "Pure[State, M]":
         if isinstance(updates, Module):
-            states = (updates.partition()[0],)
-        elif isinstance(updates, PureModule):
-            states = (updates.state,)
+            states = (updates.get_state(),)
+        elif isinstance(updates, Pure):
+            if isinstance(updates.states, tuple):
+                states = updates.states
+            elif isinstance(updates.states, State):
+                states = (updates.states,)
+            else:
+                raise TypeError(
+                    f"Expected Module, PureModule, State or tuple of State, "
+                    f"got {type(updates.states).__name__}"
+                )
         elif isinstance(updates, State):
             states = (updates,)
         elif isinstance(updates, tuple):
             states = updates
         else:
             raise TypeError(
                 f"Expected Module, PureModule, State or tuple of State, "
                 f"got {type(updates).__name__}"
             )
 
+        if isinstance(self.states, tuple):
+            states += self.states
+        else:
+            states += (self.states,)
+
         state = State.merge(*states)
-        return PureModule.new(state, self.moduledef)
+        return Pure.new(state, self.moduledef)
 
 
-def _pure_module_flatten(bounded: PureModule[M]):
+def _pure_module_flatten(bounded: Pure[S, M]):
     return tuple(bounded), None
 
 
-def _pure_module_unflatten(_, values: tp.Tuple[State, ModuleDef[M]]):
-    return PureModule(values)
-
-
-jtu.register_pytree_node(PureModule, _pure_module_flatten, _pure_module_unflatten)
-
-
-class _ProxyContext(tp.Protocol):
-    def __call__(self, __fn: tp.Callable[..., tp.Any], *args, **kwargs) -> tp.Any:
-        ...
-
+def _pure_module_unflatten(_, values: tp.Tuple[S, ModuleDef[M]]):
+    return Pure(values)
 
-@dataclasses.dataclass
-class CallableProxy:
-    _proxy_context: _ProxyContext
-    _proxy_callable: tp.Callable[..., tp.Any]
 
-    def __call__(self, *args, **kwargs):
-        return self._proxy_context(self._proxy_callable, *args, **kwargs)
+jtu.register_pytree_node(Pure, _pure_module_flatten, _pure_module_unflatten)
 
-    def __getattr__(self, name) -> "CallableProxy":
-        return CallableProxy(self._proxy_context, getattr(self._proxy_callable, name))
-
-    def __getitem__(self, key) -> "CallableProxy":
-        return CallableProxy(self._proxy_context, self._proxy_callable[key])
-
-
-def _identity(x):
-    return x
-
-
-@dataclasses.dataclass
-class DelayedAccessor:
-    accessor: tp.Callable[[tp.Any], tp.Any] = _identity
-
-    def __call__(self, x):
-        return self.accessor(x)
-
-    def __getattr__(self, name):
-        return DelayedAccessor(lambda x: getattr(x, name))
-
-    def __getitem__(self, key):
-        return DelayedAccessor(lambda x: x[key])
+PureModule = Pure[tp.Union[State, tp.Tuple[State, ...]], M]
 
 
 SEEN_MODULES_REPR: tp.Set[int] = set()
 
 
 class ModuleState(reprlib.Representable):
     __slots__ = ("_trace_state",)
@@ -341,17 +341,17 @@
         yield reprlib.Attr("trace_state", self._trace_state)
 
 
 class ModuleMeta(ABCMeta):
     if not tp.TYPE_CHECKING:
 
         def __call__(self, *args: Any, **kwargs: Any) -> Any:
-            return self.call(*args, **kwargs)
+            return self._meta_call(*args, **kwargs)
 
-    def call(self: tp.Type[M], *args, **kwargs) -> M:
+    def _meta_call(self: tp.Type[M], *args, **kwargs) -> M:
         module = self.__new__(self, *args, **kwargs)
         vars(module)["_module__state"] = ModuleState(tracers.TraceState())
         module.__init__(*args, **kwargs)
 
         if dataclasses.is_dataclass(module):
             assert isinstance(module, Module)
             for field in dataclasses.fields(module):
@@ -415,133 +415,132 @@
         finally:
             SEEN_MODULES_REPR.remove(id(self))
 
     def clone(self: M) -> M:
         return self.partition().merge()
 
     @tp.overload
-    def partition(self: M) -> PureModule[M]:
+    def partition(self: M) -> Pure[State, M]:
         ...
 
     @tp.overload
-    def partition(self: M, first: partitioning.CollectionFilter, /) -> PureModule[M]:
+    def partition(self: M, first: partitioning.Filter, /) -> Pure[State, M]:
         ...
 
     @tp.overload
     def partition(
         self: M,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
+        first: partitioning.Filter,
+        second: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]:
+        *filters: partitioning.Filter,
+    ) -> Pure[tp.Tuple[State, ...], M]:
         ...
 
     def partition(
-        self: M,
-        *filters: partitioning.CollectionFilter,
-    ) -> tp.Union[PureModule[M], tp.Tuple[tp.Tuple[State, ...], ModuleDef[M]]]:
+        self: M, *filters: partitioning.Filter
+    ) -> tp.Union[Pure[State, M], Pure[tp.Tuple[State, ...], M]]:
         moduledef = _get_module_def(self)
         state = _get_module_state(self)
 
         if len(filters) == 0:
             states = state
         elif len(filters) == 1:
             states = state.partition(filters[0])
         else:
             states = state.partition(filters[0], filters[1], *filters[2:])
 
         if isinstance(states, tuple):
-            return states, moduledef
+            return Pure.new(states, moduledef)
         else:
-            return PureModule.new(states, moduledef)
+            return Pure.new(states, moduledef)
 
     def get_state(self) -> State:
         return _get_module_state(self)
 
     @tp.overload
-    def filter(self, first: partitioning.CollectionFilter, /) -> State:
+    def filter(self, first: partitioning.Filter, /) -> State:
         ...
 
     @tp.overload
     def filter(
         self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
+        first: partitioning.Filter,
+        second: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Tuple[State, ...]:
         ...
 
     def filter(
         self,
-        first: partitioning.CollectionFilter,
+        first: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Union[State, tp.Tuple[State, ...]]:
         state = _get_module_state(self)
 
         if len(filters) == 0:
             states = state.filter(first)
         else:
             states = state.filter(first, filters[0], *filters[1:])
 
         return states
 
     @tp.overload
     def pop_state(
         self,
-        filter: partitioning.CollectionFilter,
+        filter: partitioning.Filter,
         /,
     ) -> State:
         ...
 
     @tp.overload
     def pop_state(
         self,
-        filter: partitioning.CollectionFilter,
-        filter2: partitioning.CollectionFilter,
+        filter: partitioning.Filter,
+        filter2: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Tuple[State, ...]:
         ...
 
     def pop_state(
-        self, *filters: partitioning.CollectionFilter
+        self, *filters: partitioning.Filter
     ) -> tp.Union[State, tp.Tuple[State, ...]]:
         if len(filters) == 0:
             raise ValueError("Expected at least one filter")
 
         states = _pop(self, filters)
 
         if len(states) == 1:
             return states[0]
         else:
             return states
 
     @property
     def apply(self: M) -> ApplyCaller[M]:
-        accessesor = DelayedAccessor()
+        accessesor = utils.DelayedAccessor()
 
         def _context(accessesor, *args, **kwargs) -> tp.Tuple[tp.Any, M]:
             module = self.clone()
             fn = accessesor(module)
             out = fn(*args, **kwargs)
             return out, module
 
-        return CallableProxy(_context, accessesor)  # type: ignore
+        return utils.CallableProxy(_context, accessesor)  # type: ignore
 
     def update_state(
         self: M,
-        updates: tp.Union[M, PureModule[M], State, tp.Tuple[State, ...]],
+        updates: tp.Union[M, Pure[S, M], State, tp.Tuple[State, ...]],
     ) -> None:
         current_state = _get_module_state(self)
 
-        if isinstance(updates, PureModule):
-            updates = updates.state
+        if isinstance(updates, Pure):
+            updates = updates.states
         elif isinstance(updates, Module):
             assert type(self) == type(updates)
             updates = _get_module_state(updates)
 
         _update_module(self, current_state, updates)
 
     @tp.overload
@@ -747,15 +746,15 @@
     vars(module)["_module__state"] = ModuleState(tracers.TraceState())
 
     return module
 
 
 def _pop(
     module: Module,
-    filters: tp.Tuple[partitioning.CollectionFilter, ...],
+    filters: tp.Tuple[partitioning.Filter, ...],
 ) -> tp.Tuple[State, ...]:
     module_index: tp.Dict[int, int] = {}
     path: Path = ()
     predicates = tuple(partitioning.to_predicate(filter) for filter in filters)
     states = tuple({} for _ in predicates)
     _pop_recursive(module, module_index, path, states, predicates)
 
@@ -805,8 +804,8 @@
 
     for path, value in state.items():
         _set_value_at_path(module, path, value)
 
 
 # register nodes
 nodes.register_node_type(Module)
-nodes.register_node_type(PureModule)
+nodes.register_node_type(Pure)
```

### Comparing `nnx-0.0.5/nnx/nn/activations.py` & `nnx-0.0.6/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/nn/dtypes.py` & `nnx-0.0.6/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/nn/initializers.py` & `nnx-0.0.6/nnx/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/nn/linear.py` & `nnx-0.0.6/nnx/nn/linear.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/nn/normalization.py` & `nnx-0.0.6/nnx/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/nn/stochastic.py` & `nnx-0.0.6/nnx/nn/stochastic.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/pytreelib.py` & `nnx-0.0.6/nnx/pytreelib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/reprlib.py` & `nnx-0.0.6/nnx/reprlib.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/nnx/state.py` & `nnx-0.0.6/nnx/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,34 +48,32 @@
     def __nnx_repr__(self):
         yield reprlib.Object(type(self), value_sep=": ", start="({", end="})")
 
         for k, v in self._mapping.items():
             yield reprlib.Attr(str(k), v)
 
     @tp.overload
-    def partition(self, first: partitioning.CollectionFilter, /) -> "State":
+    def partition(self, first: partitioning.Filter, /) -> "State":
         ...
 
     @tp.overload
     def partition(
         self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
+        first: partitioning.Filter,
+        second: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Tuple["State", ...]:
         ...
 
     def partition(
-        self,
-        first: partitioning.CollectionFilter,
-        /,
-        *filters: partitioning.CollectionFilter,
+        self, first: partitioning.Filter, /, *filters: partitioning.Filter
     ) -> tp.Union["State", tp.Tuple["State", ...]]:
-        *states, rest = _split_state(self, first, *filters)
+        filters = (first, *filters)
+        *states, rest = _split_state(self, *filters)
 
         if rest:
             raise ValueError(
                 f"Non-exhaustive filters, got a non-empty remainder: "
                 f"{list(rest.keys())}.\nUse `...` to match all remaining elements."
             )
 
@@ -84,36 +82,36 @@
         else:
             states = tuple(State(state) for state in states)
         return states
 
     @tp.overload
     def filter(
         self,
-        first: partitioning.CollectionFilter,
+        first: partitioning.Filter,
         /,
     ) -> "State":
         ...
 
     @tp.overload
     def filter(
         self,
-        first: partitioning.CollectionFilter,
-        second: partitioning.CollectionFilter,
+        first: partitioning.Filter,
+        second: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Tuple["State", ...]:
         ...
 
     def filter(
         self,
-        first: partitioning.CollectionFilter,
+        first: partitioning.Filter,
         /,
-        *filters: partitioning.CollectionFilter,
+        *filters: partitioning.Filter,
     ) -> tp.Union["State", tp.Tuple["State", ...]]:
-        (*states, _rest) = _split_state(self, first, *filters)
+        *states, _rest = _split_state(self, first, *filters)
 
         assert len(states) == len(filters) + 1
 
         if len(states) == 1:
             states = State(states[0])
         else:
             states = tuple(State(state) for state in states)
@@ -169,16 +167,22 @@
 jax.tree_util.register_pytree_with_keys(
     State, _state_flatten_with_keys, _state_unflatten
 )
 
 
 def _split_state(
     state: StateMapping,
-    *filters: partitioning.CollectionFilter,
+    *filters: partitioning.Filter,
 ) -> tp.Tuple[StateDict, ...]:
+    for i, filter_ in enumerate(filters):
+        if filter_ is ... and i != len(filters) - 1:
+            raise ValueError(
+                f"Ellipsis `...` can only be used as the last filter, "
+                f"got it at index {i}."
+            )
     predicates = tuple(map(partitioning.to_predicate, filters))
 
     # we have n + 1 states, where n is the number of predicates
     # the last state is for values that don't match any predicate
     states: tp.Tuple[StateDict, ...] = tuple({} for _ in range(len(predicates) + 1))
 
     for path, value in state.items():
```

### Comparing `nnx-0.0.5/nnx/tracers.py` & `nnx-0.0.6/nnx/tracers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.5/pyproject.toml` & `nnx-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 jax = "*"
```

### Comparing `nnx-0.0.5/PKG-INFO` & `nnx-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnx
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Cristian Garcia
 Author-email: cgarcia.e88@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -77,48 +77,17 @@
 y = model(x)
 assert model.count == 1
 ```
 
 In this example `nnx.context(0)` create a `PRNGKey` for `params` with seed `0`, this is used by `make_rng`
 inside `__init__` to generate a random key to initialize the parameters.
 
-### Training
+### Training with the Functional API
 
-Here we show case two different approaches to training the model defined in the previous secition. The first one uses lifted transforms and the second one uses the functional API. Both approaches are equivalent and produce the same results.
-
-<details><summary>Lifted Transforms</summary>
-
-In this example, we uset the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD) and `train_step` doesn't require a return statement in this case as the model's state is automatically updated.
-
-```python
-@nnx.jit
-def train_step(model, x, y):
-    def loss_fn(model):
-        y_pred = model(x)
-        return jax.numpy.mean((y_pred - y) ** 2)
-    
-    # compute gradient
-    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
-    # SGD update
-    model.update_state(
-        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
-    )
-
-# execute the training step
-train_step(model, x, y)
-assert model.count == 2
-```
-
-**Note**: Using `nnx.jit` can introduce some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes and getting started quickly. For more advanced use cases, use the functional API.
-
-</details>
-
-<details><summary>Functional API </summary>
-
-In this example, we utilize the functional API for training. This approach provides more control over the state and allows you to use regular JAX transformations. The model is also trained using Stochastic Gradient Descent (SGD).
+The [Functional API](#functional-api) converts an NNX Module python semantics into pure pytree object with functional semantics. It is the recommended way to use NNX as it provides tight control over the state, allows you to use regular JAX transformations, and it minimizes overhead. In this example the model will be trained using Stochastic Gradient Descent (SGD).
 
 ```python
 (params, counts), moduledef = model.partition("params", "counts")
 
 @jax.jit
 def train_step(params, counts, x, y):
     def loss_fn(params):
@@ -135,15 +104,38 @@
 
 # execute the training step
 params, counts = train_step(params, counts, x, y)
 model = moduledef.merge(params, counts)
 assert model.count == 2
 ```
 
-</details>
+### Training with Lifted Transforms
+
+[Lifted Transforms](#lifted-transforms) provide a convenient way interact with NNX Modules. In this example, we use the `nnx.jit` and `nnx.grad` lifted transforms to define the training step. The model is trained using Stochastic Gradient Descent (SGD). Because lifted transforms automatically update the Module's state, `train_step` doesn't require a return statement.
+
+```python
+@nnx.jit
+def train_step(model, x, y):
+    def loss_fn(model):
+        y_pred = model(x)
+        return jax.numpy.mean((y_pred - y) ** 2)
+    
+    # compute gradient
+    grads: nnx.State = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model.update_state(
+        jax.tree_map(lambda w, g: w - 0.1 * g, model.filter("params"), grads)
+    )
+
+# execute the training step
+train_step(model, x, y)
+assert model.count == 2
+```
+
+**Note**: Using `nnx.jit` introduces some overhead when compared to using `jax.jit` directly. Use `nnx.jit` for simple prototypes, but for production code use `jax.jit` directly.
 
 ## Examples
 
 * [Using Lifted Transforms](https://github.com/cgarciae/nnx/blob/main/examples/01_jit_transform.py): Shows how to train a simple model using lifted transforms.
 * [Using the Functional API](https://github.com/cgarciae/nnx/blob/main/examples/02_functional_api.py): Shows how to train a simple model using the functional API.
 * [Using TrainState](https://github.com/cgarciae/nnx/blob/main/examples/03_train_state.py): Shows how to train a simple model using the functional API with the help of `TrainState`.
 * [Using PureModule](https://github.com/cgarciae/nnx/blob/main/examples/04_pure.py) (experimental): Shows how to train a simple model using the functional API and leveraging `PureModule` to simplify the code.
@@ -191,15 +183,15 @@
         self.int = 1
         self.float = 2.0
         self.str = "hello"
         self.list = [1, 2, 3]
 
 model = Foo(din=12, dout=2, ctx=nnx.context(0))
 ```
-As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Map` Modules.
+As shown above, python container types such as `list`, `tuple`, and `dict` are treated as static attributes, if similar functionality is needed, NNX provides the `Sequence` and `Dict` Modules.
 
 ### Functional API
 
 NNX Modules are not pytrees so they cannot be passed to JAX transformations. In order to interact with JAX, a Module must be partitioned into a `State` and `ModuleDef` objects. The `State` object is a flat dictionary-like pytree structure that contains all the deduplicated node attributes, and the `ModuleDef` contains the static attributes and structural information needed to reconstruct the Module.
 
 ```python
 state, moduledef = model.partition()
@@ -279,14 +271,36 @@
 ```python
 # only get params
 params = state.filter("params")
 # get params and batch_stats
 params, batch_stats = state.filter("params", "batch_stats")
 ```
 
+### Filters
+
+Filters let you select subsets of nodes based on some criteria. These are use throughout the API in method like `partition`, `filter`, and `pop_state`. There are 4 types of filters:
+
+* `str`: matches all `Variable` nodes (e.g. `nnx.param` or `nnx.var`) with the given `collection` name.
+* `type`: matches all node instances of the given type.
+* `...`: matches all nodes.
+* `(path, any) -> bool`: a predicate function that takes a node path and value and returns a boolean.
+* `Tuple[Filter, ...]`: a tuple of filters, matches all nodes that match any of the filters.
+
+NNX also provides the following custom filters:
+
+* `nnx.Not(filter)`: matches all nodes that do not match the given filter
+* `nnx.buffers`: matches all `numpy.ndarray` and `jax.Array` nodes
+
+Here is an example of how to use `Not` and `buffers`:
+```python
+rest = module.filter(nnx.Not("params"))
+buffers = module.filter(nnx.buffers)
+```
+
+
 ### Capturing Intermediate Values
 In NNX you can easily propagate intemediate values by simply assigning them to an attribute at runtime. For convenience, you should assign them to a `Variable` attribute with a `collection` name by using `nnx.var` so you can easily retrieve them later.
 
 Here is an example of how to create a `Linear` module that captures its output into a `Variable` attribute with the `intermediates` collection name:
 
 ```python
 class Linear(nnx.Module):
@@ -328,15 +342,15 @@
 intermediates, state = state.partition("intermediates", ...)
 ```
 
 Alternatively, you can use `State.filter` to retrieve the `intermediates` nodes without removing them from the `state`.
 
 
 
-### Stateful Transforms
+### Lifted Transforms
 
 Stateful transforms take a Module as their first argument, track changes in the state that occur within the transformation, and automatically propagate those changes to the input Module outside the transformation. In general, they behave as stateful functions with respect to the first argument.
 
 Here's a diagram illustrating how stateful transformations work:
 
 ![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
```

