# Comparing `tmp/next-bus-bot-1.3.0.tar.gz` & `tmp/next-bus-bot-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-bus-bot-1.3.0.tar", last modified: Sun Jun 18 13:23:04 2023, max compression
+gzip compressed data, was "next-bus-bot-1.3.1.tar", last modified: Mon Jun 19 07:22:22 2023, max compression
```

## Comparing `next-bus-bot-1.3.0.tar` & `next-bus-bot-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.526615 next-bus-bot-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.530615 next-bus-bot-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.github/workflows/linters.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.526615 next-bus-bot-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.530615 next-bus-bot-1.3.0/src/nbb/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/nbb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/bot_discord.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/idfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/nbb_conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.github/workflows/linters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/src/nbb/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/nbb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/bot_discord.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/idfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/nbb_conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/top_level.txt
```

### Comparing `next-bus-bot-1.3.0/.github/workflows/linters.yml` & `next-bus-bot-1.3.1/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/.github/workflows/python-publish.yml` & `next-bus-bot-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/LICENSE.txt` & `next-bus-bot-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/PKG-INFO` & `next-bus-bot-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.3.0
+Version: 1.3.1
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `next-bus-bot-1.3.0/README.rst` & `next-bus-bot-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/pyproject.toml` & `next-bus-bot-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/nbb/api_call.py` & `next-bus-bot-1.3.1/src/nbb/api_call.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/nbb/bot_discord.py` & `next-bus-bot-1.3.1/src/nbb/bot_discord.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/nbb/cli.py` & `next-bus-bot-1.3.1/src/nbb/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # /usr/bin/env python3
 """
 CLI frontend.
 """
 import argparse
-import datetime
 
-from nbb.api_call import get_next_passes
-from nbb.config import get_config, get_stop_infos
+from nbb.config import get_config
 
 from nbb.models import get_message
 
 
 def parser():
     """Initialize parser."""
     parser = argparse.ArgumentParser()
```

### Comparing `next-bus-bot-1.3.0/src/nbb/config.py` & `next-bus-bot-1.3.1/src/nbb/config.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/nbb/idfm.py` & `next-bus-bot-1.3.1/src/nbb/idfm.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/nbb/models.py` & `next-bus-bot-1.3.1/src/nbb/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,26 @@
 
         stop_area_id = _get_value_id(data, "MonitoringRef")
         stop_area_name = call["StopPointName"][0]["value"]
         # TODO Save the mapping stop_area_id -> stop_area_name
         # Or dowload the full dataset from IDFM.
         line_id = _get_value_id(journey, "LineRef")[-1]
         line_name = KNOWN_LINES.get(line_id, line_id)
+        time = None
+        for k in ["ExpectedArrivalTime", "ExpectedDepartureTime", "AimedDepartureTime"]:
+            try:
+                time = datetime.fromisoformat(call[k])
+            except KeyError:
+                continue
+        if time is None:
+            raise KeyError("No time found in the data.")
+
         return cls(
             destination=journey["DestinationName"][0]["value"],
-            time=datetime.fromisoformat(call["ExpectedArrivalTime"]).astimezone(),
+            time=time.astimezone(),
             arrival_status=call["ArrivalStatus"],
             stop_area_name=stop_area_name,
             stop_area_id=stop_area_id,
             line_id=line_id,
             line_name=line_name,
         )
 
@@ -90,15 +99,18 @@
 
         if compact:
             destination = "".join(
                 [i for i in self.destination if i.isnumeric() or i.isupper()]
             )
             time_str = self.time.astimezone().strftime("%H:%M")
         else:
-            time_str = f"{self.delta_time.seconds // 60:>2}min. ({self.time.strftime('%H:%M')})"
+            time_str = (
+                f"{self.delta_time.seconds // 60:>2}min."
+                f"({self.time.strftime('%H:%M')})"
+            )
             destination = self.destination
 
         if pretty:
             # bus_pretty_name = "".join([NUM2EMOJI.get(i, "") for i in self.line_name])
             # return f"⏰ {time_str} {bus_pretty_name: <{padding}} 🚍▶ {destination}"
             return f"{time_str} 🚍 ▶ {destination} [{self.line_name}]"
 
@@ -139,15 +151,18 @@
         "StopMonitoringDelivery",
         0,
         "MonitoredStopVisit",
     ]:
         monit_list = monit_list[f]
 
     for monitored in monit_list:
-        next_passes.append(NextPass.from_v2(monitored))
+        try:
+            next_passes.append(NextPass.from_v2(monitored))
+        except KeyError:
+            print(monitored)
     return next_passes
 
 
 def get_message(conf, stop_name, simple=False, compact=False, padding=5):
     """Returns a message from a list of NextPass objects."""
 
     stop_full_name, stop_code, filters = get_stop_infos(conf, stop_name)
```

### Comparing `next-bus-bot-1.3.0/src/nbb/nbb_conf.toml` & `next-bus-bot-1.3.1/src/nbb/nbb_conf.toml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.0/src/next_bus_bot.egg-info/PKG-INFO` & `next-bus-bot-1.3.1/src/next_bus_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.3.0
+Version: 1.3.1
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `next-bus-bot-1.3.0/src/next_bus_bot.egg-info/SOURCES.txt` & `next-bus-bot-1.3.1/src/next_bus_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

