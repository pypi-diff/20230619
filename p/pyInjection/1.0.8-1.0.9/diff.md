# Comparing `tmp/pyInjection-1.0.8.tar.gz` & `tmp/pyInjection-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyInjection-1.0.8.tar", last modified: Sat May 20 22:19:06 2023, max compression
+gzip compressed data, was "pyInjection-1.0.9.tar", last modified: Mon Jun 19 19:53:46 2023, max compression
```

## Comparing `pyInjection-1.0.8.tar` & `pyInjection-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.902705 pyInjection-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     4139 2023-05-20 22:19:06.902705 pyInjection-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3874 2023-05-20 22:18:55.000000 pyInjection-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 22:19:06.902705 pyInjection-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-05-20 22:18:55.000000 pyInjection-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.895705 pyInjection-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.897705 pyInjection-1.0.8/src/pyInjection/
--rwxrwxrwx   0 root         (0) root         (0)       43 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.899705 pyInjection-1.0.8/src/pyInjection/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3515 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/container/container_instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.899705 pyInjection-1.0.8/src/pyInjection/dtos/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/dtos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/dtos/registration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.900705 pyInjection-1.0.8/src/pyInjection/enums/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/enums/scope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.900705 pyInjection-1.0.8/src/pyInjection/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/container_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/helpers/type_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.901705 pyInjection-1.0.8/src/pyInjection/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/iscope_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/interfaces/ivalidator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.901705 pyInjection-1.0.8/src/pyInjection/scope_managers/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1799 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/singleton_scope_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/scope_managers/transient_scope_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.902705 pyInjection-1.0.8/src/pyInjection/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/decorator_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-20 22:18:55.000000 pyInjection-1.0.8/src/pyInjection/validators/primitive_dependency_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 22:19:06.898705 pyInjection-1.0.8/src/pyInjection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4139 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-20 22:19:06.000000 pyInjection-1.0.8/src/pyInjection.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.233243 pyInjection-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-06-19 19:53:46.233243 pyInjection-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3874 2023-06-19 19:53:34.000000 pyInjection-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 19:53:46.233243 pyInjection-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-06-19 19:53:34.000000 pyInjection-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.227243 pyInjection-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.229243 pyInjection-1.0.9/src/pyInjection/
+-rwxrwxrwx   0 root         (0) root         (0)       43 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.230243 pyInjection-1.0.9/src/pyInjection/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/container/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/container/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3515 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/container/container_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.230243 pyInjection-1.0.9/src/pyInjection/dtos/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/dtos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/dtos/registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.231243 pyInjection-1.0.9/src/pyInjection/enums/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/enums/scope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.231243 pyInjection-1.0.9/src/pyInjection/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/helpers/container_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/helpers/type_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.232243 pyInjection-1.0.9/src/pyInjection/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/interfaces/iscope_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/interfaces/ivalidator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.232243 pyInjection-1.0.9/src/pyInjection/scope_managers/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/scope_managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/scope_managers/singleton_scope_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/scope_managers/transient_scope_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.233243 pyInjection-1.0.9/src/pyInjection/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/validators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/validators/decorator_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-06-19 19:53:34.000000 pyInjection-1.0.9/src/pyInjection/validators/primitive_dependency_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:53:46.229243 pyInjection-1.0.9/src/pyInjection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-06-19 19:53:46.000000 pyInjection-1.0.9/src/pyInjection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-19 19:53:46.000000 pyInjection-1.0.9/src/pyInjection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 19:53:46.000000 pyInjection-1.0.9/src/pyInjection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-19 19:53:46.000000 pyInjection-1.0.9/src/pyInjection.egg-info/top_level.txt
```

### Comparing `pyInjection-1.0.8/PKG-INFO` & `pyInjection-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyInjection
-Version: 1.0.8
+Version: 1.0.9
 Summary: Dependency injection container for Python3
 Author: Joshua Loader
 Author-email: pyInjection@joshloader.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyInjection-1.0.8/README.md` & `pyInjection-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/setup.py` & `pyInjection-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description: str = ""
 root_path: str = path.abspath(path.dirname(__file__))
 with open(path.join(root_path, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pyInjection",
-    version="1.0.8",
+    version="1.0.9",
     author="Joshua Loader",
     author_email="pyInjection@joshloader.com",
     description="Dependency injection container for Python3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `pyInjection-1.0.8/src/pyInjection/container/container.py` & `pyInjection-1.0.9/src/pyInjection/container/container.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/src/pyInjection/container/container_instance.py` & `pyInjection-1.0.9/src/pyInjection/container/container_instance.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/src/pyInjection/helpers/container_helpers.py` & `pyInjection-1.0.9/src/pyInjection/helpers/container_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,43 +17,49 @@
     ignore_parameters: List[str] = ["self", "args", "kwargs"]
 
     @staticmethod
     def resolve(
         interface: Type,
         container: Dict[Type, Registration],
         is_same_registration_scope: Callable,
+        resolve_scope_decorator: Callable[[Type, Any], Any],
         base_types: List[Type],
     ) -> Any:
         error_message: str = ""
         if interface in container.keys():
             implementation: Any = container[interface].implementation
             if type(implementation) in base_types:
                 if type(implementation) == _GenericAlias:  # type: ignore
                     return ContainerHelpers.resolve_generic(
                         interface=interface,
                         container=container,
                         is_same_registration_scope=is_same_registration_scope,
+                        resolve_scope_decorator=resolve_scope_decorator,
                         base_types=base_types,
                     )
                 else:
                     kwargs: Any = {}
                     sig: Signature = signature(implementation)
                     for p in sig.parameters:
                         if p not in ContainerHelpers.ignore_parameters:
                             child_interface: Type = sig.parameters[p].annotation
                             is_same_registration_scope(
                                 interface=interface,
                                 child_interface=child_interface,
                                 container=container,
                             )
-                            instance = ContainerHelpers.resolve(
-                                interface=child_interface,
-                                container=container,
-                                is_same_registration_scope=is_same_registration_scope,
-                                base_types=base_types,
+                            instance = resolve_scope_decorator(
+                                child_interface,
+                                ContainerHelpers.resolve(
+                                    interface=child_interface,
+                                    container=container,
+                                    is_same_registration_scope=is_same_registration_scope,
+                                    resolve_scope_decorator=resolve_scope_decorator,
+                                    base_types=base_types,
+                                ),
                             )
                             kwargs[p] = instance
                     return implementation(**kwargs)
             elif type(implementation) == type(lambda: ""):
                 return implementation()
             else:
                 return implementation
@@ -62,14 +68,15 @@
             raise Exception(error_message)
 
     @staticmethod
     def resolve_generic(
         interface: Type,
         container: Dict[Type, Registration],
         is_same_registration_scope: Callable,
+        resolve_scope_decorator: Callable[[Type, Any], Any],
         base_types: List[Type],
     ) -> Any:
         replace_child_type: bool = False
         implementation: Any = container[interface].implementation
         implementation_type: Type = implementation.__origin__
         generic_class: Type = implementation.__args__[0]
         kwargs: Any = {}
@@ -84,19 +91,23 @@
                         child_interface.__args__ = (generic_class,)
                         replace_child_type = True
                 is_same_registration_scope(
                     interface=interface,
                     child_interface=child_interface,
                     container=container,
                 )
-                instance = ContainerHelpers.resolve(
-                    interface=child_interface,
-                    container=container,
-                    is_same_registration_scope=is_same_registration_scope,
-                    base_types=base_types,
+                instance = resolve_scope_decorator(
+                    child_interface,
+                    ContainerHelpers.resolve(
+                        interface=child_interface,
+                        container=container,
+                        is_same_registration_scope=is_same_registration_scope,
+                        resolve_scope_decorator=resolve_scope_decorator,
+                        base_types=base_types,
+                    ),
                 )
                 kwargs[p] = instance
                 ## Place TypeVar back into child_interface for later resolves
                 if replace_child_type:
                     T = TypeVar("T")
                     child_interface.__args__ = (T,)
         return implementation(**kwargs)
```

### Comparing `pyInjection-1.0.8/src/pyInjection/helpers/type_helpers.py` & `pyInjection-1.0.9/src/pyInjection/helpers/type_helpers.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/src/pyInjection/scope_managers/singleton_scope_manager.py` & `pyInjection-1.0.9/src/pyInjection/scope_managers/transient_scope_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 from inspect import Signature, signature
-from typing import Any, Dict, List, Type, _GenericAlias  # type: ignore
+from typing import Any, Dict, List, Type, TypeVar, _GenericAlias  # type: ignore
 
 from ..dtos import Registration
 from ..enums import Scope
 from ..helpers import ContainerHelpers, TypeHelpers
 from ..interfaces import IScopeManager
 
 
-class SingletonScopeManager(IScopeManager):
-    __resolved_instances: Dict[Type, Any]
+class TransientScopeManager(IScopeManager):
     __base_types: List[Type]
 
     def __init__(self, base_types: List[Type]) -> None:
-        self.__resolved_instances = {}
         self.__base_types = base_types
 
     def can_resolve(self, scope: Scope) -> bool:
-        return scope == Scope.SINGLETON
+        return scope == Scope.TRANSIENT
 
     def is_same_registration_scope_v2(
         self,
         interface: Type,
         child_interface: Type,
         container: Dict[Type, Registration],
     ) -> None:
         registration: Registration = container[child_interface]
-        if registration.scope != Scope.SINGLETON:
-            warning_message: str = f"Warning Singleton type: {TypeHelpers.to_string(interface)} registered with Transient dependency: {TypeHelpers.to_string(child_interface)}"
-            print(warning_message)
+        if registration.scope != Scope.TRANSIENT:
+            error_message = f"Error Transient type: {TypeHelpers.to_string(interface)} registered with Singleton dependency: {TypeHelpers.to_string(child_interface)}"
+            raise Exception(error_message)
+
+    def resolve_scope_decorator(self, interface: Type, instance: Any) -> Any:
+        return instance
 
     def resolve(self, interface: Type, container: Dict[Type, Registration]) -> Any:
-        if interface in self.__resolved_instances.keys():
-            return self.__resolved_instances[interface]
-        else:
-            self.__resolved_instances[interface] = ContainerHelpers.resolve(
-                interface=interface,
-                container=container,
-                is_same_registration_scope=self.is_same_registration_scope_v2,
-                base_types=self.__base_types,
-            )
-            return self.__resolved_instances[interface]
-
-    @property
-    # Exposed for Unit Testing
-    def resolved_instances(self) -> Dict[Type, Any]:
-        return self.__resolved_instances
+        return ContainerHelpers.resolve(
+            interface=interface,
+            container=container,
+            is_same_registration_scope=self.is_same_registration_scope_v2,
+            resolve_scope_decorator=self.resolve_scope_decorator,
+            base_types=self.__base_types,
+        )
```

### Comparing `pyInjection-1.0.8/src/pyInjection/scope_managers/transient_scope_manager.py` & `pyInjection-1.0.9/src/pyInjection/scope_managers/singleton_scope_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 from inspect import Signature, signature
-from typing import Any, Dict, List, Type, TypeVar, _GenericAlias  # type: ignore
+from logging import warning
+from typing import Any, Dict, List, Type, _GenericAlias  # type: ignore
 
 from ..dtos import Registration
 from ..enums import Scope
 from ..helpers import ContainerHelpers, TypeHelpers
 from ..interfaces import IScopeManager
 
 
-class TransientScopeManager(IScopeManager):
+class SingletonScopeManager(IScopeManager):
+    __resolved_instances: Dict[Type, Any]
     __base_types: List[Type]
 
     def __init__(self, base_types: List[Type]) -> None:
+        self.__resolved_instances = {}
         self.__base_types = base_types
 
     def can_resolve(self, scope: Scope) -> bool:
-        return scope == Scope.TRANSIENT
+        return scope == Scope.SINGLETON
 
     def is_same_registration_scope_v2(
         self,
         interface: Type,
         child_interface: Type,
         container: Dict[Type, Registration],
     ) -> None:
         registration: Registration = container[child_interface]
-        if registration.scope != Scope.TRANSIENT:
-            error_message = f"Error Transient type: {TypeHelpers.to_string(interface)} registered with Singleton dependency: {TypeHelpers.to_string(child_interface)}"
-            raise Exception(error_message)
+        if registration.scope != Scope.SINGLETON:
+            warning_message: str = f"Warning Singleton type: {TypeHelpers.to_string(interface)} registered with Transient dependency: {TypeHelpers.to_string(child_interface)}"
+            warning(warning_message)
+
+    def resolve_scope_decorator(self, interface: Type, instance: Any) -> Any:
+        if interface not in self.__resolved_instances.keys():
+            self.__resolved_instances[interface] = instance
+        return instance
 
     def resolve(self, interface: Type, container: Dict[Type, Registration]) -> Any:
-        return ContainerHelpers.resolve(
-            interface=interface,
-            container=container,
-            is_same_registration_scope=self.is_same_registration_scope_v2,
-            base_types=self.__base_types,
-        )
+        if interface in self.__resolved_instances.keys():
+            return self.__resolved_instances[interface]
+        else:
+            self.__resolved_instances[interface] = ContainerHelpers.resolve(
+                interface=interface,
+                container=container,
+                is_same_registration_scope=self.is_same_registration_scope_v2,
+                resolve_scope_decorator=self.resolve_scope_decorator,
+                base_types=self.__base_types,
+            )
+            return self.__resolved_instances[interface]
+
+    @property
+    # Exposed for Unit Testing
+    def resolved_instances(self) -> Dict[Type, Any]:
+        return self.__resolved_instances
```

### Comparing `pyInjection-1.0.8/src/pyInjection/validators/decorator_validator.py` & `pyInjection-1.0.9/src/pyInjection/validators/decorator_validator.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/src/pyInjection/validators/primitive_dependency_validator.py` & `pyInjection-1.0.9/src/pyInjection/validators/primitive_dependency_validator.py`

 * *Files identical despite different names*

### Comparing `pyInjection-1.0.8/src/pyInjection.egg-info/PKG-INFO` & `pyInjection-1.0.9/src/pyInjection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyInjection
-Version: 1.0.8
+Version: 1.0.9
 Summary: Dependency injection container for Python3
 Author: Joshua Loader
 Author-email: pyInjection@joshloader.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyInjection-1.0.8/src/pyInjection.egg-info/SOURCES.txt` & `pyInjection-1.0.9/src/pyInjection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

