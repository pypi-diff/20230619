# Comparing `tmp/lasutils-1.0.37-py3-none-any.whl.zip` & `tmp/lasutils-1.0.50-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 11483 bytes, number of entries: 14
+Zip file size: 12948 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 lasutils/__init__.py
--rw-r--r--  2.0 unx    10464 b- defN 20-Feb-02 00:00 lasutils/api_poller.py
+-rw-r--r--  2.0 unx    10626 b- defN 20-Feb-02 00:00 lasutils/api_poller.py
 -rw-r--r--  2.0 unx     1334 b- defN 20-Feb-02 00:00 lasutils/connector.py
 -rw-r--r--  2.0 unx     2164 b- defN 20-Feb-02 00:00 lasutils/deserializer.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 lasutils/exceptions.py
--rw-r--r--  2.0 unx     2850 b- defN 20-Feb-02 00:00 lasutils/helpers.py
+-rw-r--r--  2.0 unx     3950 b- defN 20-Feb-02 00:00 lasutils/helpers.py
 -rw-r--r--  2.0 unx     2362 b- defN 20-Feb-02 00:00 lasutils/keyvault.py
--rw-r--r--  2.0 unx     7641 b- defN 20-Feb-02 00:00 lasutils/las_api.py
+-rw-r--r--  2.0 unx    10359 b- defN 20-Feb-02 00:00 lasutils/las_api.py
+-rw-r--r--  2.0 unx     1056 b- defN 20-Feb-02 00:00 lasutils/my_ffmpeg.py
 -rw-r--r--  2.0 unx     1588 b- defN 20-Feb-02 00:00 lasutils/serializer.py
 -rw-r--r--  2.0 unx      444 b- defN 20-Feb-02 00:00 lasutils/settings.py
 -rw-r--r--  2.0 unx     1025 b- defN 20-Feb-02 00:00 lasutils/variable_parser.py
-?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.37.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.37.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1070 b- defN 20-Feb-02 00:00 lasutils-1.0.37.dist-info/RECORD
-14 files, 31791 bytes uncompressed, 9731 bytes compressed:  69.4%
+?rw-r--r--  2.0 unx      650 b- defN 20-Feb-02 00:00 lasutils-1.0.50.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 lasutils-1.0.50.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1149 b- defN 20-Feb-02 00:00 lasutils-1.0.50.dist-info/RECORD
+15 files, 36906 bytes uncompressed, 11078 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -18,26 +18,29 @@
 
 Filename: lasutils/keyvault.py
 Comment: 
 
 Filename: lasutils/las_api.py
 Comment: 
 
+Filename: lasutils/my_ffmpeg.py
+Comment: 
+
 Filename: lasutils/serializer.py
 Comment: 
 
 Filename: lasutils/settings.py
 Comment: 
 
 Filename: lasutils/variable_parser.py
 Comment: 
 
-Filename: lasutils-1.0.37.dist-info/METADATA
+Filename: lasutils-1.0.50.dist-info/METADATA
 Comment: 
 
-Filename: lasutils-1.0.37.dist-info/WHEEL
+Filename: lasutils-1.0.50.dist-info/WHEEL
 Comment: 
 
-Filename: lasutils-1.0.37.dist-info/RECORD
+Filename: lasutils-1.0.50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lasutils/api_poller.py

