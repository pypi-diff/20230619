# Comparing `tmp/ahoy_dtu_webthing-0.0.5.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.5.tar", last modified: Mon Jun 19 20:05:41 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.6.tar", last modified: Mon Jun 19 20:15:22 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.5.tar` & `ahoy_dtu_webthing-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.001958 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:05:40.000000 ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:05:28.000000 ahoy_dtu_webthing-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:05:41.005958 ahoy_dtu_webthing-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.714604 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:15:22.000000 ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:14:54.000000 ahoy_dtu_webthing-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:15:22.718604 ahoy_dtu_webthing-0.0.6/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.5/LICENSE` & `ahoy_dtu_webthing-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.5/PKG-INFO` & `ahoy_dtu_webthing-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.5
+Version: 0.0.6
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.5/README.md` & `ahoy_dtu_webthing-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,14 @@
                 temp = measure['val']
 
         self.update(power_max, power_limit, p_ac, u_ac, i_ac, p_dc, efficiency, temp)
 
     def set_power_limit(self, limit_watt: int):
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_nonpersistent_absolute", "val": limit_watt})
         response = requests.post(self.update_uri, json={"id": self.id, "cmd": "limit_persistent_absolute", "val": limit_watt})
-        if response.status_code == 200 and response.json()['success'] == True:
-            self.power_limit = limit_watt
 
     def update(self, power_max: int, power_limit: int, p_ac: int, u_ac: int, i_ac: int, p_dc: int, efficiency: int, temp: int):
         self.power_max = power_max
         self.power_limit = power_limit
         self.p_ac = p_ac
         self.u_ac = u_ac
         self.i_ac = i_ac
```

### Comparing `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.5/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.6/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.5
+Version: 0.0.6
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

