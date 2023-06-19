# Comparing `tmp/ahoy_dtu_webthing-0.0.2.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.2.tar", last modified: Mon Jun 19 19:20:10 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.3.tar", last modified: Mon Jun 19 19:31:24 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.2.tar` & `ahoy_dtu_webthing-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:20:10.403553 ahoy_dtu_webthing-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:20:10.403553 ahoy_dtu_webthing-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:20:10.403553 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:20:10.403553 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:20:10.000000 ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 19:19:58.000000 ahoy_dtu_webthing-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 19:20:10.407553 ahoy_dtu_webthing-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:31:24.000000 ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 19:31:07.000000 ahoy_dtu_webthing-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 19:31:24.870229 ahoy_dtu_webthing-0.0.3/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.2/LICENSE` & `ahoy_dtu_webthing-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.2/PKG-INFO` & `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ahoy_dtu_webthing
-Version: 0.0.2
+Name: ahoy-dtu-webthing
+Version: 0.0.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.2/README.md` & `ahoy_dtu_webthing-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.3/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         self.p_dc.notify_of_external_update(self.inverter.p_dc)
         self.p_ac.notify_of_external_update(self.inverter.p_ac)
         self.i_ac.notify_of_external_update(self.inverter.i_ac)
         self.u_ac.notify_of_external_update(self.inverter.u_ac)
         self.efficiency.notify_of_external_update(self.inverter.efficiency)
         self.fetch_date.notify_of_external_update(self.inverter.fetch_date.strftime("%Y-%m-%dT%H:%M:%S"))
         self.temp.notify_of_external_update(self.inverter.temp)
+        self.power_limit.notify_of_external_update(self.inverter.power_limit)
 
 
 def run_server(description: str, port: int, base_uri: str):
     awning_webthings = [InverterWebThing(description, inverter) for inverter in  Dtu(base_uri).connect()]
     server = WebThingServer(MultipleThings(awning_webthings, 'Inverters'), port=port, disable_host_validation=True)
 
     logging.info('running webthing server http://localhost:' + str(port))
```

### Comparing `ahoy_dtu_webthing-0.0.2/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ahoy-dtu-webthing
-Version: 0.0.2
+Name: ahoy_dtu_webthing
+Version: 0.0.3
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

