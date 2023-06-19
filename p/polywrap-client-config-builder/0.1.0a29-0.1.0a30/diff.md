# Comparing `tmp/polywrap_client_config_builder-0.1.0a29.tar.gz` & `tmp/polywrap_client_config_builder-0.1.0a30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client_config_builder-0.1.0a29.tar", max compression
+gzip compressed data, was "polywrap_client_config_builder-0.1.0a30.tar", max compression
```

## Comparing `polywrap_client_config_builder-0.1.0a29.tar` & `polywrap_client_config_builder-0.1.0a30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1400 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/README.md
--rw-r--r--   0        0        0      117 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/__init__.py
--rw-r--r--   0        0        0      309 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/base_configure.py
--rw-r--r--   0        0        0     1997 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/env_configure.py
--rw-r--r--   0        0        0     1793 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/interface_configure.py
--rw-r--r--   0        0        0     1626 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/package_configure.py
--rw-r--r--   0        0        0     1510 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/redirect_configure.py
--rw-r--r--   0        0        0      884 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/resolver_configure.py
--rw-r--r--   0        0        0     1605 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/wrapper_configure.py
--rw-r--r--   0        0        0     2885 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/polywrap_client_config_builder.py
--rw-r--r--   0        0        0        0 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/py.typed
--rw-r--r--   0        0        0      164 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/__init__.py
--rw-r--r--   0        0        0      542 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/build_options.py
--rw-r--r--   0        0        0     1077 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/builder_config.py
--rw-r--r--   0        0        0     6793 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/client_config_builder.py
--rw-r--r--   0        0        0      991 2023-04-17 14:59:36.146234 polywrap_client_config_builder-0.1.0a29/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a29/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/README.md
+-rw-r--r--   0        0        0      138 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/base_configure.py
+-rw-r--r--   0        0        0     2702 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/env_configure.py
+-rw-r--r--   0        0        0     2120 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/interface_configure.py
+-rw-r--r--   0        0        0     1628 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/package_configure.py
+-rw-r--r--   0        0        0     1645 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/redirect_configure.py
+-rw-r--r--   0        0        0      965 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/resolver_configure.py
+-rw-r--r--   0        0        0     1607 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/wrapper_configure.py
+-rw-r--r--   0        0        0     4240 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/polywrap_client_config_builder.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/py.typed
+-rw-r--r--   0        0        0      164 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/__init__.py
+-rw-r--r--   0        0        0      613 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/build_options.py
+-rw-r--r--   0        0        0     1154 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/builder_config.py
+-rw-r--r--   0        0        0     6256 2023-06-19 11:25:19.297153 polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/client_config_builder.py
+-rw-r--r--   0        0        0     1108 2023-06-19 11:35:49.975540 polywrap_client_config_builder-0.1.0a30/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a30/PKG-INFO
```

### Comparing `polywrap_client_config_builder-0.1.0a29/README.md` & `polywrap_client_config_builder-0.1.0a30/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 ```python
 # accepted by the PolywrapClient
 config = builder.build()
 
 # build with a custom cache
 config = builder.build({
-  wrapperCache: WrapperCache(),
+  resolution_result_cache: ResolutionResultCache(),
 })
 
 # or build with a custom resolver
-coreClientConfig = builder.build({
+config = builder.build({
   resolver: RecursiveResolver(...),
 })
 ```
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/base_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/base_configure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """This module contains the base configure class for the client config builder."""
-from ..types import BuilderConfig, ClientConfigBuilder
+from typing import cast
 
+from ..types import BuilderConfig, ClientConfigBuilder
 
-class BaseConfigure(ClientConfigBuilder):
-    """BaseConfigure is the base configure class for the client config builder.
 
-    Attributes:
-        config (BuilderConfig): The internal configuration.
-    """
+class BaseConfigure:
+    """BaseConfigure is the base configure class for the client config builder."""
 
     config: BuilderConfig
 
     def add(self, config: BuilderConfig) -> ClientConfigBuilder:
         """Add the values from the given config to the builder's config."""
         if config.envs:
             self.config.envs.update(config.envs)
