# Comparing `tmp/tom_nonlocalizedevents-0.7.6.tar.gz` & `tmp/tom_nonlocalizedevents-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_nonlocalizedevents-0.7.6.tar", max compression
+gzip compressed data, was "tom_nonlocalizedevents-0.7.7.tar", max compression
```

## Comparing `tom_nonlocalizedevents-0.7.6.tar` & `tom_nonlocalizedevents-0.7.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35149 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/LICENSE
--rw-r--r--   0        0        0     5874 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/README.md
--rw-r--r--   0        0        0     2632 2023-05-15 22:21:57.378625 tom_nonlocalizedevents-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      144 2023-05-15 22:21:57.378625 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/__init__.py
--rw-r--r--   0        0        0      459 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/admin.py
--rw-r--r--   0        0        0        0 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/alertstream_handlers/__init__.py
--rw-r--r--   0        0        0     5307 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
--rw-r--r--   0        0        0     4766 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
--rw-r--r--   0        0        0      228 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/apps.py
--rw-r--r--   0        0        0    12766 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/healpix_utils.py
--rw-r--r--   0        0        0     3766 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/ingestion.py
--rw-r--r--   0        0        0      437 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0001_initial.py
--rw-r--r--   0        0        0      585 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0002_superevent.py
--rw-r--r--   0        0        0     1075 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
--rw-r--r--   0        0        0      460 2023-05-15 22:21:38.294449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
--rw-r--r--   0        0        0      543 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
--rw-r--r--   0        0        0     1015 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
--rw-r--r--   0        0        0      409 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
--rw-r--r--   0        0        0      411 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
--rw-r--r--   0        0        0      365 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
--rw-r--r--   0        0        0     1434 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
--rw-r--r--   0        0        0     2028 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
--rw-r--r--   0        0        0      574 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
--rw-r--r--   0        0        0     2510 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
--rw-r--r--   0        0        0     2082 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
--rw-r--r--   0        0        0     4567 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
--rw-r--r--   0        0        0     3814 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
--rw-r--r--   0        0        0      872 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py
--rw-r--r--   0        0        0        0 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/__init__.py
--rw-r--r--   0        0        0     9779 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/models.py
--rw-r--r--   0        0        0     6850 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/serializers.py
--rw-r--r--   0        0        0        0 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/signals/__init__.py
--rw-r--r--   0        0        0     1459 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/signals/handlers.py
--rw-r--r--   0        0        0       99 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
--rw-r--r--   0        0        0   218067 2023-05-15 22:21:38.298449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
--rw-r--r--   0        0        0  1780610 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
--rw-r--r--   0        0        0      416 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
--rw-r--r--   0        0        0      168 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
--rw-r--r--   0        0        0     1606 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
--rw-r--r--   0        0        0      490 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
--rw-r--r--   0        0        0        0 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/tests/__init__.py
--rw-r--r--   0        0        0      693 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/tests/factories.py
--rw-r--r--   0        0        0     2879 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/tests/tests.py
--rw-r--r--   0        0        0     1120 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/urls.py
--rw-r--r--   0        0        0     6577 2023-05-15 22:21:38.310449 tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/views.py
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/LICENSE
+-rw-r--r--   0        0        0     5878 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/README.md
+-rw-r--r--   0        0        0     2632 2023-06-19 18:44:12.267885 tom_nonlocalizedevents-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-19 18:44:12.271885 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/admin.py
+-rw-r--r--   0        0        0        0 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/alertstream_handlers/__init__.py
+-rw-r--r--   0        0        0     5307 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py
+-rw-r--r--   0        0        0     4882 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py
+-rw-r--r--   0        0        0      228 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/apps.py
+-rw-r--r--   0        0        0    13309 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/healpix_utils.py
+-rw-r--r--   0        0        0     3893 2023-06-19 18:43:53.203695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/ingestion.py
+-rw-r--r--   0        0        0      437 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0001_initial.py
+-rw-r--r--   0        0        0      585 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0002_superevent.py
+-rw-r--r--   0        0        0     1075 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py
+-rw-r--r--   0        0        0      460 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0004_superevent_superevent_type.py
+-rw-r--r--   0        0        0      543 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py
+-rw-r--r--   0        0        0     1015 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py
+-rw-r--r--   0        0        0      409 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0007_eventcandidate_viable.py
+-rw-r--r--   0        0        0      411 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0008_eventcandidate_priority.py
+-rw-r--r--   0        0        0      365 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0009_rename_superevent_nonlocalizedevent.py
+-rw-r--r--   0        0        0     1434 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py
+-rw-r--r--   0        0        0     2028 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py
+-rw-r--r--   0        0        0      574 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py
+-rw-r--r--   0        0        0     2510 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py
+-rw-r--r--   0        0        0     2082 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py
+-rw-r--r--   0        0        0     4567 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py
+-rw-r--r--   0        0        0     3814 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py
+-rw-r--r--   0        0        0      872 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/__init__.py
+-rw-r--r--   0        0        0     9779 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/models.py
+-rw-r--r--   0        0        0     6850 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/serializers.py
+-rw-r--r--   0        0        0        0 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/signals/__init__.py
+-rw-r--r--   0        0        0     1459 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/signals/handlers.py
+-rw-r--r--   0        0        0       99 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/css/main.css
+-rw-r--r--   0        0        0   218067 2023-06-19 18:43:53.207695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css
+-rw-r--r--   0        0        0  1780882 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js
+-rw-r--r--   0        0        0      416 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/webpack-stats.json
+-rw-r--r--   0        0        0      168 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/detail.html
+-rw-r--r--   0        0        0     1606 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html
+-rw-r--r--   0        0        0      490 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/superevent_vue_app.html
+-rw-r--r--   0        0        0        0 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/tests/__init__.py
+-rw-r--r--   0        0        0      693 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/tests/factories.py
+-rw-r--r--   0        0        0     2879 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/tests/tests.py
+-rw-r--r--   0        0        0     1120 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/urls.py
+-rw-r--r--   0        0        0     6577 2023-06-19 18:43:53.215695 tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/views.py
+-rw-r--r--   0        0        0     7878 1970-01-01 00:00:00.000000 tom_nonlocalizedevents-0.7.7/PKG-INFO
```

### Comparing `tom_nonlocalizedevents-0.7.6/LICENSE` & `tom_nonlocalizedevents-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/README.md` & `tom_nonlocalizedevents-0.7.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ```
 
     If `WEBPACK_LOADER` is already defined in your settings, then integrate these values in to it.
 
     Also add the following to your settings if they are not already there, setting whatever default values you need for your setup. These point to your deployed TOM toolkit instance, and to a hermes instance:
     ```python
     TOM_API_URL = os.getenv('TOM_API_URL', 'http://127.0.0.1:8000')
