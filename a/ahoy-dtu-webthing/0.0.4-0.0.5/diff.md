# Comparing `tmp/ahoy_dtu_webthing-0.0.4.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.4.tar", last modified: Mon Jun 19 19:55:58 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.5.tar", last modified: Mon Jun 19 20:05:41 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.4.tar` & `ahoy_dtu_webthing-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.001958 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.4/LICENSE` & `ahoy_dtu_webthing-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.4/PKG-INFO` & `ahoy_dtu_webthing-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.4/README.md` & `ahoy_dtu_webthing-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,80 @@
 from threading import Thread
-from typing import List
 import re
 import requests
 from time import sleep
 from datetime import datetime
 
 class Inverter:
 
     def __init__(self, base_uri: str, id: int, channels: int, name: str, serial: str):
         self.update_uri = re.sub("^/|/$", "", base_uri) + '/api/ctrl'
+        self.uri = re.sub("^/|/$", "", base_uri) + '/api/record/live'
+        self.config_uri = re.sub("^/|/$", "", base_uri) + '/api/record/config'
+        self.inverter_uri = re.sub("^/|/$", "", base_uri) + '/api/inverter/list'
+
         self.id = id
         self.channel = channels
         self.name = name
         self.serial = serial
         self.p_dc = 0
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
         self.fetch_date = datetime.now()
         self.listener = None
+        self.refresh()
+        self.set_power_limit(self.power_max)
 
+    def refresh(self):
+        # fetch power limit
+        response = requests.get(self.config_uri)
+        inverter_configs = response.json()['inverter']
+
+        # fetch inverter info
+        response = requests.get(self.inverter_uri)
+        inverter_infos = response.json()['inverter']
+
+        # fetch temp, power, etc
+        response = requests.get(self.uri)
+        inverter_measures = response.json()['inverter']
+
+        p_ac = 0
+        i_ac = 0
+        u_ac  =0
+        p_dc = 0
+        efficiency = 0
+        temp = 0
+        power_limit = 0
+        power_max = sum(inverter_infos[self.id]['ch_max_pwr'])
+
+        for config in inverter_configs[self.id]:
+            if config['fld'] == 'active_PowerLimit':
+                power_limit_percent = float(config['val'])
+                power_limit = int(power_max * power_limit_percent / 100)
+
+        for measure in inverter_measures[self.id]:
+            if measure['fld'] == 'P_AC':
+                p_ac = measure['val']
+            elif measure['fld'] == 'I_AC':
+                i_ac = measure['val']
+            elif measure['fld'] == 'U_AC':
+                u_ac = measure['val']
+            elif measure['fld'] == 'P_DC':
+                p_dc = measure['val']
+            elif measure['fld'] == 'Efficiency':
+                efficiency = measure['val']
+            elif measure['fld'] == 'Temp':
+                temp = measure['val']
+
+        self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
 
     def set_power_limit(self, limit_watt: int):
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_persistent_absolute", "val": limit_watt})
         if response.status_code == 200 and response.json()['success'] == True:
             self.power_limit = limit_watt
 
@@ -55,83 +102,35 @@
                 ", P_DC: " + str(self.p_dc) + ", EFFICIENCY: " + str(self.efficiency) +  ")"
 
     def __repr__(self):
         return  self.__str__()
 
 
 
-class Updater:
+class Dtu:
 
-    def __init__(self, base_uri: str, inverters: List[Inverter], interval: int):
-        self.uri = re.sub("^/|/$", "", base_uri) + '/api/record/live'
-        self.config_uri = re.sub("^/|/$", "", base_uri) + '/api/record/config'
-        self.inverter_uri = re.sub("^/|/$", "", base_uri) + '/api/inverter/list'
-        self.inverters = inverters
-        self.interval = interval
+    def __init__(self, base_uri: str):
+        self.is_running = True
+        self.base_uri = base_uri
+        uri = re.sub("^/|/$", "", self.base_uri) + '/api/inverter/list'
+        response = requests.get(uri)
+        data = response.json()
+        self.interval = int(data['interval'])
+        self.inverters = [Inverter(self.base_uri, entry['id'], entry['channels'], entry['name'], entry['serial']) for entry in data['inverter']]
+        Thread(target=self.__periodic_refresh, daemon=True)
 
     def __periodic_refresh(self):
-        while True:
+        while self.is_running:
             try:
-                # fetch power limit
-                response = requests.get(self.config_uri)
-                inverter_configs = response.json()['inverter']
-
-                # fetch inverter info
-                response = requests.get(self.inverter_uri)
-                inverter_infos = response.json()['inverter']
-
-                # fetch temp, power, etc
-                response = requests.get(self.uri)
-                inverter_measures = response.json()['inverter']
-                for i in range(0, len(inverter_measures)):
-                    p_ac = 0
-                    i_ac = 0
-                    u_ac  =0
-                    p_dc = 0
-                    efficiency = 0
-                    temp = 0
-                    power_limit = 0
-                    power_max = sum(inverter_infos[i]['ch_max_pwr'])
-
-                    for config in inverter_configs[i]:
-                        if config['fld'] == 'active_PowerLimit':
-                            power_limit_percent = float(config['val'])
-                            power_limit = int(power_max * power_limit_percent / 100)
-
-                    for measure in inverter_measures[i]:
-                        if measure['fld'] == 'P_AC':
-                            p_ac = measure['val']
-                        elif measure['fld'] == 'I_AC':
-                            i_ac = measure['val']
-                        elif measure['fld'] == 'U_AC':
-                            u_ac = measure['val']
-                        elif measure['fld'] == 'P_DC':
-                            p_dc = measure['val']
-                        elif measure['fld'] == 'Efficiency':
-                            efficiency = measure['val']
-                        elif measure['fld'] == 'Temp':
-                            temp = measure['val']
-
-                    self.inverters[i].update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
+                for inverter in self.inverters:
+                    inverter.refresh()
             except Exception as e:
                 print(e)
             sleep(self.interval)
 
-    def listen(self):
-        Thread(target=self.__periodic_refresh, daemon=True).start()
-
-
-
-class Dtu:
-
-    def __init__(self, base_uri: str):
-        self.base_uri = base_uri
+    @staticmethod
+    def connect(base_uri: str):
+        return Dtu(base_uri)
 
-    def connect(self) -> List[Inverter]:
-        uri = re.sub("^/|/$", "", self.base_uri) + '/api/inverter/list'
-        response = requests.get(uri)
-        data = response.json()
-        interval = int(data['interval'])
-        inverters = [Inverter(self.base_uri, entry['id'], entry['channels'], entry['name'], entry['serial']) for entry in data['inverter']]
-        Updater(self.base_uri, inverters, interval).listen()
-        return inverters
+    def close(self):
+        self.is_running = False
```

### Comparing `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         self.fetch_date.notify_of_external_update(self.inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
         self.power_max.notify_of_external_update(self.inverter.power_max)
         self.power_limit.notify_of_external_update(self.inverter.power_limit)
 
 
 def run_server(description: str, port: int, base_uri: str):
-    awning_webthings = [InverterWebThing(description, inverter) for inverter in  Dtu(base_uri).connect()]
+    awning_webthings = [InverterWebThing(description, inverter) for inverter in  Dtu.connect(base_uri).inverters]
     server = WebThingServer(MultipleThings(awning_webthings, 'Inverters'), port=port, disable_host_validation=True)
 
     logging.info('running webthing server http://localhost:' + str(port))
     try:
         server.start()
     except KeyboardInterrupt:
         logging.info('stopping webthing server')
```

### Comparing `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

