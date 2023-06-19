# Comparing `tmp/gordo_client-6.2.0rc0-py3-none-any.whl.zip` & `tmp/gordo_client-6.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 45010 bytes, number of entries: 16
+Zip file size: 44602 bytes, number of entries: 17
 -rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx      497 b- defN 80-Jan-01 00:00 gordo_client/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 gordo_client/cli/__init__.py
 -rw-r--r--  2.0 unx     8256 b- defN 80-Jan-01 00:00 gordo_client/cli/client.py
--rw-r--r--  2.0 unx     1308 b- defN 80-Jan-01 00:00 gordo_client/cli/custom_types.py
--rw-r--r--  2.0 unx    23791 b- defN 80-Jan-01 00:00 gordo_client/client.py
--rw-r--r--  2.0 unx     5471 b- defN 80-Jan-01 00:00 gordo_client/dataframe.py
--rw-r--r--  2.0 unx     8715 b- defN 80-Jan-01 00:00 gordo_client/forwarders.py
--rw-r--r--  2.0 unx     3564 b- defN 80-Jan-01 00:00 gordo_client/io.py
--rw-r--r--  2.0 unx     1769 b- defN 80-Jan-01 00:00 gordo_client/schemas.py
--rw-r--r--  2.0 unx     2703 b- defN 80-Jan-01 00:00 gordo_client/utils.py
-?rw-r--r--  2.0 unx       69 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3842 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/METADATA
-?rw-r--r--  2.0 unx     1307 b- defN 16-Jan-01 00:00 gordo_client-6.2.0rc0.dist-info/RECORD
-16 files, 129939 bytes uncompressed, 42864 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1282 b- defN 80-Jan-01 00:00 gordo_client/cli/custom_types.py
+-rw-r--r--  2.0 unx    22869 b- defN 80-Jan-01 00:00 gordo_client/client.py
+-rw-r--r--  2.0 unx     5351 b- defN 80-Jan-01 00:00 gordo_client/dataframe.py
+-rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 gordo_client/dist.py
+-rw-r--r--  2.0 unx     8574 b- defN 80-Jan-01 00:00 gordo_client/forwarders.py
+-rw-r--r--  2.0 unx     3545 b- defN 80-Jan-01 00:00 gordo_client/io.py
+-rw-r--r--  2.0 unx     1741 b- defN 80-Jan-01 00:00 gordo_client/schemas.py
+-rw-r--r--  2.0 unx     2669 b- defN 80-Jan-01 00:00 gordo_client/utils.py
+-rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2544 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1368 b- defN 16-Jan-01 00:00 gordo_client-6.2.2.dist-info/RECORD
+17 files, 127764 bytes uncompressed, 42370 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -15,35 +15,38 @@
 
 Filename: gordo_client/client.py
 Comment: 
 
 Filename: gordo_client/dataframe.py
 Comment: 
 
+Filename: gordo_client/dist.py
+Comment: 
+
 Filename: gordo_client/forwarders.py
 Comment: 
 
 Filename: gordo_client/io.py
 Comment: 
 
 Filename: gordo_client/schemas.py
 Comment: 
 
 Filename: gordo_client/utils.py
 Comment: 
 
-Filename: gordo_client-6.2.0rc0.dist-info/entry_points.txt
+Filename: gordo_client-6.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: gordo_client-6.2.0rc0.dist-info/LICENSE
+Filename: gordo_client-6.2.2.dist-info/METADATA
 Comment: 
 
-Filename: gordo_client-6.2.0rc0.dist-info/WHEEL
+Filename: gordo_client-6.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: gordo_client-6.2.0rc0.dist-info/METADATA
+Filename: gordo_client-6.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gordo_client-6.2.0rc0.dist-info/RECORD
+Filename: gordo_client-6.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gordo_client/cli/custom_types.py

```diff
@@ -1,8 +1,7 @@
-"""Custom click types."""
 import os
 import typing
 
 import click
 import yaml
 from dateutil import parser
 from gordo_core.data_providers.base import GordoBaseDataProvider
```

## gordo_client/client.py

