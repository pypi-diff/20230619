# Comparing `tmp/homeassistant-historical-sensor-1.0.0a0.tar.gz` & `tmp/homeassistant-historical-sensor-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant-historical-sensor-1.0.0a0.tar", last modified: Sun Jun 18 15:36:02 2023, max compression
+gzip compressed data, was "homeassistant-historical-sensor-1.0.0a1.tar", last modified: Mon Jun 19 12:45:46 2023, max compression
```

## Comparing `homeassistant-historical-sensor-1.0.0a0.tar` & `homeassistant-historical-sensor-1.0.0a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/recorderutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:36:02.220721 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 15:36:02.000000 homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-18 15:35:51.000000 homeassistant-historical-sensor-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-18 15:36:02.224722 homeassistant-historical-sensor-1.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:45:46.136509 homeassistant-historical-sensor-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 12:45:46.136509 homeassistant-historical-sensor-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:45:46.132509 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/recorderutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:45:46.136509 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-19 12:45:46.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 12:45:46.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:45:46.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-19 12:45:46.000000 homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-19 12:45:35.000000 homeassistant-historical-sensor-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-19 12:45:46.136509 homeassistant-historical-sensor-1.0.0a1/setup.cfg
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/PKG-INFO` & `homeassistant-historical-sensor-1.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/README.md` & `homeassistant-historical-sensor-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/__init__.py` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,34 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301,
 # USA.
 
 
 import logging
 
-from homeassistant.const import MAJOR_VERSION, MINOR_VERSION
+from homeassistant.const import (
+    MAJOR_VERSION,
+    MINOR_VERSION,
+    __version__ as HA_FULL_VERSION,
+)
 
 from .sensor import HistoricalSensor, PollUpdateMixin
 from .state import HistoricalState
+from .consts import MIN_REQ_MAJOR_VERSION, MIN_REQ_MINOR_VERSION
 
 LOGGER = logging.getLogger(__name__)
 
-if not (MAJOR_VERSION >= 2023 and MINOR_VERSION >= 6):
-    msg = "Required homeassistant version >={MAJOR_VERSION}.{MINOR_VERSION}.0"
+if not (
+    (MAJOR_VERSION >= MIN_REQ_MAJOR_VERSION)
+    and (MINOR_VERSION >= MIN_REQ_MINOR_VERSION)
+):
+    msg = (
+        f"Running HomeAssistant {HA_FULL_VERSION}, "
+        f"Minimum required version >={MIN_REQ_MAJOR_VERSION}.{MIN_REQ_MINOR_VERSION}.0"
+    )
     LOGGER.debug(msg)
     raise SystemError(msg)
 
 __all__ = [
     "HistoricalSensor",
     "HistoricalState",
     "PollUpdateMixin",
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/patches.py` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/patches.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/recorderutil.py` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/recorderutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @contextmanager
 def hass_recorder_session(hass: HomeAssistant):
     r = recorder.get_instance(hass)
-    with (recorder.util.session_scope(session=r.get_session())) as session:
+    with recorder.util.session_scope(session=r.get_session()) as session:
         yield session
 
 
 async def get_last_statistics_wrapper(
     hass: HomeAssistant, statistic_id: str
 ) -> Optional[StatisticsRow]:
     res = await recorder.get_instance(hass).async_add_executor_job(
@@ -79,15 +79,15 @@
         ret = db_schema.StatesMeta(entity_id=entity.entity_id)
         session.add(ret)
         session.commit()
 
         return ret
 
 
-def delete_entity_invalid_states(session: Session, entity: Entity):
+def delete_entity_invalid_states(session: Session, entity: Entity) -> int:
     stmt = _entity_id_states_stmt(session, entity).order_by(
         db_schema.States.last_updated_ts.asc()
     )
 
     prev = None
     to_delete = []
 
@@ -100,14 +100,16 @@
             prev = state
 
     for state in to_delete:
         session.delete(state)
 
     session.commit()
 
+    return len(to_delete)
+
 
 def get_entity_latest_state(session: Session, entity: Entity):
     stmt = (
         _entity_id_states_stmt(session, entity)
         .where(
             not_(
                 or_(
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/sensor.py` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,23 @@
     split_statistic_id,
     valid_statistic_id,
 )
 from homeassistant.components.sensor import SensorEntity
 from homeassistant.helpers.event import async_track_time_interval
 from homeassistant.util import dt as dtutil
 
+from .patches import _build_attributes, _stringify_state
 from .recorderutil import (
     delete_entity_invalid_states,
-    get_entity_states_meta,
     get_entity_latest_state,
-    hass_recorder_session,
+    get_entity_states_meta,
     get_last_statistics_wrapper,
+    hass_recorder_session,
     save_states,
 )
