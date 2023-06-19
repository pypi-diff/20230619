# Comparing `tmp/python-matter-server-3.5.0.tar.gz` & `tmp/python-matter-server-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.5.0.tar", last modified: Fri Jun  2 12:09:44 2023, max compression
+gzip compressed data, was "python-matter-server-3.5.1.tar", last modified: Mon Jun 19 13:39:41 2023, max compression
```

## Comparing `python-matter-server-3.5.0.tar` & `python-matter-server-3.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.966092 python-matter-server-3.5.0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-02 12:09:30.000000 python-matter-server-3.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:09:43.000000 python-matter-server-3.5.0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 12:09:44.000000 python-matter-server-3.5.0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 12:09:44.970092 python-matter-server-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25613 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:39:38.000000 python-matter-server-3.5.1/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/setup.cfg
```

### Comparing `python-matter-server-3.5.0/LICENSE` & `python-matter-server-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/PKG-INFO` & `python-matter-server-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.5.0/README.md` & `python-matter-server-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/client/client.py` & `python-matter-server-3.5.1/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/client/connection.py` & `python-matter-server-3.5.1/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/client/exceptions.py` & `python-matter-server-3.5.1/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/client/models/device_types.py` & `python-matter-server-3.5.1/matter_server/client/models/device_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """Register a subclass."""
         super().__init_subclass__(**kwargs)
         cls.device_type = device_type
         ALL_TYPES[device_type] = cls
 
     def __hash__(self) -> int:
         """Return unique hash for this object."""
-        return hash(self.device_type)
+        return self.device_type
 
 
 class OrphanClusters(DeviceType, device_type=0xF001):
     """Orphan Clusters."""
 
     clusters = {
         all_clusters.ProxyConfiguration,
```

### Comparing `python-matter-server-3.5.0/matter_server/client/models/node.py` & `python-matter-server-3.5.1/matter_server/client/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         attributes_data: dict[str, Any],
         node: MatterNode,
     ) -> None:
         """Initialize MatterEndpoint."""
         self.node = node
         self.endpoint_id = endpoint_id
         self.clusters: dict[int, Clusters.Cluster] = {}
-        self.device_types: set[DeviceType] = set()
+        self.device_types: set[type[DeviceType]] = set()
         self.update(attributes_data)
 
     @property
     def is_bridged_device(self) -> bool:
         """Return if this endpoint represents a Bridged device."""
         return BridgedDevice in self.device_types
