# Comparing `tmp/bods-client-0.9.0.tar.gz` & `tmp/bods-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bods-client-0.9.0.tar", max compression
+gzip compressed data, was "bods-client-0.9.1.tar", max compression
```

## Comparing `bods-client-0.9.0.tar` & `bods-client-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1104 2022-09-17 17:29:10.483929 bods-client-0.9.0/LICENSE
--rw-r--r--   0        0        0     3808 2022-09-17 17:29:10.483929 bods-client-0.9.0/README.md
--rw-r--r--   0        0        0       24 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/__init__.py
--rw-r--r--   0        0        0    10576 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/client.py
--rw-r--r--   0        0        0      472 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/constants.py
--rw-r--r--   0        0        0      450 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/__init__.py
--rw-r--r--   0        0        0     1148 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/avl.py
--rw-r--r--   0        0        0     1682 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/base.py
--rw-r--r--   0        0        0      690 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/fares.py
--rw-r--r--   0        0        0     7125 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/siri.py
--rw-r--r--   0        0        0     1533 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/models/timetables.py
--rw-r--r--   0        0        0        0 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/py.typed
--rw-r--r--   0        0        0      102 2022-09-17 17:29:10.483929 bods-client-0.9.0/bods_client/types.py
--rw-r--r--   0        0        0     1184 2022-09-17 17:29:10.483929 bods-client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4815 1970-01-01 00:00:00.000000 bods-client-0.9.0/setup.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 bods-client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1104 2022-09-30 18:15:32.873000 bods-client-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3808 2022-09-30 18:15:32.873000 bods-client-0.9.1/README.md
+-rw-r--r--   0        0        0       24 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/__init__.py
+-rw-r--r--   0        0        0    10576 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/client.py
+-rw-r--r--   0        0        0      472 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/constants.py
+-rw-r--r--   0        0        0      450 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/__init__.py
+-rw-r--r--   0        0        0     1148 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/avl.py
+-rw-r--r--   0        0        0     1682 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/base.py
+-rw-r--r--   0        0        0      690 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/fares.py
+-rw-r--r--   0        0        0     7125 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/siri.py
+-rw-r--r--   0        0        0     1926 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/models/timetables.py
+-rw-r--r--   0        0        0        0 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/py.typed
+-rw-r--r--   0        0        0      102 2022-09-30 18:15:32.873000 bods-client-0.9.1/bods_client/types.py
+-rw-r--r--   0        0        0     1184 2022-09-30 18:15:32.876999 bods-client-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4815 1970-01-01 00:00:00.000000 bods-client-0.9.1/setup.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 bods-client-0.9.1/PKG-INFO
```

### Comparing `bods-client-0.9.0/LICENSE` & `bods-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/README.md` & `bods-client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/client.py` & `bods-client-0.9.1/bods_client/client.py`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/models/avl.py` & `bods-client-0.9.1/bods_client/models/avl.py`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/models/base.py` & `bods-client-0.9.1/bods_client/models/base.py`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/models/fares.py` & `bods-client-0.9.1/bods_client/models/fares.py`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/models/siri.py` & `bods-client-0.9.1/bods_client/models/siri.py`

 * *Files identical despite different names*

### Comparing `bods-client-0.9.0/bods_client/models/timetables.py` & `bods-client-0.9.1/bods_client/models/timetables.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,10 +35,22 @@
     start_date_start: Optional[datetime] = Field(None, alias="startDateEnd")
     start_date_end: Optional[datetime] = Field(None, alias="startDateStart")
     end_date_start: Optional[datetime] = Field(None, alias="endDateStart")
     end_date_end: Optional[datetime] = Field(None, alias="endDateEnd")
     dq_rag: Optional[str] = Field(None, alias="dqRag")
     bods_compliance: Optional[bool] = Field(None, alias="bodsCompliance")
 
+    def dict(self, *args, **kwargs):
+        """Custom dict method to convert list of noc strings to a cvs.
+
+        There's a bug in the BODS timetables API where ?noc=NOC1&noc=NOC2
+        only recognises the last parameter.
+        """
+        dict_ = super().dict(*args, **kwargs)
+
+        if "noc" in dict_:
+            dict_["noc"] = ",".join(dict_.get("noc", []))
+        return dict_
+
 
 class TimetableResponse(BaseAPIResponse):
     results: List[Timetable]
```

### Comparing `bods-client-0.9.0/pyproject.toml` & `bods-client-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "bods-client"
 description = "A Python client for the Department for Transport Bus Open Data Service API"
-version = "0.9.0"
+version = "0.9.1"
 license = "MIT"
 
 authors = ["Ciaran McCormick"]
 
 readme = "README.md"
 
 repository = "https://github.com/ciaranmccormick/python-bods-client"