@@ -21,8 +19,8 @@
             self.config.redirects.update(config.redirects)
         if config.resolvers:
             self.config.resolvers.extend(config.resolvers)
         if config.wrappers:
             self.config.wrappers.update(config.wrappers)
         if config.packages:
             self.config.packages.update(config.packages)
-        return self
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/interface_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/interface_configure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """This module contains the interface configure class for the client config builder."""
-from typing import Dict, List, Union
+from typing import Dict, List, Union, cast
 
 from polywrap_core import Uri
 
-from ..types import ClientConfigBuilder
+from ..types import BuilderConfig, ClientConfigBuilder
 
 
-class InterfaceConfigure(ClientConfigBuilder):
+class InterfaceConfigure:
     """Allows configuring the interface-implementations."""
 
+    config: BuilderConfig
+
     def get_interfaces(self) -> Dict[Uri, List[Uri]]:
         """Return all registered interface and its implementations\
             from the builder's config."""
         return self.config.interfaces
 
     def get_interface_implementations(self, uri: Uri) -> Union[List[Uri], None]:
         """Return the interface for the given uri."""
         return self.config.interfaces.get(uri)
 
     def add_interface_implementations(
         self, interface_uri: Uri, implementations_uris: List[Uri]
     ) -> ClientConfigBuilder:
         """Add a list of implementation URIs for the given interface URI to the builder's config."""
         if interface_uri in self.config.interfaces.keys():
-            self.config.interfaces[interface_uri].extend(implementations_uris)
+            existing_implementations = set(self.config.interfaces[interface_uri])
+            for implementation_uri in implementations_uris:
+                if implementation_uri not in existing_implementations:
+                    self.config.interfaces[interface_uri].append(implementation_uri)
         else:
             self.config.interfaces[interface_uri] = implementations_uris
-        return self
+        return cast(ClientConfigBuilder, self)
 
     def remove_interface_implementations(
         self, interface_uri: Uri, implementations_uris: List[Uri]
     ) -> ClientConfigBuilder:
         """Remove the implementations for the given interface uri."""
         self.config.interfaces[interface_uri] = [
             uri
             for uri in self.config.interfaces[interface_uri]
             if uri not in implementations_uris
         ]
-        return self
+        return cast(ClientConfigBuilder, self)
 
     def remove_interface(self, interface_uri: Uri) -> ClientConfigBuilder:
         """Remove the interface for the given uri."""
         self.config.interfaces.pop(interface_uri, None)
-        return self
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/package_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/package_configure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 """This module contains the package configure class for the client config builder."""
-from typing import Dict, List, Union
+from typing import Dict, List, Union, cast
 
-from polywrap_core import Uri, UriPackageOrWrapper, WrapPackage
+from polywrap_core import Uri, WrapPackage
 
-from ..types import ClientConfigBuilder
+from ..types import BuilderConfig, ClientConfigBuilder
 
 
-class PackageConfigure(ClientConfigBuilder):
+class PackageConfigure:
     """Allows configuring the WRAP packages."""
 
-    def get_package(self, uri: Uri) -> Union[WrapPackage[UriPackageOrWrapper], None]:
+    config: BuilderConfig
+
+    def get_package(self, uri: Uri) -> Union[WrapPackage, None]:
         """Return the package for the given uri."""
         return self.config.packages.get(uri)
 
-    def get_packages(self) -> Dict[Uri, WrapPackage[UriPackageOrWrapper]]:
+    def get_packages(self) -> Dict[Uri, WrapPackage]:
         """Return the packages from the builder's config."""
         return self.config.packages
 
-    def set_package(
-        self, uri: Uri, package: WrapPackage[UriPackageOrWrapper]
-    ) -> ClientConfigBuilder:
+    def set_package(self, uri: Uri, package: WrapPackage) -> ClientConfigBuilder:
         """Set the package by uri in the builder's config, overiding any existing values."""
         self.config.packages[uri] = package
-        return self
+        return cast(ClientConfigBuilder, self)
 
