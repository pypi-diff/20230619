# Comparing `tmp/socketapp-0.1.4.tar.gz` & `tmp/socketapp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketapp-0.1.4.tar", max compression
+gzip compressed data, was "socketapp-0.1.5.tar", max compression
```

## Comparing `socketapp-0.1.4.tar` & `socketapp-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1211 2023-01-12 19:34:28.680149 socketapp-0.1.4/LICENSE
--rw-r--r--   0        0        0       79 2023-01-12 19:34:28.680149 socketapp-0.1.4/README.md
--rw-r--r--   0        0        0      683 2023-01-12 19:34:39.688242 socketapp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      120 2023-01-12 19:34:28.684149 socketapp-0.1.4/socketapp/__init__.py
--rw-r--r--   0        0        0     2871 2023-01-12 19:34:28.684149 socketapp-0.1.4/socketapp/client.py
--rw-r--r--   0        0        0     1170 2023-01-12 19:34:28.684149 socketapp-0.1.4/socketapp/event.py
--rw-r--r--   0        0        0     3705 2023-01-12 19:34:28.684149 socketapp-0.1.4/socketapp/server.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 socketapp-0.1.4/setup.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 socketapp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-19 16:18:04.689263 socketapp-0.1.5/LICENSE
+-rw-r--r--   0        0        0       79 2023-06-19 16:18:04.689263 socketapp-0.1.5/README.md
+-rw-r--r--   0        0        0      681 2023-06-19 16:18:21.037644 socketapp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/__init__.py
+-rw-r--r--   0        0        0     2871 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/client.py
+-rw-r--r--   0        0        0     1141 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/event.py
+-rw-r--r--   0        0        0     3705 2023-06-19 16:18:04.689263 socketapp-0.1.5/socketapp/server.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 socketapp-0.1.5/PKG-INFO
```

### Comparing `socketapp-0.1.4/LICENSE` & `socketapp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `socketapp-0.1.4/pyproject.toml` & `socketapp-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "socketapp"
-version = "v0.1.4"
+version = "v0.1.5"
 description = "An opinionated library for creating websocket-based applications."
 authors = ["CircuitSacul <circuitsacul@gmail.com>"]
 license = "Unlicense"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-websockets = "^10.4"
-pydantic = "^1.10.2"
+websockets = "^11.0"
+pydantic = "^1.10.9"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.168"
-nox = "^2022.11.21"
-black = "^22.10.0"
-mypy = "^0.991"
+ruff = "^0.0.272"
+nox = "^2023.4.22"
+black = "^23.3.0"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 warn_return_any=true
```

### Comparing `socketapp-0.1.4/socketapp/client.py` & `socketapp-0.1.5/socketapp/client.py`

 * *Files identical despite different names*

### Comparing `socketapp-0.1.4/socketapp/event.py` & `socketapp-0.1.5/socketapp/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import pydantic
 
 if t.TYPE_CHECKING:
     from socketapp.client import Client
     from socketapp.server import Server
 
 
-class Event(pydantic.BaseModel):
-    event_map: t.ClassVar[dict[int, type["Event"]]] = {}
+event_map: dict[int, type[Event]] = {}
+
 
+class Event(pydantic.BaseModel):
     event_id: t.ClassVar[int]
     process_locally: t.ClassVar[bool] = True
 
     def __init_subclass__(cls) -> None:
         assert cls.event_id is not None
-        assert cls.event_id not in Event.event_map
+        assert cls.event_id not in event_map
 
-        Event.event_map[cls.event_id] = cls
+        event_map[cls.event_id] = cls
 
     async def process_server(self, server: "Server", author: int, to: set[int]) -> bool:
         return True
 
     async def process_client(self, client: "Client", author: int) -> bool:
         return True
```

### Comparing `socketapp-0.1.4/socketapp/server.py` & `socketapp-0.1.5/socketapp/server.py`

 * *Files identical despite different names*

