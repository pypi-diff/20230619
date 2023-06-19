# Comparing `tmp/remotivelabs_cli-0.0.1a2.tar.gz` & `tmp/remotivelabs_cli-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a2.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a3.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a2.tar` & `remotivelabs_cli-0.0.1a3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a2/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a2/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a2/cli/__init__.py
--rw-r--r--   0        0        0     3392 2023-06-09 09:05:12.660223 remotivelabs_cli-0.0.1a2/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a2/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3675 2023-06-09 11:46:02.064612 remotivelabs_cli-0.0.1a2/cli/cloud/auth.py
--rw-r--r--   0        0        0     2284 2023-05-30 06:23:51.161239 remotivelabs_cli-0.0.1a2/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1691 2023-06-08 05:58:07.097588 remotivelabs_cli-0.0.1a2/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3153 2022-10-25 11:06:37.541648 remotivelabs_cli-0.0.1a2/cli/cloud/configs.py
--rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a2/cli/cloud/recordings.py
--rw-r--r--   0        0        0     2861 2023-06-09 09:54:06.620182 remotivelabs_cli-0.0.1a2/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1580 2023-06-09 11:33:01.362939 remotivelabs_cli-0.0.1a2/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1251 2023-06-08 05:57:20.045566 remotivelabs_cli-0.0.1a2/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a2/cli/lib/__about__.py
--rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a2/cli/lib/broker.py
--rw-r--r--   0        0        0      342 2023-06-18 17:02:58.041218 remotivelabs_cli-0.0.1a2/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a2/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a2/cli/test/test_simple.py
--rw-r--r--   0        0        0      535 2023-06-19 12:45:41.156706 remotivelabs_cli-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a3/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a3/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a3/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-06-19 13:36:54.800059 remotivelabs_cli-0.0.1a3/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a3/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3675 2023-06-09 11:46:02.064612 remotivelabs_cli-0.0.1a3/cli/cloud/auth.py
+-rw-r--r--   0        0        0     2284 2023-05-30 06:23:51.161239 remotivelabs_cli-0.0.1a3/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1605 2023-06-19 13:52:07.761595 remotivelabs_cli-0.0.1a3/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3132 2023-06-19 13:52:07.776885 remotivelabs_cli-0.0.1a3/cli/cloud/configs.py
+-rw-r--r--   0        0        0     6887 2023-06-19 12:26:04.278978 remotivelabs_cli-0.0.1a3/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     2861 2023-06-09 09:54:06.620182 remotivelabs_cli-0.0.1a3/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1580 2023-06-09 11:33:01.362939 remotivelabs_cli-0.0.1a3/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1176 2023-06-19 13:50:30.024795 remotivelabs_cli-0.0.1a3/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a3/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a3/cli/lib/broker.py
+-rw-r--r--   0        0        0      292 2023-06-19 13:37:13.805682 remotivelabs_cli-0.0.1a3/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a3/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a3/cli/test/test_simple.py
+-rw-r--r--   0        0        0      535 2023-06-19 13:52:43.274331 remotivelabs_cli-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a3/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a2/README.md` & `remotivelabs_cli-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/brokers.py` & `remotivelabs_cli-0.0.1a3/cli/brokers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,93 @@
 import json
-import time
-import typer
-#import network
-from .lib.broker import Broker
-#from network import MDNS
-
-
-import argparse
-import logging
 from time import sleep
-from typing import cast
 
+import typer
 from zeroconf import (
     IPVersion,
     ServiceBrowser,
     ServiceStateChange,
     Zeroconf,
-    ZeroconfServiceTypes,
 )
 
-app = typer.Typer()
-
+from .lib.broker import Broker
 
+app = typer.Typer()
 
 
 @app.command(help="List signals on broker")
 def signals(
         url: str = typer.Option(..., help="Broker URL", envvar='REMOTIVE_BROKER_URL'),
         api_key: str = typer.Option("offline", help="Cloud Broker API-KEY", envvar='REMOTIVE_BROKER_API_KEY')
 ):
     broker = Broker(url, api_key)
-    print("Listing available signals")
+    # print("Listing available signals")
     available_signals = broker.list_signal_names()
     print(json.dumps(available_signals))
 
 
 @app.command(help="List namespaces on broker")
 def namespaces(
         url: str = typer.Option(..., help="Broker URL", envvar='REMOTIVE_BROKER_URL'),
         api_key: str = typer.Option("offline", help="Cloud Broker API-KEY", envvar='REMOTIVE_BROKER_API_KEY')
 ):
     broker = Broker(url, api_key)