```diff
@@ -1,8 +1,7 @@
-"""Gordo client."""
 import itertools
 import logging
 import pickle
 import copy
 
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
@@ -60,50 +59,50 @@
         session: Optional[requests.Session] = None,
         all_columns: bool = False,
     ):
         """
 
         Parameters
         ----------
-        project: str
+        project
             Name of the project.
-        host: str
+        host
             Host of where to find controller and other services.
-        port: int
+        port
             Port to communicate on.
-        scheme: str
+        scheme
             The request scheme to use, ie 'https'.
-        metadata: Optional[dict]
+        metadata
             Arbitrary mapping of key-value pairs to save to influx with
             prediction runs in 'tags' property
-        data_provider: Optional[GordoBaseDataProvider]
+        data_provider
             The data provider to use for the dataset. If not set, the client
-            will fall back to using the GET /prediction machine
-        prediction_forwarder: Optional[Callable[[pd.DataFrame, Machine, dict, pd.DataFrame], None]]
+            will fall back to using the ``GET /prediction`` machine
+        prediction_forwarder
             callable which will take a dataframe of predictions,
             ``Machine``, the metadata, and the dataframe of resampled sensor
             values and forward them somewhere.
-        batch_size: int
+        batch_size
             How many samples to send to the server, only applicable when data
             provider is supplied.
-        parallelism: int
+        parallelism
             The maximum number of tasks to run at a given time when
             running predictions
-        forward_resampled_sensors: bool
+        forward_resampled_sensors
             If true then forward resampled sensor values to the prediction_forwarder
-        n_retries: int
+        n_retries
             Number of times the client should attempt to retry a failed prediction request. Each time the client
             retires the time it sleeps before retrying is exponentially calculated.
-        use_parquet: bool
+        use_parquet
             Pass the data to the server using the parquet protocol. Default is True
             and recommended as it's more efficient for larger batch sizes. If False JSON
             is used for sending the data back and forth.
-        session: Optional[requests.Session]
+        session
             The http session object to use for making requests.
-        all_columns: bool
+        all_columns
             Return all columns for prediction. Including `smooth-..` columns
         """
 
         self.base_url = f"{scheme}://{host}:{port}"
         self.server_endpoint = f"{self.base_url}/gordo/v0/{project}"
         self.metadata = metadata if metadata is not None else dict()
         self.prediction_forwarder = prediction_forwarder
@@ -125,17 +124,16 @@
     @cached(TTLCache(maxsize=1, ttl=5))
     def get_revisions(self):
         """
         Gets the available revisions served by the server.
 
         Returns
         ------
-        dict
-            Dictionary with two keys, `available-revisions` and `latest`. The first is
-            a list of all available revisions, and `latest` is the latest and default
+            Dictionary with two keys, ``available-revisions`` and ``latest``. The first is
+            a list of all available revisions, and ``latest`` is the latest and default
             revision.
         """
         resp = self.session.get(f"{self.base_url}/gordo/v0/{self.project_name}/revisions")
         resp_json = _handle_response(resp=resp, resource_name="List of available revisions from server")
         return resp_json
 
     def _get_latest_revision(self) -> str:
@@ -148,45 +146,44 @@
         model_response = _handle_response(resp=resp, resource_name=f"Model name listing for revision {revision}")
         if "models" not in model_response:
             raise ValueError(f"Invalid response from server, key 'model' not found in: {model_response}")
         model_response["revision"] = model_response.get("revision", revision)
         return model_response
 
     def get_available_machines(self, revision: Optional[str] = None):
-        """Returns a dict representing the /models endpoint of the project for the given revision.
+        """Returns a dict representing the ``/models`` endpoint of the project for the given revision.
 
-        Contains at least a key `models` which contains the name of the models the
-        server can serve for that revision, and a key `revision` containing the
+        Contains at least a key ``models`` which contains the name of the models the
+        server can serve for that revision, and a key ``revision`` containing the
         revision."""
         return self._get_available_machines(revision=revision or self._get_latest_revision())
 
     def get_machine_names(self, revision: Optional[str] = None):
         """Returns the list of machine names served by a given revision, or latest
         revision if no revision is passed"""
         model_response = self._get_available_machines(revision=revision or self._get_latest_revision())
         return model_response.get("models")
 
     def _get_machines(self, revision: Optional[str] = None, machine_names: Optional[List[str]] = None) -> List[Machine]:
         """
-        Returns a list of :class:`gordo.workflow.config_elements.machine.Machine` elements served by the server for
+        Returns a list of :class:`gordo_client.schemas.Machine` elements served by the server for
         the provided machine names.
 
         Parameters
         ----------
-        revision: Optional[str]
+        revision
             Revision to fetch machines for. If None then the latest revision is fetched
             from the server.
-        machine_names: Optional[List[str]]
+        machine_names
             List of names of machines to fetch metadata for. If None then all machines
             for the given revision is fetched.
 
 
         Returns
         -------
-        List[Machine]
         """
         _machine_names: List[str] = machine_names or self.get_machine_names(revision=revision)
         with ThreadPoolExecutor(max_workers=self.parallelism) as executor:
             machines = executor.map(
                 lambda machine: self.machine_from_server(
                     name=machine, revision=revision or self._get_latest_revision()
                 ),
@@ -204,19 +201,18 @@
         if isinstance(metadata, dict) and metadata.get("metadata", None):
             return Machine(**metadata.get("metadata", None))
         else:
             raise NotFound(f"Machine {name} not found")
 
     def download_model(self, revision=None, targets: Optional[List[str]] = None) -> Dict[str, BaseEstimator]:
         """
-        Download the actual model(s) from the ML server /download-model.
+        Download the actual model(s) from the ML server ``/download-model``.
 
         Returns
         -------
-        Dict[str, BaseEstimator]
             Mapping of target name to the model
         """
         models = dict()
         for machine_name in targets or self.get_machine_names(revision=revision):
             resp = self.session.get(f"{self.base_url}/gordo/v0/{self.project_name}/{machine_name}/download-model")
             content = _handle_response(resp, resource_name=f"Model download for model {machine_name}")
             if isinstance(content, bytes):
@@ -230,57 +226,54 @@
 
     def get_metadata(self, revision: Optional[str] = None, targets: Optional[List[str]] = None) -> Dict[str, Metadata]:
         """
         Get the machine metadata for provided machines, or all if no machine names are provided.
 
         Parameters
         ----------
-        revision: Optional[str]
+        revision
             Revision to fetch machines for. If None then the latest revision is fetched
             from the server.
-        targets: Optional[List[str]]
+        targets
             List of names of machines to fetch metadata for. If None then all machines
             for the given revision is fetched.
 
         Returns
         -------
-        Dict[str, Metadata]
             Mapping of target names to their metadata
         """
         #  Value expression in dictionary comprehension has incompatible type "Optional[Metadata]"; expected type "Metadata"
         machines = self._get_machines(revision=revision, machine_names=targets)
         return {ep.name: copy.copy(ep.metadata) for ep in machines}
 
     def predict(
         self, start: datetime, end: datetime, targets: Optional[List[str]] = None, revision: Optional[str] = None
     ) -> Iterable[Tuple[str, pd.DataFrame, List[str]]]:
         """
         Start the prediction process.
 
         Parameters
         ----------
-        start: datetime
-        end: datetime
-        targets: Optional[List[str]]
+        start
+        end
+        targets
             Optionally only target certain machines, referring to them by name.
-        revision: Optional[str]
+        revision
             Revision of the model to run predictions again, defaulting to latest.
 
         Raises
         -----
         ResourceGone
             If the sever returns a 410, most likely because the revision is too old
 
         Returns
         -------
-        List[Tuple[str, pandas.core.DataFrame, List[str]]
-            A list of tuples, where:
-              0th element is the target name
-              1st element is the dataframe of the predictions; complete with a DateTime index.
-              2nd element is a list of error messages (if any) for running the predictions
+            0th element is the target name
+            1st element is the dataframe of the predictions; complete with a DateTime index.
+            2nd element is a list of error messages (if any) for running the predictions
         """
         rev = revision or self._get_latest_revision()
         machines = self._get_machines(revision=rev, machine_names=targets)
 
         # For every machine, start making predictions for the time range
         with ThreadPoolExecutor(max_workers=self.parallelism) as executor:
             jobs = executor.map(
@@ -288,29 +281,28 @@
             )
             return [(j.name, j.predictions, j.error_messages) for j in jobs]
 
     def predict_single_machine(
         self, machine: Machine, start: datetime, end: datetime, revision: str
     ) -> PredictionResult:
         """
-        Get predictions based on the /prediction POST machine of Gordo ML Servers.
+        Get predictions based on the ``/prediction`` POST machine of Gordo ML Servers.
 
         Parameters
         ----------
-        machine: Machine
+        machine
             Named tuple which has 'machine' specifying the full url to the base ml server
-        start: datetime
-        end: datetime
-        revision: str
+        start
+        end
+        revision
             Revision of the model to use
 
         Returns
         -------
-        dict
-            Prediction response from /prediction GET
+            Prediction response from ``/prediction`` GET
         """
 
         # Fetch all of the raw data
         X, y = self._raw_data(machine, start, end)
 
         # Forward sensor data
         if self.prediction_forwarder is not None and self.forward_resampled_sensors:
@@ -355,25 +347,25 @@
         revision: str,
     ):
         """
         Post a slice of data to the machine.
 
         Parameters
         ----------
-        X: pandas.core.DataFrame
+        X
             The data for the model, in pandas representation
-        chunk: slice
-            The slice to take from DataFrame.iloc for the batch size
-        machine: Machine
-        start: datetime
-        end: datetime
+        chunk
+            The slice to take from :func:`pandas.DataFrame.iloc` for the batch size
+        machine
+        start
+        end
 
         Notes
         -----
-        PredictionResult.predictions may be None if the prediction process fails
+        ``PredictionResult.predictions`` may be None if the prediction process fails
 
         Returns
         -------
         PredictionResult
 
         Raises
         -----
@@ -449,22 +441,18 @@
 
     def _get_dataset(self, machine: Machine, start: datetime, end: datetime) -> GordoBaseDataset:
         """
         Apply client setting to machine dataset.
 
         Parameters
         ----------
-        machine: Machine
+        machine
             Named tuple representing the machine info from controller
-        start: datetime
-        end: datetime
-
-        Returns
-        -------
-        GordoBaseDataset
+        start
+        end
         """
         # We want to adjust for any model offset. If the model outputs less than it got in, it requires
         # extra data than what we're being asked to get predictions for.
         # just to give us some buffer zone.
 
         resolution = machine.dataset["resolution"]
         n_intervals = machine.metadata.build_metadata.model.model_offset + 5
@@ -491,26 +479,25 @@
     @staticmethod
     def _extract_build_metadata(machine: Machine) -> dict:
         metadata = machine.metadata
         return metadata.build_metadata.dataset.dict()
 
     def _raw_data(self, machine: Machine, start: datetime, end: datetime) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
-        Fetch the required raw data in this time range which would satisfy this machine's /prediction POST.
+        Fetch the required raw data in this time range which would satisfy this machine's ``POST /prediction``.
 
         Parameters
         ----------
-        machine: Machine
+        machine
             Named tuple representing the machine info from controller
-        start: datetime
-        end: datetime
+        start
+        end
 
         Returns
         -------
-        Tuple[pandas.core.DataFrame, pandas.core.DataFrame]
             The dataframes representing X and y.
         """
         dataset = self._get_dataset(machine, start, end)
         build_metadata = self._extract_build_metadata(machine)
         return dataset.get_client_data(build_metadata)
 
     @staticmethod
@@ -519,19 +506,19 @@
         Adjust the given date by multiplying ``n_intervals`` by ``resolution``.
 
         Such that a date of 12:00:00 with ``n_intervals=2`` and ``resolution='10m'`` (10 minutes)
         would result in 11:40
 
         Parameters
         ----------
-        dt: datetime
+        dt
             Initial datetime to adjust.
-        resolution: str
+        resolution
             A string code capable of being parsed by :meth::`pandas.Timedelta`.
-        n_intervals: int
+        n_intervals
             Number of resolution steps to take earlier than the given date.
 
         Returns
         -------
         datetime
             The new offset datetime object.
 
@@ -547,19 +534,19 @@
 
     @staticmethod
     def dataframe_from_response(response: Union[dict, bytes]) -> pd.DataFrame:
         """
         Convert response from server into dataframe.
 
         The response from the server, parsed as either JSON / dict or raw bytes,
-        of which would be expected to be loadable from :func:`server.utils.dataframe_from_parquet_bytes`
+        of which would be expected to be loadable from ``gordo.server.utils.dataframe_from_parquet_bytes``
 
         Parameters
         ----------
-        response: Union[dict, bytes]
+        response
             The parsed response from the ML server.
 
         Returns
         -------
         pandas.DataFrame
         """
         if isinstance(response, dict):
@@ -574,23 +561,19 @@
     If the interval between start and end is less than ``max_interval_days`` then
     the resulting list will contain the original start & end. ie. [(start, end)]
 
     Otherwise it will split the intervals by ``freq``, parse-able by pandas.
 
     Parameters
     ----------
-    start: datetime
-    end: datetime
-    max_interval_days: int
+    start
+    end
+    max_interval_days
         Maximum days between start and end before splitting into intervals
-    freq: str
+    freq
         String frequency parse-able by Pandas
-
-    Returns
-    -------
-    List[Tuple[datetime, datetime]]
     """
     if (end - start).days >= max_interval_days:
         # Split into 1hr data ranges
         date_range = pd.date_range(start, end, freq=freq)
         return [(date_range[i], date_range[i + 1]) for i in range(0, len(date_range) - 1)]
     return [(start, end)]
```