-    def set_packages(
-        self, uri_packages: Dict[Uri, WrapPackage[UriPackageOrWrapper]]
-    ) -> ClientConfigBuilder:
+    def set_packages(self, uri_packages: Dict[Uri, WrapPackage]) -> ClientConfigBuilder:
         """Set the packages in the builder's config, overiding any existing values."""
         self.config.packages.update(uri_packages)
-        return self
+        return cast(ClientConfigBuilder, self)
 
     def remove_package(self, uri: Uri) -> ClientConfigBuilder:
         """Remove the package for the given uri."""
         self.config.packages.pop(uri, None)
-        return self
+        return cast(ClientConfigBuilder, self)
 
     def remove_packages(self, uris: List[Uri]) -> ClientConfigBuilder:
         """Remove the packages for the given uris."""
         for uri in uris:
             self.remove_package(uri)
-        return self
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/redirect_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/wrapper_configure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-"""This module contains the redirect configure class for the client config builder."""
-from typing import Dict, List, Union
+"""This module contains the wrapper configure class for the client config builder."""
+from typing import Dict, List, Union, cast
 
-from polywrap_core import Uri
+from polywrap_core import Uri, Wrapper
 
-from ..types import ClientConfigBuilder
+from ..types import BuilderConfig, ClientConfigBuilder
 
 
-class RedirectConfigure(ClientConfigBuilder):
-    """Allows configuring the URI redirects."""
+class WrapperConfigure:
+    """Allows configuring the wrappers."""
 
-    def get_redirect(self, uri: Uri) -> Union[Uri, None]:
-        """Return the redirect for the given uri."""
-        return self.config.redirects.get(uri)
+    config: BuilderConfig
 
-    def get_redirects(self) -> Dict[Uri, Uri]:
-        """Return the redirects from the builder's config."""
-        return self.config.redirects
+    def get_wrapper(self, uri: Uri) -> Union[Wrapper, None]:
+        """Return the set wrapper for the given uri."""
+        return self.config.wrappers.get(uri)
 
-    def set_redirect(self, from_uri: Uri, to_uri: Uri) -> ClientConfigBuilder:
-        """Set the redirect from a URI to another URI in the builder's config,\
-            overiding any existing values."""
-        self.config.redirects[from_uri] = to_uri
-        return self
+    def get_wrappers(self) -> Dict[Uri, Wrapper]:
+        """Return the wrappers from the builder's config."""
+        return self.config.wrappers
 
-    def set_redirects(self, uri_redirects: Dict[Uri, Uri]) -> ClientConfigBuilder:
-        """Set the redirects in the builder's config, overiding any existing values."""
-        self.config.redirects.update(uri_redirects)
-        return self
+    def set_wrapper(self, uri: Uri, wrapper: Wrapper) -> ClientConfigBuilder:
+        """Set the wrapper by uri in the builder's config, overiding any existing values."""
+        self.config.wrappers[uri] = wrapper
+        return cast(ClientConfigBuilder, self)
 
-    def remove_redirect(self, uri: Uri) -> ClientConfigBuilder:
-        """Remove the redirect for the given uri."""
-        self.config.redirects.pop(uri, None)
-        return self
+    def set_wrappers(self, uri_wrappers: Dict[Uri, Wrapper]) -> ClientConfigBuilder:
+        """Set the wrappers in the builder's config, overiding any existing values."""
+        self.config.wrappers.update(uri_wrappers)
+        return cast(ClientConfigBuilder, self)
 
-    def remove_redirects(self, uris: List[Uri]) -> ClientConfigBuilder:
-        """Remove the redirects for the given uris."""
+    def remove_wrapper(self, uri: Uri) -> ClientConfigBuilder:
+        """Remove the wrapper for the given uri."""
+        self.config.wrappers.pop(uri, None)
+        return cast(ClientConfigBuilder, self)
+
+    def remove_wrappers(self, uris: List[Uri]) -> ClientConfigBuilder:
+        """Remove the wrappers for the given uris."""
         for uri in uris:
-            self.remove_redirect(uri)
-        return self
+            self.remove_wrapper(uri)
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/resolver_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/resolver_configure.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """This module contains the resolver configure class for the client config builder."""
-from typing import List
+from typing import List, cast
 
 from polywrap_core import UriResolver
 
-from ..types import ClientConfigBuilder
+from ..types import BuilderConfig, ClientConfigBuilder
 
 
-class ResolverConfigure(ClientConfigBuilder):
+class ResolverConfigure:
     """Allows configuring the URI resolvers."""
 
+    config: BuilderConfig
+
     def get_resolvers(self) -> List[UriResolver]:
         """Return the resolvers from the builder's config."""
         return self.config.resolvers
 
     def add_resolver(self, resolver: UriResolver) -> ClientConfigBuilder:
         """Add a resolver to the builder's config."""
         self.config.resolvers.append(resolver)
-        return self
+        return cast(ClientConfigBuilder, self)
 
     def add_resolvers(self, resolvers_list: List[UriResolver]) -> ClientConfigBuilder:
         """Add a list of resolvers to the builder's config."""
         for resolver in resolvers_list:
             self.add_resolver(resolver)
-        return self
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/wrapper_configure.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/configures/redirect_configure.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-"""This module contains the wrapper configure class for the client config builder."""
-from typing import Dict, List, Union
+"""This module contains the redirect configure class for the client config builder."""
+from typing import Dict, List, Union, cast
 
-from polywrap_core import Uri, UriPackageOrWrapper, Wrapper
+from polywrap_core import Uri
 
-from ..types import ClientConfigBuilder
+from ..types import BuilderConfig, ClientConfigBuilder
 
 
-class WrapperConfigure(ClientConfigBuilder):
-    """Allows configuring the wrappers."""
-
-    def get_wrapper(self, uri: Uri) -> Union[Wrapper[UriPackageOrWrapper], None]:
-        """Return the set wrapper for the given uri."""
-        return self.config.wrappers.get(uri)
-
-    def get_wrappers(self) -> Dict[Uri, Wrapper[UriPackageOrWrapper]]:
-        """Return the wrappers from the builder's config."""
-        return self.config.wrappers
-
-    def set_wrapper(
-        self, uri: Uri, wrapper: Wrapper[UriPackageOrWrapper]
-    ) -> ClientConfigBuilder:
-        """Set the wrapper by uri in the builder's config, overiding any existing values."""
-        self.config.wrappers[uri] = wrapper
-        return self
-
-    def set_wrappers(
-        self, uri_wrappers: Dict[Uri, Wrapper[UriPackageOrWrapper]]
-    ) -> ClientConfigBuilder:
-        """Set the wrappers in the builder's config, overiding any existing values."""
-        self.config.wrappers.update(uri_wrappers)
-        return self
-
-    def remove_wrapper(self, uri: Uri) -> ClientConfigBuilder:
-        """Remove the wrapper for the given uri."""
-        self.config.wrappers.pop(uri, None)
-        return self
+class RedirectConfigure:
+    """Allows configuring the URI redirects."""
 
-    def remove_wrappers(self, uris: List[Uri]) -> ClientConfigBuilder:
-        """Remove the wrappers for the given uris."""
+    config: BuilderConfig
+
+    def get_redirect(self, uri: Uri) -> Union[Uri, None]:
+        """Return the redirect for the given uri."""
+        return self.config.redirects.get(uri)
+
+    def get_redirects(self) -> Dict[Uri, Uri]:
+        """Return the redirects from the builder's config."""
+        return self.config.redirects
+
+    def set_redirect(self, from_uri: Uri, to_uri: Uri) -> ClientConfigBuilder:
+        """Set the redirect from a URI to another URI in the builder's config,\
+            overiding any existing values."""
+        self.config.redirects[from_uri] = to_uri
+        return cast(ClientConfigBuilder, self)
+
+    def set_redirects(self, uri_redirects: Dict[Uri, Uri]) -> ClientConfigBuilder:
+        """Set the redirects in the builder's config, overiding any existing values."""
+        self.config.redirects.update(uri_redirects)
+        return cast(ClientConfigBuilder, self)
+
+    def remove_redirect(self, uri: Uri) -> ClientConfigBuilder:
+        """Remove the redirect for the given uri."""
+        self.config.redirects.pop(uri, None)
+        return cast(ClientConfigBuilder, self)
+
+    def remove_redirects(self, uris: List[Uri]) -> ClientConfigBuilder:
+        """Remove the redirects for the given uris."""
         for uri in uris:
-            self.remove_wrapper(uri)
-        return self
+            self.remove_redirect(uri)
+        return cast(ClientConfigBuilder, self)
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/build_options.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/build_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """This module contains the BuildOptions class."""
 from dataclasses import dataclass
 from typing import Optional
 
 from polywrap_core import UriResolver
-from polywrap_uri_resolvers import WrapperCache
+from polywrap_uri_resolvers import ResolutionResultCache
 
 
 @dataclass(slots=True, kw_only=True)
 class BuildOptions:
     """BuildOptions defines the options for build method of the client config builder.
 
-    Attributes:
-        wrapper_cache: The wrapper cache.
+    Args:
+        resolution_result_cache: The Resolution Result Cache.
         resolver: The URI resolver.
     """
 
-    wrapper_cache: Optional[WrapperCache] = None
+    resolution_result_cache: Optional[ResolutionResultCache] = None
     resolver: Optional[UriResolver] = None
+
+
+__all__ = ["BuildOptions"]
```

### Comparing `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/client_config_builder.py` & `polywrap_client_config_builder-0.1.0a30/polywrap_client_config_builder/types/client_config_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,195 +1,183 @@
 """This module contains the client config builder class."""
 # pylint: disable=too-many-public-methods
-from abc import ABC, abstractmethod
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Protocol, Union
 
-from polywrap_core import (
-    ClientConfig,
-    Env,
-    Uri,
-    UriPackageOrWrapper,
-    UriResolver,
-    WrapPackage,
-    Wrapper,
-)
+from polywrap_core import ClientConfig, Uri, UriResolver, WrapPackage, Wrapper
 
 from .build_options import BuildOptions
 from .builder_config import BuilderConfig
 
 
-class ClientConfigBuilder(ABC):
+class ClientConfigBuilder(Protocol):
     """Defines the interface for the client config builder."""
 
     config: BuilderConfig
 
-    @abstractmethod
     def build(self, options: Optional[BuildOptions] = None) -> ClientConfig:
         """Build the ClientConfig object from the builder's config."""
+        ...
 
-    @abstractmethod
     def add(self, config: BuilderConfig) -> "ClientConfigBuilder":
         """Add the values from the given config to the builder's config."""
+        ...
 
     # ENV CONFIGURE
 
-    @abstractmethod
-    def get_env(self, uri: Uri) -> Union[Env, None]:
+    def get_env(self, uri: Uri) -> Union[Any, None]:
         """Return the env for the given uri."""
+        ...
 
-    @abstractmethod
-    def get_envs(self) -> Dict[Uri, Env]:
+    def get_envs(self) -> Dict[Uri, Any]:
         """Return the envs from the builder's config."""
+        ...
 
-    @abstractmethod
-    def set_env(self, uri: Uri, env: Env) -> "ClientConfigBuilder":
+    def set_env(self, uri: Uri, env: Any) -> "ClientConfigBuilder":
         """Set the env by uri in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
-    def set_envs(self, uri_envs: Dict[Uri, Env]) -> "ClientConfigBuilder":
+    def set_envs(self, uri_envs: Dict[Uri, Any]) -> "ClientConfigBuilder":
         """Set the envs in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
-    def add_env(self, uri: Uri, env: Env) -> "ClientConfigBuilder":
+    def add_env(self, uri: Uri, env: Any) -> "ClientConfigBuilder":
         """Add an env for the given uri.
 
-        If an Env is already associated with the uri, it is modified.
+        If an Any is already associated with the uri, it is modified.
         """
+        ...
 
-    @abstractmethod
-    def add_envs(self, uri_envs: Dict[Uri, Env]) -> "ClientConfigBuilder":
+    def add_envs(self, uri_envs: Dict[Uri, Any]) -> "ClientConfigBuilder":
         """Add a list of envs to the builder's config."""
