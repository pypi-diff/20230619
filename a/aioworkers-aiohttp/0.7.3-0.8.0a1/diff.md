# Comparing `tmp/aioworkers-aiohttp-0.7.3.tar.gz` & `tmp/aioworkers_aiohttp-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworkers-aiohttp-0.7.3.tar", last modified: Tue May  4 21:51:00 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioworkers-aiohttp-0.7.3.tar` & `aioworkers_aiohttp-0.8.0a1.tar`

### file list

```diff
@@ -1,22 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 21:51:00.729369 aioworkers-aiohttp-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2021-05-04 21:51:00.729369 aioworkers-aiohttp-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 21:51:00.729369 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/
--rw-r--r--   0 runner    (1001) docker     (121)      931 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5445 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/plugin.ini
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/router.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-04 21:50:59.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 21:51:00.729369 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2021-05-04 21:51:00.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-05-04 21:51:00.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 21:51:00.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-05-04 21:51:00.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-05-04 21:51:00.000000 aioworkers-aiohttp-0.7.3/aioworkers_aiohttp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-05-04 21:51:00.729369 aioworkers-aiohttp-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-05-04 21:50:47.000000 aioworkers-aiohttp-0.7.3/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/abc.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/app.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/plugin.ini
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/router.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/server.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/storage.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/supervisor.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/LICENSE
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/README.rst
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 aioworkers_aiohttp-0.8.0a1/PKG-INFO
```

### Comparing `aioworkers-aiohttp-0.7.3/README.rst` & `aioworkers_aiohttp-0.8.0a1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 aioworkers-aiohttp
 ==================
 
 The package to integration aioworkers with aiohttp
 
+.. image:: https://img.shields.io/pypi/v/aioworkers-aiohttp.svg
+  :target: https://pypi.org/project/aioworkers-aiohttp
+
 .. image:: https://github.com/aioworkers/aioworkers-aiohttp/workflows/Tests/badge.svg
   :target: https://github.com/aioworkers/aioworkers-aiohttp/actions?query=workflow%3ATests
 
 .. image:: https://codecov.io/gh/aioworkers/aioworkers-aiohttp/branch/master/graph/badge.svg
   :target: https://codecov.io/gh/aioworkers/aioworkers-aiohttp
+  :alt: Coverage
 
-.. image:: https://img.shields.io/pypi/v/aioworkers-aiohttp.svg
-  :target: https://pypi.org/project/aioworkers-aiohttp
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json
+  :target: https://github.com/charliermarsh/ruff
+  :alt: Code style: ruff
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+  :target: https://github.com/psf/black
+  :alt: Code style: black
+
+.. image:: https://img.shields.io/badge/types-Mypy-blue.svg
+  :target: https://github.com/python/mypy
+  :alt: Code style: Mypy
 
 .. image:: https://readthedocs.org/projects/aioworkers-aiohttp/badge/?version=latest
-  :target: http://aioworkers-aiohttp.readthedocs.io/en/latest/?badge=latest
+  :target: https://github.com/aioworkers/aioworkers-aiohttp#readme
   :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/pyversions/aioworkers-aiohttp.svg
   :target: https://pypi.org/project/aioworkers-aiohttp
+  :alt: Python versions
+
+.. image:: https://img.shields.io/pypi/dm/aioworkers-aiohttp.svg
+  :target: https://pypi.org/project/aioworkers-aiohttp
+
+.. image:: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
+  :alt: Hatch project
+  :target: https://github.com/pypa/hatch
 
 
 Features
 --------
 
 - Building of the routing from config like swagger
 - Start aiohttp project with multiprocessing mode
@@ -62,12 +83,38 @@
               responses:
                 200:
                   description: OK
                 400:
                   description: Validation error
                 404:
                   description: Not found
-  logging:
-    version: 1
-    formatters:
-      access:
-        format: %a %t "%r" %s %b "%{Referer}i" "%{User-Agent}i"
+
+
+Development
+-----------
+
+Check code:
+
+.. code-block:: shell
+
+    hatch run lint:all
+
+
+Format code:
+
+.. code-block:: shell
+
+    hatch run lint:fmt
+
+
+Run tests:
+
+.. code-block:: shell
+
+    hatch run pytest
+
+
+Run tests with coverage:
+
+.. code-block:: shell
+
+    hatch run cov
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/__init__.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,21 @@
 from typing import Dict, Iterable, Tuple
 
 from aioworkers.core.plugin import Plugin
 
 from .server import WebServer
 
 