## gordo_client/dataframe.py

```diff
@@ -1,25 +1,24 @@
-"""Gordo client dataframes methods."""
 import io
 
 import dateutil
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 
 def dataframe_into_parquet_bytes(df: pd.DataFrame, compression: str = "snappy") -> bytes:
     """
     Convert a dataframe into bytes representing a parquet table.
 
     Parameters
     ----------
-    df: pd.DataFrame
+    df
         DataFrame to be compressed
-    compression: str
+    compression
         Compression to use, passed to  :func:`pyarrow.parquet.write_table`
 
     Returns
     -------
     bytes
     """
     table = pa.Table.from_pandas(df)
@@ -30,17 +29,17 @@
 
 def dataframe_from_parquet_bytes(buf: bytes) -> pd.DataFrame:
     """
     Convert bytes representing a parquet table into a pandas dataframe.
 
     Parameters
     ----------
-    buf: bytes
+    buf
         Bytes representing a parquet table. Can be the direct result from
-        `func`::gordo.server.utils.dataframe_into_parquet_bytes
+        ``gordo.server.utils.dataframe_into_parquet_bytes``
 
     Returns
     -------
     pandas.DataFrame
     """
     table = pq.read_table(io.BytesIO(buf))
     return table.to_pandas()
@@ -51,25 +50,24 @@
     Convert a dataframe can have a :class:`pandas.MultiIndex` as columns into a dict.
 
     Each key is the top level column name, and the value is the array
     of columns under the top level name. If it's a simple dataframe, :meth:`pandas.core.DataFrame.to_dict`
     will be used.
 
     This allows :func:`json.dumps` to be performed, where :meth:`pandas.DataFrame.to_dict()`
-    would convert such a multi-level column dataframe into keys of ``tuple`` objects, which are
-    not json serializable. However this ends up working with :meth:`pandas.DataFrame.from_dict`
+    would convert such a multi-level column dataframe into keys of :func:`tuple` objects, which are
+    not json serializable. However this ends up working with :func:`pandas.DataFrame.from_dict`
 
     Parameters
     ----------
-    df: pandas.DataFrame
+    df
         Dataframe expected to have columns of type :class:`pandas.MultiIndex` 2 levels deep.
 
     Returns
     -------
-    List[dict]
         List of records representing the dataframe in a 'flattened' form.
 
 
     Examples
     --------
     >>> import pprint
     >>> import pandas as pd
@@ -102,28 +100,27 @@
     else:
         return data.to_dict()
 
 
 def dataframe_from_dict(data: dict) -> pd.DataFrame:
     """
     The inverse procedure done by :func:`.multi_lvl_column_dataframe_from_dict`
-    Reconstructed a MultiIndex column dataframe from a previously serialized one.
+    Reconstructed a ``pandas.MultiIndex`` column dataframe from a previously serialized one.
 
     Expects ``data`` to be a nested dictionary where each top level key has a value
-    capable of being loaded from :func:`pandas.core.DataFrame.from_dict`
+    capable of being loaded from :func:`pandas.DataFrame.from_dict`
 
     Parameters
     ----------
-    data: dict
+    data
         Data to be loaded into a MultiIndex column dataframe
 
     Returns
     -------
-    pandas.core.DataFrame
-        MultiIndex column dataframe.
+        ``MultiIndex`` column dataframe.
 
     Examples
     --------
     >>> serialized = {
     ... 'feature0': {'sub-feature-0': {'2019-01-01': 0, '2019-02-01': 4},
     ...              'sub-feature-1': {'2019-01-01': 1, '2019-02-01': 5}},
     ... 'feature1': {'sub-feature-0': {'2019-01-01': 2, '2019-02-01': 6},
```

