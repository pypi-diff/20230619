# Comparing `tmp/hikari_clusters-1.1.3.tar.gz` & `tmp/hikari_clusters-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_clusters-1.1.3.tar", max compression
+gzip compressed data, was "hikari_clusters-1.1.4.tar", max compression
```

## Comparing `hikari_clusters-1.1.3.tar` & `hikari_clusters-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1077 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/LICENSE
--rw-r--r--   0        0        0     1628 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/README.md
--rw-r--r--   0        0        0      886 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/hikari_clusters/__init__.py
--rw-r--r--   0        0        0       65 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/hikari_clusters/__main__.py
--rw-r--r--   0        0        0     2977 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/hikari_clusters/base_client.py
--rw-r--r--   0        0        0     6766 2023-01-13 22:12:44.383597 hikari_clusters-1.1.3/hikari_clusters/brain.py
--rw-r--r--   0        0        0     3851 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/callbacks.py
--rw-r--r--   0        0        0      103 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/close_codes.py
--rw-r--r--   0        0        0     4486 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/cluster.py
--rw-r--r--   0        0        0     3537 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/commands.py
--rw-r--r--   0        0        0     2683 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/events.py
--rw-r--r--   0        0        0      483 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/exceptions.py
--rw-r--r--   0        0        0     2659 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/info_classes.py
--rw-r--r--   0        0        0     1216 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/ipc_base.py
--rw-r--r--   0        0        0    11987 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/ipc_client.py
--rw-r--r--   0        0        0     5098 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/ipc_server.py
--rw-r--r--   0        0        0     3256 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/payload.py
--rw-r--r--   0        0        0        0 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/py.typed
--rw-r--r--   0        0        0     4539 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/server.py
--rw-r--r--   0        0        0     3490 2023-01-13 22:12:44.387597 hikari_clusters-1.1.3/hikari_clusters/task_manager.py
--rw-r--r--   0        0        0      844 2023-01-13 22:12:54.955827 hikari_clusters-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 hikari_clusters-1.1.3/setup.py
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 hikari_clusters-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1628 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/README.md
+-rw-r--r--   0        0        0      886 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/__main__.py
+-rw-r--r--   0        0        0     2977 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/base_client.py
+-rw-r--r--   0        0        0     6766 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/brain.py
+-rw-r--r--   0        0        0     3851 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/callbacks.py
+-rw-r--r--   0        0        0      103 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/close_codes.py
+-rw-r--r--   0        0        0     4486 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/cluster.py
+-rw-r--r--   0        0        0     3537 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/commands.py
+-rw-r--r--   0        0        0     2683 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/events.py
+-rw-r--r--   0        0        0      483 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/exceptions.py
+-rw-r--r--   0        0        0     2691 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/info_classes.py
+-rw-r--r--   0        0        0     1216 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/ipc_base.py
+-rw-r--r--   0        0        0    11987 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/ipc_client.py
+-rw-r--r--   0        0        0     5098 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/ipc_server.py
+-rw-r--r--   0        0        0     3255 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/payload.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/py.typed
+-rw-r--r--   0        0        0     4539 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/server.py
+-rw-r--r--   0        0        0     3490 2023-06-19 16:28:27.810743 hikari_clusters-1.1.4/hikari_clusters/task_manager.py
+-rw-r--r--   0        0        0      854 2023-06-19 16:28:39.554743 hikari_clusters-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 hikari_clusters-1.1.4/PKG-INFO
```

### Comparing `hikari_clusters-1.1.3/LICENSE` & `hikari_clusters-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/README.md` & `hikari_clusters-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/__init__.py` & `hikari_clusters-1.1.4/hikari_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/base_client.py` & `hikari_clusters-1.1.4/hikari_clusters/base_client.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/brain.py` & `hikari_clusters-1.1.4/hikari_clusters/brain.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/callbacks.py` & `hikari_clusters-1.1.4/hikari_clusters/callbacks.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/cluster.py` & `hikari_clusters-1.1.4/hikari_clusters/cluster.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/commands.py` & `hikari_clusters-1.1.4/hikari_clusters/commands.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/events.py` & `hikari_clusters-1.1.4/hikari_clusters/events.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/info_classes.py` & `hikari_clusters-1.1.4/hikari_clusters/info_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 f"{used_by}"
             )
         BaseInfo._info_classes[cls._info_class_id] = cls
 
     def asdict(self) -> dict[str, Any]:
         """Convert this info class to a dictionary."""
 
