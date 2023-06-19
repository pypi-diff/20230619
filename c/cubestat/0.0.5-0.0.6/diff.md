# Comparing `tmp/cubestat-0.0.5.tar.gz` & `tmp/cubestat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.5.tar", last modified: Fri Jun 16 01:14:51 2023, max compression
+gzip compressed data, was "cubestat-0.0.6.tar", last modified: Mon Jun 19 01:25:08 2023, max compression
```

## Comparing `cubestat-0.0.5.tar` & `cubestat-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:14:41.000000 cubestat-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:14:51.312181 cubestat-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 01:14:41.000000 cubestat-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:41.000000 cubestat-0.0.5/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15100 2023-06-16 01:14:41.000000 cubestat-0.0.5/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:14:51.312181 cubestat-0.0.5/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 01:14:51.000000 cubestat-0.0.5/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:14:51.312181 cubestat-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 01:14:41.000000 cubestat-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.401373 cubestat-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-19 01:24:58.000000 cubestat-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 01:25:08.397374 cubestat-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-19 01:24:58.000000 cubestat-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.397374 cubestat-0.0.6/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 01:24:58.000000 cubestat-0.0.6/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15236 2023-06-19 01:24:58.000000 cubestat-0.0.6/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 01:25:08.397374 cubestat-0.0.6/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 01:25:08.000000 cubestat-0.0.6/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 01:25:08.401373 cubestat-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 01:24:58.000000 cubestat-0.0.6/setup.py
```

### Comparing `cubestat-0.0.5/LICENSE` & `cubestat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.5/README.md` & `cubestat-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-# Horizon charts for Apple M1/M2 monitoring
+# system monitoring horizon charts for terminal
 
-In progress: also working for linux with nVidia GPUs
+Let's start with example: running [deep RL loop](https://github.com/okuvshynov/rlscout) on a single MacBook Air M2:
 