## gordo_client/forwarders.py

```diff
@@ -1,8 +1,7 @@
-"""Gordo client forwarders."""
 import abc
 import itertools
 import logging
 import time
 from typing import Any, Dict, Optional
 
 import numpy as np
@@ -12,26 +11,27 @@
 from gordo_client.utils import influx_client_from_uri
 from gordo_core.sensor_tag import extract_tag_name
 
 logger = logging.getLogger(__name__)
 
 
 class PredictionForwarder(metaclass=abc.ABCMeta):
-
     """
-    Definition of a callable which the :class:`gordo_client.Client`
-    will call after each successful prediction response::
+        Definition of a callable which the :class:`gordo_client.client.Client`
+        will call after each successful prediction response.
+
+    .. code-block:: python
 
-        def my_forwarder(
-            predictions: pd.DataFrame = None,
-            machine: Machine = None,
-            metadata: dict = dict(),
-            resampled_sensor_data: pd.DataFrame = None
-        ):
-            ...
+            def my_forwarder(
+                predictions: pd.DataFrame = None,
+                machine: Machine = None,
+                metadata: dict = dict(),
+                resampled_sensor_data: pd.DataFrame = None
+            ):
+                ...
     """
 
     @abc.abstractmethod
     def __call__(
         self,
         *,
         predictions: pd.DataFrame = None,
@@ -43,15 +43,15 @@
 
 
 class ForwardPredictionsIntoInflux(PredictionForwarder):
     """
     To be used as a 'forwarder' for the prediction client
 
     After instantiation, it is a coroutine which accepts prediction dataframes
-    which it will pass onto influx
+    which it will pass onto Influx
     """
 
     def __init__(
         self,
         destination_influx_uri: Optional[str] = None,
         destination_influx_api_key: Optional[str] = None,
         destination_influx_recreate: bool = False,
@@ -59,20 +59,20 @@
     ):
         """
         Create an instance which, when called, is a coroutine capable of
         being sent dataframes generated from the '/anomaly/prediction' machine
 
         Parameters
         ----------
-        destination_influx_uri: str
+        destination_influx_uri
             Connection string for destination influx -
-            format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
-        destination_influx_api_key: str
+            format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
+        destination_influx_api_key
             API key if needed for destination db
-        destination_influx_recreate: bool
+        destination_influx_recreate
             Drop the database before filling it with data?
         """
         # Create df client if provided
         self.n_retries = n_retries
         self.dataframe_client = (
             influx_client_from_uri(
                 destination_influx_uri,
@@ -110,40 +110,32 @@
     @staticmethod
     def _clean_df(df: pd.DataFrame) -> pd.DataFrame:
         """
         Ensure dataframe doesn't have inf / nan values which influx can't handle
 
         Parameters
         ----------
-        df: pandas.DataFrame
-
-        Returns
-        -------
-        pandas.DataFrame
+        df
         """
         return df.replace([np.inf, -np.inf], np.nan).dropna()
 
     def forward_predictions(self, predictions: pd.DataFrame, machine: Machine, metadata: dict = dict()):
         """
-        Takes a multi-layed column dataframe and write points to influx where
+        Takes a multi-layed column dataframe and write points to Influx where
         each top level name is treated as the measurement name.
 
-        How the data is written via InfluxDB DataFrameClient in this method
+        How the data is written via InfluxDB ``DataFrameClient`` in this method
         determines the schema of the database.
 
         Parameters
         ----------
-        predictions: pd.DataFrame
+        predictions
             Multi layed column dataframe, where top level names will be treated
             as the 'measurement' name in influx and 2nd level will be the fields
             under those measurements.
-
-        Returns
-        -------
-        None
         """
         # Setup tags; metadata (if any) and other key value pairs.
         tags = {"machine": f"{machine.name}"}
         tags.update(metadata)
 
         # The measurements to be posted to Influx
         top_lvl_names = predictions.columns.get_level_values(0).unique()
@@ -167,15 +159,15 @@
             if len(sub_df.columns) == len(tag_list):
                 sub_df.columns = tag_list
                 # sub_df.columns = [tag['name'] for tag in machine.dataset['tag_list']]
             self._write_to_influx_with_retries(sub_df, top_lvl_name, tags)
 
     def _write_to_influx_with_retries(self, df, measurement, tags: Dict[str, Any] = {}):
         """
-        Write data to influx with retries and exponential backof. Will sleep
+        Write data to Influx with retries and exponential backof. Will sleep
         exponentially longer between each retry, starting at 8 seconds, capped at 5 min.
         """
         logger.info(f"Writing {len(df)} points to Influx for measurement: {measurement}")
 
         df = ForwardPredictionsIntoInflux._stack_to_name_value_columns(df)
 
         for current_attempt in itertools.count(start=1):
@@ -190,51 +182,50 @@
                 )
             except OSError as exc:
                 # TODO Prometheus Gauge with current_attempt
                 if current_attempt <= self.n_retries:
                     # Sleep at most 5 min
                     time_to_sleep = min(2 ** (current_attempt + 2), 300)
                     logger.warning(
-                        f"Failed to forward data to influx on attempt "
+                        f"Failed to forward data to Influx on attempt "
                         f"{current_attempt} out of {self.n_retries}.\n"
                         f"Error: {exc}.\n"
                         f"Sleeping {time_to_sleep} seconds and trying again."
                     )
                     time.sleep(time_to_sleep)
                     continue
                 else:
-                    msg = f"Failed to forward data to influx. Error: {exc}"
+                    msg = f"Failed to forward data to Influx. Error: {exc}"
                     logger.error(msg)
                     raise exc
             else:
                 break
 
     def send_sensor_data(self, sensors: pd.DataFrame):
         """
-        Write sensor-data to influx
+        Write sensor-data to Influx
         """
-        # Write the per-sensor points to influx
+        # Write the per-sensor points to Influx
         logger.info(f"Writing {len(sensors)} sensor points to Influx")
         self._write_to_influx_with_retries(sensors, "resampled")
-        logger.debug("Done writing resampled sensor values to influx")
+        logger.debug("Done writing resampled sensor values to Influx")
 
     @staticmethod
     def _stack_to_name_value_columns(df: pd.DataFrame) -> pd.DataFrame:
         """
         Stack a DataFrame with a range of tag columns to one with name and value columns
 
         Parameters
         ----------
-        df: pd.DataFrame
+        df
             Source dataframe with individual columns for tags.
 
         Returns
         -------
-        df: pd.DataFrame
-            Stacked dataframe with columns `sensor_name` and `sensor_value`.
+            Stacked dataframe with columns ``sensor_name`` and ``sensor_value``.
         """
         # String column names are necessary for stacking
         # (as opposed to integers when df created from np.ndarray)
         df.columns = df.columns.astype(str)
 
         df = df.stack().to_frame(name="sensor_value")
         df = df.reset_index(level=1).rename(columns={"level_1": "sensor_name"})
```

