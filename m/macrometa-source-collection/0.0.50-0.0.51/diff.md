# Comparing `tmp/macrometa-source-collection-0.0.50.tar.gz` & `tmp/macrometa-source-collection-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.50.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.51.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.50.tar` & `macrometa-source-collection-0.0.51.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11137 2023-06-16 12:00:33.237896 macrometa-source-collection-0.0.50/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9960 2023-06-16 12:00:33.237896 macrometa-source-collection-0.0.50/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-16 12:00:33.477900 macrometa-source-collection-0.0.50/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.50/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-06-19 03:18:54.842554 macrometa-source-collection-0.0.51/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    10129 2023-06-19 03:18:54.842554 macrometa-source-collection-0.0.51/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-19 03:18:55.094558 macrometa-source-collection-0.0.51/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.51/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.51/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.50/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.51/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.50/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.51/macrometa_source_collection/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,34 +63,37 @@
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             columns = list(stream.schema.properties.keys())
             columns.remove("_sdc_deleted_at")
             schema_properties = stream.schema.properties
-            self.load_existing_data(stream, columns, schema_properties)
-            LOGGER.info("Full table sync completed.")
-
             # pulsar client throws some messages into stdout when subscribed to a topic. Meltano tap/target doesn't like
             # this and tries to process the pulsar log messages in stdout as input singer records. Therefore we are trying
             #  to turn off pulsar logging here. This is the best way I found with the current pulsar client API.
             _pulsar_logger = logging.getLogger("pulsar-logger")
             _pulsar_logger.setLevel(logging.CRITICAL)
             _pulsar_logger.addHandler(logging.NullHandler())
 
+            # Create a consumer before hand so as to capture changes done while loading existing data
             _pulsar_client = pulsar.Client(
                 f"pulsar+ssl://{self._host}:6651/",
                 authentication=self._auth,
                 tls_allow_insecure_connection=False,
                 logger=_pulsar_logger,
             )
             _sub_name = self._wf_uuid if self._wf_uuid else f"cs_{uuid.uuid1()}"
             _topic = f"persistent://{self._tenant}/c8local.{self._fabric}/{self._collection}"
             _consumer: pulsar.Consumer = _pulsar_client.subscribe(_topic, _sub_name)
 
+            # Load existing data
+            self.load_existing_data(stream, columns, schema_properties)
+            LOGGER.info("Full table sync completed.")
+
+            # Change data capture
             while True:
                 try: 
                     msg = _consumer.receive()
                     data = msg.data()
                     if data == None or not data:
                         continue
                     props = msg.properties()
```

### Comparing `macrometa-source-collection-0.0.50/pyproject.toml` & `macrometa-source-collection-0.0.51/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.50'
+version='0.0.51'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.50/setup.py` & `macrometa-source-collection-0.0.51/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.50',
+    'version': '0.0.51',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.50/PKG-INFO` & `macrometa-source-collection-0.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.50
+Version: 0.0.51
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

