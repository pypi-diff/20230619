# Comparing `tmp/maddaq-0.7.7.tar.gz` & `tmp/maddaq-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.7.tar", last modified: Tue May  9 16:09:43 2023, max compression
+gzip compressed data, was "maddaq-0.7.8.tar", last modified: Mon Jun 19 14:59:29 2023, max compression
```

## Comparing `maddaq-0.7.7.tar` & `maddaq-0.7.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-09 16:09:43.074965 maddaq-0.7.7/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-05-09 16:09:43.074591 maddaq-0.7.7/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.7/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-09 16:09:43.067066 maddaq-0.7.7/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.7/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.7/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.7/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.7/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.7/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-05-09 16:09:02.000000 maddaq-0.7.7/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-09 16:09:43.073427 maddaq-0.7.7/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.7/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.7/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.7/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.7/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8208 2023-05-09 14:06:08.000000 maddaq-0.7.7/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.7/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.7/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-09 16:09:43.069514 maddaq-0.7.7/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-05-09 16:09:43.000000 maddaq-0.7.7/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-05-09 16:09:02.000000 maddaq-0.7.7/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-09 16:09:43.075079 maddaq-0.7.7/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.339249 maddaq-0.7.8/
+-rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-19 14:59:29.338836 maddaq-0.7.8/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4786 2023-06-19 14:58:03.000000 maddaq-0.7.8/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.332092 maddaq-0.7.8/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.8/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7804 2023-05-25 17:24:23.000000 maddaq-0.7.8/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.8/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.8/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.8/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-05-29 09:45:06.000000 maddaq-0.7.8/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.338255 maddaq-0.7.8/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.8/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.8/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.8/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.8/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     9493 2023-05-29 09:52:27.000000 maddaq-0.7.8/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.8/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.8/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.334849 maddaq-0.7.8/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-05-29 09:45:06.000000 maddaq-0.7.8/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-06-19 14:59:29.339385 maddaq-0.7.8/setup.cfg
```

### Comparing `maddaq-0.7.7/PKG-INFO` & `maddaq-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.7
+Version: 0.7.8
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -67,15 +67,20 @@
 
 ````
 
 ### `MadDAQModule`
 `MadDAQModule`contains all the information relative to a module. The main role of this object is to analyze the module data.
 
 ### Python examples.
-There are a number or examples to read data with Python.
+There are a number or examples to read data with Python. 
+
+#### Command line programs
+- getSpectrum to make a very rough analysis and show the energy distribution.
+- show_data to see the raw data in the file.
+- getFileInfo to get information about the data file (date, no. of events, etc.)
 
 #### `fit-utils.py`
 Some utilities to fit different distributions.
 
 #### `read_data.py`
 Shows how to iterate on the data
```

### Comparing `maddaq-0.7.7/README.md` & `maddaq-0.7.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,20 @@
 
 ````
 
 ### `MadDAQModule`
 `MadDAQModule`contains all the information relative to a module. The main role of this object is to analyze the module data.
 
 ### Python examples.
-There are a number or examples to read data with Python.
+There are a number or examples to read data with Python. 
+
+#### Command line programs
+- getSpectrum to make a very rough analysis and show the energy distribution.
+- show_data to see the raw data in the file.
+- getFileInfo to get information about the data file (date, no. of events, etc.)
 
 #### `fit-utils.py`
 Some utilities to fit different distributions.
 
 #### `read_data.py`
 Shows how to iterate on the data
```

### Comparing `maddaq-0.7.7/maddaq/GTimer.py` & `maddaq-0.7.8/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/MadDAQData.py` & `maddaq-0.7.8/maddaq/MadDAQData.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,21 @@
         if show_modules:
             print("\nNumber of modules: ", len(self.modules))
             for m in self.modules.values():
                 print("+ Module: ", m.id,
                       " n. evts", m.data.shape[0],
                       " fw: %d.%d" % ((m.firmware & 0xff00) >> 8, m.firmware & 0xff))
 
+    def get_duration(self):
+        """Return the run duration in seconds."""
+        rr = self.F["/header/run_records"]
+        t0 = get_run_info_time(rr[0]['time'])
+        t1 = get_run_info_time(rr[1]['time'])
+        return (t1-t0).total_seconds()
+    
     def has_scan(self):
         """Tell if the file has scan data."""
         try:
             self.F["/scan"]
             return True
         except KeyError:
             return False
```

### Comparing `maddaq-0.7.7/maddaq/MadDAQModule.py` & `maddaq-0.7.8/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/Progress.py` & `maddaq-0.7.8/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/ScanManager.py` & `maddaq-0.7.8/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.8/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/cmmds/file_info.py` & `maddaq-0.7.8/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.8/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.8/maddaq/cmmds/getSpectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import sys
 from pathlib import Path
 from argparse import Action
 from argparse import ArgumentParser
 
 import matplotlib.pyplot as plt