## gordo_client/io.py

```diff
@@ -1,17 +1,16 @@
-"""Gordo client io."""
 from typing import Optional, Union
 
 import requests
 
 
 class HttpUnprocessableEntity(Exception):
     """
-    Represents an error from an HTTP status code of 422: UnprocessableEntity.
-    Used in our case for calling /anomaly/prediction on a model which does not
+    Represents an error from an HTTP status code of ``422: UnprocessableEntity``.
+    Used in our case for calling ``/anomaly/prediction`` on a model which does not
     support anomaly behavior.
     """
 
 
 class ResourceGone(Exception):
     """
     Represents an error from an HTTP status code of 410: Gone.
@@ -55,18 +54,16 @@
     Handle the response from the server.
     Either returning the parsed json (if it is json), the pure bytestream of the content, or raise an exception
     if something went wrong.
 
 
     Parameters
     ----------
-    resp:
-        The request to inspect for a result
-    resource_name:
-        An optional name to add to error messages. Should describe the resource we
+    resp        The request to inspect for a result
+    resource_name        An optional name to add to error messages. Should describe the resource we
         attempted to GET
 
     Returns
     -------
      Union[dict, bytes]
 
     Raises
```

## gordo_client/schemas.py

```diff
@@ -1,8 +1,7 @@
-"""Gordo client schemas."""
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, Field
 
 
 class CrossValidationMetaData(BaseModel):
     """Cross validation metadata schema."""
```

