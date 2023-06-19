# Comparing `tmp/ahoy_dtu_webthing-0.0.3.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.3.tar", last modified: Mon Jun 19 19:31:24 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.4.tar", last modified: Mon Jun 19 19:55:58 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.3.tar` & `ahoy_dtu_webthing-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:55:58.000000 ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 19:55:45.000000 ahoy_dtu_webthing-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 19:55:58.554858 ahoy_dtu_webthing-0.0.4/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.3/LICENSE` & `ahoy_dtu_webthing-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.3/PKG-INFO` & `ahoy_dtu_webthing-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.3/README.md` & `ahoy_dtu_webthing-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,28 @@
         self.serial = serial
         self.p_dc = 0
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
         self.efficiency = 0
+        self.power_max = 0
         self.power_limit = 0
         self.fetch_date = datetime.now()
         self.listener = None
 
+
     def set_power_limit(self, limit_watt: int):
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
+        response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_persistent_absolute", "val": limit_watt})
         if response.status_code == 200 and response.json()['success'] == True:
             self.power_limit = limit_watt
 
-    def update(self, power_limit: int, p_ac: int, u_ac: int, i_ac: int, p_dc: int, efficiency: int, temp: int):
+    def update(self, power_max: int, power_limit: int, p_ac: int, u_ac: int, i_ac: int, p_dc: int, efficiency: int, temp: int):
+        self.power_max = power_max
         self.power_limit = power_limit
         self.p_ac = p_ac
         self.u_ac = u_ac
         self.i_ac = i_ac
         self.p_dc = p_dc
         self.efficiency = efficiency
         self.temp = temp
@@ -103,15 +107,15 @@
                         elif measure['fld'] == 'P_DC':
                             p_dc = measure['val']
                         elif measure['fld'] == 'Efficiency':
                             efficiency = measure['val']
                         elif measure['fld'] == 'Temp':
                             temp = measure['val']
 
-                    self.inverters[i].update(power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
+                    self.inverters[i].update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
             except Exception as e:
                 print(e)
             sleep(self.interval)
 
     def listen(self):
         Thread(target=self.__periodic_refresh, daemon=True).start()
```

### Comparing `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,26 @@
                      metadata={
                          'title': 'serial',
                          "type": "string",
                          'description': 'The serial number',
                          'readOnly': True,
                      }))
 
+        self.power_max = Value(inverter.power_max)
+        self.add_property(
+            Property(self,
+                     'power_max',
+                     self.power_max,
+                     metadata={
+                         'title': 'power_max',
+                         "type": "integer",
+                         'description': 'The max power [W]',
+                         'readOnly': True,
+                     }))
+
         self.power_limit = Value(inverter.power_limit, inverter.set_power_limit)
         self.add_property(
             Property(self,
                      'power_limit',
                      self.power_limit,
                      metadata={
                          'title': 'power_limit',
@@ -151,14 +163,15 @@
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
         self.efficiency.notify_of_external_update(self.inverter.efficiency)
         self.fetch_date.notify_of_external_update(self.inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
+        self.power_max.notify_of_external_update(self.inverter.power_max)
         self.power_limit.notify_of_external_update(self.inverter.power_limit)
 
 
 def run_server(description: str, port: int, base_uri: str):
     awning_webthings = [InverterWebThing(description, inverter) for inverter in  Dtu(base_uri).connect()]
     server = WebThingServer(MultipleThings(awning_webthings, 'Inverters'), port=port, disable_host_validation=True)
```

### Comparing `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.4/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.3
+Version: 0.0.4
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