-try:
-    from .version import __version__
-except ImportError:
-    __version__ = 'dev'
+__version__ = "0.8.0a1"
 
 BASE = Path(__file__).parent
 
 
 class plugin(Plugin):
-    configs = (
-        BASE / 'plugin.ini',
-    )
+    configs = (BASE / "plugin.ini",)
 
     def __init__(self):
         super().__init__()
         self._config = {}
 
     def get_config(self) -> Dict:
         return self._config
@@ -30,13 +25,14 @@
     def add_arguments(self, parser: argparse.ArgumentParser):
         try:
             parser.add_argument('--port', type=int)
         except argparse.ArgumentError:
             pass
 
     def parse_known_args(
-        self, args: Iterable[str],
+        self,
+        args: Iterable[str],
         namespace: argparse.Namespace,
     ) -> Tuple[argparse.Namespace, Iterable[str]]:
         if namespace.port:
             WebServer.set_port(namespace.port)
         return namespace, args
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/app.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,71 @@
-from collections import Mapping
+from typing import Mapping, Optional
 
+import aiohttp
 from aiohttp import web
 from aioworkers.humanize import parse_size
 from aioworkers.utils import import_name
 
-from .abc import AbstractSwaggerRouter
+from .abc import AbstractSwaggerRouter, PRouter
+
+
+AIOHTTP_MAJOR_VERSION = int(aiohttp.__version__.split(".")[0])
 
 
 class Application(web.Application):
     def __init__(self, config, *, context, **kwargs):
         self.config = config
         self.context = context
+        self._custom_router: Optional[PRouter] = None
+        self._router_setup = AIOHTTP_MAJOR_VERSION > 3
         cors = None
 
+        kwargs = {}
         debug = config.get('debug')
         if isinstance(debug, bool):
             kwargs.setdefault('debug', debug)
 
         if 'client_max_size' in config:
             kwargs['client_max_size'] = parse_size(config.client_max_size)
 
         if not config.get('router'):
             pass
         elif isinstance(config.router, str):
             cls = import_name(config.router)
-            kwargs['router'] = cls()
+            self._custom_router = cls()
         else:
             cfg = dict(config.router)
             cls = import_name(cfg.pop('cls'))
+            self._router_setup |= cfg.pop("setup", self._router_setup)
             cors = cfg.pop('cors', None)
-            kwargs['router'] = cls(**cfg)
+            self._custom_router = cls(**cfg)
+
+        if self._custom_router is not None and not self._router_setup:
+            kwargs['router'] = self._custom_router
 
         if not config.get('middlewares'):
             pass
         elif isinstance(config.middlewares, list):
             kwargs['middlewares'] = map(
-                self.context.get_object, config.middlewares,
+                self.context.get_object,
+                config.middlewares,
             )
         else:
             raise TypeError('Middlewares should be described in list')
 
         super().__init__(**kwargs)
 
-        if cors is not None:
-            kwargs['router'].set_cors(self, **cors)
+        if self._custom_router is not None and cors is not None:
+            self._custom_router.set_cors(self, **cors)
 
         for signal in (
-            'on_startup', 'cleanup_ctx',
-            'on_cleanup', 'on_response_prepare',
+            "on_startup",
+            "cleanup_ctx",
+            "on_cleanup",
+            "on_response_prepare",
         ):
             sigs = config.get(signal)
             signals = getattr(self, signal, None)
             if sigs and signals is not None:
                 for _, s in sorted(sigs.items(), key=lambda x: x[0]):
                     coro = self.context.get_object(s)
                     signals.append(coro)
@@ -60,63 +74,71 @@
         for routes_line in self.config.get('routes') or ():
             routes = self.context.get_object(routes_line)
             if isinstance(routes, web.AbstractRouteDef):
                 self.add_routes([routes])
             else:
                 self.add_routes(routes)
         resources = self.config.get('resources')
-        is_swagger = isinstance(self.router, AbstractSwaggerRouter)
+        is_swagger = isinstance(self._custom_router, AbstractSwaggerRouter)
         default_validate = self.config.get('router.default_validate', True)
         for url, name, routes in sort_resources(resources):
             if 'include' in routes:
-                self.router.include(**routes)
+                self._custom_router.include(**routes)  # type: ignore
                 continue
             if 'static' in routes:
                 static_params = routes.pop('static')
                 if isinstance(static_params, Mapping):
                     kwargs = static_params
                 else:
                     kwargs = {'path': static_params}
                 self.router.add_static(url, **kwargs)
-            resource = self.router.add_resource(url, name=name)
+            if self._custom_router is not None:
+                resource = self._custom_router.add_resource(url, name=name)
+            else:
+                resource = self.router.add_resource(url, name=name)
             for method, operation in routes.items():
                 if not isinstance(operation, Mapping):
                     raise TypeError(
                         'operation for {method} {url} expected Mapping, '
                         'not {t}'.format(
-                            method=method.upper(), url=url, t=type(operation),
+                            method=method.upper(),
+                            url=url,
+                            t=type(operation),
                         )
                     )
                 operation = dict(operation)
                 handler = operation.pop('handler')
                 validate = operation.pop('validate', default_validate)
                 if not is_swagger or handler.startswith('.'):
                     handler = self.context.get_object(handler)
                 if is_swagger:
                     resource.add_route(
-                        method.upper(), handler,
-                        swagger_data=operation, validate=validate,
+                        method.upper(),
+                        handler,
+                        swagger_data=operation,  # type: ignore
+                        validate=validate,  # type: ignore
                     )
                 else:
                     resource.add_route(method.upper(), handler)
 
+        if self._router_setup and self._custom_router is not None:
+            self._custom_router.setup(self)
+
 
 def iter_resources(resources, prefix=''):
     if not resources:
         return
     elif not isinstance(resources, Mapping):
-        raise TypeError(
-            'Resources should be described in dict %s' % resources)
+        raise TypeError("Resources should be described in dict %s" % resources)
     prefix += resources.get('prefix', '')
     for name, sub in resources.items():
         if name == 'prefix':
             continue
         elif not isinstance(sub, Mapping):
-            raise TypeError(
-                'Resource should be described in dict %s' % sub)
+            raise TypeError("Resource should be described in dict %s" % sub)
         routes = dict(sub)
         priority = routes.pop('priority', 0)
         if 'include' in routes:
             url = name if name.startswith('/') else None
             if url:
                 url = prefix + url
             else:
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/router.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/router.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,9 @@
     def __init__(self, search_in_modules=(), search_dirs=(), **kwargs):
         modules = map(import_name, search_in_modules)
         dirs = [Path(x.__file__).parent for x in modules]
         dirs.extend(search_dirs)
         kwargs['search_dirs'] = dirs
         super().__init__(**kwargs)
 
-    def include(self, include, *,
-                prefix=None,
-                mapping=None,
-                name=None):
-
-        return super().include(
-            include, basePath=prefix,
-            operationId_mapping=mapping,
-            name=name)
+    def include(self, include, *, prefix=None, mapping=None, name=None):
+        return super().include(include, basePath=prefix, operationId_mapping=mapping, name=name)
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/server.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+import socket
+from typing import List
+
 from aiohttp import web
 from aioworkers.net.server import SocketServer
 from aioworkers.utils import import_name
 
 
 class WebServer(SocketServer):
     port = None
+    _sockets: List[socket.socket]
 
     @classmethod
     def set_port(cls, port: int) -> None:
         cls.port = port
 
     def __init__(self, *args, **kwargs):
         self._runner = None
@@ -44,8 +48,9 @@
     async def start(self):
         self._runner = web.AppRunner(self.context.app, **self._kwargs)
         await self._runner.setup()
         for sock in self._sockets:
             await web.SockSite(self._runner, sock).start()
 
     async def stop(self):
+        assert self._runner
         await self._runner.cleanup()
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/storage.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import json
 import logging
-from collections import Mapping, Sequence
+from typing import Mapping, Sequence
 
 from aiohttp import ClientOSError, client
 from aioworkers.storage import StorageError, base
 from yarl import URL
 
 
 class RoStorage(base.AbstractStorageReadOnly):
-    """ ReadOnly storage over http GET
+    """ReadOnly storage over http GET
     config:
         semaphore: int
         allow_hosts: list
         return_status: bool, method get returns tuple (CODE, VALUE)
         prefix: url prefix
         headers: Mapping or None
         template: url template
