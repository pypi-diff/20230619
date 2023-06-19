# Comparing `tmp/next-bus-bot-1.3.1.tar.gz` & `tmp/next-bus-bot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-bus-bot-1.3.1.tar", last modified: Mon Jun 19 07:22:22 2023, max compression
+gzip compressed data, was "next-bus-bot-1.3.2.tar", last modified: Mon Jun 19 12:11:49 2023, max compression
```

## Comparing `next-bus-bot-1.3.1.tar` & `next-bus-bot-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.github/workflows/linters.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.963070 next-bus-bot-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/src/nbb/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/nbb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/bot_discord.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/idfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-19 07:22:06.000000 next-bus-bot-1.3.1/src/nbb/nbb_conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:22:22.967070 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 07:22:22.000000 next-bus-bot-1.3.1/src/next_bus_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.453782 next-bus-bot-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/.github/workflows/linters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.453782 next-bus-bot-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/src/nbb/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/nbb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/bot_discord.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/idfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-19 12:11:33.000000 next-bus-bot-1.3.2/src/nbb/nbb_conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:11:49.457782 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-19 12:11:49.000000 next-bus-bot-1.3.2/src/next_bus_bot.egg-info/top_level.txt
```

### Comparing `next-bus-bot-1.3.1/.github/workflows/linters.yml` & `next-bus-bot-1.3.2/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/.github/workflows/python-publish.yml` & `next-bus-bot-1.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/LICENSE.txt` & `next-bus-bot-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/PKG-INFO` & `next-bus-bot-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `next-bus-bot-1.3.1/README.rst` & `next-bus-bot-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/pyproject.toml` & `next-bus-bot-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/api_call.py` & `next-bus-bot-1.3.2/src/nbb/api_call.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/bot_discord.py` & `next-bus-bot-1.3.2/src/nbb/bot_discord.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/cli.py` & `next-bus-bot-1.3.2/src/nbb/cli.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/config.py` & `next-bus-bot-1.3.2/src/nbb/config.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/idfm.py` & `next-bus-bot-1.3.2/src/nbb/idfm.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/nbb/models.py` & `next-bus-bot-1.3.2/src/nbb/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,22 +65,35 @@
 
         stop_area_id = _get_value_id(data, "MonitoringRef")
         stop_area_name = call["StopPointName"][0]["value"]
         # TODO Save the mapping stop_area_id -> stop_area_name
         # Or dowload the full dataset from IDFM.
         line_id = _get_value_id(journey, "LineRef")[-1]
         line_name = KNOWN_LINES.get(line_id, line_id)
-        time = None
+
+        # Find the time string and parse it.
+        time_str = None
         for k in ["ExpectedArrivalTime", "ExpectedDepartureTime", "AimedDepartureTime"]:
             try:
-                time = datetime.fromisoformat(call[k])
+                time_str = call[k]
             except KeyError:
                 continue
-        if time is None:
+            else:
+                break
+        if time_str is None:
             raise KeyError("No time found in the data.")
+        try:
+            time = datetime.fromisoformat(time_str)
+        except ValueError as e:
+            # The Z at the end of the time string is not supported by fromisoformat
+            # until 3.11
+            if time_str[-1] == "Z":
+                time = datetime.fromisoformat(time_str[:-1])
+            else:
+                raise e
 
         return cls(
             destination=journey["DestinationName"][0]["value"],
             time=time.astimezone(),
             arrival_status=call["ArrivalStatus"],
             stop_area_name=stop_area_name,
             stop_area_id=stop_area_id,
```

### Comparing `next-bus-bot-1.3.1/src/nbb/nbb_conf.toml` & `next-bus-bot-1.3.2/src/nbb/nbb_conf.toml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.3.1/src/next_bus_bot.egg-info/PKG-INFO` & `next-bus-bot-1.3.2/src/next_bus_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `next-bus-bot-1.3.1/src/next_bus_bot.egg-info/SOURCES.txt` & `next-bus-bot-1.3.2/src/next_bus_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