-    HERMES_API_URL = os.getenv('HERMES_API_URL', 'http://hermes-dev.lco.gtn')
+    HERMES_API_URL = os.getenv('HERMES_API_URL', 'https://hermes-dev.lco.global')
 
     ```
 
 3. Include the tom_nonlocalizedevent URLconf in your project `urls.py`:
    ```python
    urlpatterns = [
         ...
```

### Comparing `tom_nonlocalizedevents-0.7.6/pyproject.toml` & `tom_nonlocalizedevents-0.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-nonlocalizedevents"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.7.6"
+version = "0.7.7"
 description = "Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations."
 authors = ["TOM Toolkit Project <tomtoolkit@lco.global>", "David Collom <dcollom@lco.global>", "Lindy Lindstrom <llindstrom@lco.global>", "Jonathan Nation <jnation@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/TOMToolkit/tom_nonlocalizedevents"
 keywords = ["tomtoolkit", "astronomy", "astrophysics", "cosmology", "science"]
 classifiers = [
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/alertstream_handlers/gcn_event_handler.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/alertstream_handlers/igwn_event_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,33 +50,35 @@
         event_type=NonLocalizedEvent.NonLocalizedEventType.GRAVITATIONAL_WAVE,
     )
     if nle_created:
         logger.info(f"Ingested a new GW event with id {alert['superevent_id']} from IGWN alertstream")
 
     # Here we do a bit of pre-processing for IGWN alerts in order to be able to remove the skymap before saving the file
     localization = None
+    pipeline = alert.get('event', {}).get('pipeline', '')
     if alert.get('event'):
         skymap_bytes = alert['event'].pop('skymap')
         if skymap_bytes:
             try:
                 localization = create_localization_for_skymap(
-                    nonlocalizedevent=nonlocalizedevent, skymap_bytes=skymap_bytes
+                    nonlocalizedevent=nonlocalizedevent, skymap_bytes=skymap_bytes, pipeline=pipeline
                 )
             except Exception as e:
                 localization = None
                 logger.error(f'Could not create EventLocalization for event: {alert["superevent_id"]}. Exception: {e}')
                 logger.error(traceback.format_exc())
 
     external_coincidence = None
     if alert.get('external_coinc', {}):
         combined_skymap_bytes = alert['external_coinc'].pop('combined_skymap')
         if combined_skymap_bytes:
             try:
                 combined_localization = create_localization_for_skymap(
-                    nonlocalizedevent=nonlocalizedevent, skymap_bytes=combined_skymap_bytes, is_combined=True
+                    nonlocalizedevent=nonlocalizedevent, skymap_bytes=combined_skymap_bytes,
+                    is_combined=True, pipeline=pipeline
                 )
                 external_coincidence, _ = ExternalCoincidence.objects.get_or_create(
                     localization=combined_localization,
                     defaults={'details': alert.get('external_coinc')}
                 )
             except Exception as e:
                 external_coincidence = None
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/healpix_utils.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/healpix_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -118,41 +118,49 @@
                 return sequence.localization.skymap_version + 1
         return 0
     except NonLocalizedEvent.DoesNotExist:
         return 0  # The nonlocalizedevent doesnt exist in our system yet, so this must be the first skymap version
 
 
 def create_localization_for_skymap(nonlocalizedevent: NonLocalizedEvent, skymap_bytes: bytes, skymap_url: str = '',
-                                   is_combined=False):
+                                   is_combined: bool = False, pipeline: str = ''):
     """ Create localization from skymap bytes and related fields """
     logger.info(f"Creating localization for {nonlocalizedevent.event_id} with skymap {skymap_url}")
     skymap_hash = hashlib.md5(skymap_bytes).hexdigest()
     try:
         localization = EventLocalization.objects.get(nonlocalizedevent=nonlocalizedevent, skymap_hash=skymap_hash)
     except EventLocalization.DoesNotExist:
         skymap = Table.read(BytesIO(skymap_bytes))
-        distance_mean = skymap.meta['DISTMEAN']
-        distance_std = skymap.meta['DISTSTD']
+        is_burst = pipeline in ['CWB', 'oLIB', 'mLy']
+        if not is_burst:
+            distance_mean = skymap.meta['DISTMEAN']
+            distance_std = skymap.meta['DISTSTD']
+            row_dist_mean, row_dist_std, _ = distance.parameters_to_moments(
+                skymap['DISTMU'], skymap['DISTSIGMA'])
+        else:
+            distance_mean = 0
+            distance_std = 0
+            row_dist_mean = None
+            row_dist_std = None
         date = parse(skymap.meta['DATE']).replace(tzinfo=timezone.utc)
         skymap_uuid = uuid.UUID(skymap_hash)
         skymap_version = get_skymap_version(nonlocalizedevent, skymap_hash=skymap_uuid, is_combined=is_combined)
         if not skymap_url:
-            if is_combined:
-                skymap_url = (
-                    f"https://gracedb.ligo.org/api/superevents/{nonlocalizedevent.event_id}"
-                    f"/files/combined-ext.multiorder.fits,{skymap_version}"
-                )
-            else:
-                skymap_url = (
-                    f"https://gracedb.ligo.org/api/superevents/{nonlocalizedevent.event_id}"
-                    f"/files/bayestar.multiorder.fits,{skymap_version}"
-                )
+            base_url = f"https://gracedb.ligo.org/api/superevents/{nonlocalizedevent.event_id}/files/"
+            if pipeline in ['pycbc', 'gstlal', 'MBTA', 'MBTAOnline', 'spiir']:
+                if is_combined:
+                    skymap_url = f"{base_url}combined-ext.multiorder.fits,{skymap_version}"
+                else:
+                    skymap_url = f"{base_url}bayestar.multiorder.fits,{skymap_version}"
+            elif pipeline == 'CWB' and not is_combined:
+                skymap_url = f"{base_url}cwb.multiorder.fits,{skymap_version}"
+            elif pipeline == 'oLIB' and not is_combined:
+                skymap_url = f"{base_url}olib.multiorder.fits,{skymap_version}"
         area_50, area_90 = get_confidence_regions(skymap)
-        row_dist_mean, row_dist_std, _ = distance.parameters_to_moments(
-            skymap['DISTMU'], skymap['DISTSIGMA'])
+
         with transaction.atomic():
             localization = EventLocalization.objects.create(
                 nonlocalizedevent=nonlocalizedevent,
                 distance_mean=distance_mean,
                 distance_std=distance_std,
                 skymap_version=skymap_version,
                 skymap_hash=skymap_uuid,
@@ -165,16 +173,16 @@
                 # This is necessary to make sure we don't get an underflow error in postgres
                 # when operating with the probdensity float field
                 probdensity = row['PROBDENSITY'] if row['PROBDENSITY'] > sys.float_info.min else 0
                 SkymapTile.objects.create(
                     localization=localization,
                     tile=uniq_to_bigintrange(row['UNIQ']),
                     probdensity=probdensity,
-                    distance_mean=row_dist_mean[i],
-                    distance_std=row_dist_std[i]
+                    distance_mean=row_dist_mean[i] if row_dist_mean is not None else 0,
+                    distance_std=row_dist_std[i] if row_dist_std is not None else 0
                 )
     return localization
 
 
 # healpix_alchemy models pointing to django ORM models, for building a sql alchemy query
 class SaSkymap(Base):
     __tablename__ = 'tom_nonlocalizedevents_eventlocalization'
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/ingestion.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/ingestion.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,22 +30,24 @@
         event_type=NonLocalizedEvent.NonLocalizedEventType.GRAVITATIONAL_WAVE,
     )
     if nle_created:
         logger.info(f"Ingested a new GW event with id {event_id} from HermesBroker")
 
     localization = None
     skymap_url = data.get('urls', {}).get('skymap')
+    pipeline = data.get('event', {}).get('pipeline', '')
     if skymap_url:
         try:
             skymap_resp = requests.get(skymap_url)
             skymap_resp.raise_for_status()
             localization = create_localization_for_skymap(
                 nonlocalizedevent=nonlocalizedevent,
                 skymap_bytes=skymap_resp.content,
-                skymap_url=skymap_url
+                skymap_url=skymap_url,
+                pipeline=pipeline
             )
         except Exception as e:
             localization = None
             logger.error(
                 f"Failed to retrieve and process localization from skymap file at {skymap_url}. Exception: {e}"
             )
             logger.error(traceback.format_exc())
@@ -56,15 +58,16 @@
         try:
             combined_skymap_resp = requests.get(combined_skymap_url)
             combined_skymap_resp.raise_for_status()
             combined_localization = create_localization_for_skymap(
                 nonlocalizedevent=nonlocalizedevent,
                 skymap_bytes=combined_skymap_resp.content,
                 skymap_url=combined_skymap_url,
-                is_combined=True
+                is_combined=True,
+                pipeline=pipeline
             )
             external_coincidence, _ = ExternalCoincidence.objects.get_or_create(
                 localization=combined_localization,
                 defaults={'details': data.get('external_coinc')}
             )
         except Exception as e:
             combined_localization = None
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0002_superevent.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0002_superevent.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0003_auto_20210225_0034.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0005_auto_20210319_2241.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0006_auto_20210827_2346.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0010_rename_more_superevent_fields.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0011_eventcandidate_viability_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0012_nonlocalizedevent_event_subtype.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0013_eventcandidate_healpix_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0014_credibleregion_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0015_eventsequence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0016_externalcoincidence_alter_eventsequence_options_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/migrations/0017_alter_eventsequence_external_coincidence_and_more.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/models.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/models.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/serializers.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/serializers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/signals/handlers.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/css/superevent_vue_app.css`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 00000240: 746c 696e 653a 3270 7820 736f 6c69 6420  tline:2px solid 
 00000250: 2330 6535 3338 657d 2373 7570 6572 6576  #0e538e}#superev
 00000260: 656e 742d 7365 7175 656e 6365 7320 2e6e  ent-sequences .n
 00000270: 6176 2d6c 696e 6b2e 6163 7469 7665 7b63  av-link.active{c
 00000280: 6f6c 6f72 3a23 6666 663b 6261 636b 6772  olor:#fff;backgr
 00000290: 6f75 6e64 2d63 6f6c 6f72 3a23 3065 3533  ound-color:#0e53
 000002a0: 3865 7d23 616c 6572 7473 2d74 6162 6c65  8e}#alerts-table
-000002b0: 5b64 6174 612d 762d 3061 6362 6162 3561  [data-v-0acbab5a
+000002b0: 5b64 6174 612d 762d 3631 6633 3865 6363  [data-v-61f38ecc
 000002c0: 5d7b 6865 6967 6874 3a34 3030 7078 7d0a  ]{height:400px}.
 000002d0: 0a2f 2a21 0a20 2a20 426f 6f74 7374 7261  ./*!. * Bootstra
 000002e0: 7020 7634 2e36 2e32 2028 6874 7470 733a  p v4.6.2 (https:
 000002f0: 2f2f 6765 7462 6f6f 7473 7472 6170 2e63  //getbootstrap.c
 00000300: 6f6d 2f29 0a20 2a20 436f 7079 7269 6768  om/). * Copyrigh
 00000310: 7420 3230 3131 2d32 3032 3220 5468 6520  t 2011-2022 The 
 00000320: 426f 6f74 7374 7261 7020 4175 7468 6f72  Bootstrap Author
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/static/tom_nonlocalizedevents/vue/js/superevent_vue_app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1296,14 +1296,15 @@
                     y: "1 ปี",
                     yy: "%d ปี"
                 }
             });
             return t
         }))
     },
+    1191: function(e, t, a) {},
     "13d2": function(e, t, a) {
         var n = a("d039"),
             r = a("1626"),
             i = a("1a2d"),
             o = a("83ab"),
             s = a("5e77").CONFIGURABLE,
             l = a("8925"),
@@ -1540,15 +1541,14 @@
                     dow: 1,
                     doy: 4
                 }
             });
             return t
         }))
     },
-    "16d2": function(e, t, a) {},
     "1a2d": function(e, t, a) {
         var n = a("e330"),
             r = a("7b0b"),
             i = n({}.hasOwnProperty);
         e.exports = Object.hasOwn || function(e, t) {
             return i(r(e), t)
         }
@@ -8660,15 +8660,15 @@
                     on: {
                         "selected-alert": e.onSelectAlert
                     }
                 })], 1), a("b-col", {
                     attrs: {
                         cols: "4"
                     }
-                }, [a("h3", [e._v("GraceDB BAYESTAR Images")]), a("b-row", [a("b-img-lazy", {
+                }, [a("h3", [e._v("GraceDB BAYESTAR Images")]), e.isBurstEvent ? e._e() : a("b-row", [a("b-img-lazy", {
                     attrs: {
                         src: e.getVolumeImageUrl(e.volume_image = !0),
                         fluid: ""
                     }
                 })], 1), a("b-row", [a("b-img-lazy", {
                     attrs: {
                         src: e.getVolumeImageUrl(e.volume_image = !1),
@@ -8907,15 +8907,15 @@
                 methods: {
                     getTargets(e, t, a) {
                         let n = "";
                         e && (n += "name=" + e), t && a && (n += `&cone_search=${t},${a},5`), r.a.get(`${this.$store.state.tomApiBaseUrl}/api/targets/?${n}`, this.$store.state.tomAxiosConfig).then(e => {
                             this.matches = e["data"]["results"], this.matches = this.matches.filter(e => {
                                 let t = !1;
                                 return this.existingEventCandidates.forEach(a => {
-                                    e.id === a.id && (t = !0)
+                                    e.id === a.target.id && (t = !0)
                                 }), !t
                             })
                         }).catch(e => {
                             console.log(`Unable to retrieve targets: ${e}.`)
                         })
                     },
                     targetFormValid() {
@@ -9085,15 +9085,19 @@
                                     click: e.toggleDetails
                                 }
                             }, [a("b-icon-caret-right")], 1)]
                         }
                     }, {
                         key: "row-details",
                         fn: function(t) {
-                            return [t.item.topic.toUpperCase().includes("circular") ? a("span", [e._v(e._s(t.item.message_text))]) : t.item.topic.toUpperCase().includes("LVC_COUNTERPART") ? a("div", e._l(Object.entries(t.item.data), (function(t) {
+                            return [t.item.topic.toLowerCase().includes("circular") ? a("span", {
+                                staticStyle: {
+                                    "white-space": "pre-wrap"
+                                }
+                            }, [e._v(e._s(t.item.message_text))]) : t.item.topic.toUpperCase().includes("LVC_COUNTERPART") ? a("div", e._l(Object.entries(t.item.data), (function(t) {
                                 var n = t[0],
                                     r = t[1];
                                 return a("dl", {
                                     key: [n, r],
                                     staticClass: "row"
                                 }, [a("dt", {
                                     staticClass: "col-md-3"
@@ -9166,15 +9170,15 @@
                         type: Array,
                         required: !0
                     }
                 },
                 mounted() {},
                 methods: {
                     getAlertUrl(e) {
-                        return `${this.$store.state.hermesApiBaseUrl}/api/v0/messages/${e.id}`
+                        return `${this.$store.state.hermesApiBaseUrl}/api/v0/messages/${e.uuid}`
                     },
                     getAlertsFromAlertData() {
                         return this.alerts.filter(e => "GCN/LVC NOTICE" !== e.title)
                     },
                     getAlertDate(e) {
                         return I()(e.published).format("YYYY-MM-DD hh:mm:ss")
                     },
@@ -9183,15 +9187,15 @@
                     },
                     showRowDetails(e, t, a) {
                         e._showDetails = !e._showDetails
                     }
                 }
             },
             E = F,
-            $ = (a("620a"), C(E, B, Y, !1, null, "0acbab5a", null)),
+            $ = (a("c737"), C(E, B, Y, !1, null, "61f38ecc", null)),
             R = $.exports,
             N = function() {
                 var e = this,
                     t = e.$createElement,
                     a = e._self._c || t;
                 return a("b-container", [a("b-table", {
                     attrs: {
@@ -9558,14 +9562,17 @@
                         messages: [],
                         eventCandidates: [],
                         selectedAlerts: [],
                         superevent_data: {}
                     }
                 },
                 computed: {
+                    isBurstEvent() {
+                        return ["oLIB", "CWB", "mLy"].includes(k.a.get(this.sequence, "details.pipeline", ""))
+                    },
                     hasExternalCoincidence() {
                         return !k.a.isNil(this.sequence.external_coincidence) && !k.a.isEmpty(this.sequence.external_coincidence)
                     },
                     skymapVersion() {
                         return this.hasExternalCoincidence ? k.a.get(this.sequence, "external_coincidence.localization.skymap_version", void 0) : k.a.get(this.sequence, "localization.skymap_version", void 0)
                     },
                     skymapUrl() {
@@ -9594,18 +9601,19 @@
                                 this.sequence.sequence_id.toString() in e["credible_regions"] ? e["credible_region"] = e["credible_regions"][this.sequence.sequence_id.toString()] : e["credible_region"] = 100, this.eventCandidates.push(e)
                             })
                         }).catch(t => {
                             console.log(`getSupereventData: Error getting database data for pk ${this.supereventPk}: ${t}`), this.eventCandidates = e
                         })
                     },
                     getVolumeImageUrl(e = !0) {
-                        let t = "";
-                        t = e ? "bayestar.volume.png" : this.hasExternalCoincidence ? "combined-ext.png" : "bayestar.png";
-                        let a = "https://gracedb.ligo.org/api/superevents/" + this.supereventId + "/files/" + t;
-                        return void 0 !== this.skymapVersion && (a = a + "," + this.skymapVersion), a
+                        let t = k.a.get(this.sequence, "details.pipeline", ""),
+                            a = "";
+                        a = "CWB" == t ? "cwb.png" : "oLIB" == t ? "olib.png" : "mLy" == t ? "mly.png" : e ? "bayestar.volume.png" : this.hasExternalCoincidence ? "combined-ext.png" : "bayestar.png";
+                        let n = "https://gracedb.ligo.org/api/superevents/" + this.supereventId + "/files/" + a;
+                        return void 0 !== this.skymapVersion && (n = n + "," + this.skymapVersion), n
                     },
                     onCreatedCandidates(e) {
                         this.messages.push(`Successfully added ${e} candidates.`), this.getSupereventData()
                     },
                     onSelectAlert(e, t) {
                         !0 === t ? k.a.includes(this.selectedAlerts, e.item) || this.selectedAlerts.push(e.item) : this.selectedAlerts = this.selectedAlerts.filter((function(t) {
                             return t !== e.item
@@ -9635,15 +9643,15 @@
                         console.log("onChangePriority -        row.item.id: " + e.item.id), console.log("onChangePriority -  row.item.priority: " + e.item.priority), console.log("onChangePriority - candidate.priority: " + a.priority), console.log("onChangePriority -              event: " + t), r.a.patch(n, o).then(e => {}).catch(e => {
                             console.error("onChangePriority - url: " + n), console.error("onChangePriority - patch: " + JSON.stringify(o)), console.error(`onChangePriority: Error getting database data for ${JSON.stringify(a)}: ${e}`)
                         }), console.log("after PATCH..."), console.log("onChangePriority - candidate.priority: " + a.priority), console.log("onChangePriority -              event: " + t), console.log()
                     }
                 }
             },
             ce = le,
-            ue = C(ce, A, S, !1, null, "32b2a06c", null),
+            ue = C(ce, A, S, !1, null, "4c1c9402", null),
             de = ue.exports,
             he = {
                 name: "SupereventSequences",
                 props: {
                     superevent: String,
                     hermes_api_url: String,
                     tom_api_url: String
@@ -36634,18 +36642,14 @@
                     dow: 1,
                     doy: 7
                 }
             });
             return t
         }))
     },
-    "620a": function(e, t, a) {
-        "use strict";
-        a("16d2")
-    },
     "62e4": function(e, t) {
         e.exports = function(e) {
             return e.webpackPolyfill || (e.deprecate = function() {}, e.paths = [], e.children || (e.children = []), Object.defineProperty(e, "loaded", {
                 enumerable: !0,
                 get: function() {
                     return e.l
                 }
@@ -52972,14 +52976,18 @@
     c6cd: function(e, t, a) {
         var n = a("da84"),
             r = a("6374"),
             i = "__core-js_shared__",
             o = n[i] || r(i, {});
         e.exports = o
     },
+    c737: function(e, t, a) {
+        "use strict";
+        a("1191")
+    },
     c7aa: function(e, t, a) {
         (function(e, t) {
             t(a("c1df"))
         })(0, (function(e) {
             "use strict";
             //! moment.js locale configuration
             var t = e.defineLocale("he", {
```

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/templates/tom_nonlocalizedevents/index.html`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/tests/factories.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/tests/tests.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/urls.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/urls.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/tom_nonlocalizedevents/views.py` & `tom_nonlocalizedevents-0.7.7/tom_nonlocalizedevents/views.py`

 * *Files identical despite different names*

### Comparing `tom_nonlocalizedevents-0.7.6/PKG-INFO` & `tom_nonlocalizedevents-0.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-nonlocalizedevents
-Version: 0.7.6
+Version: 0.7.7
 Summary: Reusable TOMToolkit app to support gravitational wave superevent and other nonlocalized event EM follow-up observations.
 Home-page: https://github.com/TOMToolkit/tom_nonlocalizedevents
 License: GPL-3.0-only
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science
 Author: TOM Toolkit Project
 Author-email: tomtoolkit@lco.global
 Requires-Python: >=3.8,<3.12
@@ -18,19 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: MOCPy (>=0.12.2)
 Requires-Dist: SQLAlchemy (>=1.4.42)
 Requires-Dist: astropy (>=5.2)
 Requires-Dist: astropy-healpix (>=0.7)
 Requires-Dist: django-filter (>=21.0,<22.0)
@@ -94,15 +90,15 @@
     ```
 
     If `WEBPACK_LOADER` is already defined in your settings, then integrate these values in to it.
 
     Also add the following to your settings if they are not already there, setting whatever default values you need for your setup. These point to your deployed TOM toolkit instance, and to a hermes instance:
     ```python
     TOM_API_URL = os.getenv('TOM_API_URL', 'http://127.0.0.1:8000')
-    HERMES_API_URL = os.getenv('HERMES_API_URL', 'http://hermes-dev.lco.gtn')
+    HERMES_API_URL = os.getenv('HERMES_API_URL', 'https://hermes-dev.lco.global')
 
     ```
 
 3. Include the tom_nonlocalizedevent URLconf in your project `urls.py`:
    ```python
    urlpatterns = [
         ...
```

