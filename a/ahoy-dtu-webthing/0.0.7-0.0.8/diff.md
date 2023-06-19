# Comparing `tmp/ahoy_dtu_webthing-0.0.7.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.7.tar", last modified: Mon Jun 19 20:25:51 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.8.tar", last modified: Mon Jun 19 20:31:18 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.7.tar` & `ahoy_dtu_webthing-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.133482 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:25:51.000000 ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:25:36.000000 ahoy_dtu_webthing-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:25:51.137482 ahoy_dtu_webthing-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:31:18.800286 ahoy_dtu_webthing-0.0.8/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.7/LICENSE` & `ahoy_dtu_webthing-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.7/PKG-INFO` & `ahoy_dtu_webthing-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.7/README.md` & `ahoy_dtu_webthing-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
-        self.fetch_date = datetime.now()
+        self.last_update = datetime.now()
         self.is_available = False
         self.is_producing = False
         self.listener = None
         self.refresh()
         self.set_power_limit(self.power_max)
 
     def refresh(self):
@@ -92,15 +92,15 @@
         self.power_limit = power_limit
         self.p_ac = p_ac
         self.u_ac = u_ac
         self.i_ac = i_ac
         self.p_dc = p_dc
         self.efficiency = efficiency
         self.temp = temp
-        self.fetch_date = datetime.now()
+        self.last_update = datetime.now()
         self.__notify_Listener()
 
     def register_listener(self, listener):
         self.listener = listener
 
     def __notify_Listener(self):
         if self.listener is not None:
```

### Comparing `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,23 @@
             ('Inverter ' + inverter.name).strip(),
             ['MultiLevelSensor'],
             description
         )
 
         self.inverter = inverter
 
-        self.fetch_date = Value(inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
+        self.last_update = Value(inverter.last_update.strftime("%Y-%m-%dT%H:%M:%S"))
         self.add_property(
             Property(self,
-                     'fetch_date',
-                     self.fetch_date,
+                     'last_update',
+                     self.last_update,
                      metadata={
-                         'title': 'fetch_date',
+                         'title': 'last_update',
                          "type": "string",
-                         'description': 'The date [ISO DateTime]',
+                         'description': 'The last update [ISO DateTime]',
                          'readOnly': True,
                      }))
 
         self.name = Value(inverter.name)
         self.add_property(
             Property(self,
                      'name',
@@ -187,15 +187,15 @@
         self.is_producing.notify_of_external_update(self.inverter.is_producing)
         self.is_available.notify_of_external_update(self.inverter.is_available)
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
         self.efficiency.notify_of_external_update(self.inverter.efficiency)
-        self.fetch_date.notify_of_external_update(self.inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
+        self.last_update.notify_of_external_update(self.inverter.last_update.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
         self.power_max.notify_of_external_update(self.inverter.power_max)
         self.power_limit.notify_of_external_update(self.inverter.power_limit)
 
 
 def run_server(description: str, port: int, base_uri: str):
     awning_webthings = [InverterWebThing(description, inverter) for inverter in  Dtu.connect(base_uri).inverters]
```

### Comparing `ahoy_dtu_webthing-0.0.7/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

