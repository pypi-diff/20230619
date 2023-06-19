# Comparing `tmp/ahoy_dtu_webthing-0.0.6.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.6.tar", last modified: Mon Jun 19 20:15:22 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.7.tar", last modified: Mon Jun 19 20:25:51 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.6.tar` & `ahoy_dtu_webthing-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.714604 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.133482 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.6/LICENSE` & `ahoy_dtu_webthing-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.6/PKG-INFO` & `ahoy_dtu_webthing-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.6/README.md` & `ahoy_dtu_webthing-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 
 class Inverter:
 
     def __init__(self, base_uri: str, id: int, channels: int, name: str, serial: str):
         self.update_uri = re.sub("^/|/$", "", base_uri) + '/api/ctrl'
         self.uri = re.sub("^/|/$", "", base_uri) + '/api/record/live'
+        self.index_uri = re.sub("^/|/$", "", base_uri) + '/api/index'
         self.config_uri = re.sub("^/|/$", "", base_uri) + '/api/record/config'
         self.inverter_uri = re.sub("^/|/$", "", base_uri) + '/api/inverter/list'
 
         self.id = id
         self.channel = channels
         self.name = name
         self.serial = serial
@@ -21,60 +22,70 @@
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
         self.fetch_date = datetime.now()
+        self.is_available = False
+        self.is_producing = False
         self.listener = None
         self.refresh()
         self.set_power_limit(self.power_max)
 
     def refresh(self):
-        # fetch power limit
-        response = requests.get(self.config_uri)
-        inverter_configs = response.json()['inverter']
-
-        # fetch inverter info
-        response = requests.get(self.inverter_uri)
-        inverter_infos = response.json()['inverter']
-
-        # fetch temp, power, etc
-        response = requests.get(self.uri)
-        inverter_measures = response.json()['inverter']
-
-        p_ac = 0
-        i_ac = 0
-        u_ac  =0
-        p_dc = 0
-        efficiency = 0
-        temp = 0
-        power_limit = 0
-        power_max = sum(inverter_infos[self.id]['ch_max_pwr'])
-
-        for config in inverter_configs[self.id]:
-            if config['fld'] == 'active_PowerLimit':
-                power_limit_percent = float(config['val'])
-                power_limit = int(power_max * power_limit_percent / 100)
-
-        for measure in inverter_measures[self.id]:
-            if measure['fld'] == 'P_AC':
-                p_ac = measure['val']
-            elif measure['fld'] == 'I_AC':
-                i_ac = measure['val']
-            elif measure['fld'] == 'U_AC':
-                u_ac = measure['val']
-            elif measure['fld'] == 'P_DC':
-                p_dc = measure['val']
-            elif measure['fld'] == 'Efficiency':
-                efficiency = measure['val']
-            elif measure['fld'] == 'Temp':
-                temp = measure['val']
+       # fetch inverter info
+        response = requests.get(self.index_uri)
+        inverter_state = response.json()['inverter']
+
+        self.is_available = inverter_state[self.id]['is_avail']
+        self.is_producing = inverter_state[self.id]['is_producing']
+
+        if self.is_producing:
+            # fetch power limit
+            response = requests.get(self.config_uri)
+            inverter_configs = response.json()['inverter']
+
+            # fetch inverter info
+            response = requests.get(self.inverter_uri)
+            inverter_infos = response.json()['inverter']
+
+            # fetch temp, power, etc
+            response = requests.get(self.uri)
+            inverter_measures = response.json()['inverter']
+
+            p_ac = 0
+            i_ac = 0
+            u_ac  =0
+            p_dc = 0
+            efficiency = 0
+            temp = 0
+            power_limit = 0
+            power_max = sum(inverter_infos[self.id]['ch_max_pwr'])
+
+            for config in inverter_configs[self.id]:
+                if config['fld'] == 'active_PowerLimit':
+                    power_limit_percent = float(config['val'])
+                    power_limit = int(power_max * power_limit_percent / 100)
+
+            for measure in inverter_measures[self.id]:
+                if measure['fld'] == 'P_AC':
+                    p_ac = measure['val']
+                elif measure['fld'] == 'I_AC':
+                    i_ac = measure['val']
+                elif measure['fld'] == 'U_AC':
+                    u_ac = measure['val']
+                elif measure['fld'] == 'P_DC':
+                    p_dc = measure['val']
+                elif measure['fld'] == 'Efficiency':
+                    efficiency = measure['val']
+                elif measure['fld'] == 'Temp':
+                    temp = measure['val']
 
-        self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
+            self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
 
     def set_power_limit(self, limit_watt: int):
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_persistent_absolute", "val": limit_watt})
 
     def update(self, power_max: int, power_limit: int, p_ac: int, u_ac: int, i_ac: int, p_dc: int, efficiency: int, temp: int):
         self.power_max = power_max
```

### Comparing `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,38 @@
                      metadata={
                          'title': 'serial',
                          "type": "string",
                          'description': 'The serial number',
                          'readOnly': True,
                      }))
 
+        self.is_available = Value(inverter.is_available)
+        self.add_property(
+            Property(self,
+                     'is_available',
+                     self.is_available,
+                     metadata={
+                         'title': 'is_available',
+                         "type": "boolean",
+                         'description': 'True, if is available',
+                         'readOnly': True,
+                     }))
+
+        self.is_producing = Value(inverter.is_producing)
+        self.add_property(
+            Property(self,
+                 'is_producing',
+                 self.is_producing,
+                 metadata={
+                     'title': 'is_producing',
+                     "type": "boolean",
+                     'description': 'True, if is producing',
+                     'readOnly': True,
+                 }))
+
         self.power_max = Value(inverter.power_max)
         self.add_property(
             Property(self,
                      'power_max',
                      self.power_max,
                      metadata={
                          'title': 'power_max',
@@ -156,14 +180,16 @@
         self.ioloop = tornado.ioloop.IOLoop.current()
         self.inverter.register_listener(self.on_value_changed)
 
     def on_value_changed(self):
         self.ioloop.add_callback(self.__on_value_changed)
 
     def __on_value_changed(self):
+        self.is_producing.notify_of_external_update(self.inverter.is_producing)
+        self.is_available.notify_of_external_update(self.inverter.is_available)
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
         self.efficiency.notify_of_external_update(self.inverter.efficiency)
         self.fetch_date.notify_of_external_update(self.inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
```

### Comparing `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.6
+Version: 0.0.7
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

