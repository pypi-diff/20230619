# Comparing `tmp/optscale_arcee-0.1.34.tar.gz` & `tmp/optscale_arcee-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.34.tar", last modified: Tue May 30 12:07:27 2023, max compression
+gzip compressed data, was "optscale_arcee-0.1.35.tar", last modified: Mon Jun 19 06:55:38 2023, max compression
```

## Comparing `optscale_arcee-0.1.34.tar` & `optscale_arcee-0.1.35.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/
--rw-rw-r--   0 am        (1000) am        (1000)    11304 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/LICENSE.txt
--rw-rw-r--   0 am        (1000) am        (1000)     2211 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)     1393 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/README.rst
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/
--rw-rw-r--   0 am        (1000) am        (1000)       95 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4021 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/arcee.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4103 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/collector.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/module_collector/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/module_collector/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     2633 2023-04-07 12:57:57.000000 optscale_arcee-0.1.34/optscale_arcee/module_collector/collector.py
--rw-rw-r--   0 am        (1000) am        (1000)     6757 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/name_generator.py
--rw-rw-r--   0 am        (1000) am        (1000)     9821 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platform.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     2469 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/platforms_meta/azure.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee/sender/
--rw-rw-r--   0 am        (1000) am        (1000)        0 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/optscale_arcee/sender/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4567 2023-05-30 12:01:34.000000 optscale_arcee-0.1.34/optscale_arcee/sender/sender.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/optscale_arcee.egg-info/
--rw-rw-r--   0 am        (1000) am        (1000)     2211 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)      734 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/SOURCES.txt
--rw-rw-r--   0 am        (1000) am        (1000)        1 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/dependency_links.txt
--rw-rw-r--   0 am        (1000) am        (1000)       60 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/requires.txt
--rw-rw-r--   0 am        (1000) am        (1000)       15 2023-05-30 12:07:27.000000 optscale_arcee-0.1.34/optscale_arcee.egg-info/top_level.txt
--rw-rw-r--   0 am        (1000) am        (1000)      524 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/setup.cfg
--rw-rw-r--   0 am        (1000) am        (1000)       69 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/setup.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-05-30 12:07:27.844956 optscale_arcee-0.1.34/tests/
--rw-rw-r--   0 am        (1000) am        (1000)     4593 2023-03-24 12:30:15.000000 optscale_arcee-0.1.34/tests/test_data.py
--rw-rw-r--   0 am        (1000) am        (1000)     3850 2023-04-07 12:57:57.000000 optscale_arcee-0.1.34/tests/test_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/arcee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee/hw_stat_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/hw_stat_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/hw_stat_collector/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee/module_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/module_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/module_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee/platforms_meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/platforms_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/platforms_meta/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee/sender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/optscale_arcee/sender/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/optscale_arcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-19 06:55:38.000000 optscale_arcee-0.1.35/optscale_arcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-19 06:55:38.000000 optscale_arcee-0.1.35/optscale_arcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:55:38.000000 optscale_arcee-0.1.35/optscale_arcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 06:55:38.000000 optscale_arcee-0.1.35/optscale_arcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 06:55:38.000000 optscale_arcee-0.1.35/optscale_arcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-19 06:55:38.628536 optscale_arcee-0.1.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 06:55:33.000000 optscale_arcee-0.1.35/setup.py
```

### Comparing `optscale_arcee-0.1.34/LICENSE.txt` & `optscale_arcee-0.1.35/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- Apache License
+                                 Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `optscale_arcee-0.1.34/README.rst` & `optscale_arcee-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.34/optscale_arcee/arcee.py` & `optscale_arcee-0.1.35/optscale_arcee/arcee.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             self.job()
             time.sleep(sleep)
 
 
 @single
 class Arcee:
     def __init__(
-            self, token=None, model_key=None, endpoint_url=None, ssl=True
+        self, token=None, model_key=None, endpoint_url=None, ssl=True
     ):
         self.shutdown_flag = threading.Event()
         self.token = token
         self.model_key = model_key
         self.sender = Sender(endpoint_url, ssl, self.shutdown_flag)
         self.hb = None
         self._run = None
@@ -87,22 +87,29 @@
         if exc_type is None:
             finish()
         else:
             error()
         return exc_type is None
 
 
-def init(token, model_key, run_name=None, endpoint_url=None, ssl=True, period=1):
+def init(
+    token, model_key, run_name=None, endpoint_url=None, ssl=True, period=1
+):
     arcee = Arcee(token, model_key, endpoint_url, ssl)
-    name = run_name if run_name is not None else NameGenerator.get_random_name()
+    name = (
+        run_name if run_name is not None else NameGenerator.get_random_name()
+    )
     run_id = asyncio.run(arcee.sender.get_run_id(model_key, token, name))["id"]
     arcee.run = run_id
     arcee.name = name
-    arcee.hb = Job(meth_args=(arcee.sender, run_id, token), sleep=period,
-                   shutdown_flag=arcee.shutdown_flag)
+    arcee.hb = Job(
+        meth_args=(arcee.sender, run_id, token),
+        sleep=period,
+        shutdown_flag=arcee.shutdown_flag,
+    )
     arcee.hb.start()
     asyncio.run(
         arcee.sender.send_stats(
             arcee.token,
             {"project": arcee.model_key, "run": arcee.run, "data": {}},
         )
     )
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/hw_stat_collector/collector.py` & `optscale_arcee-0.1.35/optscale_arcee/hw_stat_collector/collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
     @staticmethod
     def _gpu_stats():
         gpus = GPUtil.getGPUs()
         len_gpus = len(gpus)
         if len_gpus < 1:
             return {}
-        avg_gpu_load = reduce(lambda x, y: x + y, map(lambda z: z.load, gpus)) / len(
-            gpus
-        )
+        avg_gpu_load = reduce(
+            lambda x, y: x + y, map(lambda z: z.load, gpus)
+        ) / len(gpus)
         avg_gpu_memory_free = reduce(
             lambda x, y: x + y, map(lambda z: z.memoryFree, gpus)
         ) / len(gpus)
         avg_gpu_memory_total = reduce(
             lambda x, y: x + y, map(lambda z: z.memoryTotal, gpus)
         ) / len(gpus)
         avg_gpu_memory_used = reduce(
@@ -65,15 +65,17 @@
         # virtual memory used by process
         proc_vmem = process.memory_info().vms
         # resident state memory used by process
         proc_rss = process.memory_info().rss
         cpu_proc = min(
             [
                 round(
-                    process.cpu_percent(interval=proc_interval) / psutil.cpu_count(), 2
+                    process.cpu_percent(
+                        interval=proc_interval) / psutil.cpu_count(),
+                    2,
                 ),
                 cpu_percent,
             ]
         )
 
         ps_stats = {
             "cpu_count": psutil.cpu_count(),
@@ -87,15 +89,17 @@
 
         proc_stats = {
             # process cpu usage in % (per core)
             "cpu": cpu_proc,
             "mem": {
                 # process virtual memory usage, p - percent, t - value
                 "vms": {
-                    "p": "{:.3f}".format(proc_vmem / (physical_mem + swap_mem)),
+                    "p": "{:.3f}".format(
+                        proc_vmem / (physical_mem + swap_mem)
+                    ),
                     "t": proc_vmem,
                 },
                 # process resident state memory usage, p - percent, t - value
                 "rss": {
                     "p": "{:.3f}".format(proc_rss / physical_mem),
                     "t": proc_rss,
                 },
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/module_collector/collector.py` & `optscale_arcee-0.1.35/optscale_arcee/module_collector/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from modulefinder import ModuleFinder
 import os
 import sys
 import __main__
 
 
 class Collector:
-
     executor = concurrent.futures.ThreadPoolExecutor(max_workers=3)
 
     """
     Modules collector
     """
 
     __filter__ = [
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.35/optscale_arcee/name_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from random import choice
 
 
 class NameGenerator:
-
     __left__ = (
         "admiring",
         "adoring",
         "affectionate",
         "agitated",
         "amazing",
         "angry",
@@ -351,8 +350,10 @@
         "yalow",
         "yonath",
         "zhukovsky",
     )
 
     @classmethod
     def get_random_name(cls, seperator="_"):
-        return "{}{}{}".format(choice(cls.__left__), seperator, choice(cls.__right__))
+        return "{}{}{}".format(
+            choice(cls.__left__), seperator, choice(cls.__right__)
+        )
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/platform.py` & `optscale_arcee-0.1.35/optscale_arcee/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.availability_zone = availability_zone
 
     def to_dict(self) -> dict:
         return json.loads(json.dumps(self, default=serialise))
 
 
 class Platform:
-
     match = {
         "Amazon EC2": PlatformType.aws,
         "Google": PlatformType.gcp,
         "Microsoft Corporation": PlatformType.azure,
         "Alibaba Cloud": PlatformType.ali,
     }
 
@@ -86,24 +85,28 @@
         except (OSError, IOError):
             pass
         return PlatformType.unknown
 
     @classmethod
     async def board_version(cls) -> PlatformType:
         try:
-            async with aiofiles.open("/sys/class/dmi/id/board_vendor", "r") as board:
+            async with aiofiles.open(
+                "/sys/class/dmi/id/board_vendor", "r"
+            ) as board:
                 data = await board.read()
                 return cls.match.get(data.rstrip(), PlatformType.unknown)
         except (OSError, IOError):
             pass
 
     @classmethod
     async def sys_vendor(cls) -> PlatformType:
         try:
-            async with aiofiles.open("/sys/class/dmi/id/sys_vendor", "r") as board:
+            async with aiofiles.open(
+                "/sys/class/dmi/id/sys_vendor", "r"
+            ) as board:
                 data = await board.read()
                 return cls.match.get(data.rstrip(), PlatformType.unknown)
         except (OSError, IOError):
             pass
 
     @classmethod
     async def platform(cls) -> PlatformType:
@@ -113,55 +116,64 @@
         if pl == PlatformType.unknown:
             pl = await cls.sys_vendor()
         return pl
 
 
 class BaseCollector:
     @staticmethod
-    async def send_request(url, headers=None, params=None, response="json") -> str:
+    async def send_request(
+        url, headers=None, params=None, response="json"
+    ) -> str:
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.get(url, params=params) as response:
                 if response == "json":
                     resp = await response.json()
                 else:
                     resp = await response.text()
                 return resp
 
 
 class AwsCollector(BaseCollector):
-
     base_url = "http://169.254.169.254/latest/meta-data/%s"
 
     async def get_instance_id(self):
-        return await self.send_request(self.base_url % "instance-id", response="text")
+        return await self.send_request(
+            self.base_url % "instance-id", response="text"
+        )
 
     async def get_account_id(self):
         acc_info = await self.send_request(
             self.base_url % "identity-credentials/ec2/info", response="json"
         )
         return json.loads(acc_info).get("AccountId", "")
 
     async def get_local_ip(self):
-        return await self.send_request(self.base_url % "local-ipv4", response="text")
+        return await self.send_request(
+            self.base_url % "local-ipv4", response="text"
+        )
 
     async def get_public_ip(self):
-        return await self.send_request(self.base_url % "public-ipv4", response="text")
+        return await self.send_request(
+            self.base_url % "public-ipv4", response="text"
+        )
 
     async def get_life_cycle(self):
         match = {
             "spot": InstanceLifeCycle.Spot,
             "on-demand": InstanceLifeCycle.OnDemand,
         }
         lc_fut = await self.send_request(
             self.base_url % "instance-life-cycle", response="text"
         )
         return match.get(lc_fut.lower(), InstanceLifeCycle.Unknown)
 
     async def get_instance_type(self):
-        return await self.send_request(self.base_url % "instance-type", response="text")
+        return await self.send_request(
+            self.base_url % "instance-type", response="text"
+        )
 
     async def get_az(self):
         return await self.send_request(
             self.base_url % "placement/availability-zone", response="text"
         )
 
     async def get_region(self):
@@ -180,26 +192,29 @@
             await self.get_instance_type(),
             await self.get_region(),
             await self.get_az(),
         )
 
 
 class GcpCollector(BaseCollector):
-
     base_url = "http://169.254.169.254/computeMetadata/v1/%s"
     headers = {"Metadata-Flavor": "Google"}
 
     async def get_instance_id(self):
         return await self.send_request(
-            self.base_url % "instance/id", headers=self.headers, response="text"
+            self.base_url % "instance/id",
+            headers=self.headers,
+            response="text",
         )
 
     async def get_account_id(self):
         return await self.send_request(
-            self.base_url % "project/project-id", headers=self.headers, response="text"
+            self.base_url % "project/project-id",
+            headers=self.headers,
+            response="text",
         )
 
     async def get_local_ip(self):
         return await self.send_request(
             self.base_url % "instance/network-interfaces/0/ip",
             headers=self.headers,
             response="text",
@@ -257,15 +272,14 @@
             await self.get_instance_type(),
             await self.get_region(),
             await self.get_az(),
         )
 
 
 class AzureCollector(BaseCollector):
-
     base_url = "http://169.254.169.254/metadata/instance/"
 
     async def collect(self) -> str:
         """
         Collects data from metadata server
         :return: (str) metadata json
         """
@@ -277,17 +291,21 @@
         meta_response = await self.collect()
         if meta_response:
             meta = AzureMeta.from_dict(json.loads(meta_response))
             private_ip = public_ip = ""
             # TODO: check usage
             if meta.network and meta.network.interface:
                 private_ip = (
-                    meta.network.interface[0].ipv4.ipAddress[0].privateIpAddress
+                    meta.network.interface[0]
+                    .ipv4.ipAddress[0]
+                    .privateIpAddress
+                )
+                public_ip = (
+                    meta.network.interface[0].ipv4.ipAddress[0].publicIpAddress
                 )
-                public_ip = meta.network.interface[0].ipv4.ipAddress[0].publicIpAddress
             return PlatformMeta(
                 PlatformType.azure,
                 meta.compute.resourceId,
                 meta.compute.subscriptionId,
                 private_ip,
                 public_ip,
                 InstanceLifeCycle.Unknown,
@@ -296,24 +314,25 @@
                 meta.compute.zone,
             )
         return PlatformMeta(PlatformType.azure)
 
 
 class UnknownCollector(BaseCollector):
     @staticmethod
-    async def send_request(url, headers=None, params=None, response="json") -> str:
+    async def send_request(
+        url, headers=None, params=None, response="json"
+    ) -> str:
         return await asyncio.sleep(0)
 
     @staticmethod
     async def get_platform_meta() -> PlatformMeta:
         return PlatformMeta(PlatformType.unknown, Platform.platform_name())
 
 
 class CollectorFactory:
-
     match = {
         PlatformType.azure: AzureCollector,
         PlatformType.aws: AwsCollector,
     }
 
     @classmethod
     async def get(cls):
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.35/optscale_arcee/platforms_meta/azure.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self,
         name: str,
         location: str,
         resourceId: str,
         vmSize: str,
         zone: str,
         subscriptionId: str,
-        **kwargs
+        **kwargs,
     ):
         self.name = name
         self.location = location
         self.resourceId = resourceId.lower()
         self.vmSize = vmSize
         self.zone = zone
         self.subscriptionId = subscriptionId
@@ -34,15 +34,18 @@
     def __init__(self, address: str, prefix: str):
         self.address = address
         self.prefix = prefix
 
 
 class AzureIPv4Meta:
     def __init__(
-        self, ipAddress: List[AzureIpMeta], subnet: List[AzureSubnetMeta], **kwargs
+        self,
+        ipAddress: List[AzureIpMeta],
+        subnet: List[AzureSubnetMeta],
+        **kwargs,
     ):
         self.ipAddress = ipAddress
         self.subnet = subnet
 
     @classmethod
     def from_dict(cls, d):
         ipAddress = d.get("ipAddress")
@@ -71,20 +74,24 @@
     def __init__(self, interface: List[AzureInterfaceMeta]):
         self.interface = interface
 
     @classmethod
     def from_dict(cls, d):
         interface = d.get("interface")
         if interface:
-            d["interface"] = [AzureInterfaceMeta.from_dict(i) for i in interface]
+            d["interface"] = [
+                AzureInterfaceMeta.from_dict(i) for i in interface
+            ]
         return cls(**d)
 
 
 class AzureMeta:
-    def __init__(self, compute: AzureComputeMeta, network: AzureNetworkMeta, **kwargs):
+    def __init__(
+        self, compute: AzureComputeMeta, network: AzureNetworkMeta, **kwargs
+    ):
         self.compute = compute
         self.network = network
 
     @classmethod
     def from_dict(cls, d):
         compute = d.get("compute")
         if compute:
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.35/optscale_arcee/sender/sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import aiohttp
 import threading
 
 from optscale_arcee.platform import CollectorFactory
-from optscale_arcee.module_collector.collector import Collector as ImportsCollector
+from optscale_arcee.module_collector.collector import (
+    Collector as ImportsCollector,
+)
 from optscale_arcee.hw_stat_collector.collector import Collector as HwCollector
 
 
 def check_shutdown_flag_set(function):
     async def inner(self, *args, **kwargs):
         if not self.shutdown_flag.is_set():
             return await function(self, *args, **kwargs)
+
     return inner
 
 
 class Sender:
-
     # default OptScale url
     base_url = "https://my.optscale.com:443/arcee/v2"
 
     def __init__(self, endpoint_url=None, ssl=True, shutdown_flag=None):
         if endpoint_url is None:
             endpoint_url = self.base_url
         self.endpoint_url = endpoint_url
```