@@ -22,16 +22,15 @@
 
     async def init(self):
         await super().init()
         self._prefix = self.config.get('prefix')
         self._template = self.config.get('template')
         if self._prefix:
             self._prefix = URL(self._prefix)
-        self._semaphore = asyncio.Semaphore(
-            self.config.get('semaphore', 20), loop=self.loop)
+        self._semaphore = asyncio.Semaphore(self.config.get("semaphore", 20))
         self._allow_hosts = self.config.get('allow_hosts')
         self._format = self.config.get('format', 'json')
         self._return_status = self.config.get('return_status', False)
 
         headers = self.config.get('headers')
         self.session_params = {}
         if headers:
@@ -46,15 +45,15 @@
         session = getattr(self, 'session', None)
         if session:
             asyncio.ensure_future(session.close(), loop=self.loop)
         if kwargs:
             kwargs = {**self.session_params, **kwargs}
         else:
             kwargs = self.session_params
-        self.session = client.ClientSession(loop=self.loop, **kwargs)
+        self.session = client.ClientSession(**kwargs)
 
     async def cleanup_session(self):
         await self.session.close()
 
     def raw_key(self, key):
         if self._prefix:
             if isinstance(key, str):
@@ -105,43 +104,45 @@
         return data
 
     def get(self, key):
         url = self.raw_key(key)
         return self.request(url)
 
     async def copy(self, key_source, storage_dest, key_dest):
-        """ Return True if data are copied
+        """Return True if data are copied
         * optimized for http->fs copy
         * not supported return_status
         """
         from aioworkers.storage.filesystem import FileSystemStorage
+
         if not isinstance(storage_dest, FileSystemStorage):
-            return super().copy(key_source, storage_dest, key_dest)
+            return super().copy(key_source, storage_dest, key_dest)  # type: ignore
         url = self.raw_key(key_source)
         logger = self.context.logger
         async with self._semaphore:
             async with self.session.get(url) as response:
                 if response.status == 404:
                     return
                 elif response.status >= 400:
                     if logger.getEffectiveLevel() == logging.DEBUG:
                         logger.debug(
-                            'HttpStorage request to %s '
-                            'returned code %s:\n%s' % (
-                                url, response.status,
-                                (await response.read()).decode()))
+                            "HttpStorage request to %s returned code %s: %s",
+                            url,
+                            response.status,
+                            await response.text(),
+                        )
                     return
                 async with storage_dest.raw_key(key_dest).open('wb') as f:
                     async for chunk in response.content.iter_any():
                         await f.write(chunk)
                     return True
 
 
 class Storage(RoStorage, base.AbstractStorageWriteOnly):
-    """ RW storage over http
+    """RW storage over http
     config:
         semaphore: int
         allow_hosts: list
         return_status: bool, method get returns tuple (CODE, VALUE)
         prefix: url prefix
         template: url template
         headers: Mapping or None
@@ -159,10 +160,8 @@
                 dumps = json.dumps
             data = dumps(value)
             headers = {'content-type': 'application/json'}
         else:
             data = value
             headers = {}
 
-        return self.request(
-            url, method=self.config.get('set', 'post'),
-            data=data, headers=headers)
+        return self.request(url, method=self.config.get("set", "post"), data=data, headers=headers)
```

### Comparing `aioworkers-aiohttp-0.7.3/aioworkers_aiohttp/supervisor.py` & `aioworkers_aiohttp-0.8.0a1/aioworkers_aiohttp/supervisor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import Mapping
+from typing import Mapping
 
 from aioworkers import utils
 from aioworkers.worker import subprocess, supervisor
 
 
 class Supervisor(supervisor.Supervisor):
     def __init__(self, *args, **kwargs):
@@ -23,16 +23,16 @@
             last_port = next(p, last_port)
         elif isinstance(ports, int):
             first_port = ports
         else:
             raise ValueError('Error value for ports {}'.format(ports))
         return iter(range(first_port, last_port))
 
-    def get_child_config(self):
-        c = super().get_child_config()
+    def get_child_config(self, *args, **kwargs):
+        c = super().get_child_config(*args, **kwargs)
         params = c.get('params') or {}
         if params:
             params = dict(params)
         params['port'] = next(self._iterport)
         cls = c.get('cls') or utils.import_uri(subprocess.Subprocess)
         c = c.new_child(params=params, daemon=True, cls=cls)
         return c
```