-from .patches import _stringify_state
 from .state import HistoricalState
 
 _LOGGER = logging.getLogger(__name__)
 
 
 # You must know:
 # * DB keeps datetime object as utc
@@ -125,44 +125,46 @@
         if any([True for x in hist_states if x.dt.tzinfo is None]):
             _LOGGER.error("historical_states MUST include tzinfo")
             return
 
         hist_states = list(sorted(hist_states, key=lambda x: x.dt))
         _LOGGER.debug(
             f"{self.entity_id}: "
-            f"{len(hist_states)} historical states collected from sensor"
+            f"{len(hist_states)} historical states present in sensor"
         )
 
         if not hist_states:
             return
 
         # Write states
-        await self._async_write_recorder_states(hist_states)
+        n = len(await self._async_write_recorder_states(hist_states))
+        _LOGGER.debug(f"{self.entity_id}: {n} states written into the database")
 
         # Write statistics
-        await self._async_write_statistic_data(hist_states)
+        n = len(await self._async_write_statistic_data(hist_states))
+        _LOGGER.debug(f"{self.entity_id}: {n} statistics points written into database")
 
     async def _async_write_recorder_states(
         self, hist_states: List[HistoricalState]
-    ) -> None:
+    ) -> List[HistoricalState]:
         return await recorder.get_instance(self.hass).async_add_executor_job(
             self._write_recorder_states, hist_states
         )
 
-    def _write_recorder_states(self, hist_states: List[HistoricalState]):
+    def _write_recorder_states(
+        self, hist_states: List[HistoricalState]
+    ) -> List[HistoricalState]:
         with hass_recorder_session(self.hass) as session:
             #
             # Delete invalid states
             #
 
             try:
                 n_states = delete_entity_invalid_states(session, self)