+        ...
 
-    @abstractmethod
     def remove_env(self, uri: Uri) -> "ClientConfigBuilder":
         """Remove the env for the given uri."""
+        ...
 
-    @abstractmethod
     def remove_envs(self, uris: List[Uri]) -> "ClientConfigBuilder":
         """Remove the envs for the given uris."""
+        ...
 
     # INTERFACE IMPLEMENTATIONS CONFIGURE
 
-    @abstractmethod
     def get_interfaces(self) -> Dict[Uri, List[Uri]]:
         """Return all registered interface and its implementations from the builder's config."""
+        ...
 
-    @abstractmethod
     def get_interface_implementations(self, uri: Uri) -> Union[List[Uri], None]:
         """Return the interface for the given uri."""
+        ...
 
-    @abstractmethod
     def add_interface_implementations(
         self, interface_uri: Uri, implementations_uris: List[Uri]
     ) -> "ClientConfigBuilder":
         """Add a list of implementation URIs for the given interface URI to the builder's config."""
+        ...
 
-    @abstractmethod
     def remove_interface_implementations(
         self, interface_uri: Uri, implementations_uris: List[Uri]
     ) -> "ClientConfigBuilder":
         """Remove the implementations for the given interface uri."""
+        ...
 
-    @abstractmethod
     def remove_interface(self, interface_uri: Uri) -> "ClientConfigBuilder":
         """Remove the interface for the given uri."""
+        ...
 
     # PACKAGE CONFIGURE
 
-    @abstractmethod
-    def get_package(self, uri: Uri) -> Union[WrapPackage[UriPackageOrWrapper], None]:
+    def get_package(self, uri: Uri) -> Union[WrapPackage, None]:
         """Return the package for the given uri."""
+        ...
 
-    @abstractmethod
-    def get_packages(self) -> Dict[Uri, WrapPackage[UriPackageOrWrapper]]:
+    def get_packages(self) -> Dict[Uri, WrapPackage]:
         """Return the packages from the builder's config."""
+        ...
 
-    @abstractmethod
-    def set_package(
-        self, uri: Uri, package: WrapPackage[UriPackageOrWrapper]
-    ) -> "ClientConfigBuilder":
+    def set_package(self, uri: Uri, package: WrapPackage) -> "ClientConfigBuilder":
         """Set the package by uri in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
     def set_packages(
-        self, uri_packages: Dict[Uri, WrapPackage[UriPackageOrWrapper]]
+        self, uri_packages: Dict[Uri, WrapPackage]
     ) -> "ClientConfigBuilder":
         """Set the packages in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
     def remove_package(self, uri: Uri) -> "ClientConfigBuilder":
         """Remove the package for the given uri."""
+        ...
 
-    @abstractmethod
     def remove_packages(self, uris: List[Uri]) -> "ClientConfigBuilder":
         """Remove the packages for the given uris."""
+        ...
 
     # REDIRECT CONFIGURE
 
-    @abstractmethod
     def get_redirect(self, uri: Uri) -> Union[Uri, None]:
         """Return the redirect for the given uri."""
+        ...
 
-    @abstractmethod
     def get_redirects(self) -> Dict[Uri, Uri]:
         """Return the redirects from the builder's config."""
+        ...
 
-    @abstractmethod
     def set_redirect(self, from_uri: Uri, to_uri: Uri) -> "ClientConfigBuilder":
         """Set the redirect from a URI to another URI in the builder's config,\
             overiding any existing values."""
+        ...
 
-    @abstractmethod
     def set_redirects(self, uri_redirects: Dict[Uri, Uri]) -> "ClientConfigBuilder":
         """Set the redirects in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
     def remove_redirect(self, uri: Uri) -> "ClientConfigBuilder":
         """Remove the redirect for the given uri."""
+        ...
 
-    @abstractmethod
     def remove_redirects(self, uris: List[Uri]) -> "ClientConfigBuilder":
         """Remove the redirects for the given uris."""
+        ...
 
     # RESOLVER CONFIGURE
 
-    @abstractmethod
     def get_resolvers(self) -> List[UriResolver]:
         """Return the resolvers from the builder's config."""