-    namespaces = broker.list_namespaces()
-    print(json.dumps(namespaces))
+    namespaces_json = broker.list_namespaces()
+    print(json.dumps(namespaces_json))
+
 
 @app.command(help="Discover brokers on this network")
 def discover():
-    #print("Not implemented")
+    # print("Not implemented")
 
     zeroconf = Zeroconf(ip_version=IPVersion.V4Only)
 
-    services = ["_remotivebroker._tcp.local.","_googlecast._tcp.local."]
-    #services = list(ZeroconfServiceTypes.find(zc=zeroconf))
+    services = ["_remotivebroker._tcp.local.", "_googlecast._tcp.local."]
+    # services = list(ZeroconfServiceTypes.find(zc=zeroconf))
 
     print("\nLooking for RemotiveBrokers on your network, press Ctrl-C to exit...\n")
     browser = ServiceBrowser(zeroconf, services, handlers=[on_service_state_change])
 
     try:
         while True:
             sleep(0.1)
     except KeyboardInterrupt:
         pass
     finally:
         zeroconf.close()
 
-    #network.MDNS.init()
-
-    # Perform a query for 2000 ms
-    #q = MDNS.query(2000, "broker", MDNS.PROTO_TCP)
-
-    # Print out the query's result
-    #if q is not None:
-    #    for elem in q:
-    #        print(elem.instance_name())
-    #        print(elem.hostname())
-    #        print(elem.addr())
-    #        print(elem.port())
-    #        print(elem.txt())
-
 
 def on_service_state_change(
         zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange
 ) -> None:
-    #print(f"Service {name} state changed: {state_change}")
+    # print(f"Service {name} state changed: {state_change}")
 
     if state_change is ServiceStateChange.Removed:
         print(f"Service {name} was removed")
 
     if state_change is ServiceStateChange.Updated:
         print(f"Service {name} was updated")
 
     if state_change is ServiceStateChange.Added:
         print(f"Discovered {name} ")
         info = zeroconf.get_service_info(service_type, name)
-        #print("Info from zeroconf.get_service_info: %r" % (info))
+        # print("Info from zeroconf.get_service_info: %r" % (info))
 
         if info:
-            #addresses = ["%s:%d" % (addr, cast(int, info.port)) for addr in info.parsed_scoped_addresses()]
+            # addresses = ["%s:%d" % (addr, cast(int, info.port)) for addr in info.parsed_scoped_addresses()]
             for addr in info.parsed_scoped_addresses():
                 print(addr)
-            #print("  Weight: %d, priority: %d" % (info.weight, info.priority))
-            #print(f"  Server: {info.server}")
-            #if info.properties:
+            # print("  Weight: %d, priority: %d" % (info.weight, info.priority))
+            # print(f"  Server: {info.server}")
+            # if info.properties:
             #    print("  Properties are:")
             #    for key, value in info.properties.items():
             #        print(f"    {key}: {value}")
-            #else:
+            # else:
             #    print("  No properties")
         else:
             print("  No info")
         print('\n')
 
+
 if __name__ == "__main__":
     app()
```

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/cloud_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import time
-
 import typer
-import json
-from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from . import recordings, brokers, configs, auth, service_accounts
 from . import rest_helper as rest
 
 app = typer.Typer()
 
 
 @app.command(help="Who am I?")
```

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import shutil
 import sys
 
-import typer
 import requests
-import os
-import json
-import shutil
+import typer
 from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from . import rest_helper as rest
 
 app = typer.Typer()
 
 
 @app.command("list")
 def list(type: str = typer.Argument(default="all", help="all, processing, recent")):
```

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a3/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a3/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a2/pyproject.toml` & `remotivelabs_cli-0.0.1a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remotivelabs-cli"
-version = "0.0.1.a2"
+version = "0.0.1.a3"
 description = ""
 authors = ["Johan Rask <johan.rask@remotivelabs.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `remotivelabs_cli-0.0.1a2/PKG-INFO` & `remotivelabs_cli-0.0.1a3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotivelabs-cli
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: 
 Author: Johan Rask
 Author-email: johan.rask@remotivelabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