-                _LOGGER.debug(
-                    f"{self.entity_id}: " f"{n_states} invalid states deleted"
-                )
+                _LOGGER.debug(f"{self.entity_id}: cleaned {n_states} invalid states")
 
             except sqlalchemy.exc.IntegrityError:
                 session.rollback()
                 _LOGGER.debug("Warning: Current recorder schema is not supported")
                 _LOGGER.debug(
                     "Invalid states can't be deleted from recorder."
                     + "This is not critical just unsightly for some graphs "
@@ -176,15 +178,15 @@
                 latest = get_entity_latest_state(session, self)
 
             except sqlalchemy.exc.DatabaseError:
                 _LOGGER.debug(
                     "Error: Current recorder schema is not supported. "
                     + "This error is fatal, please file a bug"
                 )
-                return
+                return []
 
             #
             # Drop historical states older than lastest db state
             #
 
             # About deleting intersecting states instead of drop incomming
             # overlapping states: This approach has been tested several times and
@@ -192,76 +194,82 @@
             # schema changes and sometimes, depending on the engine, integrity
             # failures appear. It is better to discard the new overlapping states
             # than to delete them from the database.
 
             if latest:
                 cutoff = dtutil.utc_from_timestamp(latest.last_updated_ts or 0)
                 _LOGGER.debug(
-                    f"{self.entity_id}: " f"lastest state: {latest.state} @ {cutoff}"
+                    f"{self.entity_id}: "
+                    f"lastest state found at {cutoff} ({latest.state})"
                 )
                 hist_states = [x for x in hist_states if x.dt > cutoff]
 
             else:
-                _LOGGER.debug(f"{self.entity_id}: no previous states found")
+                _LOGGER.debug(f"{self.entity_id}: no previous state found")
 
             #
             # Check if there are any states left
             #
             if not hist_states:
                 _LOGGER.debug(f"{self.entity_id}: no new states")
-                return
+                return []
+
+            n_hist_states = len(hist_states)
+            _LOGGER.debug(f"{self.entity_id}: found {n_hist_states} new states")
 
             #
             # Build recorder States
             #
             state_meta = get_entity_states_meta(session, self)
 
             db_states: List[db_schema.States] = []
             for idx, hist_state in enumerate(hist_states):
-                # attrs_as_dict = _build_attributes(self, hist_state.state)
-                # attrs_as_dict.update(hist_state.attributes)
-                # attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
+                attrs_as_dict = _build_attributes(self, hist_state.state)
+                attrs_as_dict.update(hist_state.attributes)
+                attrs_as_str = db_schema.JSON_DUMP(attrs_as_dict)
 
-                # attrs_as_bytes = (
-                #     b"{}" if hist_state.state is None else attrs_as_str.encode("utf-8")
-                # )
+                attrs_as_bytes = (
+                    b"{}" if hist_state.state is None else attrs_as_str.encode("utf-8")
+                )
 
-                # attrs_hash = db_schema.StateAttributes.hash_shared_attrs_bytes(
-                #     attrs_as_bytes
-                # )
+                attrs_hash = db_schema.StateAttributes.hash_shared_attrs_bytes(
+                    attrs_as_bytes
+                )
 
-                # state_attributes = db_schema.StateAttributes(
-                #     hash=attrs_hash, shared_attrs=attrs_as_str
-                # )
+                state_attributes = db_schema.StateAttributes(
+                    hash=attrs_hash, shared_attrs=attrs_as_str
+                )
 
                 ts = dtutil.as_timestamp(hist_state.dt)
                 state = db_schema.States(
                     # entity_id=self.entity_id,
                     states_meta_rel=state_meta,
                     last_changed_ts=ts,
                     last_updated_ts=ts,
                     old_state=db_states[idx - 1] if idx else latest,
                     state=_stringify_state(self, hist_state.state),
-                    # state_attributes=state_attributes,
+                    state_attributes=state_attributes,
                 )
 
                 # _LOGGER.debug(
                 #     f"new state: "
                 #     f"dt={dtutil.as_local(hist_state.dt)} value={hist_state.state}"
                 # )
                 db_states.append(state)
 
             save_states(session, db_states)
 
-            _LOGGER.debug(f"{self.entity_id}: {len(db_states)} saved into the database")
+            return hist_states
 
-    async def _async_write_statistic_data(self, hist_states: List[HistoricalState]):
+    async def _async_write_statistic_data(
+        self, hist_states: List[HistoricalState]
+    ) -> List[HistoricalState]:
         if self.statatistic_id is None:
             _LOGGER.debug(f"{self.entity_id}: statistics are not enabled")
-            return
+            return []
 
         statistics_meta = self.get_statatistic_metadata()
 
         latest = await get_last_statistics_wrapper(
             self.hass, statistics_meta["statistic_id"]
         )
 
@@ -308,17 +316,15 @@
             _LOGGER.debug(f"new statistic: start={start_dt}, value={tmp!r}")
 
         if valid_statistic_id(self.statatistic_id):
             async_add_external_statistics(self.hass, statistics_meta, statistics_data)
         else:
             async_import_statistics(self.hass, statistics_meta, statistics_data)
 
-        _LOGGER.debug(
-            f"{self.entity_id}: collected {len(statistics_data)} statistic points"
-        )
+        return hist_states
 
     @property
     def statatistic_id(self) -> Optional[str]:
         return None
 
     def get_statatistic_metadata(self) -> StatisticMetaData:
         if self.statatistic_id is None:
@@ -337,15 +343,15 @@
             statistic_id=self.statatistic_id,
             unit_of_measurement=self.unit_of_measurement,
         )
 
         return metadata
 
     async def async_calculate_statistic_data(
-        self, hist_states: List[HistoricalState], *, latest: Optional[dict]
+        self, hist_states: List[HistoricalState], *, latest: Optional[dict] = None
     ) -> List[StatisticData]:
         raise NotImplementedError()
 
 
 class PollUpdateMixin(HistoricalSensor):
     """PollUpdateMixin for simulate poll update model
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor/state.py` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor/state.py`

 * *Files identical despite different names*

### Comparing `homeassistant-historical-sensor-1.0.0a0/homeassistant_historical_sensor.egg-info/PKG-INFO` & `homeassistant-historical-sensor-1.0.0a1/homeassistant_historical_sensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-historical-sensor
-Version: 1.0.0a0
+Version: 1.0.0a1
 Summary: Historical sensors for HomeAssistant
 Home-page: https://github.com/ldotlopez/ha-historical-sensor
 Author: Luis López
 Author-email: luis@cuarentaydos.com
 Project-URL: Repository, https://github.com/ldotlopez/ha-historical-sensor/
 Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-historical-sensor/issues
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a0
+Metadata-Version: 2.1 Name: homeassistant-historical-sensor Version: 1.0.0a1
 Summary: Historical sensors for HomeAssistant Home-page: https://github.com/
 ldotlopez/ha-historical-sensor Author: Luis LÃ³pez Author-email:
 luis@cuarentaydos.com Project-URL: Repository, https://github.com/ldotlopez/ha-
 historical-sensor/ Project-URL: Bug Tracker, https://github.com/ldotlopez/ha-
 historical-sensor/issues Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # Historical sensors for Home Assistant ![](icon-64.png)  ![GitHub
 Release (latest SemVer including pre-releases)](https://img.shields.io/github/
```

### Comparing `homeassistant-historical-sensor-1.0.0a0/setup.cfg` & `homeassistant-historical-sensor-1.0.0a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = homeassistant-historical-sensor
-version = 1.0.0a0
+version = 1.0.0a1
 author = Luis López
 author_email = luis@cuarentaydos.com
 description = Historical sensors for HomeAssistant
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ldotlopez/ha-historical-sensor
 project_urls =
```

