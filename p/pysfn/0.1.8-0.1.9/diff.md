# Comparing `tmp/pysfn-0.1.8.tar.gz` & `tmp/pysfn-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfn-0.1.8.tar", max compression
+gzip compressed data, was "pysfn-0.1.9.tar", max compression
```

## Comparing `pysfn-0.1.8.tar` & `pysfn-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      413 2022-12-28 23:19:43.381466 pysfn-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-19 15:52:12.171276 pysfn-0.1.8/pysfn/__init__.py
--rw-r--r--   0        0        0     2463 2022-11-03 16:28:04.966839 pysfn-0.1.8/pysfn/condition.py
--rw-r--r--   0        0        0      410 2022-12-20 01:35:16.647954 pysfn-0.1.8/pysfn/dynamo.py
--rw-r--r--   0        0        0     4531 2022-11-19 17:02:23.029885 pysfn-0.1.8/pysfn/function.py
--rw-r--r--   0        0        0     7037 2022-11-27 17:45:18.274425 pysfn-0.1.8/pysfn/lmbda.py
--rw-r--r--   0        0        0     1861 2022-12-21 17:04:31.333804 pysfn-0.1.8/pysfn/s3.py
--rw-r--r--   0        0        0    52932 2022-12-28 20:23:04.603842 pysfn-0.1.8/pysfn/steps.py
--rw-r--r--   0        0        0    21703 2022-11-21 17:48:05.342006 pysfn-0.1.8/README.md
--rw-r--r--   0        0        0    23067 1970-01-01 00:00:00.000000 pysfn-0.1.8/setup.py
--rw-r--r--   0        0        0    22330 1970-01-01 00:00:00.000000 pysfn-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      413 2023-01-05 01:01:39.389185 pysfn-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-19 15:52:12.171276 pysfn-0.1.9/pysfn/__init__.py
+-rw-r--r--   0        0        0     3698 2023-01-05 00:58:41.131286 pysfn-0.1.9/pysfn/condition.py
+-rw-r--r--   0        0        0      410 2022-12-20 01:35:16.647954 pysfn-0.1.9/pysfn/dynamo.py
+-rw-r--r--   0        0        0     4665 2023-01-03 01:10:19.118811 pysfn-0.1.9/pysfn/function.py
+-rw-r--r--   0        0        0     7037 2022-11-27 17:45:18.274425 pysfn-0.1.9/pysfn/lmbda.py
+-rw-r--r--   0        0        0     1861 2022-12-21 17:04:31.333804 pysfn-0.1.9/pysfn/s3.py
+-rw-r--r--   0        0        0    53329 2023-01-03 01:10:19.118811 pysfn-0.1.9/pysfn/steps.py
+-rw-r--r--   0        0        0    21703 2022-11-21 17:48:05.342006 pysfn-0.1.9/README.md
+-rw-r--r--   0        0        0    23067 1970-01-01 00:00:00.000000 pysfn-0.1.9/setup.py
+-rw-r--r--   0        0        0    22330 1970-01-01 00:00:00.000000 pysfn-0.1.9/PKG-INFO
```

### Comparing `pysfn-0.1.8/pysfn/function.py` & `pysfn-0.1.9/pysfn/function.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-import ast
-import inspect
-from typing import Callable, Type, Mapping, Union, List
-from dataclasses import dataclass
-from itertools import zip_longest, islice
-
-
-def get_function_ast(func: Callable):
-    # Retrieve the source code for the function with any indent removed
-    src_code = inspect.getsource(func).split("\n")
-    indent = len(src_code[0]) - len(src_code[0].lstrip())
-    src_code = [c[indent:] for c in src_code]
-
-    # Build the AST
-    return ast.parse("\n".join(src_code))
-
-
-@dataclass
-class FunctionAttributes:
-    func: Callable
-    tree: ast.expr
-    name: str
-    module: str
-    input: Mapping[str, Type]
-    output: Mapping[str, Type]
-
-
-def gather_function_attributes(
-    func,
-    in_: Union[List[str], Mapping[str, Type]] = None,
-    out_: Union[List[str], Mapping[str, Type]] = None,
-    src_dir: str = None,
-):
-    tree = get_function_ast(func)
-    arg_spec = inspect.getfullargspec(func)
-
-    # TODO: Explore a better alternative to this approach for ensuring valid import path
-    module_parts = func.__module__.split(".")
-    if module_parts[0] == src_dir:
-        module = ".".join(module_parts[1:])
-    else:
-        module = func.__module__
-
-    # Build inputs
-    args = {a: arg_spec.annotations.get(a) for a in arg_spec.args}
-    if in_ and len(in_) != len(args):
-        raise Exception("Input argument count mismatch")
-    if isinstance(in_, List):
-        input_vars = {k: arg_spec.annotations.get(k) for k in in_}
-    elif isinstance(in_, Mapping):
-        input_vars = in_
-    elif in_ is None:
-        input_vars = args
-    else:
-        raise Exception("Invalid in_ parameter")
-
-    # Build return vars
-    return_annotation = arg_spec.annotations.get("return")
-    if return_annotation is not None and not isinstance(return_annotation, tuple):
-        return_annotation = (return_annotation,)
-    return_vars = get_function_return_var_names(tree, func.__name__)
-    if (out_ and len(return_vars) != len(out_)) or (
-        out_ and return_annotation and len(out_) != len(return_annotation)
-    ):
-        raise Exception("out_ does not match return")
-    if isinstance(out_, List):
-        if return_annotation:
-            output_vars = {k: v for k, v in zip(out_, return_annotation)}
-        else:
-            output_vars = {k: None for k in out_}
-    elif isinstance(out_, Mapping):
-        output_vars = out_
-    elif out_ is None:
-        if return_vars is None or len(return_vars) == 0:
-            output_vars = {}
-        else:
-            return_vars = [v if v else f"arg{i}" for i, v in enumerate(return_vars)]
-            if return_annotation:
-                output_vars = {
-                    k: v
-                    for k, v in zip_longest(
-                        return_vars, islice(return_annotation, len(return_vars))
-                    )
-                }
-            else:
-                output_vars = {k: None for k in return_vars}
-    else:
-        raise Exception("Invalid out_ parameter")
-
-    return FunctionAttributes(
-        func, tree, func.__name__, module, input_vars, output_vars
-    )
-
-
-def find_returns(node: ast.expr):
-    rets = []
-    if isinstance(node, ast.Return):
-        return [node]
-    if hasattr(node, "body"):
-        for n in node.body:
-            res = find_returns(n)
-            if res:
-                rets.extend(res)
-    if hasattr(node, "handlers"):
-        for n in node.handlers:
-            res = find_returns(n)
-            if res:
-                rets.extend(res)
-    return rets
-
-
-def get_function_return_var_names(tree: ast.expr, name: str):
-    rets = find_returns(tree)
-    names = None
-    for ret in rets:
-        if ret and isinstance(ret.value, ast.Name):
-            if names is not None and len(names) != 1:
-                raise Exception(f"Different return lengths in {name}")
-            names = [ret.value.id]
-        elif ret and isinstance(ret.value, ast.Constant):
-            if names is not None and len(names) != 1:
-                raise Exception(f"Different return lengths in {name}")
-            names = [None]
-        elif ret and isinstance(ret.value, ast.Tuple):
-            if names is not None and len(names) != len(ret.value.elts):
-                raise Exception(f"Different return lengths in {name}")
-            if names is None:
-                names = [None for _ in range(len(ret.value.elts))]
-            for i, elt in enumerate(ret.value.elts):
-                if isinstance(elt, ast.Name):
-                    names[i] = elt.id
-        else:
-            names = [None]
-    return names
+import ast
+import inspect
+from typing import Callable, Type, Mapping, Union, List
+from dataclasses import dataclass
+from itertools import zip_longest, islice
+
+
+def get_function_ast(func: Callable):
+    # Retrieve the source code for the function with any indent removed
+    src_code = inspect.getsource(func).split("\n")
+    indent = len(src_code[0]) - len(src_code[0].lstrip())
+    src_code = [c[indent:] for c in src_code]
+
+    # Build the AST
+    return ast.parse("\n".join(src_code))
+
+
+@dataclass
+class FunctionAttributes:
+    func: Callable
+    tree: ast.expr
+    name: str
+    module: str
+    input: Mapping[str, Type]
+    output: Mapping[str, Type]
+
+
+def gather_function_attributes(
+    func,
+    in_: Union[List[str], Mapping[str, Type]] = None,
+    out_: Union[List[str], Mapping[str, Type]] = None,
+    src_dir: str = None,
+):
+    tree = get_function_ast(func)
+    arg_spec = inspect.getfullargspec(func)
+
+    # TODO: Explore a better alternative to this approach for ensuring valid import path
+    module_parts = func.__module__.split(".")
+    if module_parts[0] == src_dir:
+        module = ".".join(module_parts[1:])
+    else:
+        module = func.__module__
+
+    # Build inputs
+    args = {a: arg_spec.annotations.get(a) for a in arg_spec.args}
+    if in_ and len(in_) != len(args):
+        raise Exception("Input argument count mismatch")
+    if isinstance(in_, List):
+        input_vars = {k: arg_spec.annotations.get(k) for k in in_}
+    elif isinstance(in_, Mapping):
+        input_vars = in_
+    elif in_ is None:
+        input_vars = args
+    else:
+        raise Exception("Invalid in_ parameter")
+
+    # Build return vars
+    return_annotation = arg_spec.annotations.get("return")
+    if return_annotation is not None and not isinstance(return_annotation, tuple):
+        return_annotation = (return_annotation,)
+    return_vars = get_function_return_var_names(tree, func.__name__)
+    if (out_ and len(return_vars) != len(out_)) or (
+        out_ and return_annotation and len(out_) != len(return_annotation)
+    ):
+        raise Exception("out_ does not match return")
+    if isinstance(out_, List):
+        if return_annotation:
+            output_vars = {k: v for k, v in zip(out_, return_annotation)}
+        else:
+            output_vars = {k: None for k in out_}
+    elif isinstance(out_, Mapping):
+        output_vars = out_
+    elif out_ is None:
+        if return_vars is None or len(return_vars) == 0:
+            output_vars = {}
+        else:
+            return_vars = [v if v else f"arg{i}" for i, v in enumerate(return_vars)]
+            if return_annotation:
+                output_vars = {
+                    k: v
+                    for k, v in zip_longest(
+                        return_vars, islice(return_annotation, len(return_vars))
+                    )
+                }
+            else:
+                output_vars = {k: None for k in return_vars}
+    else:
+        raise Exception("Invalid out_ parameter")
+
+    return FunctionAttributes(
+        func, tree, func.__name__, module, input_vars, output_vars
+    )
+
+
+def find_returns(node: ast.expr):
+    rets = []
+    if isinstance(node, ast.Return):
+        return [node]
+    if hasattr(node, "body"):
+        for n in node.body:
+            res = find_returns(n)
+            if res:
+                rets.extend(res)
+    if hasattr(node, "handlers"):
+        for n in node.handlers:
+            res = find_returns(n)
+            if res:
+                rets.extend(res)
+    return rets
+
+
+def get_function_return_var_names(tree: ast.expr, name: str):
+    rets = find_returns(tree)
+    names = None
+    for ret in rets:
+        if ret and isinstance(ret.value, ast.Name):
+            if names is not None and len(names) != 1:
+                raise Exception(f"Different return lengths in {name}")
+            names = [ret.value.id]
+        elif ret and isinstance(ret.value, ast.Constant):
+            if names is not None and len(names) != 1:
+                raise Exception(f"Different return lengths in {name}")
+            names = [None]
+        elif ret and isinstance(ret.value, ast.Tuple):
+            if names is not None and len(names) != len(ret.value.elts):
+                raise Exception(f"Different return lengths in {name}")
+            if names is None:
+                names = [None for _ in range(len(ret.value.elts))]
+            for i, elt in enumerate(ret.value.elts):
+                if isinstance(elt, ast.Name):
+                    names[i] = elt.id
+        else:
+            names = [None]
+    return names
```

### Comparing `pysfn-0.1.8/pysfn/lmbda.py` & `pysfn-0.1.9/pysfn/lmbda.py`

 * *Files identical despite different names*

### Comparing `pysfn-0.1.8/pysfn/s3.py` & `pysfn-0.1.9/pysfn/s3.py`

 * *Files identical despite different names*

### Comparing `pysfn-0.1.8/pysfn/steps.py` & `pysfn-0.1.9/pysfn/steps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1357 +1,1325 @@
-import inspect
-import pathlib
-import ast
-import json
-import typing
-from .function import gather_function_attributes, FunctionAttributes
-from dataclasses import dataclass
-from types import BuiltinFunctionType
-from typing import Dict, List, Callable, Mapping, Any, Union, Iterable, Optional, Type
-
-from aws_cdk import (
-    aws_stepfunctions as sfn,
-    aws_stepfunctions_tasks as tasks,
-    Duration,
-    Stack,
-)
-from aws_cdk.aws_stepfunctions import JsonPath
-
-from .condition import build_condition
-from .s3 import write_json, read_json, build_s3_write_json_step, build_s3_read_json_step
-
-SFN_INDEX = 0
-
-
-@dataclass
-class Retry:
-    errors: List[str]
-    interval_seconds: int
-    max_attempts: int
-    backoff_rate: float = None
-
-
-@dataclass
-class CatchHandler:
-    errors: List[str]
-    body: List[sfn.IChainable]
-    result_path: str = "$.error-info"
-
-
-def concurrent(
-    iterable,
-    max_concurrency: Optional[int] = None,
-    distributed=False,
-    tolerated_failure_percentage=None,
-    tolerated_failure_count=None,
-):
-    pass
-
-
-def event(func: Callable):
-    pass
-
-
-def execution_start_time() -> str:
-    pass
-
-
-def state_entered_time() -> str:
-    pass
-
-
-def await_token(
-    func: Callable,
-    return_args: Union[List[str], Mapping[str, Type]],
-    duration: Duration = None,
-):
-    pass
-
-
-def state_machine(
-    cdk_stack: Stack,
-    sfn_name: str,
-    local_values,
-    express=False,
-    skip_pass=True,
-    return_vars: Optional[Union[List[str], Mapping[str, typing.Type]]] = None,
-):
-    """
-    Function decorator to trigger creation of an AWS Step Functions state machine construct
-    from the instructions in the function.
-    """
-
-    def decorator(func):
-        func_attrs = gather_function_attributes(func, None, return_vars)
-        fts = FunctionToSteps(cdk_stack, func_attrs, local_values, skip_pass=skip_pass)
-        func.state_machine = sfn.StateMachine(
-            cdk_stack,
-            sfn_name,
-            state_machine_name=sfn_name,
-            state_machine_type=sfn.StateMachineType.EXPRESS
-            if express
-            else sfn.StateMachineType.STANDARD,
-            definition=fts.build_sfn_definition(),
-        )
-        func.output = func_attrs.output
-        return func
-
-    return decorator
-
-
-class FunctionToSteps:
-    def __init__(
-        self,
-        cdk_stack: Stack,
-        func_attrs: FunctionAttributes,
-        local_values,
-        skip_pass=True,
-    ):
-        global SFN_INDEX
-        self.cdk_stack = cdk_stack
-        self.func = func_attrs.func
-        self.output = func_attrs.output
-        self.local_values = local_values
-        self.state_number = 0
-        self.sfn_number = SFN_INDEX
-        self.skip_pass = skip_pass
-        SFN_INDEX += 1
-
-        self.ast = func_attrs.tree
-        with open(pathlib.Path("build", f"{func_attrs.name}_ast.txt"), "w") as fp:
-            fp.write(ast.dump(self.ast, indent=2))
-
-        # Get the function root
-        if (
-            isinstance(self.ast, ast.Module)
-            and len(self.ast.body) == 1
-            and isinstance(self.ast.body[0], ast.FunctionDef)
-        ):
-            self.function_def: ast.FunctionDef
-            self.function_def = self.ast.body[0]
-        else:
-            raise Exception("Unexpected function definition")
-
-    def state_name(self, name):
-        self.state_number += 1
-        return f"{name} [{self.sfn_number}:{self.state_number}]"
-
-    def build_sfn_definition(self):
-
-        # TODO: Capture the parameter types to use elsewhere
-        req_params, opt_params = _get_parameters(self.func)
-
-        # Get the root of the function body
-        scope = SFNScope(self)
-        start, next_ = scope.generate_entry_steps(req_params, opt_params)
-        c, n = scope.handle_body(self.function_def.body)
-        advance(next_, c, n)
-
-        write_definition_json(self.func.__name__, start)
-        return start
-
-
-class SFNScope:
-    def __init__(self, fts: FunctionToSteps):
-        self.fts = fts
-        self.cdk_stack = fts.cdk_stack
-        self.state_name = fts.state_name
-        self.variables: Dict[str, typing.Type] = {}
-        self.output = fts.output
-        self.parent_scope = None
-
-    def generate_entry_steps(
-        self, required_parameters, optional_parameters: Mapping[str, Any] = None
-    ):
-        self.variables.update({param: typing.Any for param in required_parameters})
-
-        # The first step will always be to put the inputs on the register
-        start = sfn.Pass(
-            self.cdk_stack, self.state_name("Register Input"), result_path="$.register",
-        )
-        # For optional parameters we'll check if they are present and default them if they aren't
-        c, n = self.build_optional_parameter_steps(optional_parameters)
-        next_ = advance(start.next, c, n)
-        return start, next_
-
-    def build_register_assignment(self, values: Dict, register_path: str = ""):
-        params = values.copy()
-        for k, v in params.items():
-            self._updated_var(k)
-            # CDK is dropping None from parameters for some reason, using this to hack around it
-            if v is None:
-                params[k] = ""
-        # Copy over any variables that aren't in the params
-        for v in self.variables.keys():
-            if v not in params:
-                params[v] = JsonPath.string_at(f"$.{register_path}{v}")
-        for key in values.keys():
-            if key not in self.variables:
-                # TODO: Assign the type of the value
-                self.add_var(key)
-
-        params = {update_param_name(k, v): v for k, v in params.items()}
-        return params
-
-    def add_var(self, key: str, var_type: Type = Any):
-        self.variables[key] = var_type
-        self._added_var(key)
-
-    def _added_var(self, var: str):
-        pass
-
-    def _updated_var(self, var: str):
-        if self.parent_scope:
-            self.parent_scope._updated_var(var)
-
-    def handle_body(self, body: List[ast.stmt]) -> (List[sfn.IChainable], Callable):
-        chain = []
-        next_ = None
-        for stmt in body:
-            c, n = self.handle_op(stmt)
-            chain.extend(c)
-            if next_:
-                next_ = advance(next_, c, n)
-            else:
-                next_ = n
-        return chain, next_
-
-    def handle_op(self, stmt: ast.stmt) -> (List[sfn.IChainable], Callable):
-        if isinstance(stmt, ast.AnnAssign) or isinstance(stmt, ast.Assign):
-            # if isinstance(stmt.value, ast.Constant):
-            #    return self.handle_assign_value(stmt)
-            if isinstance(stmt.value, ast.Call) and isinstance(
-                stmt.value.func, ast.Name
-            ):
-                return self.handle_call_function(stmt.value, stmt)
-            if isinstance(stmt.value, ast.ListComp):
-                return self.handle_list_comp(stmt)
-            else:
-                return self.handle_assign_value(stmt)
-        elif isinstance(stmt, ast.If):
-            return self.handle_if(stmt)
-        elif isinstance(stmt, ast.Return):
-            return self.handle_return(stmt)
-        elif isinstance(stmt, ast.Expr) and isinstance(stmt.value, ast.Call):
-            if isinstance(stmt.value.func, ast.Name):
-                return self.handle_call_function(stmt.value)
-            elif isinstance(stmt.value.func, ast.Attribute):
-                if stmt.value.func.attr == "append":
-                    return self.handle_array_append(stmt.value)
-                elif stmt.value.func.attr == "extend":
-                    # TODO
-                    pass
-        elif isinstance(stmt, ast.With):
-            return self.handle_with(stmt)
-        elif isinstance(stmt, ast.Try):
-            return self.handle_try(stmt)
-        elif isinstance(stmt, ast.For):
-            return self.handle_for(stmt)
-        elif isinstance(stmt, ast.AugAssign) and (
-            isinstance(stmt.op, ast.Add) or isinstance(stmt.op, ast.Sub)
-        ):
-            return self.handle_math_add(stmt)
-        elif isinstance(stmt, ast.Pass):
-            if self.fts.skip_pass:
-                return [], None
-            else:
-                pass_step = sfn.Pass(self.cdk_stack, self.state_name("Pass"))
-                return [pass_step], pass_step.next
-
-        # Treat unhandled statements as a no-op
-        print(f"Unhandled {repr(stmt)}")
-        print(ast.dump(stmt, indent=2))
-        return [], None
-
-    def handle_with(self, stmt: ast.With):
-        w_val = self.build_with(stmt)
-        chain, n = self.handle_body(stmt.body)
-        for s in chain:
-            if hasattr(s, "add_retry"):
-                s.add_retry(
-                    errors=w_val.errors,
-                    max_attempts=w_val.max_attempts,
-                    interval=Duration.seconds(w_val.interval_seconds),
-                    backoff_rate=w_val.backoff_rate,
-                )
-        return chain, n
-
-    def handle_try(self, stmt: ast.Try):
-        chain, n = ChildScope(self).handle_body(stmt.body)
-        nexts = [n]
-        handlers = []
-        for handler in stmt.handlers:
-            child_scope = ChildScope(self)
-            result_path = None
-            h_chain, h_n = child_scope.handle_body(handler.body)
-            if handler.name:
-                result_path = f"$.register.{handler.name}"
-                child_scope.add_var(handler.name)
-                if h_chain:
-                    process_exception = sfn.Pass(
-                        self.cdk_stack,
-                        self.state_name(f"Interpret {handler.name}"),
-                        input_path="$.register",
-                        parameters=child_scope.build_register_assignment(
-                            {
-                                handler.name: JsonPath.string_at(
-                                    f"States.StringToJson($.{handler.name}.Cause)"
-                                )
-                            }
-                        ),
-                        result_path="$.register",
-                    )
-                    process_exception_choice = sfn.Choice(
-                        self.cdk_stack,
-                        self.state_name(f"Interpret Choice {handler.name}"),
-                    )
-                    process_exception_cause = sfn.Pass(
-                        self.cdk_stack,
-                        self.state_name(f"Interpret {handler.name}"),
-                        input_path="$.register",
-                        parameters=child_scope.build_register_assignment(
-                            {
-                                handler.name: {
-                                    "Cause": JsonPath.string_at(
-                                        f"States.StringToJson($.{handler.name}.Cause)"
-                                    ),
-                                    "Error": JsonPath.string_at(
-                                        f"$.{handler.name}.Error"
-                                    ),
-                                    "ExecutionArn": JsonPath.string_at(
-                                        f"$.{handler.name}.ExecutionArn"
-                                    ),
-                                    "Name": JsonPath.string_at(
-                                        f"$.{handler.name}.Name"
-                                    ),
-                                    "Status": JsonPath.string_at(
-                                        f"$.{handler.name}.Status"
-                                    ),
-                                }
-                            }
-                        ),
-                        result_path="$.register",
-                    )
-                    format_string = "{}{}"
-                    split = "{"
-                    process_exception_malformed_cause = sfn.Pass(
-                        self.cdk_stack,
-                        self.state_name(f"Interpret {handler.name}"),
-                        input_path="$.register",
-                        parameters=child_scope.build_register_assignment(
-                            {
-                                handler.name: {
-                                    "Cause": JsonPath.string_at(
-                                        f"States.StringToJson(States.Format('{format_string}', '{split}', States.ArrayGetItem(States.StringSplit($.{handler.name}.Cause, '{split}'), 1)))"
-                                    ),
-                                    "Error": JsonPath.string_at(
-                                        f"$.{handler.name}.Error"
-                                    ),
-                                    "ExecutionArn": JsonPath.string_at(
-                                        f"$.{handler.name}.ExecutionArn"
-                                    ),
-                                    "Name": JsonPath.string_at(
-                                        f"$.{handler.name}.Name"
-                                    ),
-                                    "Status": JsonPath.string_at(
-                                        f"$.{handler.name}.Status"
-                                    ),
-                                }
-                            }
-                        ),
-                        result_path="$.register",
-                    )
-                    process_exception_default = sfn.Pass(
-                        self.cdk_stack,
-                        self.state_name(f"Interpret {handler.name}"),
-                        input_path="$.register",
-                        parameters=child_scope.build_register_assignment(
-                            {
-                                handler.name: {
-                                    "ExecutionArn": JsonPath.string_at(
-                                        f"$.{handler.name}.ExecutionArn"
-                                    ),
-                                    "Name": JsonPath.string_at(
-                                        f"$.{handler.name}.Name"
-                                    ),
-                                    "Status": JsonPath.string_at(
-                                        f"$.{handler.name}.Status"
-                                    ),
-                                }
-                            }
-                        ),
-                        result_path="$.register",
-                    )
-                    process_exception.next(process_exception_choice)
-                    process_exception_choice.when(
-                        sfn.Condition.and_(
-                            sfn.Condition.is_present(
-                                f"$.register.{handler.name}.Cause"
-                            ),
-                            sfn.Condition.string_matches(
-                                f"$.register.{handler.name}.Cause",
-                                "The cause could not be determined*",
-                            ),
-                        ),
-                        process_exception_malformed_cause,
-                    )
-                    process_exception_choice.when(
-                        sfn.Condition.is_present(f"$.register.{handler.name}.Cause"),
-                        process_exception_cause,
-                    )
-                    process_exception_choice.otherwise(process_exception_default)
-                    process_exception_cause.next(h_chain[0])
-                    process_exception_malformed_cause.next(h_chain[0])
-                    process_exception_default.next(h_chain[0])
-                    h_chain = [
-                        process_exception,
-                        process_exception_choice,
-                        process_exception_cause,
-                        process_exception_malformed_cause,
-                        process_exception_default,
-                    ] + h_chain
-
-            # If the handler body isn't empty, add it in
-            if h_chain:
-                chain.extend(h_chain)
-                nexts.append(h_n)
-            handlers.append(self.build_exception_handler(handler, h_chain, result_path))
-
-        for s in chain:
-            if hasattr(s, "add_catch"):
-                for handler in handlers:
-                    nn = self.attach_catch(s, handler)
-                    if nn:
-                        nexts.append(nn)
-
-        return chain, nexts
-
-    def build_exception_handler(
-        self,
-        handler: ast.ExceptHandler,
-        chain: List[sfn.IChainable],
-        result_path: str = None,
-    ):
-        if isinstance(handler.type, ast.Name) and handler.type.id == "Exception":
-            return CatchHandler(["States.ALL"], chain, result_path=result_path)
-        raise Exception(f"Unhandled exception of type {handler.type}")
-
-    @staticmethod
-    def attach_catch(step, handler):
-        def inner_next(n):
-            step.add_catch(
-                n, errors=handler.errors, result_path=handler.result_path,
-            )
-
-        if handler.body:
-            advance(inner_next, handler.body, None)
-            return None
-        else:
-            return inner_next
-
-    def build_with(self, stmt: ast.With):
-        if len(stmt.items) != 1:
-            raise Exception(f"With statements can only support a single item")
-        call = stmt.items[0].context_expr
-        if isinstance(call, ast.Call):
-            if call.func.id == "Retry":
-                params = self.build_parameters(call, Retry, False)
-                return Retry(**params)
-        raise Exception(f"Unhandled with operation: {call}")
-
-    @staticmethod
-    def map_arg(arg: ast.expr, var_path: str = ""):
-        if isinstance(arg, ast.Name):
-            return f"$.{var_path}{arg.id}"
-        elif isinstance(arg, ast.Constant):
-            return arg.value
-        elif (
-            isinstance(arg, ast.Subscript)
-            and isinstance(arg.value, ast.Name)
-            and isinstance(arg.slice, ast.Constant)
-        ):
-            return f"$.{var_path}{arg.value.id}[{arg.slice.value}]"
-        else:
-            raise Exception("Args must be Name or Constant")
-
-    def _get_iterator(self, iterator: ast.expr) -> (str, str, sfn.State, int):
-        # TODO: Support enumerate
-        # TODO: Support callable iterator
-        max_concurrency = 1
-        iterator_step = None
-        distributed = False
-        tol_fail_perc = None
-        tol_fail_count = None
-
-        # if the iterator is wrapped in a 'concurrent' function, capture the parameter as the concurrency for the map
-        if (
-            isinstance(iterator, ast.Call)
-            and isinstance(iterator.func, ast.Name)
-            and iterator.func.id == "concurrent"
-        ):
-            args, kwargs = get_call_args(iterator)
-            m_c = kwargs.get("max_concurrency")
-            if len(args) > 1 and isinstance(args[1], ast.Constant):
-                # TODO: Check for type other than constant
-                max_concurrency = args[1].value
-            if m_c and isinstance(m_c, ast.Constant):
-                max_concurrency = m_c.value
-            else:
-                max_concurrency = 0
-            distributed = kwargs.get("distributed", False)
-            tol_fail_perc = kwargs.get("tolerated_failure_percentage")
-            tol_fail_count = kwargs.get("tolerated_failure_count")
-
-            iterator = iterator.args[0]
-
-        if isinstance(iterator, ast.Call) and self._is_intrinsic_function(iterator):
-            items_path, iter_var = self._intrinsic_function(iterator)
-            iterator_step = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Build {iter_var}"),
-                input_path="$.register",
-                result_path="$.iter",
-                parameters={iter_var: items_path},
-            )
-            iter_var = iterator.func.id
-            items_path = f"$.iter.{iter_var}"
-        elif isinstance(iterator, ast.Call) and isinstance(iterator.func, ast.Name):
-            (
-                iterator_step,
-                return_vars,
-                func_name,
-                result_prefix,
-            ) = self._build_func_call(iterator, "$.iter")
-            iter_var = iterator.func.id
-            items_path = f"$.iter{result_prefix}.{return_vars[0]}"
-
-        # If the iterator is a name, use that value
-        elif isinstance(iterator, ast.Name):
-            iter_var = iterator.id
-            items_path = f"$.register.{iter_var}"
-        else:
-            raise Exception("Unsupported for-loop iterator, variables only")
-        return (
-            iter_var,
-            items_path,
-            iterator_step,
-            max_concurrency,
-            distributed,
-            tol_fail_perc,
-            tol_fail_count,
-        )
-
-    def handle_for(self, stmt: ast.For):
-        (
-            iter_var,
-            items_path,
-            iterator_step,
-            max_concurrency,
-            distributed,
-            tol_fail_perc,
-            tol_fail_count,
-        ) = self._get_iterator(stmt.iter)
-        if not isinstance(stmt.target, ast.Name):
-            raise Exception("Unsupported for-loop target, variables only")
-
-        map_state = sfn.Map(
-            self.cdk_stack,
-            self.state_name(f"For {iter_var}"),
-            max_concurrency=max_concurrency,
-            items_path=items_path,
-            parameters={
-                "register.$": f"$.register",
-                f"{stmt.target.id}.$": "$$.Map.Item.Value",
-            },
-            result_path="$.register.loopResult",
-        )
-
-        # Create a scope for the for loop contents and build the contained steps
-        # Also build an entry step to capture the iterator target
-        map_scope = MapScope(self)
-        entry_step = map_scope.build_entry_step(stmt.target.id)
-        chain, map_next_ = map_scope.handle_body(stmt.body)
-        entry_step.next(chain[0])
-        map_state.iterator(entry_step)
-        next_ = map_state.next
-
-        # if any vars from the outer scope were updated, add a 'return' step to the map operations and
-        # logic to pull those results into the register after the map completes
-        map_return_step_name = self.state_name("Map return")
-        if map_scope.updated_vars:
-            return_params = {
-                v: JsonPath.string_at(f"$.register.{v}") for v in map_scope.updated_vars
-            }
-            map_return_step = sfn.Pass(
-                self.cdk_stack, map_return_step_name, parameters=return_params
-            )
-            consolidate_params = {
-                v: JsonPath.string_at(f"$.register.loopResult[*].{v}[*]")
-                for v in map_scope.updated_vars
-            }
-            consolidate_step = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Consolidate map results"),
-                result_path="$.register",
-                parameters=self.build_register_assignment(
-                    consolidate_params, "register."
-                ),
-            )
-            map_state.next(consolidate_step)
-            next_ = consolidate_step.next
-        else:
-            map_return_step = sfn.Pass(
-                self.cdk_stack, map_return_step_name, parameters={}
-            )
-        advance(map_next_, [map_return_step], map_return_step.next)
-
-        # finalize the steps
-        if iterator_step:
-            iterator_step.next(map_state)
-            return [iterator_step, map_state], next_
-        else:
-            return [map_state], next_
-
-    def handle_list_comp(self, stmt: Union[ast.Assign, ast.AnnAssign]):
-        target = stmt.targets[0] if isinstance(stmt, ast.Assign) else stmt.target
-        if isinstance(target, ast.Name):
-            target = target.id
-        else:
-            raise Exception("Unsupported list comp target, variables only")
-
-        list_comp = stmt.value
-        if not isinstance(list_comp, ast.ListComp):
-            raise Exception("Unhandled list comp value")
-        if len(list_comp.generators) != 1:
-            raise Exception("List comp can only support a single generator")
-        comp = list_comp.generators[0]
-        if not isinstance(comp, ast.comprehension):
-            raise Exception(f"Unhandled generator {type(comp)}")
-
-        # TODO: Support enumerate...
-        if (
-            isinstance(comp.iter, ast.Call)
-            and isinstance(comp.iter.func, ast.Name)
-            and comp.iter.func.id == "concurrent"
-        ):
-            max_concurrency = comp.iter.args[1].value
-            iter_var = comp.iter.args[0].id
-        elif isinstance(comp.iter, ast.Name):
-            max_concurrency = 0
-            iter_var = comp.iter.id
-        else:
-            raise Exception("Unsupported list comp iterator, variables only")
-        if not isinstance(comp.target, ast.Name):
-            raise Exception("Unsupported list comp target, variables only")
-
-        choice_name = self.state_name(f"Has {iter_var} to map")
-        map_state = sfn.Map(
-            self.cdk_stack,
-            self.state_name(f"For {iter_var}"),
-            max_concurrency=max_concurrency,
-            items_path=f"$.register.{iter_var}",
-            parameters={
-                "register.$": f"$.register",
-                f"{comp.target.id}.$": "$$.Map.Item.Value",
-            },
-            result_path="$.loopResult",
-        )
-        choice = sfn.Choice(self.cdk_stack, choice_name)
-        choice.when(
-            sfn.Condition.and_(
-                sfn.Condition.is_present(f"$.register.{iter_var}"),
-                sfn.Condition.is_present(f"$.register.{iter_var}[0]"),
-            ),
-            map_state,
-        )
-
-        call_func = sfn.Pass(
-            self.cdk_stack,
-            self.state_name(f"Call function..."),
-            parameters={"loopResult": JsonPath.string_at(f"$.{comp.target.id}")},
-        )
-
-        map_state.iterator(call_func)
-        consolidate_step = sfn.Pass(
-            self.cdk_stack,
-            self.state_name(f"Consolidate map results"),
-            result_path="$.register",
-            parameters=self.build_register_assignment(
-                {target: JsonPath.string_at(f"$.loopResult[*][*]")},
-                "loopResult[0].register.",
-            ),
-        )
-        map_state.next(consolidate_step)
-
-        return [choice, map_state], [choice.otherwise, consolidate_step.next]
-
-    def handle_math_add(self, stmt: ast.AugAssign):
-        if isinstance(stmt.target, ast.Name):
-            target = stmt.target.id
-        else:
-            raise Exception(f"Unexpected MathAdd target {type(stmt.target)}")
-        if isinstance(stmt.value, ast.Constant):
-            if isinstance(stmt.op, ast.Add):
-                value = stmt.value.value
-            elif isinstance(stmt.op, ast.Sub):
-                value = -stmt.value.value
-            else:
-                raise Exception(f"Unsupported MathAdd op {type(stmt.op)}")
-        else:
-            raise Exception(f"Unsupported MathAdd target {type(stmt.value)}")
-        add_step = sfn.Pass(
-            self.cdk_stack,
-            self.state_name(f"Add {value} to {target}"),
-            input_path="$.register",
-            result_path="$.register",
-            parameters=self.build_register_assignment(
-                {target: JsonPath.string_at(f"States.MathAdd($.{target}, {value})")}
-            ),
-        )
-        return [add_step], add_step.next
-
-    def handle_array_append(self, stmt: ast.Call):
-        array_name = stmt.func.value.id
-        array_path = f"$.register.{array_name}"
-        arg = stmt.args[0]
-        if isinstance(arg, ast.Name):
-            value = arg.id
-            path_to_add = f"$.register.{arg.id}"
-        elif isinstance(arg, ast.Constant):
-            value = arg.value
-            path_to_add = arg.value
-        else:
-            raise Exception(f"Unexpected type {type(arg)} for list append")
-        list_step = sfn.Pass(
-            self.cdk_stack,
-            self.state_name(f"Append {value} to {array_name}"),
-            result_path="$.meta",
-            parameters={
-                "arrayConcat": JsonPath.string_at(
-                    f"States.Array({array_path}, States.Array({path_to_add}))"
-                )
-            },
-        )
-        flatten_step = sfn.Pass(
-            self.cdk_stack,
-            self.state_name(f"Flatten {array_name}"),
-            result_path="$.register",
-            parameters=self.build_register_assignment(
-                {array_name: JsonPath.string_at("$.meta.arrayConcat[*][*]")},
-                "register.",
-            ),
-        )
-        list_step.next(flatten_step)
-        return [list_step, flatten_step], flatten_step.next
-
-    def handle_assign_value(
-        self, stmt: Union[ast.AnnAssign, ast.Assign]
-    ) -> (List[sfn.IChainable], Callable):
-        sub_target = None
-        if isinstance(stmt, ast.AnnAssign):
-            if isinstance(stmt.target, ast.Name):
-                var_name = stmt.target.id
-            elif (
-                isinstance(stmt.target, ast.Subscript)
-                and isinstance(stmt.target.value, ast.Name)
-                and isinstance(stmt.target.slice, ast.Constant)
-            ):
-                var_name = stmt.target.value.id
-                sub_target = stmt.target.slice.value
-            else:
-                raise Exception(
-                    f"Unexpected assignment target of type {type(stmt.target)}"
-                )
-        else:
-            if len(stmt.targets) == 1 and isinstance(stmt.targets[0], ast.Name):
-                var_name = stmt.targets[0].id
-            elif (
-                isinstance(stmt.targets[0], ast.Subscript)
-                and isinstance(stmt.targets[0].value, ast.Name)
-                and isinstance(stmt.targets[0].slice, ast.Constant)
-            ):
-                var_name = stmt.targets[0].value.id
-                sub_target = stmt.targets[0].slice.value
-            else:
-                raise Exception("Unexpected assignment")
-        if sub_target:
-            prep = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Prep assign {var_name}.{sub_target}"),
-                input_path="$.register",
-                result_path="$.register.itm",
-                parameters={sub_target: self.generate_value_repr(stmt.value)},
-            )
-            assign = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Assign {var_name}.{sub_target}"),
-                input_path="$.register",
-                result_path="$.register",
-                parameters=self.build_register_assignment(
-                    # {f"{var_name}": JsonPath.json_merge(f"$.{var_name}", "$.itm")}
-                    {f"{var_name}": f"States.JsonMerge($.{var_name}, $.itm, false)"}
-                ),
-            )
-            prep.next(assign)
-            return [prep, assign], assign.next
-        else:
-            value = self.generate_value_repr(stmt.value)
-            assign = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Assign {var_name}"),
-                input_path="$.register",
-                result_path="$.register",
-                parameters=self.build_register_assignment({var_name: value}),
-            )
-            return [assign], assign.next
-
-    def handle_if(self, stmt: ast.If) -> (List[sfn.IChainable], Callable):
-        condition, name = build_condition(stmt.test)
-        choice = sfn.Choice(self.cdk_stack, self.state_name(name))
-
-        def if_next(step):
-            choice.when(condition, step)
-
-        if_c, if_n = ChildScope(self).handle_body(stmt.body)
-        else_c, else_n = ChildScope(self).handle_body(stmt.orelse)
-        if_n = advance(if_next, if_c, if_n)
-        else_n = advance(choice.otherwise, else_c, else_n)
-        chain = [choice]
-        if if_c:
-            chain.extend(if_c)
-        if else_c:
-            chain.extend(else_c)
-        return chain, [if_n, else_n]
-
-    def _is_intrinsic_function(self, call: ast.Call):
-        return isinstance(call.func, ast.Name) and call.func.id in [
-            "range",
-            "len",
-            "execution_start_time",
-            "state_entered_time",
-        ]
-
-    def _intrinsic_function(self, call: ast.Call, var_path: str = ""):
-        if isinstance(call.func, ast.Name):
-            args = [self.map_arg(arg, var_path) for arg in call.args]
-            if call.func.id == "range":
-                start_val = 0
-                end_val = 0
-                step_val = 1
-                if len(args) == 1:
-                    end_val = args[0]
-                elif len(args) >= 2:
-                    start_val = args[0]
-                    end_val = args[1]
-                if len(args) == 3:
-                    step_val = args[2]
-                return (
-                    JsonPath.string_at(
-                        f"States.ArrayRange({start_val}, States.MathAdd({end_val}, -1), {step_val})"
-                    ),
-                    "range",
-                )
-            elif call.func.id == "len":
-                if len(args) == 1:
-                    return (
-                        JsonPath.string_at(f"States.ArrayLength({args[0]})"),
-                        "len",
-                    )
-            elif call.func.id == "execution_start_time":
-                return (
-                    JsonPath.string_at(f"$$.Execution.StartTime"),
-                    "time",
-                )
-            elif call.func.id == "state_entered_time":
-                return (
-                    JsonPath.string_at(f"$$.State.EnteredTime"),
-                    "time",
-                )
-        raise Exception("Cannot handle intrinsic function")
-
-    def _build_func_call(
-        self,
-        call: ast.Call,
-        result_path: str = "$.register.out",
-        invoke_event_: bool = False,
-        await_token_: bool = False,
-        await_duration_: Duration = None,
-    ) -> (sfn.State, List[str], str):
-        if isinstance(call.func, ast.Name):
-            # Get the function
-            func = self.fts.local_values.get(call.func.id)
-            result_prefix = ""
-
-            # Build the parameters
-            if func:
-                params = self.build_parameters(call, func)
-                if hasattr(func, "get_additional_params"):
-                    params.update(func.get_additional_params())
-            elif call.func.id == write_json.__name__:
-                params = self.build_parameters(call, write_json, False)
-            elif call.func.id == read_json.__name__:
-                params = self.build_parameters(call, read_json, False)
-            elif call.func.id in [
-                "time.sleep",
-                "sleep",
-                event.__name__,
-                await_token.__name__,
-            ]:
-                params = {}
-            else:
-                raise Exception(f"Unable to find function {call.func.id}")
-
-            if call.func.id in ["time.sleep", "sleep"]:
-                invoke = sfn.Wait(
-                    self.cdk_stack,
-                    self.state_name("Wait"),
-                    time=sfn.WaitTime.duration(Duration.seconds(call.args[0].value)),
-                )
-                return_vars = []
-            elif (
-                call.func.id == event.__name__
-                and len(call.args) > 0
-                and isinstance(call.args[0], ast.Call)
-            ):
-                return self._build_func_call(
-                    call.args[0], result_path=result_path, invoke_event_=True
-                )
-            elif (
-                call.func.id == await_token.__name__
-                and len(call.args) >= 2
-                and isinstance(call.args[0], ast.Call)
-            ):
-                duration = None
-                if len(call.args) == 3:
-                    duration_arg = call.args[2]
-                    if isinstance(duration_arg, ast.Call) and isinstance(
-                        duration_arg.func, ast.Attribute
-                    ):
-                        attr_name = duration_arg.func.attr
-                        if len(duration_arg.args) > 0:
-                            duration_arg_value = duration_arg.args[0]
-                            if isinstance(duration_arg_value, ast.Constant):
-                                duration = getattr(Duration, attr_name)(
-                                    duration_arg_value.value
-                                )
-                invoke, return_vars, name, result_prefix = self._build_func_call(
-                    call.args[0],
-                    result_path=result_path,
-                    invoke_event_=True,
-                    await_token_=True,
-                    await_duration_=duration,
-                )
-                return_arg = call.args[1]
-                if isinstance(return_arg, ast.List) and all(
-                    isinstance(a, ast.Constant) for a in return_arg.elts
-                ):
-                    return_vars = [a.value for a in return_arg.elts]
-                return invoke, return_vars, name, ""
-            elif hasattr(func, "definition"):
-                invocation_type = tasks.LambdaInvocationType.REQUEST_RESPONSE
-                integration_pattern = sfn.IntegrationPattern.REQUEST_RESPONSE
-                if invoke_event_:
-                    invocation_type = tasks.LambdaInvocationType.EVENT
-                if await_token_:
-                    integration_pattern = sfn.IntegrationPattern.WAIT_FOR_TASK_TOKEN
-                invoke = tasks.LambdaInvoke(
-                    self.cdk_stack,
-                    self.state_name(f"Call {call.func.id}"),
-                    lambda_function=func.get_lambda(),
-                    payload=sfn.TaskInput.from_object(params),
-                    input_path="$.register",
-                    result_path=result_path,
-                    invocation_type=invocation_type,
-                    integration_pattern=integration_pattern,
-                    heartbeat=await_duration_,
-                )
-                return_vars = list(func.definition.output.keys())
-                result_prefix = ".Payload"
-            elif hasattr(func, "state_machine"):
-                invoke = tasks.StepFunctionsStartExecution(
-                    self.cdk_stack,
-                    self.state_name(f"Call {func.state_machine.state_machine_name}"),
-                    state_machine=func.state_machine,
-                    input_path="$.register",
-                    result_path=result_path,
-                    integration_pattern=sfn.IntegrationPattern.RUN_JOB,
-                    input=sfn.TaskInput.from_object(params),
-                )
-                return_vars = list(func.output.keys())
-                result_prefix = ".Output"
-            elif call.func.id == write_json.__name__:
-                invoke = build_s3_write_json_step(
-                    self.cdk_stack, self.state_name("S3 Write JSON"), **params
-                )
-                return_vars = ["ETag"]
-                result_prefix = ""
-            elif call.func.id == read_json.__name__:
-                invoke = build_s3_read_json_step(
-                    self.cdk_stack, self.state_name("S3 Read JSON"), **params
-                )
-                return_vars = ["Body", "LastModified", "ETag"]
-                result_prefix = ""
-            else:
-                raise Exception(
-                    f"Function without an associated Lambda: {call.func.id}"
-                )
-            return invoke, return_vars, call.func.id, result_prefix
-        else:
-            raise Exception(
-                f"Function attribute is not of type name: {type(call.func)}"
-            )
-
-    def handle_call_function(
-        self, call: ast.Call, assign: Union[ast.Assign, ast.AnnAssign] = None,
-    ) -> (List[sfn.IChainable], Callable):
-        if self._is_intrinsic_function(call):
-            if not assign:
-                raise Exception(
-                    f"Call to intrinsic function {call.func.id} must be assigned to a value"
-                )
-            val, name = self._intrinsic_function(call)
-            target = (
-                assign.targets[0] if isinstance(assign, ast.Assign) else assign.target
-            )
-            if isinstance(target, ast.Name):
-                result_target = target.id
-            else:
-                raise Exception("Invalid intrinsic function target")
-
-            register = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Register {name}"),
-                input_path="$.register",
-                result_path="$.register",
-                parameters=self.build_register_assignment({result_target: val}),
-            )
-            return [register], register.next
-        else:
-            invoke, return_vars, name, result_prefix = self._build_func_call(
-                call, "$.register.out"
-            )
-            chain = [invoke]
-            next_ = invoke.next
-
-            if assign:
-                # Get the result variable names
-                target = (
-                    assign.targets[0]
-                    if isinstance(assign, ast.Assign)
-                    else assign.target
-                )
-                if isinstance(target, ast.Name):
-                    result_targets = [target.id]
-                elif isinstance(target, ast.Tuple) and all(
-                    isinstance(t, ast.Name) for t in target.elts
-                ):
-                    result_targets = [n.id for n in target.elts]
-                else:
-                    raise Exception(
-                        f"Unexpected result target of type {type(assign.target)}"
-                    )
-                result_params = {
-                    v: JsonPath.string_at(f"$.out{result_prefix}.{r}")
-                    for v, r in zip(result_targets, return_vars)
-                }
-                if len(result_params) < len(result_targets):
-                    raise Exception(
-                        f"Unable to map all response targets to return values for {name}"
-                    )
-                register = sfn.Pass(
-                    self.cdk_stack,
-                    self.state_name(f"Register {call.func.id}"),
-                    input_path="$.register",
-                    result_path="$.register",
-                    parameters=self.build_register_assignment(result_params),
-                )
-                invoke.next(register)
-                chain.append(register)
-                next_ = register.next
-
-            return chain, next_
-
-    def _return_value(self, value: Union[ast.expr, ast.stmt]):
-        if isinstance(value, ast.Name):
-            return JsonPath.string_at(f"$.register.{value.id}")
-        elif isinstance(value, ast.Constant):
-            return value.value
-        elif isinstance(value, ast.Call) and self._is_intrinsic_function(value):
-            val, name = self._intrinsic_function(value)
-            return val
-        else:
-            raise Exception(f"Unanticipated return type: {value}")
-
-    def handle_return(self, stmt: ast.Return):
-        if isinstance(stmt.value, ast.Tuple):
-            if len(self.output) != len(stmt.value.elts):
-                raise Exception("Mismatched return value counts")
-            return_step = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Return"),
-                parameters={
-                    k: self._return_value(v)
-                    for k, v in zip(self.output.keys(), stmt.value.elts)
-                },
-            )
-        elif isinstance(stmt.value, ast.Name) or isinstance(stmt.value, ast.Constant):
-            if len(self.output) != 1:
-                raise Exception("Mismatched return value counts")
-            return_step = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Return"),
-                parameters={
-                    list(self.output.keys())[0]: self._return_value(stmt.value)
-                },
-            )
-        elif stmt.value is None:
-            return_step = sfn.Pass(self.cdk_stack, self.state_name(f"Return"))
-        else:
-            raise Exception(f"Unhandled return value type {stmt.value}")
-        return [return_step], return_step.next
-
-    def build_parameters(self, call: ast.Call, func: Callable, gen_jsonpath=True):
-        params = {}
-
-        # TODO: Handle kwonly args
-        if hasattr(func, "definition"):
-            args = func.definition.input.keys()
-        elif isinstance(func, BuiltinFunctionType):
-            return None
-        else:
-            args = inspect.getfullargspec(func).args
-            if len(args) > 0 and args[0] == "self":
-                args = args[1:]
-
-        # Add the positional parameters
-        for arg_value, arg_name in zip(call.args, args):
-            params[arg_name] = self.generate_value_repr(arg_value, gen_jsonpath)
-
-        # Add the keyword parameters
-        for kw in call.keywords:
-            params[kw.arg] = self.generate_value_repr(kw.value, gen_jsonpath)
-        return params
-
-    def build_optional_parameter_steps(self, optional_parameters: Mapping[str, Any]):
-        chain = []
-        next_ = None
-        for name, value in optional_parameters.items():
-            choice_name = self.state_name(f"Has {name}")
-            assign = sfn.Pass(
-                self.cdk_stack,
-                self.state_name(f"Assign {name} default"),
-                input_path="$.register",
-                result_path="$.register",
-                parameters=self.build_register_assignment({name: value}),
-            )
-            choice = sfn.Choice(self.cdk_stack, choice_name)
-            choice.when(sfn.Condition.is_not_present(f"$.register.{name}"), assign)
-            chain.extend([choice, assign])
-            if next_:
-                next_ = advance(next_, choice, [choice.otherwise, assign.next])
-            else:
-                next_ = [choice.otherwise, assign.next]
-        return chain, next_
-
-    def evaluate_path(self, stmt: ast.Subscript) -> str:
-        if isinstance(stmt.slice, ast.Constant):
-            if isinstance(stmt.slice.value, int):
-                slce = f"[{stmt.slice.value}]"
-            else:
-                slce = f".{stmt.slice.value}"
-        else:
-            raise Exception("Subscript slice that's not a Constant")
-        if isinstance(stmt.value, ast.Name):
-            return stmt.value.id + slce
-        elif isinstance(stmt.value, ast.Subscript):
-            return self.evaluate_path(stmt.value) + slce
-        else:
-            raise Exception("Unexpected Subscript value")
-
-    def generate_value_repr(self, arg_value, gen_jsonpath=True):
-        if isinstance(arg_value, ast.Name):
-            # if arg_value.id not in self.variables:
-            #    raise Exception(f"Undefined variable {arg_value.id}")
-            expr = f"$.{arg_value.id}"
-            return JsonPath.string_at(expr) if gen_jsonpath else expr
-        elif isinstance(arg_value, ast.Constant):
-            return arg_value.value
-        elif isinstance(arg_value, ast.List):
-            expr = [self.generate_value_repr(val, False) for val in arg_value.elts]
-            return JsonPath.array(*expr) if gen_jsonpath else expr
-        elif isinstance(arg_value, ast.Subscript):
-            expr = "$." + self.evaluate_path(arg_value)
-            return JsonPath.string_at(expr) if gen_jsonpath else expr
-        elif isinstance(arg_value, ast.Call) and self._is_intrinsic_function(arg_value):
-            path, name = self._intrinsic_function(arg_value)
-            return path
-        elif isinstance(arg_value, ast.Dict):
-            obj = {}
-            for k, v in zip(arg_value.keys, arg_value.values):
-                if not isinstance(k, ast.Constant):
-                    raise Exception("Dict keys must be a constant")
-                else:
-                    obj[k.value] = self.generate_value_repr(v, gen_jsonpath)
-            return obj
-        # TODO: evaluate if this hack for handling JsonPath values is the best approach
-        elif isinstance(arg_value, ast.Attribute) and (
-            (
-                isinstance(arg_value.value, ast.Attribute)
-                and arg_value.value.attr == "JsonPath"
-            )
-            or (
-                isinstance(arg_value.value, ast.Name)
-                and arg_value.value.id == "JsonPath"
-            )
-        ):
-            return getattr(JsonPath, arg_value.attr)
-        elif (
-            isinstance(arg_value, ast.Call)
-            and isinstance(arg_value.func, ast.Attribute)
-            and (
-                (
-                    isinstance(arg_value.func.value, ast.Name)
-                    and arg_value.func.value.id == "JsonPath"
-                )
-                or (
-                    isinstance(arg_value.func.value, ast.Attribute)
-                    and arg_value.func.value.attr == "JsonPath"
-                )
-            )
-        ):
-            return getattr(JsonPath, arg_value.func.attr)(
-                *[self.generate_value_repr(arg, gen_jsonpath) for arg in arg_value.args]
-            )
-        elif (
-            isinstance(arg_value, ast.Attribute)
-            and isinstance(arg_value.value, ast.Name)
-            and arg_value.value.id == "self"
-        ):
-            s = self.fts.local_values.get(arg_value.value.id)
-            var = s.__getattribute__(arg_value.attr)
-            return var
-        elif isinstance(arg_value, ast.Call) and (
-            (
-                isinstance(arg_value.func, ast.Attribute)
-                and isinstance(arg_value.func.value, ast.Name)
-                and arg_value.func.value.id == "JsonPath"
-            )
-        ):
-            # TODO: Handle multi arg inputs
-            arg = self.generate_value_repr(arg_value.args[0], gen_jsonpath=True)
-            return getattr(JsonPath, arg_value.func.attr)(arg)
-        else:
-            print(ast.dump(arg_value, indent=2))
-            raise Exception(f"Unexpected argument: {ast.dump(arg_value)}")
-
-
-class MapScope(SFNScope):
-    def __init__(self, parent_scope: SFNScope):
-        super(MapScope, self).__init__(parent_scope.fts)
-        self.variables = parent_scope.variables.copy()
-        self.scoped_variables = set()
-        self._updated_vars = set()
-        self.parent_scope = parent_scope
-
-    def _added_var(self, var: str):
-        self.scoped_variables.add(var)
-
-    def _updated_var(self, var: str):
-        self._updated_vars.add(var)
-
-    def build_entry_step(self, entry_var: str):
-        return sfn.Pass(
-            self.cdk_stack,
-            self.state_name("Register loop value"),
-            result_path="$.register",
-            parameters=self.build_register_assignment(
-                {entry_var: JsonPath.string_at(f"$.{entry_var}")}, "register."
-            ),
-        )
-
-    @property
-    def updated_vars(self):
-        return [v for v in self._updated_vars if v not in self.scoped_variables]
-
-
-class ChildScope(SFNScope):
-    def __init__(self, parent_scope: SFNScope):
-        super(ChildScope, self).__init__(parent_scope.fts)
-        self.variables = parent_scope.variables.copy()
-        self.scoped_variables = []
-        self.parent_scope = parent_scope
-
-    def _added_var(self, var: str):
-        self.scoped_variables.append(var)
-        if self.parent_scope:
-            self.parent_scope._added_var(var)
-
-
-def advance(
-    next_: Union[Callable, List[Callable]],
-    chain: Union[List[sfn.IChainable], sfn.IChainable, None],
-    new_next: Union[Callable, List[Callable], None],
-):
-    if chain:
-        if isinstance(chain, list):
-            chain = chain[0]
-        if isinstance(next_, list):
-            for i in flatten(next_):
-                i(chain)
-        else:
-            next_(chain)
-        return new_next
-    else:
-        return next_
-
-
-def _get_parameters(func) -> (List[str], Mapping[str, Any]):
-    # TODO: Should I use the AST instead of this to get the original parameters?
-    sig = inspect.signature(func)
-    req_params = [
-        p.name for p in sig.parameters.values() if p.default == inspect._empty
-    ]
-    opt_params = {
-        p.name: p.default
-        for p in sig.parameters.values()
-        if p.default != inspect._empty
-    }
-    return req_params, opt_params
-
-
-def flatten(items):
-    for x in items:
-        if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
-            for sub_x in flatten(x):
-                yield sub_x
-        else:
-            yield x
-
-
-def write_definition_json(name, start):
-    with open(pathlib.Path("build", f"{name}.json"), "w") as fp:
-        states = sfn.State.find_reachable_states(start, include_error_handlers=True)
-        states.sort(
-            key=lambda state: int(state.id.split("[")[1].split("]")[0].split(":")[1])
-        )
-        json.dump(
-            {"StartAt": start.id, "States": {s.id: s.to_state_json() for s in states},},
-            fp,
-            indent=4,
-        )
-
-
-def update_param_name(key, value):
-    if isinstance(value, str) and value.startswith("States"):
-        return f"{key}.$"
-    else:
-        return key
-
-
-def get_call_args(call: ast.Call) -> (List, Mapping):
-    args = []
-    kwargs = {}
-    for arg in call.args:
-        args.append(arg)
-    for kw in call.keywords:
-        kwargs[kw.arg] = kw.value
-    return args, kwargs
+import inspect
+import pathlib
+import ast
+import json
+import typing
+from .function import gather_function_attributes, FunctionAttributes
+from dataclasses import dataclass
+from types import BuiltinFunctionType
+from typing import Dict, List, Callable, Mapping, Any, Union, Iterable, Optional, Type
+
+from aws_cdk import (
+    aws_stepfunctions as sfn,
+    aws_stepfunctions_tasks as tasks,
+    Duration,
+    Stack,
+)
+from aws_cdk.aws_stepfunctions import JsonPath
+
+from .condition import build_condition
+from .s3 import write_json, read_json, build_s3_write_json_step, build_s3_read_json_step
+
+SFN_INDEX = 0
+
+
+@dataclass
+class Retry:
+    errors: List[str]
+    interval_seconds: int
+    max_attempts: int
+    backoff_rate: float = None
+
+
+@dataclass
+class CatchHandler:
+    errors: List[str]
+    body: List[sfn.IChainable]
+    result_path: str = "$.error-info"
+
+
+def concurrent(iterable, max_concurrency: Optional[int] = None):
+    pass
+
+
+def event(func: Callable):
+    pass
+
+
+def execution_start_time() -> str:
+    pass
+
+
+def state_entered_time() -> str:
+    pass
+
+
+def await_token(
+    func: Callable,
+    return_args: Union[List[str], Mapping[str, Type]],
+    duration: Duration = None,
+):
+    pass
+
+
+def state_machine(
+    cdk_stack: Stack,
+    sfn_name: str,
+    local_values,
+    express=False,
+    skip_pass=True,
+    return_vars: Optional[Union[List[str], Mapping[str, typing.Type]]] = None,
+):
+    """
+    Function decorator to trigger creation of an AWS Step Functions state machine construct
+    from the instructions in the function.
+    """
+
+    def decorator(func):
+        func_attrs = gather_function_attributes(func, None, return_vars)
+        fts = FunctionToSteps(cdk_stack, func_attrs, local_values, skip_pass=skip_pass)
+        func.state_machine = sfn.StateMachine(
+            cdk_stack,
+            sfn_name,
+            state_machine_name=sfn_name,
+            state_machine_type=sfn.StateMachineType.EXPRESS
+            if express
+            else sfn.StateMachineType.STANDARD,
+            definition=fts.build_sfn_definition(),
+        )
+        func.output = func_attrs.output
+        return func
+
+    return decorator
+
+
+class FunctionToSteps:
+    def __init__(
+        self,
+        cdk_stack: Stack,
+        func_attrs: FunctionAttributes,
+        local_values,
+        skip_pass=True,
+    ):
+        global SFN_INDEX
+        self.cdk_stack = cdk_stack
+        self.func = func_attrs.func
+        self.output = func_attrs.output
+        self.local_values = local_values
+        self.state_number = 0
+        self.sfn_number = SFN_INDEX
+        self.skip_pass = skip_pass
+        SFN_INDEX += 1
+
+        self.ast = func_attrs.tree
+        with open(pathlib.Path("build", f"{func_attrs.name}_ast.txt"), "w") as fp:
+            fp.write(ast.dump(self.ast, indent=2))
+
+        # Get the function root
+        if (
+            isinstance(self.ast, ast.Module)
+            and len(self.ast.body) == 1
+            and isinstance(self.ast.body[0], ast.FunctionDef)
+        ):
+            self.function_def: ast.FunctionDef
+            self.function_def = self.ast.body[0]
+        else:
+            raise Exception("Unexpected function definition")
+
+    def state_name(self, name):
+        self.state_number += 1
+        return f"{name} [{self.sfn_number}:{self.state_number}]"
+
+    def build_sfn_definition(self):
+
+        # TODO: Capture the parameter types to use elsewhere
+        req_params, opt_params = _get_parameters(self.func)
+
+        # Get the root of the function body
+        scope = SFNScope(self)
+        start, next_ = scope.generate_entry_steps(req_params, opt_params)
+        c, n = scope.handle_body(self.function_def.body)
+        advance(next_, c, n)
+
+        write_definition_json(self.func.__name__, start)
+        return start
+
+
+class SFNScope:
+    def __init__(self, fts: FunctionToSteps):
+        self.fts = fts
+        self.cdk_stack = fts.cdk_stack
+        self.state_name = fts.state_name
+        self.variables: Dict[str, typing.Type] = {}
+        self.output = fts.output
+        self.parent_scope = None
+
+    def generate_entry_steps(
+        self, required_parameters, optional_parameters: Mapping[str, Any] = None
+    ):
+        self.variables.update({param: typing.Any for param in required_parameters})
+
+        # The first step will always be to put the inputs on the register
+        start = sfn.Pass(
+            self.cdk_stack, self.state_name("Register Input"), result_path="$.register",
+        )
+        # For optional parameters we'll check if they are present and default them if they aren't
+        c, n = self.build_optional_parameter_steps(optional_parameters)
+        next_ = advance(start.next, c, n)
+        return start, next_
+
+    def build_register_assignment(self, values: Dict, register_path: str = ""):
+        params = values.copy()
+        for k, v in params.items():
+            self._updated_var(k)
+            # CDK is dropping None from parameters for some reason, using this to hack around it
+            if v is None:
+                params[k] = ""
+        # Copy over any variables that aren't in the params
+        for v in self.variables.keys():
+            if v not in params:
+                params[v] = JsonPath.string_at(f"$.{register_path}{v}")
+        for key in values.keys():
+            if key not in self.variables:
+                # TODO: Assign the type of the value
+                self.add_var(key)
+
+        params = {update_param_name(k, v): v for k, v in params.items()}
+        return params
+
+    def add_var(self, key: str, var_type: Type = Any):
+        self.variables[key] = var_type
+        self._added_var(key)
+
+    def _added_var(self, var: str):
+        pass
+
+    def _updated_var(self, var: str):
+        if self.parent_scope:
+            self.parent_scope._updated_var(var)
+
+    def handle_body(self, body: List[ast.stmt]) -> (List[sfn.IChainable], Callable):
+        chain = []
+        next_ = None
+        for stmt in body:
+            c, n = self.handle_op(stmt)
+            chain.extend(c)
+            if next_:
+                next_ = advance(next_, c, n)
+            else:
+                next_ = n
+        return chain, next_
+
+    def handle_op(self, stmt: ast.stmt) -> (List[sfn.IChainable], Callable):
+        if isinstance(stmt, ast.AnnAssign) or isinstance(stmt, ast.Assign):
+            # if isinstance(stmt.value, ast.Constant):
+            #    return self.handle_assign_value(stmt)
+            if isinstance(stmt.value, ast.Call) and isinstance(
+                stmt.value.func, ast.Name
+            ):
+                return self.handle_call_function(stmt.value, stmt)
+            if isinstance(stmt.value, ast.ListComp):
+                return self.handle_list_comp(stmt)
+            else:
+                return self.handle_assign_value(stmt)
+        elif isinstance(stmt, ast.If):
+            return self.handle_if(stmt)
+        elif isinstance(stmt, ast.Return):
+            return self.handle_return(stmt)
+        elif isinstance(stmt, ast.Expr) and isinstance(stmt.value, ast.Call):
+            if isinstance(stmt.value.func, ast.Name):
+                return self.handle_call_function(stmt.value)
+            elif isinstance(stmt.value.func, ast.Attribute):
+                if stmt.value.func.attr == "append":
+                    return self.handle_array_append(stmt.value)
+                elif stmt.value.func.attr == "extend":
+                    # TODO
+                    pass
+        elif isinstance(stmt, ast.With):
+            return self.handle_with(stmt)
+        elif isinstance(stmt, ast.Try):
+            return self.handle_try(stmt)
+        elif isinstance(stmt, ast.For):
+            return self.handle_for(stmt)
+        elif isinstance(stmt, ast.AugAssign) and (
+            isinstance(stmt.op, ast.Add) or isinstance(stmt.op, ast.Sub)
+        ):
+            return self.handle_math_add(stmt)
+        elif isinstance(stmt, ast.Pass):
+            if self.fts.skip_pass:
+                return [], None
+            else:
+                pass_step = sfn.Pass(self.cdk_stack, self.state_name("Pass"))
+                return [pass_step], pass_step.next
+
+        # Treat unhandled statements as a no-op
+        print(f"Unhandled {repr(stmt)}")
+        print(ast.dump(stmt, indent=2))
+        return [], None
+
+    def handle_with(self, stmt: ast.With):
+        w_val = self.build_with(stmt)
+        chain, n = self.handle_body(stmt.body)
+        for s in chain:
+            if hasattr(s, "add_retry"):
+                s.add_retry(
+                    errors=w_val.errors,
+                    max_attempts=w_val.max_attempts,
+                    interval=Duration.seconds(w_val.interval_seconds),
+                    backoff_rate=w_val.backoff_rate,
+                )
+        return chain, n
+
+    def handle_try(self, stmt: ast.Try):
+        chain, n = ChildScope(self).handle_body(stmt.body)
+        nexts = [n]
+        handlers = []
+        for handler in stmt.handlers:
+            child_scope = ChildScope(self)
+            result_path = None
+            h_chain, h_n = child_scope.handle_body(handler.body)
+            if handler.name:
+                result_path = f"$.register.{handler.name}"
+                child_scope.add_var(handler.name)
+                if h_chain:
+                    process_exception = sfn.Pass(
+                        self.cdk_stack,
+                        self.state_name(f"Interpret {handler.name}"),
+                        input_path="$.register",
+                        parameters=child_scope.build_register_assignment(
+                            {
+                                handler.name: JsonPath.string_at(
+                                    f"States.StringToJson($.{handler.name}.Cause)"
+                                )
+                            }
+                        ),
+                        result_path="$.register",
+                    )
+                    process_exception_choice = sfn.Choice(
+                        self.cdk_stack,
+                        self.state_name(f"Interpret Choice {handler.name}"),
+                    )
+                    process_exception_cause = sfn.Pass(
+                        self.cdk_stack,
+                        self.state_name(f"Interpret {handler.name}"),
+                        input_path="$.register",
+                        parameters=child_scope.build_register_assignment(
+                            {
+                                handler.name: {
+                                    "Cause": JsonPath.string_at(
+                                        f"States.StringToJson($.{handler.name}.Cause)"
+                                    ),
+                                    "Error": JsonPath.string_at(
+                                        f"$.{handler.name}.Error"
+                                    ),
+                                    "ExecutionArn": JsonPath.string_at(
+                                        f"$.{handler.name}.ExecutionArn"
+                                    ),
+                                    "Name": JsonPath.string_at(
+                                        f"$.{handler.name}.Name"
+                                    ),
+                                    "Status": JsonPath.string_at(
+                                        f"$.{handler.name}.Status"
+                                    ),
+                                }
+                            }
+                        ),
+                        result_path="$.register",
+                    )
+                    format_string = "{}{}"
+                    split = "{"
+                    process_exception_malformed_cause = sfn.Pass(
+                        self.cdk_stack,
+                        self.state_name(f"Interpret {handler.name}"),
+                        input_path="$.register",
+                        parameters=child_scope.build_register_assignment(
+                            {
+                                handler.name: {
+                                    "Cause": JsonPath.string_at(
+                                        f"States.StringToJson(States.Format('{format_string}', '{split}', States.ArrayGetItem(States.StringSplit($.{handler.name}.Cause, '{split}'), 1)))"
+                                    ),
+                                    "Error": JsonPath.string_at(
+                                        f"$.{handler.name}.Error"
+                                    ),
+                                    "ExecutionArn": JsonPath.string_at(
+                                        f"$.{handler.name}.ExecutionArn"
+                                    ),
+                                    "Name": JsonPath.string_at(
+                                        f"$.{handler.name}.Name"
+                                    ),
+                                    "Status": JsonPath.string_at(
+                                        f"$.{handler.name}.Status"
+                                    ),
+                                }
+                            }
+                        ),
+                        result_path="$.register",
+                    )
+                    process_exception_default = sfn.Pass(
+                        self.cdk_stack,
+                        self.state_name(f"Interpret {handler.name}"),
+                        input_path="$.register",
+                        parameters=child_scope.build_register_assignment(
+                            {
+                                handler.name: {
+                                    "ExecutionArn": JsonPath.string_at(
+                                        f"$.{handler.name}.ExecutionArn"
+                                    ),
+                                    "Name": JsonPath.string_at(
+                                        f"$.{handler.name}.Name"
+                                    ),
+                                    "Status": JsonPath.string_at(
+                                        f"$.{handler.name}.Status"
+                                    ),
+                                }
+                            }
+                        ),
+                        result_path="$.register",
+                    )
+                    process_exception.next(process_exception_choice)
+                    process_exception_choice.when(
+                        sfn.Condition.and_(
+                            sfn.Condition.is_present(
+                                f"$.register.{handler.name}.Cause"
+                            ),
+                            sfn.Condition.string_matches(
+                                f"$.register.{handler.name}.Cause",
+                                "The cause could not be determined*",
+                            ),
+                        ),
+                        process_exception_malformed_cause,
+                    )
+                    process_exception_choice.when(
+                        sfn.Condition.is_present(f"$.register.{handler.name}.Cause"),
+                        process_exception_cause,
+                    )
+                    process_exception_choice.otherwise(process_exception_default)
+                    process_exception_cause.next(h_chain[0])
+                    process_exception_malformed_cause.next(h_chain[0])
+                    process_exception_default.next(h_chain[0])
+                    h_chain = [
+                        process_exception,
+                        process_exception_choice,
+                        process_exception_cause,
+                        process_exception_malformed_cause,
+                        process_exception_default,
+                    ] + h_chain
+
+            # If the handler body isn't empty, add it in
+            if h_chain:
+                chain.extend(h_chain)
+                nexts.append(h_n)
+            handlers.append(self.build_exception_handler(handler, h_chain, result_path))
+
+        for s in chain:
+            if hasattr(s, "add_catch"):
+                for handler in handlers:
+                    nn = self.attach_catch(s, handler)
+                    if nn:
+                        nexts.append(nn)
+
+        return chain, nexts
+
+    def build_exception_handler(
+        self,
+        handler: ast.ExceptHandler,
+        chain: List[sfn.IChainable],
+        result_path: str = None,
+    ):
+        if isinstance(handler.type, ast.Name) and handler.type.id == "Exception":
+            return CatchHandler(["States.ALL"], chain, result_path=result_path)
+        raise Exception(f"Unhandled exception of type {handler.type}")
+
+    @staticmethod
+    def attach_catch(step, handler):
+        def inner_next(n):
+            step.add_catch(
+                n, errors=handler.errors, result_path=handler.result_path,
+            )
+
+        if handler.body:
+            advance(inner_next, handler.body, None)
+            return None
+        else:
+            return inner_next
+
+    def build_with(self, stmt: ast.With):
+        if len(stmt.items) != 1:
+            raise Exception(f"With statements can only support a single item")
+        call = stmt.items[0].context_expr
+        if isinstance(call, ast.Call):
+            if call.func.id == "Retry":
+                params = self.build_parameters(call, Retry, False)
+                return Retry(**params)
+        raise Exception(f"Unhandled with operation: {call}")
+
+    @staticmethod
+    def map_arg(arg: ast.expr, var_path: str = ""):
+        if isinstance(arg, ast.Name):
+            return f"$.{var_path}{arg.id}"
+        elif isinstance(arg, ast.Constant):
+            return arg.value
+        elif (
+            isinstance(arg, ast.Subscript)
+            and isinstance(arg.value, ast.Name)
+            and isinstance(arg.slice, ast.Constant)
+        ):
+            return f"$.{var_path}{arg.value.id}[{arg.slice.value}]"
+        else:
+            raise Exception("Args must be Name or Constant")
+
+    def _get_iterator(self, iterator: ast.expr) -> (str, str, sfn.State, int):
+        # TODO: Support enumerate
+        # TODO: Support callable iterator
+        max_concurrency = 1
+        iterator_step = None
+
+        # if the iterator is wrapped in a 'concurrent' function, capture the parameter as the concurrency for the map
+        if (
+            isinstance(iterator, ast.Call)
+            and isinstance(iterator.func, ast.Name)
+            and iterator.func.id == "concurrent"
+        ):
+            if len(iterator.args) > 1:
+                max_concurrency = iterator.args[1].value
+            else:
+                max_concurrency = 0
+            iterator = iterator.args[0]
+
+        if isinstance(iterator, ast.Call) and self._is_intrinsic_function(iterator):
+            items_path, iter_var = self._intrinsic_function(iterator)
+            iterator_step = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Build {iter_var}"),
+                input_path="$.register",
+                result_path="$.iter",
+                parameters={iter_var: items_path},
+            )
+            iter_var = iterator.func.id
+            items_path = f"$.iter.{iter_var}"
+        elif isinstance(iterator, ast.Call) and isinstance(iterator.func, ast.Name):
+            (
+                iterator_step,
+                return_vars,
+                func_name,
+                result_prefix,
+            ) = self._build_func_call(iterator, "$.iter")
+            iter_var = iterator.func.id
+            items_path = f"$.iter{result_prefix}.{return_vars[0]}"
+
+        # If the iterator is a name, use that value
+        elif isinstance(iterator, ast.Name):
+            iter_var = iterator.id
+            items_path = f"$.register.{iter_var}"
+        else:
+            raise Exception("Unsupported for-loop iterator, variables only")
+        return iter_var, items_path, iterator_step, max_concurrency
+
+    def handle_for(self, stmt: ast.For):
+        iter_var, items_path, iterator_step, max_concurrency = self._get_iterator(
+            stmt.iter
+        )
+        if not isinstance(stmt.target, ast.Name):
+            raise Exception("Unsupported for-loop target, variables only")
+
+        map_state = sfn.Map(
+            self.cdk_stack,
+            self.state_name(f"For {iter_var}"),
+            max_concurrency=max_concurrency,
+            items_path=items_path,
+            parameters={
+                "register.$": f"$.register",
+                f"{stmt.target.id}.$": "$$.Map.Item.Value",
+            },
+            result_path="$.register.loopResult",
+        )
+
+        # Create a scope for the for loop contents and build the contained steps
+        # Also build an entry step to capture the iterator target
+        map_scope = MapScope(self)
+        entry_step = map_scope.build_entry_step(stmt.target.id)
+        chain, map_next_ = map_scope.handle_body(stmt.body)
+        entry_step.next(chain[0])
+        map_state.iterator(entry_step)
+        next_ = map_state.next
+
+        # if any vars from the outer scope were updated, add a 'return' step to the map operations and
+        # logic to pull those results into the register after the map completes
+        map_return_step_name = self.state_name("Map return")
+        if map_scope.updated_vars:
+            return_params = {
+                v: JsonPath.string_at(f"$.register.{v}") for v in map_scope.updated_vars
+            }
+            map_return_step = sfn.Pass(
+                self.cdk_stack, map_return_step_name, parameters=return_params
+            )
+            consolidate_params = {
+                v: JsonPath.string_at(f"$.register.loopResult[*].{v}[*]")
+                for v in map_scope.updated_vars
+            }
+            consolidate_step = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Consolidate map results"),
+                result_path="$.register",
+                parameters=self.build_register_assignment(
+                    consolidate_params, "register."
+                ),
+            )
+            map_state.next(consolidate_step)
+            next_ = consolidate_step.next
+        else:
+            map_return_step = sfn.Pass(
+                self.cdk_stack, map_return_step_name, parameters={}
+            )
+        advance(map_next_, [map_return_step], map_return_step.next)
+
+        # finalize the steps
+        if iterator_step:
+            iterator_step.next(map_state)
+            return [iterator_step, map_state], next_
+        else:
+            return [map_state], next_
+
+    def handle_list_comp(self, stmt: Union[ast.Assign, ast.AnnAssign]):
+        target = stmt.targets[0] if isinstance(stmt, ast.Assign) else stmt.target
+        if isinstance(target, ast.Name):
+            target = target.id
+        else:
+            raise Exception("Unsupported list comp target, variables only")
+
+        list_comp = stmt.value
+        if not isinstance(list_comp, ast.ListComp):
+            raise Exception("Unhandled list comp value")
+        if len(list_comp.generators) != 1:
+            raise Exception("List comp can only support a single generator")
+        comp = list_comp.generators[0]
+        if not isinstance(comp, ast.comprehension):
+            raise Exception(f"Unhandled generator {type(comp)}")
+
+        # TODO: Support enumerate...
+        if (
+            isinstance(comp.iter, ast.Call)
+            and isinstance(comp.iter.func, ast.Name)
+            and comp.iter.func.id == "concurrent"
+        ):
+            max_concurrency = comp.iter.args[1].value
+            iter_var = comp.iter.args[0].id
+        elif isinstance(comp.iter, ast.Name):
+            max_concurrency = 0
+            iter_var = comp.iter.id
+        else:
+            raise Exception("Unsupported list comp iterator, variables only")
+        if not isinstance(comp.target, ast.Name):
+            raise Exception("Unsupported list comp target, variables only")
+
+        choice_name = self.state_name(f"Has {iter_var} to map")
+        map_state = sfn.Map(
+            self.cdk_stack,
+            self.state_name(f"For {iter_var}"),
+            max_concurrency=max_concurrency,
+            items_path=f"$.register.{iter_var}",
+            parameters={
+                "register.$": f"$.register",
+                f"{comp.target.id}.$": "$$.Map.Item.Value",
+            },
+            result_path="$.loopResult",
+        )
+        choice = sfn.Choice(self.cdk_stack, choice_name)
+        choice.when(
+            sfn.Condition.and_(
+                sfn.Condition.is_present(f"$.register.{iter_var}"),
+                sfn.Condition.is_present(f"$.register.{iter_var}[0]"),
+            ),
+            map_state,
+        )
+
+        call_func = sfn.Pass(
+            self.cdk_stack,
+            self.state_name(f"Call function..."),
+            parameters={"loopResult": JsonPath.string_at(f"$.{comp.target.id}")},
+        )
+
+        map_state.iterator(call_func)
+        consolidate_step = sfn.Pass(
+            self.cdk_stack,
+            self.state_name(f"Consolidate map results"),
+            result_path="$.register",
+            parameters=self.build_register_assignment(
+                {target: JsonPath.string_at(f"$.loopResult[*][*]")},
+                "loopResult[0].register.",
+            ),
+        )
+        map_state.next(consolidate_step)
+
+        return [choice, map_state], [choice.otherwise, consolidate_step.next]
+
+    def handle_math_add(self, stmt: ast.AugAssign):
+        if isinstance(stmt.target, ast.Name):
+            target = stmt.target.id
+        else:
+            raise Exception(f"Unexpected MathAdd target {type(stmt.target)}")
+        if isinstance(stmt.value, ast.Constant):
+            if isinstance(stmt.op, ast.Add):
+                value = stmt.value.value
+            elif isinstance(stmt.op, ast.Sub):
+                value = -stmt.value.value
+            else:
+                raise Exception(f"Unsupported MathAdd op {type(stmt.op)}")
+        else:
+            raise Exception(f"Unsupported MathAdd target {type(stmt.value)}")
+        add_step = sfn.Pass(
+            self.cdk_stack,
+            self.state_name(f"Add {value} to {target}"),
+            input_path="$.register",
+            result_path="$.register",
+            parameters=self.build_register_assignment(
+                {target: JsonPath.string_at(f"States.MathAdd($.{target}, {value})")}
+            ),
+        )
+        return [add_step], add_step.next
+
+    def handle_array_append(self, stmt: ast.Call):
+        array_name = stmt.func.value.id
+        array_path = f"$.register.{array_name}"
+        arg = stmt.args[0]
+        if isinstance(arg, ast.Name):
+            value = arg.id
+            path_to_add = f"$.register.{arg.id}"
+        elif isinstance(arg, ast.Constant):
+            value = arg.value
+            path_to_add = arg.value
+        else:
+            raise Exception(f"Unexpected type {type(arg)} for list append")
+        list_step = sfn.Pass(
+            self.cdk_stack,
+            self.state_name(f"Append {value} to {array_name}"),
+            result_path="$.meta",
+            parameters={
+                "arrayConcat": JsonPath.string_at(
+                    f"States.Array({array_path}, States.Array({path_to_add}))"
+                )
+            },
+        )
+        flatten_step = sfn.Pass(
+            self.cdk_stack,
+            self.state_name(f"Flatten {array_name}"),
+            result_path="$.register",
+            parameters=self.build_register_assignment(
+                {array_name: JsonPath.string_at("$.meta.arrayConcat[*][*]")},
+                "register.",
+            ),
+        )
+        list_step.next(flatten_step)
+        return [list_step, flatten_step], flatten_step.next
+
+    def handle_assign_value(
+        self, stmt: Union[ast.AnnAssign, ast.Assign]
+    ) -> (List[sfn.IChainable], Callable):
+        sub_target = None
+        if isinstance(stmt, ast.AnnAssign):
+            if isinstance(stmt.target, ast.Name):
+                var_name = stmt.target.id
+            elif (
+                isinstance(stmt.target, ast.Subscript)
+                and isinstance(stmt.target.value, ast.Name)
+                and isinstance(stmt.target.slice, ast.Constant)
+            ):
+                var_name = stmt.target.value.id
+                sub_target = stmt.target.slice.value
+            else:
+                raise Exception(
+                    f"Unexpected assignment target of type {type(stmt.target)}"
+                )
+        else:
+            if len(stmt.targets) == 1 and isinstance(stmt.targets[0], ast.Name):
+                var_name = stmt.targets[0].id
+            elif (
+                isinstance(stmt.targets[0], ast.Subscript)
+                and isinstance(stmt.targets[0].value, ast.Name)
+                and isinstance(stmt.targets[0].slice, ast.Constant)
+            ):
+                var_name = stmt.targets[0].value.id
+                sub_target = stmt.targets[0].slice.value
+            else:
+                raise Exception("Unexpected assignment")
+        if sub_target:
+            prep = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Prep assign {var_name}.{sub_target}"),
+                input_path="$.register",
+                result_path="$.register.itm",
+                parameters={sub_target: self.generate_value_repr(stmt.value)},
+            )
+            assign = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Assign {var_name}.{sub_target}"),
+                input_path="$.register",
+                result_path="$.register",
+                parameters=self.build_register_assignment(
+                    # {f"{var_name}": JsonPath.json_merge(f"$.{var_name}", "$.itm")}
+                    {f"{var_name}": f"States.JsonMerge($.{var_name}, $.itm, false)"}
+                ),
+            )
+            prep.next(assign)
+            return [prep, assign], assign.next
+        else:
+            value = self.generate_value_repr(stmt.value)
+            assign = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Assign {var_name}"),
+                input_path="$.register",
+                result_path="$.register",
+                parameters=self.build_register_assignment({var_name: value}),
+            )
+            return [assign], assign.next
+
+    def handle_if(self, stmt: ast.If) -> (List[sfn.IChainable], Callable):
+        condition, name = build_condition(stmt.test)
+        choice = sfn.Choice(self.cdk_stack, self.state_name(name))
+
+        def if_next(step):
+            choice.when(condition, step)
+
+        if_c, if_n = ChildScope(self).handle_body(stmt.body)
+        else_c, else_n = ChildScope(self).handle_body(stmt.orelse)
+        if_n = advance(if_next, if_c, if_n)
+        else_n = advance(choice.otherwise, else_c, else_n)
+        chain = [choice]
+        if if_c:
+            chain.extend(if_c)
+        if else_c:
+            chain.extend(else_c)
+        return chain, [if_n, else_n]
+
+    def _is_intrinsic_function(self, call: ast.Call):
+        return isinstance(call.func, ast.Name) and call.func.id in [
+            "range",
+            "len",
+            "execution_start_time",
+            "state_entered_time",
+        ]
+
+    def _intrinsic_function(self, call: ast.Call, var_path: str = ""):
+        if isinstance(call.func, ast.Name):
+            args = [self.map_arg(arg, var_path) for arg in call.args]
+            if call.func.id == "range":
+                start_val = 0
+                end_val = 0
+                step_val = 1
+                if len(args) == 1:
+                    end_val = args[0]
+                elif len(args) >= 2:
+                    start_val = args[0]
+                    end_val = args[1]
+                if len(args) == 3:
+                    step_val = args[2]
+                return (
+                    JsonPath.string_at(
+                        f"States.ArrayRange({start_val}, States.MathAdd({end_val}, -1), {step_val})"
+                    ),
+                    "range",
+                )
+            elif call.func.id == "len":
+                if len(args) == 1:
+                    return (
+                        JsonPath.string_at(f"States.ArrayLength({args[0]})"),
+                        "len",
+                    )
+            elif call.func.id == "execution_start_time":
+                return (
+                    JsonPath.string_at(f"$$.Execution.StartTime"),
+                    "time",
+                )
+            elif call.func.id == "state_entered_time":
+                return (
+                    JsonPath.string_at(f"$$.State.EnteredTime"),
+                    "time",
+                )
+        raise Exception("Cannot handle intrinsic function")
+
+    def _build_func_call(
+        self,
+        call: ast.Call,
+        result_path: str = "$.register.out",
+        invoke_event_: bool = False,
+        await_token_: bool = False,
+        await_duration_: Duration = None,
+    ) -> (sfn.State, List[str], str):
+        if isinstance(call.func, ast.Name):
+            # Get the function
+            func = self.fts.local_values.get(call.func.id)
+            result_prefix = ""
+
+            # Build the parameters
+            if func:
+                params = self.build_parameters(call, func)
+                if hasattr(func, "get_additional_params"):
+                    params.update(func.get_additional_params())
+            elif call.func.id == write_json.__name__:
+                params = self.build_parameters(call, write_json, False)
+            elif call.func.id == read_json.__name__:
+                params = self.build_parameters(call, read_json, False)
+            elif call.func.id in [
+                "time.sleep",
+                "sleep",
+                event.__name__,
+                await_token.__name__,
+            ]:
+                params = {}
+            else:
+                raise Exception(f"Unable to find function {call.func.id}")
+
+            if call.func.id in ["time.sleep", "sleep"]:
+                invoke = sfn.Wait(
+                    self.cdk_stack,
+                    self.state_name("Wait"),
+                    time=sfn.WaitTime.duration(Duration.seconds(call.args[0].value)),
+                )
+                return_vars = []
+            elif (
+                call.func.id == event.__name__
+                and len(call.args) > 0
+                and isinstance(call.args[0], ast.Call)
+            ):
+                return self._build_func_call(
+                    call.args[0], result_path=result_path, invoke_event_=True
+                )
+            elif (
+                call.func.id == await_token.__name__
+                and len(call.args) >= 2
+                and isinstance(call.args[0], ast.Call)
+            ):
+                duration = None
+                if len(call.args) == 3:
+                    duration_arg = call.args[2]
+                    if isinstance(duration_arg, ast.Call) and isinstance(
+                        duration_arg.func, ast.Attribute
+                    ):
+                        attr_name = duration_arg.func.attr
+                        if len(duration_arg.args) > 0:
+                            duration_arg_value = duration_arg.args[0]
+                            if isinstance(duration_arg_value, ast.Constant):
+                                duration = getattr(Duration, attr_name)(
+                                    duration_arg_value.value
+                                )
+                invoke, return_vars, name, result_prefix = self._build_func_call(
+                    call.args[0],
+                    result_path=result_path,
+                    invoke_event_=True,
+                    await_token_=True,
+                    await_duration_=duration,
+                )
+                return_arg = call.args[1]
+                if isinstance(return_arg, ast.List) and all(
+                    isinstance(a, ast.Constant) for a in return_arg.elts
+                ):
+                    return_vars = [a.value for a in return_arg.elts]
+                return invoke, return_vars, name, ""
+            elif hasattr(func, "definition"):
+                invocation_type = tasks.LambdaInvocationType.REQUEST_RESPONSE
+                integration_pattern = sfn.IntegrationPattern.REQUEST_RESPONSE
+                if invoke_event_:
+                    invocation_type = tasks.LambdaInvocationType.EVENT
+                if await_token_:
+                    integration_pattern = sfn.IntegrationPattern.WAIT_FOR_TASK_TOKEN
+                invoke = tasks.LambdaInvoke(
+                    self.cdk_stack,
+                    self.state_name(f"Call {call.func.id}"),
+                    lambda_function=func.get_lambda(),
+                    payload=sfn.TaskInput.from_object(params),
+                    input_path="$.register",
+                    result_path=result_path,
+                    invocation_type=invocation_type,
+                    integration_pattern=integration_pattern,
+                    heartbeat=await_duration_,
+                )
+                return_vars = list(func.definition.output.keys())
+                result_prefix = ".Payload"
+            elif hasattr(func, "state_machine"):
+                invoke = tasks.StepFunctionsStartExecution(
+                    self.cdk_stack,
+                    self.state_name(f"Call {func.state_machine.state_machine_name}"),
+                    state_machine=func.state_machine,
+                    input_path="$.register",
+                    result_path=result_path,
+                    integration_pattern=sfn.IntegrationPattern.RUN_JOB,
+                    input=sfn.TaskInput.from_object(params),
+                )
+                return_vars = list(func.output.keys())
+                result_prefix = ".Output"
+            elif call.func.id == write_json.__name__:
+                invoke = build_s3_write_json_step(
+                    self.cdk_stack, self.state_name("S3 Write JSON"), **params
+                )
+                return_vars = ["ETag"]
+                result_prefix = ""
+            elif call.func.id == read_json.__name__:
+                invoke = build_s3_read_json_step(
+                    self.cdk_stack, self.state_name("S3 Read JSON"), **params
+                )
+                return_vars = ["Body", "LastModified", "ETag"]
+                result_prefix = ""
+            else:
+                raise Exception(
+                    f"Function without an associated Lambda: {call.func.id}"
+                )
+            return invoke, return_vars, call.func.id, result_prefix
+        else:
+            raise Exception(
+                f"Function attribute is not of type name: {type(call.func)}"
+            )
+
+    def handle_call_function(
+        self, call: ast.Call, assign: Union[ast.Assign, ast.AnnAssign] = None,
+    ) -> (List[sfn.IChainable], Callable):
+        if self._is_intrinsic_function(call):
+            if not assign:
+                raise Exception(
+                    f"Call to intrinsic function {call.func.id} must be assigned to a value"
+                )
+            val, name = self._intrinsic_function(call)
+            target = (
+                assign.targets[0] if isinstance(assign, ast.Assign) else assign.target
+            )
+            if isinstance(target, ast.Name):
+                result_target = target.id
+            else:
+                raise Exception("Invalid intrinsic function target")
+
+            register = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Register {name}"),
+                input_path="$.register",
+                result_path="$.register",
+                parameters=self.build_register_assignment({result_target: val}),
+            )
+            return [register], register.next
+        else:
+            invoke, return_vars, name, result_prefix = self._build_func_call(
+                call, "$.register.out"
+            )
+            chain = [invoke]
+            next_ = invoke.next
+
+            if assign:
+                # Get the result variable names
+                target = (
+                    assign.targets[0]
+                    if isinstance(assign, ast.Assign)
+                    else assign.target
+                )
+                if isinstance(target, ast.Name):
+                    result_targets = [target.id]
+                elif isinstance(target, ast.Tuple) and all(
+                    isinstance(t, ast.Name) for t in target.elts
+                ):
+                    result_targets = [n.id for n in target.elts]
+                else:
+                    raise Exception(
+                        f"Unexpected result target of type {type(assign.target)}"
+                    )
+                result_params = {
+                    v: JsonPath.string_at(f"$.out{result_prefix}.{r}")
+                    for v, r in zip(result_targets, return_vars)
+                }
+                if len(result_params) < len(result_targets):
+                    raise Exception(
+                        f"Unable to map all response targets to return values for {name}"
+                    )
+                register = sfn.Pass(
+                    self.cdk_stack,
+                    self.state_name(f"Register {call.func.id}"),
+                    input_path="$.register",
+                    result_path="$.register",
+                    parameters=self.build_register_assignment(result_params),
+                )
+                invoke.next(register)
+                chain.append(register)
+                next_ = register.next
+
+            return chain, next_
+
+    def _return_value(self, value: Union[ast.expr, ast.stmt]):
+        if isinstance(value, ast.Name):
+            return JsonPath.string_at(f"$.register.{value.id}")
+        elif isinstance(value, ast.Constant):
+            return value.value
+        elif isinstance(value, ast.Call) and self._is_intrinsic_function(value):
+            val, name = self._intrinsic_function(value)
+            return val
+        else:
+            raise Exception(f"Unanticipated return type: {value}")
+
+    def handle_return(self, stmt: ast.Return):
+        if isinstance(stmt.value, ast.Tuple):
+            if len(self.output) != len(stmt.value.elts):
+                raise Exception("Mismatched return value counts")
+            return_step = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Return"),
+                parameters={
+                    k: self._return_value(v)
+                    for k, v in zip(self.output.keys(), stmt.value.elts)
+                },
+            )
+        elif isinstance(stmt.value, ast.Name) or isinstance(stmt.value, ast.Constant):
+            if len(self.output) != 1:
+                raise Exception("Mismatched return value counts")
+            return_step = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Return"),
+                parameters={
+                    list(self.output.keys())[0]: self._return_value(stmt.value)
+                },
+            )
+        elif stmt.value is None:
+            return_step = sfn.Pass(self.cdk_stack, self.state_name(f"Return"))
+        else:
+            raise Exception(f"Unhandled return value type {stmt.value}")
+        return [return_step], return_step.next
+
+    def build_parameters(self, call: ast.Call, func: Callable, gen_jsonpath=True):
+        params = {}
+
+        # TODO: Handle kwonly args
+        if hasattr(func, "definition"):
+            args = func.definition.input.keys()
+        elif isinstance(func, BuiltinFunctionType):
+            return None
+        else:
+            args = inspect.getfullargspec(func).args
+            if len(args) > 0 and args[0] == "self":
+                args = args[1:]
+
+        # Add the positional parameters
+        for arg_value, arg_name in zip(call.args, args):
+            params[arg_name] = self.generate_value_repr(arg_value, gen_jsonpath)
+
+        # Add the keyword parameters
+        for kw in call.keywords:
+            params[kw.arg] = self.generate_value_repr(kw.value, gen_jsonpath)
+        return params
+
+    def build_optional_parameter_steps(self, optional_parameters: Mapping[str, Any]):
+        chain = []
+        next_ = None
+        for name, value in optional_parameters.items():
+            choice_name = self.state_name(f"Has {name}")
+            assign = sfn.Pass(
+                self.cdk_stack,
+                self.state_name(f"Assign {name} default"),
+                input_path="$.register",
+                result_path="$.register",
+                parameters=self.build_register_assignment({name: value}),
+            )
+            choice = sfn.Choice(self.cdk_stack, choice_name)
+            choice.when(sfn.Condition.is_not_present(f"$.register.{name}"), assign)
+            chain.extend([choice, assign])
+            if next_:
+                next_ = advance(next_, choice, [choice.otherwise, assign.next])
+            else:
+                next_ = [choice.otherwise, assign.next]
+        return chain, next_
+
+    def evaluate_path(self, stmt: ast.Subscript) -> str:
+        if isinstance(stmt.slice, ast.Constant):
+            if isinstance(stmt.slice.value, int):
+                slce = f"[{stmt.slice.value}]"
+            else:
+                slce = f".{stmt.slice.value}"
+        else:
+            raise Exception("Subscript slice that's not a Constant")
+        if isinstance(stmt.value, ast.Name):
+            return stmt.value.id + slce
+        elif isinstance(stmt.value, ast.Subscript):
+            return self.evaluate_path(stmt.value) + slce
+        else:
+            raise Exception("Unexpected Subscript value")
+
+    def generate_value_repr(self, arg_value, gen_jsonpath=True):
+        if isinstance(arg_value, ast.Name):
+            # if arg_value.id not in self.variables:
+            #    raise Exception(f"Undefined variable {arg_value.id}")
+            expr = f"$.{arg_value.id}"
+            return JsonPath.string_at(expr) if gen_jsonpath else expr
+        elif isinstance(arg_value, ast.Constant):
+            return arg_value.value
+        elif isinstance(arg_value, ast.List):
+            expr = [self.generate_value_repr(val, False) for val in arg_value.elts]
+            return JsonPath.array(*expr) if gen_jsonpath else expr
+        elif isinstance(arg_value, ast.Subscript):
+            expr = "$." + self.evaluate_path(arg_value)
+            return JsonPath.string_at(expr) if gen_jsonpath else expr
+        elif isinstance(arg_value, ast.Call) and self._is_intrinsic_function(arg_value):
+            path, name = self._intrinsic_function(arg_value)
+            return path
+        elif isinstance(arg_value, ast.Dict):
+            obj = {}
+            for k, v in zip(arg_value.keys, arg_value.values):
+                if not isinstance(k, ast.Constant):
+                    raise Exception("Dict keys must be a constant")
+                else:
+                    obj[k.value] = self.generate_value_repr(v, gen_jsonpath)
+            return obj
+        # TODO: evaluate if this hack for handling JsonPath values is the best approach
+        elif isinstance(arg_value, ast.Attribute) and (
+            (
+                isinstance(arg_value.value, ast.Attribute)
+                and arg_value.value.attr == "JsonPath"
+            )
+            or (
+                isinstance(arg_value.value, ast.Name)
+                and arg_value.value.id == "JsonPath"
+            )
+        ):
+            return getattr(JsonPath, arg_value.attr)
+        elif (
+            isinstance(arg_value, ast.Call)
+            and isinstance(arg_value.func, ast.Attribute)
+            and (
+                (
+                    isinstance(arg_value.func.value, ast.Name)
+                    and arg_value.func.value.id == "JsonPath"
+                )
+                or (
+                    isinstance(arg_value.func.value, ast.Attribute)
+                    and arg_value.func.value.attr == "JsonPath"
+                )
+            )
+        ):
+            return getattr(JsonPath, arg_value.func.attr)(
+                *[self.generate_value_repr(arg, gen_jsonpath) for arg in arg_value.args]
+            )
+        elif (
+            isinstance(arg_value, ast.Attribute)
+            and isinstance(arg_value.value, ast.Name)
+            and arg_value.value.id == "self"
+        ):
+            s = self.fts.local_values.get(arg_value.value.id)
+            var = s.__getattribute__(arg_value.attr)
+            return var
+        elif isinstance(arg_value, ast.Call) and (
+            (
+                isinstance(arg_value.func, ast.Attribute)
+                and isinstance(arg_value.func.value, ast.Name)
+                and arg_value.func.value.id == "JsonPath"
+            )
+        ):
+            # TODO: Handle multi arg inputs
+            arg = self.generate_value_repr(arg_value.args[0], gen_jsonpath=True)
+            return getattr(JsonPath, arg_value.func.attr)(arg)
+        else:
+            print(ast.dump(arg_value, indent=2))
+            raise Exception(f"Unexpected argument: {ast.dump(arg_value)}")
+
+
+class MapScope(SFNScope):
+    def __init__(self, parent_scope: SFNScope):
+        super(MapScope, self).__init__(parent_scope.fts)
+        self.variables = parent_scope.variables.copy()
+        self.scoped_variables = set()
+        self._updated_vars = set()
+        self.parent_scope = parent_scope
+
+    def _added_var(self, var: str):
+        self.scoped_variables.add(var)
+
+    def _updated_var(self, var: str):
+        self._updated_vars.add(var)
+
+    def build_entry_step(self, entry_var: str):
+        return sfn.Pass(
+            self.cdk_stack,
+            self.state_name("Register loop value"),
+            result_path="$.register",
+            parameters=self.build_register_assignment(
+                {entry_var: JsonPath.string_at(f"$.{entry_var}")}, "register."
+            ),
+        )
+
+    @property
+    def updated_vars(self):
+        return [v for v in self._updated_vars if v not in self.scoped_variables]
+
+
+class ChildScope(SFNScope):
+    def __init__(self, parent_scope: SFNScope):
+        super(ChildScope, self).__init__(parent_scope.fts)
+        self.variables = parent_scope.variables.copy()
+        self.scoped_variables = []
+        self.parent_scope = parent_scope
+
+    def _added_var(self, var: str):
+        self.scoped_variables.append(var)
+        if self.parent_scope:
+            self.parent_scope._added_var(var)
+
+
+def advance(
+    next_: Union[Callable, List[Callable]],
+    chain: Union[List[sfn.IChainable], sfn.IChainable, None],
+    new_next: Union[Callable, List[Callable], None],
+):
+    if chain:
+        if isinstance(chain, list):
+            chain = chain[0]
+        if isinstance(next_, list):
+            for i in flatten(next_):
+                i(chain)
+        else:
+            next_(chain)
+        return new_next
+    else:
+        return next_
+
+
+def _get_parameters(func) -> (List[str], Mapping[str, Any]):
+    # TODO: Should I use the AST instead of this to get the original parameters?
+    sig = inspect.signature(func)
+    req_params = [
+        p.name for p in sig.parameters.values() if p.default == inspect._empty
+    ]
+    opt_params = {
+        p.name: p.default
+        for p in sig.parameters.values()
+        if p.default != inspect._empty
+    }
+    return req_params, opt_params
+
+
+def flatten(items):
+    for x in items:
+        if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
+            for sub_x in flatten(x):
+                yield sub_x
+        else:
+            yield x
+
+
+def write_definition_json(name, start):
+    with open(pathlib.Path("build", f"{name}.json"), "w") as fp:
+        states = sfn.State.find_reachable_states(start, include_error_handlers=True)
+        states.sort(
+            key=lambda state: int(state.id.split("[")[1].split("]")[0].split(":")[1])
+        )
+        json.dump(
+            {"StartAt": start.id, "States": {s.id: s.to_state_json() for s in states},},
+            fp,
+            indent=4,
+        )
+
+
+def update_param_name(key, value):
+    if isinstance(value, str) and value.startswith("States"):
+        return f"{key}.$"
+    else:
+        return key
+
+
+def get_call_args(call: ast.Call) -> (List, Mapping):
+    args = []
+    kwargs = {}
+    for arg in call.args:
+        args.append(arg)
+    for kw in call.keywords:
+        kwargs[kw.arg] = kw.value
+    return args, kwargs
```

### Comparing `pysfn-0.1.8/README.md` & `pysfn-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pysfn-0.1.8/setup.py` & `pysfn-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['aws-cdk-lib>=2.55.1,<3.0.0',
  'constructs>=10.1.194,<11.0.0',
  'shortuuid>=1.0.11,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysfn',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Transpiler for AWS Step Functions',
     'long_description': '# PySFN\n*A Python to AWS Step Functions transpiler for the CDK*\n\nThis package is an initial experiment in exploring ways to make AWS Step Functions more useful by allowing\ndevelopers to build state machines in the same way they would write a Python function. Users can define\nstate machines in their CDK Stack as simple functions, then apply a `@state_machine` decorator to declare\na Construct in their stack.\n\nThis is very much an experiment, and I welcome feedback on the viability and utility of this approach. \n\nNote that because it\'s Python-based it will only work when used with Python CDK stacks, and not TypeScript or \nother languages. Of course, your Lambdas can be written in any language, but Python Lambdas can take advantage\nof some additional features.\n\n## Quick start\nThere is a lot of good information below, but if you want to get started quickly and experiment with the\nprototype app, clone the repo give it a shot. Assuming you have the AWS CDK installed, you should be able to\ndeploy the app by doing the following:\n\n```shell\npip install pysfn\ncd proto_app\ncdk deploy\n```\n\nOnce you\'ve deployed it, you can submit the *basic*, *simple*, and *larger* step functions that have been \ncreated with the following input.\n\n```json\n{\n  "str_value": "html",\n  "list_value": [100, 100],\n  "option": false\n}\n```\n\nReplacing `html` with `image`, `pdf`, or some other value will trigger the different paths in the function, \nand you can also test how default values are used by leaving off the `list_value` and `option` values.\n\n## Why Step Functions?\nAWS Step Functions (SFN) is a useful tool for orchestrating processing steps in a serverless fashion. By providing \nthe ability to invoke a range of AWS services such as Lambdas, DynamoDB, SNS, and many others, it\'s significantly\neasier to componentize an application into reusable pieces that can leverage a range of programming languages,\nlibraries, and utilities, while keeping compute requirements and complexity low.\n\nFor example, I\'ve built SFN applications that combine NodeJS lambdas, Python Lambdas using a range of \ndifferent libraries, the AWS Textract service and DynamoDB into a single app that can be used in multiple\ncontexts for data processing. Building this in SFN avoids the need to launch a hosted service to manage\nthe processing flow, and keeps each resource focused on the processing needs of that particular function.\n\n## States Language Hell\nThe biggest downside of SFN is the language that AWS developed to power it.  The\n[Amazon States Language](https://states-language.net/) makes it possible to develop processing flows in\na technology-agnostic way, but it can be clumsy to pick up and use efficiently. Data moves through a state\nmachine definition as a JSON object, and each processing step must manipulate it using jsonpath.\nTo do this well, a developer needs to be aware of the inputs and outputs of each stage and handle them appropriately.\nIn addition, the use of jsonpath operations limits how these values can be assigned to the payload object. As a \nresult it\'s common to follow each processing step with a Pass stage to restructure the results into the payload\nappropriately. The alternative is to make each processing stage take on this responsibility within the processing\nflow. This works, but forces a very tight connection between the SFN definition and the Lambda or other code, and\nremoves the ability to flexibly use that component in a different context.\n\n# A new approach\nPySFN allows you to define your state machines in the same way that you would define any other function in\nPython. Look at the following function which executes a series of steps. The steps (`step[1-4]`) each refer\nto a lambda operation that we want to execute. \n\n```python\n@state_machine(self, "pysfn-basic", locals())\ndef basic(str_value: str, list_value: List[int] = None, option: bool = False):\n    uri1: Union[str, None] = None\n    uri2: Union[str, None] = None\n    (\n        available,\n        mode,\n        option,\n        processing_seconds,\n        code_value,\n        type_value,\n    ) = step1(str_value, option)\n\n    if available:\n        if mode == "html":\n            (available, list_value, uri1) = step2(str_value, list_value)\n        else:\n            (available, uri2, uri1) = step3(str_value, mode, code_value)\n        if uri1:\n            uri2 = step4(uri1)\n    return (\n        mode,\n        code_value,\n        processing_seconds,\n        available,\n        uri1,\n        uri2,\n        option,\n    )\n```\n\nBy attaching the `@statemachine` decorator to the function, we instruct the CDK to generate a State Machine\nConstruct named *pysfn-basic* that has a definition aligned with the function contents. You can see the result\nin the **long** detail below.\n\n```json\n{\n  "StartAt": "Register Input [1:1]",\n  "States": {\n    "Register Input [1:1]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "Next": "Has list_value [1:2]"\n    },\n    "Has list_value [1:2]": {\n      "Type": "Choice",\n      "Choices": [\n        {\n          "Variable": "$.register.list_value",\n          "IsPresent": false,\n          "Next": "Assign list_value default [1:3]"\n        }\n      ],\n      "Default": "Has option [1:4]"\n    },\n    "Assign list_value default [1:3]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "list_value": "",\n        "str_value.$": "$.str_value"\n      },\n      "Next": "Has option [1:4]"\n    },\n    "Has option [1:4]": {\n      "Type": "Choice",\n      "Choices": [\n        {\n          "Variable": "$.register.option",\n          "IsPresent": false,\n          "Next": "Assign option default [1:5]"\n        }\n      ],\n      "Default": "Assign uri1 [1:6]"\n    },\n    "Assign option default [1:5]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "option": false,\n        "str_value.$": "$.str_value",\n        "list_value.$": "$.list_value"\n      },\n      "Next": "Assign uri1 [1:6]"\n    },\n    "Assign uri1 [1:6]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "uri1": "",\n        "option.$": "$.option",\n        "str_value.$": "$.str_value",\n        "list_value.$": "$.list_value"\n      },\n      "Next": "Assign uri2 [1:7]"\n    },\n    "Assign uri2 [1:7]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "uri2": "",\n        "option.$": "$.option",\n        "uri1.$": "$.uri1",\n        "str_value.$": "$.str_value",\n        "list_value.$": "$.list_value"\n      },\n      "Next": "Call step1 [1:8]"\n    },\n    "Call step1 [1:8]": {\n      "Next": "Register step1 [1:9]",\n      "Retry": [\n        {\n          "ErrorEquals": [\n            "Lambda.ServiceException",\n            "Lambda.AWSLambdaException",\n            "Lambda.SdkClientException"\n          ],\n          "IntervalSeconds": 2,\n          "MaxAttempts": 6,\n          "BackoffRate": 2\n        }\n      ],\n      "Type": "Task",\n      "ResultPath": "$.register.out",\n      "Resource": "arn:aws:states:::lambda:invoke",\n      "Parameters": {\n        "FunctionName": "arn:aws:lambda:us-west-2:999999999999:function:pysfn-base-python",\n        "Payload": {\n          "str_value.$": "$.register.str_value",\n          "bool_value.$": "$.register.option",\n          "launcher_target": "step1"\n        }\n      }\n    },\n    "Register step1 [1:9]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "available.$": "$.out.Payload.arg0",\n        "mode.$": "$.out.Payload.arg1",\n        "option.$": "$.out.Payload.arg2",\n        "processing_seconds.$": "$.out.Payload.arg3",\n        "code_value.$": "$.out.Payload.arg4",\n        "type_value.$": "$.out.Payload.arg5",\n        "list_value.$": "$.list_value",\n        "uri1.$": "$.uri1",\n        "uri2.$": "$.uri2",\n        "str_value.$": "$.str_value"\n      },\n      "Next": "If available [1:10]"\n    },\n    "If available [1:10]": {\n      "Type": "Choice",\n      "Choices": [\n        {\n          "And": [\n            {\n              "Variable": "$.register.available",\n              "IsPresent": true\n            },\n            {\n              "Or": [\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.available",\n                      "IsBoolean": true\n                    },\n                    {\n                      "Variable": "$.register.available",\n                      "BooleanEquals": true\n                    }\n                  ]\n                },\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.available",\n                      "IsString": true\n                    },\n                    {\n                      "Not": {\n                        "Variable": "$.register.available",\n                        "StringEquals": ""\n                      }\n                    }\n                  ]\n                },\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.available",\n                      "IsNumeric": true\n                    },\n                    {\n                      "Not": {\n                        "Variable": "$.register.available",\n                        "NumericEquals": 0\n                      }\n                    }\n                  ]\n                }\n              ]\n            }\n          ],\n          "Next": "If mode==\'html\' [1:11]"\n        }\n      ],\n      "Default": "Return [1:19]"\n    },\n    "If mode==\'html\' [1:11]": {\n      "Type": "Choice",\n      "Choices": [\n        {\n          "Variable": "$.register.mode",\n          "StringEquals": "html",\n          "Next": "Call step2 [1:12]"\n        }\n      ],\n      "Default": "Call step3 [1:14]"\n    },\n    "Call step2 [1:12]": {\n      "Next": "Register step2 [1:13]",\n      "Retry": [\n        {\n          "ErrorEquals": [\n            "Lambda.ServiceException",\n            "Lambda.AWSLambdaException",\n            "Lambda.SdkClientException"\n          ],\n          "IntervalSeconds": 2,\n          "MaxAttempts": 6,\n          "BackoffRate": 2\n        }\n      ],\n      "Type": "Task",\n      "ResultPath": "$.register.out",\n      "Resource": "arn:aws:states:::lambda:invoke",\n      "Parameters": {\n        "FunctionName": "arn:aws:lambda:us-west-2:999999999999:function:pysfn-js",\n        "Payload": {\n          "strValue.$": "$.register.str_value",\n          "optParam.$": "$.register.list_value"\n        }\n      }\n    },\n    "Register step2 [1:13]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "available.$": "$.out.Payload.available",\n        "list_value.$": "$.out.Payload.listValue",\n        "uri1.$": "$.out.Payload.resultURI",\n        "code_value.$": "$.code_value",\n        "mode.$": "$.mode",\n        "processing_seconds.$": "$.processing_seconds",\n        "option.$": "$.option",\n        "type_value.$": "$.type_value",\n        "uri2.$": "$.uri2",\n        "str_value.$": "$.str_value"\n      },\n      "Next": "If uri1 [1:16]"\n    },\n    "Call step3 [1:14]": {\n      "Next": "Register step3 [1:15]",\n      "Retry": [\n        {\n          "ErrorEquals": [\n            "Lambda.ServiceException",\n            "Lambda.AWSLambdaException",\n            "Lambda.SdkClientException"\n          ],\n          "IntervalSeconds": 2,\n          "MaxAttempts": 6,\n          "BackoffRate": 2\n        }\n      ],\n      "Type": "Task",\n      "ResultPath": "$.register.out",\n      "Resource": "arn:aws:states:::lambda:invoke",\n      "Parameters": {\n        "FunctionName": "arn:aws:lambda:us-west-2:999999999999:function:pysfn-highmemory-python",\n        "Payload": {\n          "str_value.$": "$.register.str_value",\n          "str_value2.$": "$.register.mode",\n          "str_value3.$": "$.register.code_value",\n          "launcher_target": "step3"\n        }\n      }\n    },\n    "Register step3 [1:15]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "available.$": "$.out.Payload.arg0",\n        "uri2.$": "$.out.Payload.arg1",\n        "uri1.$": "$.out.Payload.arg2",\n        "code_value.$": "$.code_value",\n        "mode.$": "$.mode",\n        "processing_seconds.$": "$.processing_seconds",\n        "list_value.$": "$.list_value",\n        "option.$": "$.option",\n        "type_value.$": "$.type_value",\n        "str_value.$": "$.str_value"\n      },\n      "Next": "If uri1 [1:16]"\n    },\n    "If uri1 [1:16]": {\n      "Type": "Choice",\n      "Choices": [\n        {\n          "And": [\n            {\n              "Variable": "$.register.uri1",\n              "IsPresent": true\n            },\n            {\n              "Or": [\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.uri1",\n                      "IsBoolean": true\n                    },\n                    {\n                      "Variable": "$.register.uri1",\n                      "BooleanEquals": true\n                    }\n                  ]\n                },\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.uri1",\n                      "IsString": true\n                    },\n                    {\n                      "Not": {\n                        "Variable": "$.register.uri1",\n                        "StringEquals": ""\n                      }\n                    }\n                  ]\n                },\n                {\n                  "And": [\n                    {\n                      "Variable": "$.register.uri1",\n                      "IsNumeric": true\n                    },\n                    {\n                      "Not": {\n                        "Variable": "$.register.uri1",\n                        "NumericEquals": 0\n                      }\n                    }\n                  ]\n                }\n              ]\n            }\n          ],\n          "Next": "Call step4 [1:17]"\n        }\n      ],\n      "Default": "Return [1:19]"\n    },\n    "Call step4 [1:17]": {\n      "Next": "Register step4 [1:18]",\n      "Retry": [\n        {\n          "ErrorEquals": [\n            "Lambda.ServiceException",\n            "Lambda.AWSLambdaException",\n            "Lambda.SdkClientException"\n          ],\n          "IntervalSeconds": 2,\n          "MaxAttempts": 6,\n          "BackoffRate": 2\n        }\n      ],\n      "Type": "Task",\n      "ResultPath": "$.register.out",\n      "Resource": "arn:aws:states:::lambda:invoke",\n      "Parameters": {\n        "FunctionName": "arn:aws:lambda:us-west-2:999999999999:function:pysfn-base-python",\n        "Payload": {\n          "str_value.$": "$.register.uri1",\n          "launcher_target": "step4"\n        }\n      }\n    },\n    "Register step4 [1:18]": {\n      "Type": "Pass",\n      "ResultPath": "$.register",\n      "InputPath": "$.register",\n      "Parameters": {\n        "uri2.$": "$.out.Payload.arg0",\n        "available.$": "$.available",\n        "code_value.$": "$.code_value",\n        "mode.$": "$.mode",\n        "processing_seconds.$": "$.processing_seconds",\n        "list_value.$": "$.list_value",\n        "option.$": "$.option",\n        "uri1.$": "$.uri1",\n        "type_value.$": "$.type_value",\n        "str_value.$": "$.str_value"\n      },\n      "Next": "Return [1:19]"\n    },\n    "Return [1:19]": {\n      "Type": "Pass",\n      "Parameters": {\n        "mode.$": "$.register.mode",\n        "code_value.$": "$.register.code_value",\n        "processing_seconds.$": "$.register.processing_seconds",\n        "available.$": "$.register.available",\n        "uri1.$": "$.register.uri1",\n        "uri2.$": "$.register.uri2",\n        "option.$": "$.register.option"\n      },\n      "End": true\n    }\n  }\n}\n```\n\nA few items to note with this result:\n* To avoid name conflicts when the CDK generates the constructs, I\'ve added an ID suffix to each stage.\n* I treat the `register` object within the payload as my version of `locals()` to maintain a clean\n  view of the current set of vars. The first step copies the inputs into the register.\n* After this, we address any optional parameters defined in the function signature. If they aren\'t present,\n  we set the default value.\n* This function sets defaults for two `uri` values which we set using Pass states.\n* The if operations are converted to Choice states with the appropriate conditions. Note that in the case\n  of the first and last Choice states, the logic inserts a complex condition to mimic Python boolean type coercion.\n* Each call to a Lambda function is followed by a generated Pass state to move the results into the register.\n\n## About Lambdas...\nOne of the goals of this project is to make working with Python lambdas more flexible so that you don\'t have\nto spend a lot of time writing code to parse the `event` object over and over. While it\'s not necessary to\nuse it to take advantage of the transpiler, most of the Lambda steps in the proto_app are based on \n**launcher** logic I\'ve included.\n\nThe `step1` function in the `operations.py` module is defined as shown below. Note that this looks like any other \npython function and could be referenced anywhere in your code. \n\n```python\ndef step1(str_value: str, bool_value: bool) -> (bool, str, bool, int, int, str):\n    return True, str_value, False, 4, 200, "text/html"\n```\n\nTo pull this into our stack we have to start by creating a Lambda that will hold the function. \nThis looks like this:\n\n```python\nbase_lambda = PythonLambda(\n    self,\n    "pysfn-base-python",\n    os.path.join(os.getcwd(), "python"),\n    role=self.lambda_role,\n    runtime=PythonLambda.PYTHON_3_9,\n    timeout_minutes=1,\n    memory_mb=1,\n    environment=None,\n)\n```\n\nThe `PythonLambda` class allows us to define a Lambda Construct that can contain multiple functions to be \nexecuted via a launcher that it will generate. Now that we\'ve defined the container, we can add our function\nto the launcher.\n\n```python\nstep1 = base_lambda.register(operations.step1)\n```\n\nThe new `step1` variable has the same function signature as the original function, but can now be used\nwithin our state machine function. The transpiler uses the details of this lambda to produce the following\nstate in our state machine. Note the `pysfn_operation` value that is included in the Payload.\n\n```json\n    "Call step1 [1:8]": {\n      "Next": "Register step1 [1:9]",\n      "Type": "Task",\n      "ResultPath": "$.register.out",\n      "Resource": "arn:aws:states:::lambda:invoke",\n      "Parameters": {\n        "FunctionName": "arn:aws:lambda:us-west-2:999999999999:function:pysfn-base-python",\n        "Payload": {\n          "str_value.$": "$.register.str_value",\n          "bool_value.$": "$.register.option",\n          "pysfn_operation": "step1"\n        }\n      }\n    }\n```\n\nOf course, existing Lambdas are also supported. For example, we can define a Lambda construct as we normally\nwould as shown below.\n\n```python\njs_lambda = lmbda.Function(\n    self,\n    "JSLambda",\n    function_name="pysfn-js",\n    code=lmbda.Code.from_asset(\n        os.path.join(os.getcwd(), "js"), exclude=["node_modules"]\n    ),\n    handler="app.handler",\n    runtime=lmbda.Runtime.NODEJS_14_X,\n    role=self.lambda_role,\n    timeout=Duration.minutes(10),\n    memory_size=2096,\n)\n```\n\nThen we can create a pysfn function from this construct as follows by declaring the input parameters and output \nvalues.\n\n```python\nstep2 = function_for_lambda(\n    js_lambda,\n    {"strValue": str, "optParam": bool},\n    {"available": bool, "listValue": List[int], "resultURI": str},\n)\n```\n\nBy specifying the output values in the function declaration, it allows PySFN to map the results from \na call like this to the appropriate variables.\n\n```python\n(available, list_value, uri1) = step2(str_value, list_value)\n```\n\nIn the step after the Lambda is invoked, a Pass state performs the mapping.\n\n```json\n"Register step2 [1:13]": {\n  "Type": "Pass",\n  "ResultPath": "$.register",\n  "InputPath": "$.register",\n  "Parameters": {\n    "available.$": "$.out.Payload.available",\n    "list_value.$": "$.out.Payload.listValue",\n    "uri1.$": "$.out.Payload.resultURI",\n    "code_value.$": "$.code_value",\n    "mode.$": "$.mode",\n    "processing_seconds.$": "$.processing_seconds",\n    "option.$": "$.option",\n    "type_value.$": "$.type_value",\n    "uri2.$": "$.uri2",\n    "str_value.$": "$.str_value"\n  },\n  "Next": "If uri1 [1:16]"\n}\n```\n\n# More to do!\nAfter a bunch of experiments and refactoring, I think I\'ve been able to prove the utility of this approach,\nat least for the range of projects I typically use SFN for. It\'s still undocumented and has a lot of\nrough edges, but overall I\'ve been thrilled at how easy it has been to iterate on new and existing SFNs\nusing this approach. It significantly reduces the cognitive load I felt when working with the stages language\nand makes it much easier to build stable and well-managed data flows.\n\nThat said, feedback and PRs are welcome. Over the next few months I\'ll hopefully be able to address the\nfollowing:\n1. Better support for `list`, `dict`, and `attribute` access\n2. List comprehensions\n3. Support for dataclasses\n4. Real documentation\n5. Take full advantage of Python type hints\n6. Support functions with kwonly or posonly args\n7. Add support for Parallel\n8. Support the full range of likely conditions\n9. Tree shaking to better handle if/elif/elif/else, as well as assigning multiple variables\n10. Support some common integrations such as reading from S3 or performing DynamoDB writes\n',
     'author': 'Dave Schultz',
     'author_email': 'dave@daveschultzconsulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pysfn-0.1.8/PKG-INFO` & `pysfn-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfn
-Version: 0.1.8
+Version: 0.1.9
 Summary: Transpiler for AWS Step Functions
 License: MIT
 Author: Dave Schultz
 Author-email: dave@daveschultzconsulting.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