-Command-line utility to monitor CPU/GPU/NeuralEngine utilization on Apple M1/M2 devices as horizon chart. Unfortunately, it requires sudo access as it calls `powermetrics` and parses its output.
+We can see model training (on GPU), self-play (done on 4 performance CPU cores) and model evaluation, which runs inference on Neural Engine (ANE):
+![Self-play + training + eval](static/selfplay.png)
+
+cubestat is a command-line utility to monitor usual system telemetry originally created for Apple M1/M2 devices.
+At its current stage monitors:
+1. CPU utilization - configurable per core ('expanded'), cluster of cores: Efficiency/Performance ('cluster') or both. Is shown as percentage.
+2. GPU utilization per card/chip. Is shown in percentage. Works for Apple's M1/M2 SoC and nVidia GPUs.
+3. ANE (Apple's Neural Engine) power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
+4. Disk and network IO; Is shown in Kb/s.
+5. Memory usage in %
 
-cubestat is particularly useful when connecting to another device remotely over ssh. 
+Despite many monitoring tools available for monitoring typical system counters as well as GPU/Accelerators, horizon charts have a unique information density properties which makes it possible to show a history of N measurements for M metrics on a single screen for significantly large N and M. Thus, this tool was created.
+
+## Installation and Usage:
 
-Installation:
 ```
 pip3 install cubestat
-```
 
-```
-usage: ./cubestat.py [-h]
-                     [--refresh_ms REFRESH_MS]
-                     [--buffer_size BUFFER_SIZE]
-                     [--cpu {all,by_cluster,by_core}]
-                     [--color {red,green,blue,mixed}]
-                     [--percentages {hidden,last}]
-                     [--disk] [--network]
+usage: cubestat [-h] [--refresh_ms REFRESH_MS] [--buffer_size BUFFER_SIZE]
+                [--cpu {all,by_cluster,by_core}] [--color {red,green,blue,mixed}]
+                [--percentages {hidden,last}] [--disk] [--network]
 
 options:
-  -h, --help            show this help message and
-                        exit
+  -h, --help            show this help message and exit
   --refresh_ms REFRESH_MS, -i REFRESH_MS
-                        Update frequency,
-                        milliseconds
+                        Update frequency, milliseconds
   --buffer_size BUFFER_SIZE
-                        How many datapoints to
-                        store. Having it larger
-                        than screen width is a
-                        good idea as terminal
-                        window can be resized
+                        How many datapoints to store. Having it larger than screen width is a good
+                        idea as terminal window can be resized
   --cpu {all,by_cluster,by_core}
-                        CPU mode - showing all
-                        cores, only cumulative by
-                        cluster or both. Can be
+                        CPU mode - showing all cores, only cumulative by cluster or both. Can be
                         toggled by pressing c.
   --color {red,green,blue,mixed}
   --percentages {hidden,last}
-                        Show/hide numeric
-                        utilization percentage.
-                        Can be toggled by pressing
-                        p.
-  --disk                show disk read/write. Can
-                        be toggled by pressing d.
-  --network             show network io. Can be
-                        toggled by pressing n.
+                        Show/hide numeric utilization percentage. Can be toggled by pressing p.
+  --disk                show disk read/write. Can be toggled by pressing d.
+  --network             show network io. Can be toggled by pressing n.
 ```
 
-Monitors:
-1. CPU utilization - configurable per core ('expanded'), cluster of cores: Efficiency/Performance ('cluster') or both. Is shown as percentage.
-2. GPU utilization per GPU. Is shown in percentage.
-3. ANE power consumption. According to `man powermetrics` it is an estimate, but seems working good enough as a proxy to ANE utilization. Is shown as percentage.
-4. Disk and network IO; Is shown in Kb/s.
-5. Memory usage in %
-
-We could add more data from powermetrics (e.g. frequency), but it was adding too much visual noise.
-
-Example: running [deep RL loop](https://github.com/okuvshynov/rlscout) (self play to generate data, model training, model evaluation) on a single MacBook Air M2:
+Running on Apple devices will require sudo access, as `powermetrics` has such limitation. Running on Linux machines doesn't have this limitation.
 
-We can see model training (on GPU), self-play (done on 4 performance CPU cores) and model evaluation, which runs inference on Neural Engine:
-![Self-play + training + eval](static/selfplay.png)
-
-Another example running [GPT inference on ggml](https://github.com/ggerganov/ggml): 
-![GPT inference](static/ggml_gpt.png)
-
-Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 GPU instance:
+Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 nVidia GPU instance:
 ![multigpu](static/multigpu.png)
+
+## Dependencies
+* Python 3.?+
+* psutil 5.9.5
+* pynvml for nVidia cards monitoring
+
+## TODO
+* GPU aggregation
+* CPU by socket/NUMA/SMT
+* better IO scale (joint scale for all IO?)
+* status line
+* better colors (especially for dark background)
+* multi-column layout for large instances (e.g. with 100+ cores)
+* try on Windows and BSD
+* Google TPU load?
+* AMD GPU load?
+* Filter by process?
```

### Comparing `cubestat-0.0.5/cubestat/cubestat.py` & `cubestat-0.0.6/cubestat/cubestat.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,36 @@
     
 class Color(EnumStr):
     red = 'red'
     green = 'green'
     blue = 'blue'
     mixed = 'mixed'
 
-parser = argparse.ArgumentParser("./cubestat.py")
-parser.add_argument('--refresh_ms', '-i', type=int, default=500, help='Update frequency, milliseconds')
+parser = argparse.ArgumentParser("cubestat")
+parser.add_argument('--refresh_ms', '-i', type=int, default=1000, help='Update frequency, milliseconds')
 parser.add_argument('--buffer_size', type=int, default=500, help='How many datapoints to store. Having it larger than screen width is a good idea as terminal window can be resized')
 parser.add_argument('--cpu', type=CPUMode, default=CPUMode.all, choices=list(CPUMode), help='CPU mode - showing all cores, only cumulative by cluster or both. Can be toggled by pressing c.')
 parser.add_argument('--color', type=Color, default=Color.mixed, choices=list(Color))
 parser.add_argument('--percentages', type=Percentages, default=Percentages.last, choices=list(Percentages), help='Show/hide numeric utilization percentage. Can be toggled by pressing p.')
-parser.add_argument('--disk', action="store_true", help="show disk read/write. Can be toggled by pressing d.")
-parser.add_argument('--network', action="store_true", help="show network io. Can be toggled by pressing n.")
+parser.add_argument('--disk', action="store_true", default=True, help="Show disk read/write. Can be toggled by pressing d.")
+parser.add_argument('--network', action="store_true", default=True, help="Show network io. Can be toggled by pressing n.")
+parser.add_argument('--no-disk', action="store_false", dest="disk", help="Hide disk read/write. Can be toggled by pressing d.")
+parser.add_argument('--no-network', action="store_false", dest="network", help="Hide network io. Can be toggled by pressing n.")
 
 args = parser.parse_args()
 
+def snapshot_base():
+    return {
+        'cpu': {},
+        'accelerators': {},
+        'ram': {'RAM used %': psutil.virtual_memory().percent},
+        'disk': {},
+        'network': {},
+    }
+
 # psutil + nvsmi for nVidia GPU
 class LinuxReader:
     def __init__(self, interval_ms):
         self.has_nvidia = False
         self.first = True
         self.interval_ms = interval_ms
         try:
@@ -64,21 +75,15 @@
                 self.nvsmi = nvidia_smi.getInstance()
                 self.has_nvidia = True
         except Exception:
             # TODO: add logging here
             pass
 
     def read(self):
-        res = {
-            'cpu': {},
-            'accelerators': {},
-            'ram': {'RAM used %': psutil.virtual_memory().percent},
-            'disk': {},
-            'network': {},
-        }
+        res = snapshot_base()
 
         disk_load = psutil.disk_io_counters()
         disk_read_kb = disk_load.read_bytes / 2 ** 10
         disk_written_kb = disk_load.write_bytes / 2 ** 10
         nw_load = psutil.net_io_counters()
         nw_read_kb = nw_load.bytes_recv / 2 ** 10
         nw_written_kb = nw_load.bytes_sent / 2 ** 10
@@ -122,21 +127,16 @@
         return res.items(), cpu_clusters
 
 class AppleReader:
     def __init__(self, interval_ms) -> None:
         self.interval_ms = interval_ms
 
     def read(self, snapshot):
-        res = {
-            'cpu': {},
-            'accelerators': {},
-            'ram': {'RAM used %': psutil.virtual_memory().percent},
-            'disk': {},
-            'network': {},
-        }
+        res = snapshot_base()
+
         cpu_clusters = []
         for cluster in snapshot['processor']['clusters']:
             idle_cluster, total_cluster = 0.0, 0.0
             cluster_title = f'{cluster["name"]} total CPU util %'
             cpu_clusters.append(cluster_title)
             res['cpu'][cluster_title] = 0.0
             for cpu in cluster['cpus']:
@@ -277,15 +277,14 @@
                     if group_name == 'disk' or group_name == 'network':
                         B = max(data_slice)
                         B = float(1 if B == 0 else 2 ** (int((B - 1)).bit_length()))
                         strvalue =  f'last:{data_slice[-1]:3.0f}|{int(B)}Kb/s{spacing}╗' if self.percentage_mode == Percentages.last else f'{spacing}╗'
 
                     title_filling = self.filling * (self.cols - len(strvalue) - len(titlestr))
                     self.write_string(i * 2, len(titlestr), title_filling)
-
                     self.write_string(i * 2, self.cols - len(strvalue), strvalue)
 
                     border = f'{spacing}╝'
                     self.write_string(i * 2 + 1, self.cols - len(border), border)
 
                     scaler = range / B
                     
@@ -331,19 +330,19 @@
                     self.settings_changed = True
 
     def reader_loop_linux(self):
         begin_ts = time.time()
         n = 0
         d = args.refresh_ms / 1000.0
         while True:
+            snapshot, cpu_clusters = self.reader.read()
+            self.process_snapshot(snapshot, cpu_clusters)
             n += 1
             expected_time = begin_ts + n * d
             time.sleep(expected_time - time.time())
-            snapshot, cpu_clusters = self.reader.read()
-            self.process_snapshot(snapshot, cpu_clusters)
 
     def reader_loop_apple(self, powermetrics, firstline):
         buf = bytearray()
         buf.extend(firstline)
 
         while True:
             line = powermetrics.stdout.readline()
```

### Comparing `cubestat-0.0.5/setup.py` & `cubestat-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.5',
+    version='0.0.6',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for CPU/GPU/ANE monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
@@ -14,8 +14,8 @@
     ],
     url='https://github.com/okuvshynov/cubestat',
     entry_points={
         'console_scripts': [
             'cubestat = cubestat.cubestat:main'
         ]
     },
-)
+)
```

