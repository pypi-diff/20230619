# Comparing `tmp/polybeat-1.0.0.tar.gz` & `tmp/polybeat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polybeat-1.0.0.tar", last modified: Thu Jun 15 20:27:36 2023, max compression
+gzip compressed data, was "polybeat-1.1.0.tar", last modified: Mon Jun 19 07:30:32 2023, max compression
```

## Comparing `polybeat-1.0.0.tar` & `polybeat-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.186970 polybeat-1.0.0/
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1679 2023-06-15 20:27:36.184024 polybeat-1.0.0/PKG-INFO
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1141 2023-06-15 20:22:34.000000 polybeat-1.0.0/README.md
-drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:35.953982 polybeat-1.0.0/polybeat/
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)     4260 2023-06-15 20:13:07.000000 polybeat-1.0.0/polybeat/__init__.py
-drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.154998 polybeat-1.0.0/polybeat/sounds/
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.0.0/polybeat/sounds/kick_drum.wav
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.0.0/polybeat/sounds/low_bongo.wav
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.0.0/polybeat/sounds/open_conga.wav
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.0.0/polybeat/sounds/side_stick.wav
-drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-15 20:27:36.039052 polybeat-1.0.0/polybeat.egg-info/
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1679 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/PKG-INFO
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)      289 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/SOURCES.txt
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)        1 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/dependency_links.txt
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)        9 2023-06-15 20:27:35.000000 polybeat-1.0.0/polybeat.egg-info/top_level.txt
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)       38 2023-06-15 20:27:36.187986 polybeat-1.0.0/setup.cfg
--rwxrwxrwx   0 pcc       (1000) pcc       (1000)      911 2023-06-15 17:27:09.000000 polybeat-1.0.0/setup.py
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-19 07:30:32.054569 polybeat-1.1.0/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1705 2023-06-19 07:30:32.051562 polybeat-1.1.0/PKG-INFO
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1167 2023-06-19 07:28:54.000000 polybeat-1.1.0/README.md
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-19 07:30:31.806167 polybeat-1.1.0/polybeat/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     4337 2023-06-19 07:19:10.000000 polybeat-1.1.0/polybeat/__init__.py
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-19 07:30:32.022319 polybeat-1.1.0/polybeat/sounds/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.1.0/polybeat/sounds/kick_drum.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.1.0/polybeat/sounds/low_bongo.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-27 06:10:20.000000 polybeat-1.1.0/polybeat/sounds/open_conga.wav
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)   209324 2023-01-26 11:44:42.000000 polybeat-1.1.0/polybeat/sounds/side_stick.wav
+drwxrwxrwx   0 pcc       (1000) pcc       (1000)        0 2023-06-19 07:30:31.892650 polybeat-1.1.0/polybeat.egg-info/
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)     1705 2023-06-19 07:30:31.000000 polybeat-1.1.0/polybeat.egg-info/PKG-INFO
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)      289 2023-06-19 07:30:31.000000 polybeat-1.1.0/polybeat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)        1 2023-06-19 07:30:31.000000 polybeat-1.1.0/polybeat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)        9 2023-06-19 07:30:31.000000 polybeat-1.1.0/polybeat.egg-info/top_level.txt
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)       38 2023-06-19 07:30:32.055582 polybeat-1.1.0/setup.cfg
+-rwxrwxrwx   0 pcc       (1000) pcc       (1000)      911 2023-06-19 07:25:06.000000 polybeat-1.1.0/setup.py
```

### Comparing `polybeat-1.0.0/PKG-INFO` & `polybeat-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polybeat
-Version: 1.0.0
+Version: 1.1.0
 Summary: A toy for visualizing polyrhythms
 Home-page: https://github.com/chunribu/polybeat/
 Author: Jian Jiang
 Author-email: pccfreespace@gmail.com
 License: MIT
 Keywords: polybeat polyrhythm pccfs
 Classifier: Operating System :: POSIX :: Linux
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # Polybeat
 
 
 
-https://github.com/chunribu/polybeat/assets/57521167/1bad0cd3-3feb-4222-8fea-8398ac4c3689
+https://github.com/chunribu/polybeat/assets/57521167/2c2e6025-2490-4b45-b54e-92f1c06b1c04
 
 
 
 ## Installation
 ```shell
 # first, install manim from conda-forge channel
 conda install -c conda-forge manim
@@ -39,26 +39,26 @@
 # step 2:
 # primary usage
 play([3,4,12])
 
 # advanced usage
 play(
     rhythms=[3,4,6,12],
-    custom_order=None,
-    colors=[RED,YELLOW,BLUE,GREEN],
+    custom_order=[0,1,3,2],
+    # colors=[RED,YELLOW,BLUE,GREEN],
     sounds=['kick_drum','open_conga','side_stick','low_bongo'],
     volumes=[0,-2,-6,-4],
     cycle_time=1.8,
     dot_radius=0.16,
     width_range=[2.5,3.5],
     preview=True,
 )
 ```
 
-`custom_order` is None by default, which equals [0,1,2,3] in this case.
+`custom_order` is None by default, which equals to [3,2,1,0] (reverse order) in this case.
 
 `colors` should be a list of variables supported by manim or hex number strings, e.g. ['#3ec1d3', '#f6f7d7', '#ff9a00', '#ff165d'].
 
 `sounds` can be paths to custom audio files, or just leave it default.
 
 `cycle_time` has an effect on speed.