+import matplotlib.transforms as transforms
 import numpy as np
 from scipy.interpolate import CubicSpline
 from maddaq.cmmds.fit_utils import draw_best_fit, fit_gaussian, fit_two_peaks
 from maddaq import MadDAQData
 from maddaq import ShowProgress
 
 from numpy.polynomial.polynomial import polyfit, polyval
@@ -105,14 +106,15 @@
 
 
 def do_getSpectrum(files, options):
     """Main entry."""
 
     amplitudes = []
     names = []
+    weights = []
 
     if options.calib:
         _adc, _E = np.loadtxt(options.calib, skiprows=1, delimiter=',', unpack=True)
         cs = CubicSpline(_adc, _E)
         ps = np.polyfit(_adc[:4], _E[:4], 1)
         pf = np.poly1d(ps)
 
@@ -143,14 +145,19 @@
         names.append(nam)
 
         # We open here the file with MadDAQData
         print("\n\n### Opening {}".format(Path(fnam).name))
         maddaq = MadDAQData(fnam)
         maddaq.show_info(True)
 
+        if options.time:
+            weights.append(maddaq.get_duration())
+        else:
+            weights.append(1.0)
+
         # Find the module
         keys = list(maddaq.modules.keys())
         if options.mid in keys:
             mid = options.mid
         else:
             mid = keys[0]
 
@@ -184,26 +191,59 @@
 
             prg.increase(show=True)
 
         amplitudes.append(get_E(amplitude))
         prg.stop()
         print("")
 
+    # Get the normalization factors
+    if len(weights) == 0:
+        print("No valid file left for analysis. Quitting")
+        sys.exit(-1)
+        
+    vmax = np.amax(weights)
+    weights = [vmax/W for W in weights]
+
     # Draw the signal
     if options.calib:
         fig, ax = plt.subplots(1, 1)
         xxx = np.linspace(0, 1750, int(1750/2.5))
         yyy = get_E(xxx)
         ax.plot(xxx, yyy)
         ax.grid()
         ax.set_xlabel("ADC counts")
         ax.set_ylabel("Energy (keV)")
 
     fig, ax = plt.subplots(1, 1)
-    n, bins, *_ = ax.hist(amplitudes, bins=options.nbin, label=names)
+    i = 0
+    ymax = -1e100
+    for A, nam in zip(amplitudes, names):
+        n, bins, P = ax.hist(A, bins=options.nbin,
+                             histtype='stepfilled', alpha=0.25, label=nam)
+
+        if options.time:
+            W = weights[i]
+            for p in P:
+                points = p.get_xy()
+                new_points = np.zeros(points.shape)
+                ipoint = 0
+                for x in points:
+                    y = W*x[1]
+                    ymax = max(y, ymax)
+                    new_points[ipoint, :] = [x[0], y]
+                    ipoint += 1
+                    
+                p.set_xy(new_points)
+
+            i += 1
+    if options.time:
+        y0, y1 = ax.get_ylim()
+        ax.set_ylim(y0, 1.1*ymax)
+    
+    # n, bins, *_ = ax.hist(amplitudes, bins=options.nbin, label=names)
     legends = []
     if options.fit:
         for amplitude in amplitudes:
             mean = np.mean(amplitude)
             std = np.std(amplitude)
             if options.two_peaks:
                 result, out, legend = fit_two_peaks(mean, std, std, n, bins)
@@ -255,14 +295,15 @@
     parser.add_argument("--logY", default=False, action="store_true", help="Log axis")
     parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
     parser.add_argument("--two_peaks", default=False, action="store_true", help="Min E to show in histogram")
     parser.add_argument("--no-fit", dest="fit", default=True, action="store_false")
     parser.add_argument("--show-ped", action="store_true", default=False, dest="show_ped")
     parser.add_argument("--mid", dest="mid", default=-1, type=int, help="The module ID")
     parser.add_argument("--calib", default=None, help="The energy calibration file. X:adc, Y:energy")
+    parser.add_argument("--time", default=False, action="store_true", help="Normalize to duration of run when reading various files")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
         sys.exit()
```

### Comparing `maddaq-0.7.7/maddaq/cmmds/read_data.py` & `maddaq-0.7.8/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq/cmmds/show_data.py` & `maddaq-0.7.8/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.8/maddaq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.7
+Version: 0.7.8
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -67,15 +67,20 @@
 
 ````
 
 ### `MadDAQModule`
 `MadDAQModule`contains all the information relative to a module. The main role of this object is to analyze the module data.
 
 ### Python examples.
-There are a number or examples to read data with Python.
+There are a number or examples to read data with Python. 
+
+#### Command line programs
+- getSpectrum to make a very rough analysis and show the energy distribution.
+- show_data to see the raw data in the file.
+- getFileInfo to get information about the data file (date, no. of events, etc.)
 
 #### `fit-utils.py`
 Some utilities to fit different distributions.
 
 #### `read_data.py`
 Shows how to iterate on the data
```

### Comparing `maddaq-0.7.7/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.8/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.7/pyproject.toml` & `maddaq-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.7"
+version = "0.7.8"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