-        dct = asdict(self)
+        dct: dict[str, Any] = asdict(self)  # type: ignore
         dct["_info_class_id"] = self._info_class_id
         return dct
 
     @staticmethod
     def fromdict(data: dict[str, Any]) -> BaseInfo:
         """Convert a dictionary back into its info class."""
```

### Comparing `hikari_clusters-1.1.3/hikari_clusters/ipc_base.py` & `hikari_clusters-1.1.4/hikari_clusters/ipc_base.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/ipc_client.py` & `hikari_clusters-1.1.4/hikari_clusters/ipc_client.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/ipc_server.py` & `hikari_clusters-1.1.4/hikari_clusters/ipc_server.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/payload.py` & `hikari_clusters-1.1.4/hikari_clusters/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     callback: int
     """The key sent in the command payload."""
 
     opcode: ClassVar[int] = 4
 
 
 PAYLOAD_DATA = Union[
-    Command, Event, ResponseOk, ResponseTraceback, ResponseNotFound,
+    Command, Event, ResponseOk, ResponseTraceback, ResponseNotFound
 ]
 
 OPCODES: dict[int, Type[PAYLOAD_DATA]] = {
     Command.opcode: Command,
     Event.opcode: Event,
     ResponseOk.opcode: ResponseOk,
     ResponseTraceback.opcode: ResponseTraceback,
```

### Comparing `hikari_clusters-1.1.3/hikari_clusters/server.py` & `hikari_clusters-1.1.4/hikari_clusters/server.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/hikari_clusters/task_manager.py` & `hikari_clusters-1.1.4/hikari_clusters/task_manager.py`

 * *Files identical despite different names*

### Comparing `hikari_clusters-1.1.3/pyproject.toml` & `hikari_clusters-1.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.black]
 line-length=79
 skip-magic-trailing-comma=true
 
 [tool.poetry]
 name = "hikari-clusters"
-version = "v1.1.3"
+version = "v1.1.4"
 description = "An advanced yet easy-to-use clustering tool for Hikari."
 authors = ["Circuit"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TrigonDev/hikari-clusters"
 repository = "https://github.com/TrigonDev/hikari-clusters"
 documentation = "https://github.com/TrigonDev/hikari-clusters/wiki"
 keywords = ["hikari", "discord", "clustering", "bot", "ipc"]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<3.11"
+python = ">=3.8.0,<3.12"
 hikari = "^2.0.0.dev105"
-websockets = "^10.1"
+websockets = "^11.0"
 pytest-cov = ">=3,<5"
 
-[tool.poetry.dev-dependencies]
-black = "^22.1"
-isort = "^5.9.3"
-mypy = "^0.991"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+mypy = "^1.3.0"
 flake8 = "^5.0.4"
-pytest = "^7.0.0"
-nox = "^2022.1.7"
+pytest = "^7.3.2"
+nox = "^2023.4.22"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hikari_clusters-1.1.3/PKG-INFO` & `hikari_clusters-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: hikari-clusters
-Version: 1.1.3
+Version: 1.1.4
 Summary: An advanced yet easy-to-use clustering tool for Hikari.
 Home-page: https://github.com/TrigonDev/hikari-clusters
 License: MIT
 Keywords: hikari,discord,clustering,bot,ipc
 Author: Circuit
-Requires-Python: >=3.8.0,<3.11
+Requires-Python: >=3.8.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hikari (>=2.0.0.dev105,<3.0.0)
 Requires-Dist: pytest-cov (>=3,<5)
-Requires-Dist: websockets (>=10.1,<11.0)
+Requires-Dist: websockets (>=11.0,<12.0)
 Project-URL: Documentation, https://github.com/TrigonDev/hikari-clusters/wiki
 Project-URL: Repository, https://github.com/TrigonDev/hikari-clusters
 Description-Content-Type: text/markdown
 
 # hikari-clusters
 [![pypi](https://github.com/TrigonDev/hikari-clusters/actions/workflows/pypi.yml/badge.svg)](https://pypi.org/project/hikari-clusters)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/TrigonDev/hikari-clusters/main.svg)](https://results.pre-commit.ci/latest/github/TrigonDev/hikari-clusters/main)
```