```

### Comparing `python-matter-server-3.5.0/matter_server/common/errors.py` & `python-matter-server-3.5.1/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/common/helpers/api.py` & `python-matter-server-3.5.1/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/common/helpers/json.py` & `python-matter-server-3.5.1/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/common/helpers/util.py` & `python-matter-server-3.5.1/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/common/models.py` & `python-matter-server-3.5.1/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/__main__.py` & `python-matter-server-3.5.1/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/client_handler.py` & `python-matter-server-3.5.1/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/const.py` & `python-matter-server-3.5.1/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/device_controller.py` & `python-matter-server-3.5.1/matter_server/server/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,21 +281,21 @@
     async def interview_node(self, node_id: int) -> None:
         """Interview a node."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         LOGGER.debug("Interviewing node: %s", node_id)
         try:
-            await self._call_sdk(self.chip_controller.ResolveNode, nodeid=node_id)
+            await self._resolve_node(node_id=node_id)
             read_response: Attribute.AsyncReadTransaction.ReadResponse = (
                 await self.chip_controller.Read(
                     nodeid=node_id, attributes="*", events="*", fabricFiltered=False
                 )
             )
-        except ChipStackError as err:
+        except (ChipStackError, NodeNotResolving) as err:
             raise NodeInterviewFailed(f"Failed to interview node {node_id}") from err
 
         is_new_node = node_id not in self._nodes
         existing_info = self._nodes.get(node_id)
         node = MatterNodeData(
             node_id=node_id,
             date_commissioned=existing_info.date_commissioned
@@ -402,30 +402,27 @@
                 f"Node {node_id} does not exist or has not been interviewed."
             )
         assert node_id not in self._subscriptions, "Already subscribed to node"
         node_logger = LOGGER.getChild(str(node_id))
         node_logger.debug("Setting up subscriptions...")
 
         node = cast(MatterNodeData, self._nodes[node_id])
-
-        try:
-            await self._call_sdk(self.chip_controller.ResolveNode, nodeid=node_id)
-        except ChipStackError as err:
-            node.available = False
-            raise NodeNotResolving(f"Failed to resolve node {node_id}") from err
+        node.available = False
+        await self._resolve_node(node_id=node_id)
+        node.available = True
 
         # we follow the pattern of apple and google here and
         # just do a wildcard subscription for all clusters and properties
         # the client will handle filtering of the events.
         # if it turns out in the future that this is too much traffic (I don't think so now)
         # we can revisit this choice and do some selected subscriptions.
         sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
             nodeid=node_id,
             attributes="*",
-            events=[("*", 0)],
+            events=[("*", 1)],
             reportInterval=(0, 120),
             fabricFiltered=False,
         )
 
         def attribute_updated_callback(
             path: Attribute.TypedAttributePath,
             transaction: Attribute.SubscriptionTransaction,
@@ -628,7 +625,36 @@
                     # attributes are stored in form of AttributePath:
                     # ENDPOINT/CLUSTER_ID/ATTRIBUTE_ID
                     attribute_path = create_attribute_path(
                         endpoint, cluster_cls.id, attr_cls.attribute_id
                     )
                     result[attribute_path] = attr_value
         return result
+
+    async def _resolve_node(
+        self, node_id: int, retries: int = 3, allow_pase: bool = False
+    ) -> None:
+        """Resolve a Node on the network."""
+        if self.chip_controller is None:
+            raise RuntimeError("Device Controller not initialized.")
+        try:
+            if allow_pase:
+                # last attempt allows PASE connection (last resort)
+                LOGGER.debug(
+                    "Attempting to resolve node %s (with PASE connection)", node_id
+                )
+                await self._call_sdk(
+                    self.chip_controller.GetConnectedDeviceSync,
+                    nodeid=node_id,
+                    allowPASE=True,
+                )
+                return
+            LOGGER.debug("Resolving node %s", node_id)
+            await self._call_sdk(self.chip_controller.ResolveNode, nodeid=node_id)
+        except (ChipStackError, TimeoutError) as err:
+            if not retries:
+                # when we're out of retries, raise NodeNotResolving
+                raise NodeNotResolving(f"Unable to resolve Node {node_id}") from err
+            await self._resolve_node(
+                node_id=node_id, retries=retries - 1, allow_pase=retries - 1 == 0
+            )
+            await asyncio.sleep(2)
```

### Comparing `python-matter-server-3.5.0/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.5.1/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/server.py` & `python-matter-server-3.5.1/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/stack.py` & `python-matter-server-3.5.1/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/storage.py` & `python-matter-server-3.5.1/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/matter_server/server/vendor_info.py` & `python-matter-server-3.5.1/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.0/pyproject.toml` & `python-matter-server-3.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.5.0"
+version = "3.5.1"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -28,31 +28,34 @@
   "orjson",
   "home-assistant-chip-clusters==2023.6.0"
 ]
 
 [project.optional-dependencies]
 server = [
   "home-assistant-chip-core==2023.6.0",
-  "cryptography==40.0.2"
+  "cryptography==41.0.1"
 ]
 test = [
   "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
   "mypy==1.3.0",
   "pylint==2.17.4",
-  "pytest==7.3.1",
+  "pytest==7.3.2",
   "pytest-aiohttp==1.0.4",
   "pytest-cov==4.1.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
+[tool.codespell]
+ignore-words-list = "pase,"
+
 [tool.mypy]
 python_version = "3.10"
 check_untyped_defs = true
 #disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
@@ -130,7 +133,9 @@
     "matter_server",
     "tests",
 ]
 forced_separate = [
     "tests",
 ]
 combine_as_imports = true
+
+
```

### Comparing `python-matter-server-3.5.0/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.5.1/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.5.0/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.5.1/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

