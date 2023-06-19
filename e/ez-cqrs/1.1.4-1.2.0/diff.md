# Comparing `tmp/ez_cqrs-1.1.4.tar.gz` & `tmp/ez_cqrs-1.2.0.tar.gz`

## Comparing `ez_cqrs-1.1.4.tar` & `ez_cqrs-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/error.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/integration/conftest.py
--rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/PKG-INFO
```

### Comparing `ez_cqrs-1.1.4/.github/workflows/release.yml` & `ez_cqrs-1.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/.github/workflows/test.yml` & `ez_cqrs-1.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/ez_cqrs/acid_exec.py` & `ez_cqrs-1.2.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/ez_cqrs/components.py` & `ez_cqrs-1.2.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/ez_cqrs/error.py` & `ez_cqrs-1.2.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/ez_cqrs/framework.py` & `ez_cqrs-1.2.0/ez_cqrs/framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 if TYPE_CHECKING:
     from collections.abc import Coroutine
 
     import pydantic
 
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
-    from ez_cqrs.shared_state import Config
 
 T = TypeVar("T")
 
 
 @final
 @dataclass(repr=True, frozen=True, eq=False)
 class EzCqrs(Generic[C, E]):
@@ -36,40 +35,38 @@
     cmd_handler: CommandHandler[C, E]
     event_dispatcher: EventDispatcher[E]
 
     async def run(
         self,
         cmd: C,
         max_transactions: int,
-        config: Config,
     ) -> Result[Any, ExecutionError | pydantic.ValidationError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         validated = self.cmd_handler.validate(command=cmd)
         if not isinstance(validated, Ok):
             return Err(validated.err())
 
         execution_result = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
                 ops_registry=OpsRegistry[Any](max_lenght=max_transactions),
-                config=config,
             ),
         )
         if not isinstance(execution_result, Ok):
             return Err(execution_result.err())
 
         event_dispatch_tasks: list[Coroutine[Any, Any, None]] = []
 
         execution_value, list_of_events = execution_result.unwrap()
 
         for event in list_of_events:
             event_dispatch_tasks.append(
-                self.event_dispatcher.dispatch(event=event, config=config),
+                self.event_dispatcher.dispatch(event=event),
             )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
         return Ok(execution_value)
```

### Comparing `ez_cqrs-1.1.4/ez_cqrs/handler.py` & `ez_cqrs-1.2.0/ez_cqrs/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 if TYPE_CHECKING:
     import pydantic
     from result import Result
 
     from ez_cqrs.acid_exec import OpsRegistry
     from ez_cqrs.error import ExecutionError
-    from ez_cqrs.shared_state import Config
 
 
 class CommandHandler(abc.ABC, Generic[C, E]):
     """Command handler handles every command to complete one user intent."""
 
     @abc.abstractmethod
     def validate(
@@ -26,15 +25,14 @@
         """Validate command data."""
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
-        config: Config,
     ) -> Result[tuple[Any, list[E]], ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
 
@@ -48,9 +46,9 @@
 
     Some examples of tasks that event dispatcher can handle:
     - updated application state views in downstream services.
     - publish events to messaging services.
     """
 
     @abc.abstractmethod
-    async def dispatch(self, event: E, config: Config) -> None:
+    async def dispatch(self, event: E) -> None:
         """Dispatch events generated by command."""
```

### Comparing `ez_cqrs-1.1.4/ez_cqrs/testing.py` & `ez_cqrs-1.2.0/ez_cqrs/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from ez_cqrs.components import C, E
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler
-    from ez_cqrs.shared_state import Config
+
 
 NO_RESULT_MSG = "No result to evaluate."
 
 
 @final
 @dataclass(frozen=False, repr=False, eq=False)
 class CommandHandlerFramework(Generic[C, E]):
@@ -103,23 +103,21 @@
             self._is_valid = False
         self._is_valid = True
         return self
 
     async def execute(
         self,
         max_transactions: int,
-        config: Config,
     ) -> Self:
         """Execute command while asserting and validating framework's rules."""
         ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
         execution_result = await asyncio.create_task(
             self.cmd_handler.handle(
                 command=self.cmd,
                 ops_registry=ops_registry,
-                config=config,
             ),
         )
         if not ops_registry.is_empty():
             msg = "OpsRegistry is not empty after cmd execution."
             raise RuntimeError(msg)
 
         self._result = execution_result
```

### Comparing `ez_cqrs-1.1.4/ez_cqrs/utilities/cli.py` & `ez_cqrs-1.2.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/requirements/core.txt` & `ez_cqrs-1.2.0/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/requirements/dev.txt` & `ez_cqrs-1.2.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/scripts/new_release.py` & `ez_cqrs-1.2.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/tests/integration/conftest.py` & `ez_cqrs-1.2.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/tests/integration/test_execution.py` & `ez_cqrs-1.2.0/tests/integration/test_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pydantic import BaseModel, ValidationError
 from result import Err, Ok, Result
 from typing_extensions import assert_never
 
 from ez_cqrs.acid_exec import OpsRegistry
 from ez_cqrs.components import Command, DomainEvent
 from ez_cqrs.handler import CommandHandler
-from ez_cqrs.shared_state import Config
 from ez_cqrs.testing import CommandHandlerFramework
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import TypeAlias
@@ -88,18 +87,17 @@
 
         assert_never(command)
 
     async def handle(  # noqa: D102
         self,
         command: BankAccountCommand,
         ops_registry: OpsRegistry[Any],
-        config: Config,
     ) -> Result[tuple[Any, list[BankAccountEvent]], ExecutionError]:
         _ = ops_registry
-        _ = config
+
         if isinstance(command, OpenAccount):
             return Ok(
                 (
                     None,
                     [
                         AccountOpened(
                             account_id=command.account_id,
@@ -155,20 +153,19 @@
     async def test_handle(
         self,
         command: BankAccountCommand,
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test handle method."""
         cmd_handler = BankAccountCommandHandler()
-        app_config = Config()
+
         execution_result = await asyncio.create_task(
             cmd_handler.handle(
                 command=command,
                 ops_registry=OpsRegistry[Any](max_lenght=0),
-                config=app_config,
             ),
         )
         _, resultant_events = execution_result.unwrap()
         assert resultant_events == expected_events
 
     @pytest.mark.parametrize(
         argnames=["cmd_handler", "cmd", "expected_value", "expected_events"],
@@ -203,15 +200,14 @@
             cmd=cmd,
         )
 
         assert framework.validate().then_expect_is_valid()
         await asyncio.create_task(
             framework.execute(
                 max_transactions=0,
-                config=Config(),
             ),
         )
         assert framework.then_expect_events(expected_events=expected_events)
         assert framework.then_expect_value(expected_value=expected_value)
         resultant_value, resultant_events = framework.inspect_result()
         assert resultant_value == expected_value
         assert resultant_events == expected_events
```

### Comparing `ez_cqrs-1.1.4/tests/unit/test_acid_exec.py` & `ez_cqrs-1.2.0/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/.gitignore` & `ez_cqrs-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/LICENSE` & `ez_cqrs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.4/pyproject.toml` & `ez_cqrs-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.1.4"
+version = "1.2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.1.4/PKG-INFO` & `ez_cqrs-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.1.4
+Version: 1.2.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