## gordo_client/utils.py

```diff
@@ -1,8 +1,7 @@
-"""Gordo client utils."""
 from collections import namedtuple
 from typing import Dict, Optional, Tuple, Union
 
 from influxdb import DataFrameClient, InfluxDBClient
 
 # Prediction result representation, name=str, predictions=dataframe, error_messages=List[str]
 PredictionResult = namedtuple("PredictionResult", "name predictions error_messages")
@@ -10,20 +9,19 @@
 
 def _parse_influx_uri(uri: str) -> Tuple[str, str, str, str, str, str]:
     """
     Parse an influx URI.
 
     Parameters
     ----------
-    uri: str
-        Format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
+    uri
+        Format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
 
     Returns
     -------
-    (str, str, str, str, str, str)
         username, password, host, port, path, database
     """
     username, password, host, port, *path, db_name = uri.replace("/", ":").replace("@", ":").split(":")
     path_str = "/".join(path) if path else ""
     return username, password, host, port, path_str, db_name
 
 
@@ -32,34 +30,33 @@
     api_key: Optional[str] = None,
     api_key_header: Optional[str] = "Ocp-Apim-Subscription-Key",
     recreate: bool = False,
     dataframe_client: bool = False,
     proxies: Dict[str, str] = {"https": "", "http": ""},
 ) -> Union[InfluxDBClient, DataFrameClient]:
     """
-    Get a InfluxDBClient or DataFrameClient from a SqlAlchemy like URI.
+    Get a ``InfluxDBClient`` or ``DataFrameClient`` from a ``SqlAlchemy`` like URI.
+
+    .. todo::
+        Remove this function. Use :class:`gordo_core.utils.influx_client_from_uri` instead.
 
     Parameters
     ----------
-    uri: str
-        Connection string format: <username>:<password>@<host>:<port>/<optional-path>/<db_name>
-    api_key: str
+    uri
+        Connection string format: ``<username>:<password>@<host>:<port>/<optional-path>/<db_name>``
+    api_key
         Any api key required for the client connection
-    api_key_header: str
+    api_key_header
         The name of the header the api key should be assigned
-    recreate: bool
+    recreate
         Re/create the database named in the URI
-    dataframe_client: bool
-        Return a DataFrameClient instead of a standard InfluxDBClient
-    proxies: dict
+    dataframe_client
+        Return ``DataFrameClient`` instead of a standard ``InfluxDBClient``
+    proxies
         A mapping of any proxies to pass to the influx client
-
-    Returns
-    -------
-    Union[InfluxDBClient, DataFrameClient]
     """
     username, password, host, port, path, db_name = _parse_influx_uri(uri)
 
     Client = DataFrameClient if dataframe_client else InfluxDBClient
 
     client = Client(
         host=host,
```