```diff
@@ -48,14 +48,15 @@
         self.set_header_field("Cache-Control", "no-cache")
         self.set_header_field("site-id", "BACKOFFICE")
         self.set_header_field(
             "User-Agent",
             "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         )
         self._token = None
+        self._session = requests.Session()
 
     @abstractmethod
     def poll(self, resource: str, fail_retry_time: int = 0, data_path: str = ""):
         pass
 
     def deserialize(self, data: str = "", data_path: str = ""):
         return self._deserializer.deserialize(data, data_path)
@@ -73,15 +74,15 @@
         if self._token:
             return self._token
 
         payload = self._auth_config.get(CONF_API_AUTH_PAYLOAD)
         content_type = self._auth_config.get(CONF_API_AUTH_CONTENT_TYPE)
         self.set_header_field("Content-Type", f"application/{content_type}")
 
-        r = requests.post(
+        r = self._session.post(
             f"{self._auth_config.get(CONF_API_AUTH_TOKEN_URL)}",
             headers=self.get_header(),
             data=payload if content_type != "json" else json.dumps(payload),
         )
         r.raise_for_status()
         self._token = r.json().get(self._auth_config.get(CONF_API_AUTH_TOKEN_NAME))
         return self._token
@@ -106,26 +107,26 @@
             self.set_header_field(
                 "Content-Type", f"application/{self._api_config.get(CONF_API_FORMAT)}"
             )
             self.set_header_field(
                 "Accept", f"application/{self._api_config.get(CONF_API_FORMAT)}"
             )
 
-            resp = requests.post(
+            resp = self._session.post(
                 url, headers=self.get_header(), data=json.dumps(payload), timeout=180
             )
 
             resp.raise_for_status()
             if resp.status_code == 204:
                 logger.info("Got 204 (NoContent) back from API call.")
                 return
             logger.debug(f"POST response was: {resp.status_code}.")
             return resp.status_code
 
-        except HTTPError as err:
+        except Exception as err:
             logger.error(
                 f"POST request failed: {err}. Will retry in {fail_retry_time} seconds."
             )
             if fail_retry_time == 0:
                 return
             sleep(fail_retry_time)
             self.post(resource, fail_retry_time, payload=payload)
@@ -152,34 +153,37 @@
             self.set_header_field(
                 "Content-Type", f"application/{self._api_config.get(CONF_API_FORMAT)}"
             )
             self.set_header_field(
                 "Accept", f"application/{self._api_config.get(CONF_API_FORMAT)}"
             )
 
-            resp = requests.get(
+            resp = self._session.get(
                 url, headers=self.get_header(), params=params, timeout=180
             )
 
             resp.raise_for_status()
             if resp.status_code == 204:
                 logger.info("Got 204 (NoContent) back from API call.")
                 return
             # Deserialize response
             deserialized = self.deserialize(resp.text, data_path)
             logger.debug(f"GET response deserialized data: {deserialized}.")
             return deserialized
-        except HTTPError as err:
-            logger.error(
-                f"GET request failed: {err}. Will retry in {fail_retry_time} seconds."
-            )
+
+        except Exception as err:
             if fail_retry_time == 0:
+                logger.error(f"GET request failed: {err}.")
                 return
-            sleep(fail_retry_time)
-            self.poll(resource, fail_retry_time, data_path, params)
+            else:
+                logger.error(
+                    f"GET request failed: {err}. Will retry in {fail_retry_time} seconds."
+                )
+                sleep(fail_retry_time)
+                self.poll(resource, fail_retry_time, data_path, params)
 
 
 # SOAP implementation of API poller class.
 # TODO: Add warnings if SOAP settings not set
 class SoapPoller(ApiPoller):
     def __init__(self, auth_config: dict, api_config: dict):
         super().__init__(auth_config, api_config)
@@ -245,15 +249,15 @@
         if not url:
             url = self._api_config.get(CONF_API_BASEURL)
 
         try:
             # POST request
             logger.debug(f"Posting request to {url}.")
             self.set_header_field("Authorization", f"Bearer {self.get_token()}")
-            resp = requests.post(
+            resp = self._session.post(
                 url, headers=self.get_header(), data=self._get_soap_body(), timeout=180
             )
             logger.debug(f"Post response code: {resp.status_code}.")
             logger.debug(f"Post response full data: {resp.text}.")
             resp.raise_for_status()
             if resp.status_code == 204:
                 logger.info("Got 204 (NoContent) back from API call.")
```

## lasutils/helpers.py

```diff
@@ -4,14 +4,16 @@
 import os
 from pathlib import Path
 from typing import Union, Dict, List, Callable
 from dateutil.parser import parse, ParserError
 import time
 from lasutils.exceptions import MissingEnvironmentVariable, ErroneousEnvironmentVariable
 
+log = logging.getLogger()
+
 
 def get_env(
     env_var: str,
     default=None,
     required: bool = False,
     valid_options: list = None,
     is_path: bool = False,
@@ -81,19 +83,51 @@
     return hashlib.md5(json.dumps(item).encode("utf-8")).hexdigest()
 
 
 # do_every(1,<function>,<args>)
 def do_every(period, f, *args):
     def g_tick():
         t = time.time()
+        count = 0
         while True:
             t += period
-            yield max(t - time.time(), 0)
+            count += period
+            yield max(t - time.time(), 0), count
 
     g = g_tick()
     while True:
         try:
-            time.sleep(next(g))
-            f(*args)
+            sleep_time, count = next(g)
+            time.sleep(sleep_time)
+            # time.sleep(next(g))
+            f(count, *args)
         except KeyboardInterrupt:
             logging.info(f"Time loop interrupted.")
             break
+
+
+class ColorFormatter(logging.Formatter):
+    """Logging Formatter to add colors and count warning / errors"""
+
+    grey = "\x1b[90m"
+    green = "\x1b[92m"
+    yellow = "\x1b[93m"
+    red = "\x1b[91m"
+    reset = "\x1b[0m"
+    format = "%(asctime)s | %(levelname)-5.5s | %(module)-12.12s | %(message)s"
+
+    FORMATS = {
+        logging.DEBUG: grey + format + reset,
+        logging.INFO: reset + format + reset,
+        logging.WARNING: yellow + format + reset,
+        logging.ERROR: red + format + reset,
+        logging.CRITICAL: red + format + reset,
+    }
+
+    def format(self, record):
+        record.levelname = "WARN" if record.levelname == "WARNING" else record.levelname
+        record.levelname = (
+            "ERROR" if record.levelname == "CRITICAL" else record.levelname
+        )
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt)
+        return formatter.format(record)
```