+        ...
 
-    @abstractmethod
     def add_resolver(self, resolver: UriResolver) -> "ClientConfigBuilder":
         """Add a resolver to the builder's config."""
+        ...
 
-    @abstractmethod
     def add_resolvers(self, resolvers_list: List[UriResolver]) -> "ClientConfigBuilder":
         """Add a list of resolvers to the builder's config."""
+        ...
 
     # WRAPPER CONFIGURE
 
-    @abstractmethod
-    def get_wrapper(self, uri: Uri) -> Union[Wrapper[UriPackageOrWrapper], None]:
+    def get_wrapper(self, uri: Uri) -> Union[Wrapper, None]:
         """Return the set wrapper for the given uri."""
+        ...
 
-    @abstractmethod
-    def get_wrappers(self) -> Dict[Uri, Wrapper[UriPackageOrWrapper]]:
+    def get_wrappers(self) -> Dict[Uri, Wrapper]:
         """Return the wrappers from the builder's config."""
+        ...
 
-    @abstractmethod
-    def set_wrapper(
-        self, uri: Uri, wrapper: Wrapper[UriPackageOrWrapper]
-    ) -> "ClientConfigBuilder":
+    def set_wrapper(self, uri: Uri, wrapper: Wrapper) -> "ClientConfigBuilder":
         """Set the wrapper by uri in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
-    def set_wrappers(
-        self, uri_wrappers: Dict[Uri, Wrapper[UriPackageOrWrapper]]
-    ) -> "ClientConfigBuilder":
+    def set_wrappers(self, uri_wrappers: Dict[Uri, Wrapper]) -> "ClientConfigBuilder":
         """Set the wrappers in the builder's config, overiding any existing values."""
+        ...
 
-    @abstractmethod
     def remove_wrapper(self, uri: Uri) -> "ClientConfigBuilder":
         """Remove the wrapper for the given uri."""
+        ...
 
-    @abstractmethod
     def remove_wrappers(self, uris: List[Uri]) -> "ClientConfigBuilder":
         """Remove the wrappers for the given uris."""
+        ...
+
+
+__all__ = ["ClientConfigBuilder"]
```

### Comparing `polywrap_client_config_builder-0.1.0a29/pyproject.toml` & `polywrap_client_config_builder-0.1.0a30/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client-config-builder"
-version = "0.1.0a29"
+version = "0.1.0a30"
 description = ""
 authors = ["Media <media@polywrap.io>", "Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-uri-resolvers = "^0.1.0a29"
-polywrap-core = "^0.1.0a29"
+polywrap-uri-resolvers = "^0.1.0a30"
+polywrap-core = "^0.1.0a30"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
 
+[tool.poetry.group.dev.dependencies]
+hypothesis = "^6.76.0"
+
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
 
 [tool.pyright]
@@ -38,15 +41,16 @@
 asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
-
+    "unnecessary-ellipsis",
+    "too-few-public-methods"
 ]
 ignore = [
     "tests/"
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `polywrap_client_config_builder-0.1.0a29/PKG-INFO` & `polywrap_client_config_builder-0.1.0a30/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-client-config-builder
-Version: 0.1.0a29
+Version: 0.1.0a30
 Summary: 
 Author: Media
 Author-email: media@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0a29,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0a29,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0a30,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0a30,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-client-config-builder
 
 A utility class for building the PolywrapClient config. 
 
 Supports building configs using method chaining or imperatively.
@@ -64,16 +64,16 @@
 
 ```python
 # accepted by the PolywrapClient
 config = builder.build()
 
 # build with a custom cache
 config = builder.build({
-  wrapperCache: WrapperCache(),
+  resolution_result_cache: ResolutionResultCache(),
 })
 
 # or build with a custom resolver
-coreClientConfig = builder.build({
+config = builder.build({
   resolver: RecursiveResolver(...),
 })
 ```
```