```

### Comparing `polybeat-1.0.0/README.md` & `polybeat-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Polybeat
 
 
 
-https://github.com/chunribu/polybeat/assets/57521167/1bad0cd3-3feb-4222-8fea-8398ac4c3689
+https://github.com/chunribu/polybeat/assets/57521167/2c2e6025-2490-4b45-b54e-92f1c06b1c04
 
 
 
 ## Installation
 ```shell
 # first, install manim from conda-forge channel
 conda install -c conda-forge manim
@@ -23,26 +23,26 @@
 # step 2:
 # primary usage
 play([3,4,12])
 
 # advanced usage
 play(
     rhythms=[3,4,6,12],
-    custom_order=None,
-    colors=[RED,YELLOW,BLUE,GREEN],
+    custom_order=[0,1,3,2],
+    # colors=[RED,YELLOW,BLUE,GREEN],
     sounds=['kick_drum','open_conga','side_stick','low_bongo'],
     volumes=[0,-2,-6,-4],
     cycle_time=1.8,
     dot_radius=0.16,
     width_range=[2.5,3.5],
     preview=True,
 )
 ```
 
-`custom_order` is None by default, which equals [0,1,2,3] in this case.
+`custom_order` is None by default, which equals to [3,2,1,0] (reverse order) in this case.
 
 `colors` should be a list of variables supported by manim or hex number strings, e.g. ['#3ec1d3', '#f6f7d7', '#ff9a00', '#ff165d'].
 
 `sounds` can be paths to custom audio files, or just leave it default.
 
 `cycle_time` has an effect on speed.
```

### Comparing `polybeat-1.0.0/polybeat/__init__.py` & `polybeat-1.1.0/polybeat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,16 @@
                 for n in rhythms
             ]
             vs = [
                 [circs[i].point_from_proportion(p) for p in ps[i]]
                 for i in range(N)
             ]
             geoms = [Polygon(*v).set_stroke(colors[i],14,op) for i,v in enumerate(vs)]
+            for g in geoms: 
+                g.add_updater(lambda _,dt:None)
 
             dots = []
             for i in range(N):
                 dots.append(
                     Dot([0,3.5,0], dr*1.5, color=colors[i]).set_opacity(1)
                 )
                 dots[-1]._i = i
```

### Comparing `polybeat-1.0.0/polybeat/sounds/kick_drum.wav` & `polybeat-1.1.0/polybeat/sounds/kick_drum.wav`

 * *Files identical despite different names*

### Comparing `polybeat-1.0.0/polybeat/sounds/low_bongo.wav` & `polybeat-1.1.0/polybeat/sounds/low_bongo.wav`

 * *Files identical despite different names*

### Comparing `polybeat-1.0.0/polybeat/sounds/open_conga.wav` & `polybeat-1.1.0/polybeat/sounds/open_conga.wav`

 * *Files identical despite different names*

### Comparing `polybeat-1.0.0/polybeat/sounds/side_stick.wav` & `polybeat-1.1.0/polybeat/sounds/side_stick.wav`

 * *Files identical despite different names*

### Comparing `polybeat-1.0.0/polybeat.egg-info/PKG-INFO` & `polybeat-1.1.0/polybeat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polybeat
-Version: 1.0.0
+Version: 1.1.0
 Summary: A toy for visualizing polyrhythms
 Home-page: https://github.com/chunribu/polybeat/
 Author: Jian Jiang
 Author-email: pccfreespace@gmail.com
 License: MIT
 Keywords: polybeat polyrhythm pccfs
 Classifier: Operating System :: POSIX :: Linux
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # Polybeat
 
 
 
-https://github.com/chunribu/polybeat/assets/57521167/1bad0cd3-3feb-4222-8fea-8398ac4c3689
+https://github.com/chunribu/polybeat/assets/57521167/2c2e6025-2490-4b45-b54e-92f1c06b1c04
 
 
 
 ## Installation
 ```shell
 # first, install manim from conda-forge channel
 conda install -c conda-forge manim
@@ -39,26 +39,26 @@
 # step 2:
 # primary usage
 play([3,4,12])
 
 # advanced usage
 play(
     rhythms=[3,4,6,12],
-    custom_order=None,
-    colors=[RED,YELLOW,BLUE,GREEN],
+    custom_order=[0,1,3,2],
+    # colors=[RED,YELLOW,BLUE,GREEN],
     sounds=['kick_drum','open_conga','side_stick','low_bongo'],
     volumes=[0,-2,-6,-4],
     cycle_time=1.8,
     dot_radius=0.16,
     width_range=[2.5,3.5],
     preview=True,
 )
 ```
 
-`custom_order` is None by default, which equals [0,1,2,3] in this case.
+`custom_order` is None by default, which equals to [3,2,1,0] (reverse order) in this case.
 
 `colors` should be a list of variables supported by manim or hex number strings, e.g. ['#3ec1d3', '#f6f7d7', '#ff9a00', '#ff165d'].
 
 `sounds` can be paths to custom audio files, or just leave it default.
 
 `cycle_time` has an effect on speed.
```

### Comparing `polybeat-1.0.0/setup.py` & `polybeat-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='polybeat',
-    version='1.0.0',
+    version='1.1.0',
     description='A toy for visualizing polyrhythms',
     url='https://github.com/chunribu/polybeat/',
     author='Jian Jiang',
     author_email='pccfreespace@gmail.com',
     packages=find_packages(),
     license='MIT',
     long_description=long_description,
```