```

### Comparing `bods-client-0.9.0/setup.py` & `bods-client-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'protobuf>=3.20.0,<4.0.0',
  'pydantic>=1.8,<1.9',
  'python-dateutil>=2.8,<2.9',
  'requests>=2.25.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bods-client',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A Python client for the Department for Transport Bus Open Data Service API',
     'long_description': '# bods-client\n\n[![Build Status](https://github.com/ciaranmccormick/python-bods-client/workflows/test/badge.svg?branch=main&event=push)](https://github.com/ciaranmccormick/python-bods-client/actions?query=workflow%3Atest)\n[![codecov](https://codecov.io/gh/ciaranmccormick/python-bods-client/branch/main/graph/badge.svg)](https://codecov.io/gh/ciaranmccormick/python-bods-client)\n[![Python Version](https://img.shields.io/pypi/pyversions/bods-client.svg)](https://pypi.org/project/bods-client/)\n\nA Python client for the Department for Transport Bus Open Data Service API\n\n\n## Installation\n\n```bash\npip install bods-client\n```\n\n\n## Example\n\n\n### GTFS RT\n\nAll the vehicle locations for vehicles in a geographical location can be obtained\nusing the `get_gtfs_rt_data_feed` method with a bounding box.\n\n```python\n\nfrom bods_client.client import BODSClient\nfrom bods_client.models import BoundingBox, GTFSRTParams\n\n# An API key can be obtained by registering with the Bus Open Data Service\n# https://data.bus-data.dft.gov.uk/account/signup/\n>> API_KEY = "api-key"\n\n>> bods = BODSClient(api_key=API_KEY)\n>> bounding_box = BoundingBox(\n    **{\n        "min_latitude": 51.26,\n        "max_latitude": 51.75,\n        "min_longitude": -0.54,\n        "max_longitude": 0.27,\n    }\n)\n>> params = GTFSRTParams(bounding_box=bounding_box)\n>> message = bods.get_gtfs_rt_data_feed(params=params)\n>> message.entity[0]\nid: "421354378097713049"\nvehicle {\n  trip {\n    trip_id: ""\n    route_id: ""\n  }\n  position {\n    latitude: 51.712860107421875\n    longitude: -0.38401100039482117\n    bearing: 170.0\n  }\n  timestamp: 1614396229\n  vehicle {\n    id: "7214"\n  }\n}\n\n```\n\nThis returns a `google.transit.gtfs_realtime_pb2.FeedMessage` object. More details about\nGeneral Transit Feed Specification Realtime Transit (GTFS-RT) can be found\n[here](https://developers.google.com/transit/gtfs-realtime/).\n\n\n### SIRI VM\n\nVehicle locations are also provided in the SIRI-VM XML format using the\n`get_siri_vm_data_feed` method. The data can then parsed using an xml\nparser library such as `lxml`.\n\n```python\nfrom bods_client.client import BODSClient\nfrom bods_client.models import BoundingBox, Siri, SIRIVMParams\n\n\n>> API_KEY = "api-key"\n\n>> client = BODSClient(api_key=API_KEY)\n>> bounding_box = BoundingBox(\n    **{\n        "min_latitude": 51.267729,\n        "max_latitude": 51.283191,\n        "min_longitude": -0.142423,\n        "max_longitude": 0.177432,\n    }\n)\n\n>> params = SIRIVMParams(bounding_box=bounding_box)\n>> siri_response = client.get_siri_vm_data_feed(params=params)\n>> siri = Siri.from_bytes(siri_response)\n>> siri.service_delivery.vehicle_monitoring_delivery.vehicle_activities[0]\nVehicleActivity(\n    recorded_at_time=datetime.datetime(\n        2022, 1, 31, 19, 48, 24, tzinfo=datetime.timezone.utc\n    ),\n    item_identifier="05fc46f3-9629-4336-9a8d-f397030f5891",\n    valid_until_time=datetime.datetime(2022, 1, 31, 21, 5, 21, 997139),\n    monitored_vehicle_journey=MonitoredVehicleJourney(\n        bearing=135.0,\n        block_ref=None,\n        framed_vehicle_journey_ref=None,\n        vehicle_journey_ref="447183",\n        destination_name="BEDDINGTON (ABELLIO LONDON)",\n        destination_ref=None,\n        orgin_name=None,\n        origin_ref="40004410084D",\n        origin_aimed_departure_time=datetime.datetime(\n            2022, 1, 31, 19, 53, tzinfo=datetime.timezone.utc\n        ),\n        direction_ref="1",\n        published_line_name="407",\n        line_ref="296",\n        vehicle_location=VehicleLocation(longitude=-0.077464, latitude=51.282658),\n        operator_ref="TFLO",\n        vehicle_ref="16085",\n    ),\n)\n```\n\nDetails about the SIRI specification can be found [here](http://www.transmodel-cen.eu/standards/siri/).\n\n\n## License\n\n[MIT](https://github.com/ciaran.mccormick/bods-client/blob/master/LICENSE)\n',
     'author': 'Ciaran McCormick',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ciaranmccormick/python-bods-client',
```

### Comparing `bods-client-0.9.0/PKG-INFO` & `bods-client-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bods-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python client for the Department for Transport Bus Open Data Service API
 Home-page: https://github.com/ciaranmccormick/python-bods-client
 License: MIT
 Author: Ciaran McCormick
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