## lasutils/las_api.py

```diff
@@ -95,41 +95,107 @@
                 )
                 result.extend(batch)
                 log.info(f"Polled {len(result)} items")
             return result
 
     # --- API ---
     # Broadcast
-    def get_broadcasts(self, start_from: datetime, start_to: datetime):
+    def get_broadcasts(
+        self,
+        start_from: datetime = None,
+        start_to: datetime = None,
+        comp_id: str = None,
+    ):
+        sf = self._get_api_time_format(start_from) if start_from else None
+        st = self._get_api_time_format(start_to) if start_to else None
         params = {
             API_SITE_ID: self._site_id,
-            "start-from": self._get_api_time_format(start_from),
-            "start-to": self._get_api_time_format(start_to),
+            "start-from": sf,
+            "start-to": st,
+            "competition-id": comp_id,
+            "hide-cancelled": True,
         }
-        return self.poll("broadcast", params=params)
+        return self.poll("broadcast", params=params, page_size=200)
+
+    def get_broadcast_by_id(self, broadcast_id: str):
+        params = {
+            # API_SITE_ID: self._site_id,
+            "broadcastId": broadcast_id,
+        }
+        return self.poll("broadcast/internal", params=params)
 
     def get_broadcast_by_ext_id(self, match_id: str):
         params = {
             API_SITE_ID: self._site_id,
             "external-broadcast-id": match_id,
         }
         return self.poll("broadcast", params=params)
 
-    def get_broadcast_by_id(self, broadcast_id: str):
+    def get_broadcast(self, broadcast_id: str):
         params = {
             API_SITE_ID: self._site_id,
-            "broadcastId": broadcast_id,
         }
-        return self.poll("broadcast/internal", params=params)
+        return self.poll(f"broadcast/{broadcast_id}", params=params)
 
-    def get_broadcast(self, broadcast_id: str):
+    # Lineup
+    def get_line_up(self, broadcast_id: str):
         params = {
             API_SITE_ID: self._site_id,
+            "broadcast-id": broadcast_id,
         }
-        return self.poll(f"broadcast/{broadcast_id}", params=params)
+        return self.poll("match-event/lineup", params=params)
+
+    # https://api.livearenasports.com/match-event/?broadcast-id=640825720ee95b4a16dcae35&site-id=SIF
+    # Match events
+    def get_match_events(self, broadcast_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+            "broadcast-id": broadcast_id,
+        }
+        return self.poll("match-event", params=params)
+
+    # def get_match_event_standings(self, start_date: str, competition_id: str):
+    #     params = {
+    #         API_SITE_ID: self._site_id,
+    #         "start_date": start_date,
+    #         "competition_id": competition_id,
+    #     }
+    #     return self.poll("match-event/standings", params=params)
+
+    def get_match_event_standing(self, broadcast_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+        }
+        return self.poll(f"match-event/{broadcast_id}/standing", params=params)
+
+    def get_match_event_clock(self, broadcast_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+            "broadcast-id": broadcast_id,
+        }
+        return self.poll(f"match-event/clock-info", params=params)
+
+    def get_officials(self, broadcast_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+            "broadcast-id": broadcast_id,
+        }
+        officials = self.poll(f"match-event/officials", params=params)
+        return officials[0] if officials else None
+
+    # Logs
+    def get_status_logs(self, broadcast_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+            "broadcast-id": broadcast_id,
+            "type": "INFO",
+        }
+        return self.poll(
+            f"scheduler-broadcast/status-log", params=params, page_size=100
+        )
 
     # Video
     def get_video(self, id: str):
         params = {
             API_SITE_ID: self._site_id,
         }
         return self.poll(f"broadcast/video/{id}", params=params)
@@ -147,15 +213,15 @@
             "sort-column": "start",
             "sort-order": "Descending",
         }
         try:
             self._poller.set_header_field("site-id", self._site_id)
             result = self.poll(f"broadcast/download-list", params=params, page_size=25)
         except Exception as err:
-            self._poller.äset_header_field("site-id", "BACKOFFICE")
+            self._poller.set_header_field("site-id", "BACKOFFICE")
             log.error(f"Failed to get download list. Error: {err}")
 
     def get_download_access_token(self, competition_id: str):
         params = {
             "target-id": competition_id,
             "target": "COMP",
         }
@@ -167,14 +233,25 @@
             "target": "COMP",
             "note": f"Python SDK ({settings.LAS_USER})",
             "anonymous": "true",
             "siteId": self._site_id,
         }
         return self.post(f"user/access-token", payload=data)
 
+    # Competition/table
+    def get_table(self, competition_id: str):
+        params = {
+            API_SITE_ID: self._site_id,
+            "competition-id": competition_id,
+            # "competition-id": "641ad0d11004dd5827fa5158",
+            "sort-column": "created",
+            "sort-order": "Descending",
+        }
+        return self.poll(f"competition/table", params=params)
+
     # Venue
     def get_venue(self, venue_id: str):
         params = {
             API_SITE_ID: self._site_id,
         }
         return self.poll(f"venue/{venue_id}", params=params)
 
@@ -205,14 +282,20 @@
     # Groups
     def get_groups(self):
         params = {
             API_SITE_ID: self._site_id,
         }
         return self.poll("group", params=params)
 
+    def get_group(self, group_id):
+        params = {
+            # API_SITE_ID: self._site_id,
+        }
+        return self.poll(f"group/{group_id}", params=params)
+
     # Payment
     def get_payment_config(self):
         params = {
             API_SITE_ID: self._site_id,
         }
         return self.poll(f"payment/v2/config", params=params)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `lasutils-1.0.37.dist-info/METADATA` & `lasutils-1.0.50.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lasutils