## Comparing `gordo_client-6.2.0rc0.dist-info/LICENSE` & `gordo_client-6.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gordo_client-6.2.0rc0.dist-info/RECORD` & `gordo_client-6.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
 gordo_client/__init__.py,sha256=DhteHHu9xX3xDQeVav3mhwMjEvPnR06Bo0FjUVsV7Kg,497
 gordo_client/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gordo_client/cli/client.py,sha256=DP3NY2K1ezrEb5j4-a9xdRYdOl29MOuztJs4Tj-oSJI,8256
-gordo_client/cli/custom_types.py,sha256=rE6iT0cuPU8wzvFVm6HSWOka9D_Zxc9w8BcC7eNeIRM,1308
-gordo_client/client.py,sha256=_TvJTpdHZt5ZEIReZDw82yrmL-XYoC-8Tfknb-2fWFE,23791
-gordo_client/dataframe.py,sha256=NIysETom72gGyghpKtCPOYFecuGUwK1o6pb7ZeReXBc,5471
-gordo_client/forwarders.py,sha256=S80fwzAxA-luzxVq82AM4J1ZRz0NrXv12aIpM2JBvCo,8715
-gordo_client/io.py,sha256=Wmv06dwUaYxWIiHjKjBPhH8GBpNCfv7LKqCt1RJAMS8,3564
-gordo_client/schemas.py,sha256=ox7tp1ZgVWBOkmkaz0IScJ-2fozmh6u_Kaax50kp5Kc,1769
-gordo_client/utils.py,sha256=3_x-fbTQt-fOA8CFfkPVdBXhBoKwxFfvyq-dzrrX-CQ,2703
-gordo_client-6.2.0rc0.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
-gordo_client-6.2.0rc0.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
-gordo_client-6.2.0rc0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
-gordo_client-6.2.0rc0.dist-info/METADATA,sha256=dHjbxt2jyjvx_33L82Qr2DrSVsxdYCocL4ysby7WLZM,3842
-gordo_client-6.2.0rc0.dist-info/RECORD,,
+gordo_client/cli/custom_types.py,sha256=bF0DcI0KH0P-SPX8HMv6RpKg-_NXrxvGx3ibXtTKyaM,1282
+gordo_client/client.py,sha256=WpCrHmOXLbsaFWkYhkVnDMbtfT1zYhkSUzsMhAM8sX0,22869
+gordo_client/dataframe.py,sha256=8JPreh239zndjFd6qE4wvLfQrzh1EaH1dArOwwf0UXQ,5351
+gordo_client/dist.py,sha256=y18r-Cl2oHsSgy92zCRP0AvbmV-JVhu264CvgWOeOZo,347
+gordo_client/forwarders.py,sha256=VF5BrfozoU1fDmifmJPGkOGFd7b39K_k1lbFUP61Y_g,8574
+gordo_client/io.py,sha256=7EPiLCC7YOcv7A02bW9SsdQ4_n-ZvGeGaKnhATK9_rI,3545
+gordo_client/schemas.py,sha256=FBwKLa8I-9Y0rJufF0rCqDKYuvSUUyBzXQ1Ndkr5piA,1741
+gordo_client/utils.py,sha256=nkuZfOZtORlN_KPP-ydY1lsWz7Mm8Muy8HCPdbxv3s8,2669
+gordo_client-6.2.2.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
+gordo_client-6.2.2.dist-info/METADATA,sha256=TAcN6UQIqACJvTEZL1WSeB7uE_PcgnGRyzlFMjfaXA0,2544
+gordo_client-6.2.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+gordo_client-6.2.2.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
+gordo_client-6.2.2.dist-info/RECORD,,
```