### Comparing `optscale_arcee-0.1.34/optscale_arcee.egg-info/SOURCES.txt` & `optscale_arcee-0.1.35/optscale_arcee.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-LICENSE.txt
-README.rst
+LICENSE
+README.md
 setup.cfg
 setup.py
 ./optscale_arcee/__init__.py
 ./optscale_arcee/arcee.py
 ./optscale_arcee/name_generator.py
 ./optscale_arcee/platform.py
 ./optscale_arcee/hw_stat_collector/__init__.py
@@ -14,10 +14,8 @@
 ./optscale_arcee/platforms_meta/azure.py
 ./optscale_arcee/sender/__init__.py
 ./optscale_arcee/sender/sender.py
 optscale_arcee.egg-info/PKG-INFO
 optscale_arcee.egg-info/SOURCES.txt
 optscale_arcee.egg-info/dependency_links.txt
 optscale_arcee.egg-info/requires.txt
-optscale_arcee.egg-info/top_level.txt
-tests/test_data.py
-tests/test_platform.py
+optscale_arcee.egg-info/top_level.txt
```

### Comparing `optscale_arcee-0.1.34/setup.cfg` & `optscale_arcee-0.1.35/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.34
+version = 0.1.35
 author = Hystax
 description = ML profiling tool for OptScale
-long_description = file: README.rst
+long_description = file: README.md
 long_description_content_type = text/markdown
+license = "Apache License 2.0"
 url = https://my.optscale.com/
+project_urls = 
+	Source = https://github.com/hystax/optscale_arcee_dev
 keywords = arcee, ml, optscale, finops, mlops
 
 [options]
 python_requires = >=3.7, <4
 install_requires = 
 	aiohttp==3.8.4
 	aiofiles==22.1.0
@@ -18,14 +21,15 @@
 packages = find:
 package_dir = 
 	=.
 test = 
 	tox
 
 [options.packages.find]
+where = .
 exclude = 
 	tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