-Version: 1.0.37
+Version: 1.0.50
 Summary: LAS utils
 Project-URL: Homepage, https://livearenasports.com/
 Author-email: Johan Gustavsson <johan.gustavsson@sportway.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

## Comparing `lasutils-1.0.37.dist-info/RECORD` & `lasutils-1.0.50.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 lasutils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lasutils/api_poller.py,sha256=1ZzZQzp4_vYWIp2AjwSPt7HwIgnKQHL9Eu5C6Ij4MD8,10464
+lasutils/api_poller.py,sha256=7kTuoqFnJ4dQYrWqnX9HkSJexkrNmjmrhushbkO_F6E,10626
 lasutils/connector.py,sha256=r11Our5-Lk1xDhumbGYkUzsRSM5yXuam-1insi5KTtw,1334
 lasutils/deserializer.py,sha256=1_vh9iq_G5VFbgePd1doK6EMoblPw955WtsgWA6jvhY,2164
 lasutils/exceptions.py,sha256=Zhxtn9PUSiU6aDf5x-yxiWI7gpKWA9oYbrsrOJR_Dd0,112
-lasutils/helpers.py,sha256=qnlZbtMs-KUTrVFsjf_jiEOAQeS2Ecb-TabZJOnjJgg,2850
+lasutils/helpers.py,sha256=NsqFhTs3sbxPBR-nfFGZM1JUUX2MEuppPB34tZrXg7s,3950
 lasutils/keyvault.py,sha256=gS4MheMfHQ_nIkoCgEWn6vxqqF29k77nh9qH-74xZMY,2362
-lasutils/las_api.py,sha256=UnLA8SEhSp4nOwi64ceE5OkBbL9SbW3UoXzxj9ZfNg0,7641
+lasutils/las_api.py,sha256=qTceCxcJuyDXlnk8PGUWRIHbbzvIgDPzZeVl8wjohaE,10359
+lasutils/my_ffmpeg.py,sha256=vYQcpHb4X49LggfLk57QQAXZ06SUqadD1Ar-Cu_HhS0,1056
 lasutils/serializer.py,sha256=WUy6wadA_JJhWCBXuz-mJFhJRh-S9UVD2baTVzVXMus,1588
 lasutils/settings.py,sha256=fOMLXf0kBYaqdMJ9_sBjsu50XVdwi2k_AGMP7Zl0WiQ,444
 lasutils/variable_parser.py,sha256=Mt02n0wIbSO3OZwFKnDDsraDO1qhz6bpfk78ZJ002fc,1025
-lasutils-1.0.37.dist-info/METADATA,sha256=Q_ahsiQ7Yh5rKnNKk_HMCTzN2sCMbLP5SRlEcbmryME,650
-lasutils-1.0.37.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
-lasutils-1.0.37.dist-info/RECORD,,
+lasutils-1.0.50.dist-info/METADATA,sha256=pC0T6_YnJi4Y-OzcdxEJOGoGqRCCy8YNBFqojmlAx2I,650
+lasutils-1.0.50.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+lasutils-1.0.50.dist-info/RECORD,,
```

