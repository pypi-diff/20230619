# Comparing `tmp/pianoplayer-2.2.0.tar.gz` & `tmp/pianoplayer-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pianoplayer-2.2.0.tar", last modified: Sun Jan 24 22:43:29 2021, max compression
+gzip compressed data, was "pianoplayer-2.2.1.tar", last modified: Mon Jun 19 15:29:45 2023, max compression
```

## Comparing `pianoplayer-2.2.0.tar` & `pianoplayer-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 musy      (1000) musy      (1000)        0 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/
--rw-rw-r--   0 musy      (1000) musy      (1000)       31 2021-01-24 22:26:07.000000 pianoplayer-2.2.0/MANIFEST.in
--rw-rw-r--   0 musy      (1000) musy      (1000)      889 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/PKG-INFO
--rw-r--r--   0 musy      (1000) musy      (1000)     6200 2021-01-24 22:33:24.000000 pianoplayer-2.2.0/README.md
-drwxrwxr-x   0 musy      (1000) musy      (1000)        0 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/bin/
--rwxr-xr-x   0 musy      (1000) musy      (1000)     9789 2021-01-24 22:13:52.000000 pianoplayer-2.2.0/bin/pianoplayer
-drwxrwxr-x   0 musy      (1000) musy      (1000)        0 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/pianoplayer/
--rw-r--r--   0 musy      (1000) musy      (1000)      326 2021-01-24 22:40:16.000000 pianoplayer-2.2.0/pianoplayer/__init__.py
--rw-r--r--   0 musy      (1000) musy      (1000)    10900 2021-01-24 21:20:36.000000 pianoplayer-2.2.0/pianoplayer/hand.py
--rw-r--r--   0 musy      (1000) musy      (1000)     6606 2021-01-24 20:50:53.000000 pianoplayer-2.2.0/pianoplayer/scorereader.py
--rw-r--r--   0 musy      (1000) musy      (1000)     2759 2021-01-24 19:52:12.000000 pianoplayer-2.2.0/pianoplayer/utils.py
--rw-r--r--   0 musy      (1000) musy      (1000)     8759 2021-01-22 22:36:19.000000 pianoplayer-2.2.0/pianoplayer/vkeyboard.py
--rw-r--r--   0 musy      (1000) musy      (1000)     2897 2021-01-24 22:41:15.000000 pianoplayer-2.2.0/pianoplayer/wavegenerator.py
-drwxrwxr-x   0 musy      (1000) musy      (1000)        0 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/pianoplayer.egg-info/
--rw-rw-r--   0 musy      (1000) musy      (1000)      889 2021-01-24 22:43:28.000000 pianoplayer-2.2.0/pianoplayer.egg-info/PKG-INFO
--rw-rw-r--   0 musy      (1000) musy      (1000)      647 2021-01-24 22:43:28.000000 pianoplayer-2.2.0/pianoplayer.egg-info/SOURCES.txt
--rw-rw-r--   0 musy      (1000) musy      (1000)        1 2021-01-24 22:43:28.000000 pianoplayer-2.2.0/pianoplayer.egg-info/dependency_links.txt
--rw-rw-r--   0 musy      (1000) musy      (1000)       13 2021-01-24 22:43:28.000000 pianoplayer-2.2.0/pianoplayer.egg-info/requires.txt
--rw-rw-r--   0 musy      (1000) musy      (1000)       12 2021-01-24 22:43:28.000000 pianoplayer-2.2.0/pianoplayer.egg-info/top_level.txt
-drwxrwxr-x   0 musy      (1000) musy      (1000)        0 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/scores/
--rw-r--r--   0 musy      (1000) musy      (1000)   116055 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/bach_airgstring.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   181154 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/bach_invention4.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   233912 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/bach_joy.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   199109 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/bach_prelude.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   274821 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/clayderman_ladyd.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   384537 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/couperin_baricades.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   483085 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/mozart_sonfacile.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   165177 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/pachelbel_canon.xml
--rw-r--r--   0 musy      (1000) musy      (1000)    77537 2018-09-03 18:00:04.000000 pianoplayer-2.2.0/scores/test_chords.xml
--rw-rw-r--   0 musy      (1000) musy      (1000)    72972 2021-01-24 20:23:07.000000 pianoplayer-2.2.0/scores/test_octaves.xml
--rw-r--r--   0 musy      (1000) musy      (1000)   103293 2019-08-24 17:34:27.000000 pianoplayer-2.2.0/scores/test_scales.xml
--rw-rw-r--   0 musy      (1000) musy      (1000)       38 2021-01-24 22:43:29.000000 pianoplayer-2.2.0/setup.cfg
--rw-rw-r--   0 musy      (1000) musy      (1000)     1841 2021-01-24 22:40:31.000000 pianoplayer-2.2.0/setup.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-19 15:29:44.978411 pianoplayer-2.2.1/
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1067 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/LICENSE
+-rw-r-----   0 musy      (8766) sharpe    (4311)       31 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/MANIFEST.in
+-rw-r-----   0 musy      (8766) sharpe    (4311)      857 2023-06-19 15:29:44.977412 pianoplayer-2.2.1/PKG-INFO
+-rw-r-----   0 musy      (8766) sharpe    (4311)     6148 2023-06-19 15:21:56.000000 pianoplayer-2.2.1/README.md
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-19 15:29:44.765420 pianoplayer-2.2.1/bin/
+-rwxr-x---   0 musy      (8766) sharpe    (4311)     9789 2023-06-19 14:24:46.000000 pianoplayer-2.2.1/bin/pianoplayer
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-19 15:29:44.823422 pianoplayer-2.2.1/pianoplayer/
+-rw-r-----   0 musy      (8766) sharpe    (4311)      326 2023-06-19 15:26:03.000000 pianoplayer-2.2.1/pianoplayer/__init__.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)    11000 2023-06-19 14:59:24.000000 pianoplayer-2.2.1/pianoplayer/hand.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     6611 2023-06-19 14:35:21.000000 pianoplayer-2.2.1/pianoplayer/scorereader.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2755 2023-06-19 15:22:43.000000 pianoplayer-2.2.1/pianoplayer/utils.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     9402 2023-06-19 15:10:24.000000 pianoplayer-2.2.1/pianoplayer/vkeyboard.py
+-rw-r-----   0 musy      (8766) sharpe    (4311)     2897 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/pianoplayer/wavegenerator.py
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-19 15:29:44.869418 pianoplayer-2.2.1/pianoplayer.egg-info/
+-rw-r-----   0 musy      (8766) sharpe    (4311)      857 2023-06-19 15:29:44.000000 pianoplayer-2.2.1/pianoplayer.egg-info/PKG-INFO
+-rw-r-----   0 musy      (8766) sharpe    (4311)      655 2023-06-19 15:29:44.000000 pianoplayer-2.2.1/pianoplayer.egg-info/SOURCES.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)        1 2023-06-19 15:29:44.000000 pianoplayer-2.2.1/pianoplayer.egg-info/dependency_links.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)       13 2023-06-19 15:29:44.000000 pianoplayer-2.2.1/pianoplayer.egg-info/requires.txt
+-rw-r-----   0 musy      (8766) sharpe    (4311)       12 2023-06-19 15:29:44.000000 pianoplayer-2.2.1/pianoplayer.egg-info/top_level.txt
+drwxr-x---   0 musy      (8766) sharpe    (4311)        0 2023-06-19 15:29:44.972412 pianoplayer-2.2.1/scores/
+-rw-r-----   0 musy      (8766) sharpe    (4311)   116055 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/bach_airgstring.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   181154 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/bach_invention4.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   233912 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/bach_joy.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   199109 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/bach_prelude.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   274821 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/clayderman_ladyd.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   384537 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/couperin_baricades.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   483085 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/mozart_sonfacile.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   165177 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/pachelbel_canon.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)    77537 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/test_chords.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)    72972 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/test_octaves.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)   103293 2023-06-19 13:19:42.000000 pianoplayer-2.2.1/scores/test_scales.xml
+-rw-r-----   0 musy      (8766) sharpe    (4311)       38 2023-06-19 15:29:44.979416 pianoplayer-2.2.1/setup.cfg
+-rw-r-----   0 musy      (8766) sharpe    (4311)     1360 2023-06-19 15:29:01.000000 pianoplayer-2.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pianoplayer-2.2.0/PKG-INFO` & `pianoplayer-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pianoplayer
-Version: 2.2.0
+Version: 2.2.1
 Summary: Automatic piano fingering generator. Finds and shows in 3D the best fingering combination to play a score.
 Home-page: https://github.com/marcomusy/pianoplayer
 Author: Marco Musy
 Author-email: marco.musy@gmail.com
 License: MIT
-Description: Automatic piano fingering generator.
-            Finds and shows in a 3D visualization the best fingering combination to play a score.
-        
-            Check out https://github.com/marcomusy/pianoplayer for documentation.
 Keywords: piano fingering
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE
+
+Automatic piano fingering generator.
+    Finds and shows in a 3D visualization the best fingering combination to play a score.
+
+    Check out https://github.com/marcomusy/pianoplayer for documentation.
```

### Comparing `pianoplayer-2.2.0/README.md` & `pianoplayer-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 Find the optimal fingering combination to play a piano score.
 Optionally visualize it in 3D with [vedo](https://github.com/marcomusy/vedo).<br />
 
 ## Download and Install:
 ```bash
 pip install pianoplayer
 ```
-to enable sound you may need to:
-```bash
-sudo apt install libasound2-dev
-pip install simpleaudio
-```
+
+Note that this will install the `ninenotes_patch` branch.
 
 #### Installing without 3D rendering
 To only install the core functionality and skip everything else, use the following:
 ```bash
 pip install music21
 pip install --no-deps pianoplayer
 ```
@@ -37,15 +34,15 @@
 on their desktop (edit the path to your local anaconda or python installation).
 Check out [this link](https://github.com/marcomusy/pianoplayer/issues/27) in case of
 installation problems.
 
 
 ## CLI Usage:
 Example command line from terminal:<br />
-`pianoplayer scores/bach_invention4.xml --verbose -n10 -rvzm`<br />
+`pianoplayer scores/bach_invention4.xml -n10 -rvzm`<br />
 will find the right hand fingering for the first 10 measures,
 pop up a 3D rendering window and invoke *musescore*.
 
 The output is saved as a [MusicXML](https://en.wikipedia.org/wiki/MusicXML)
 file with name `output.xml`.<br />
 
 ```bash
```

### Comparing `pianoplayer-2.2.0/bin/pianoplayer` & `pianoplayer-2.2.1/bin/pianoplayer`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/pianoplayer/hand.py` & `pianoplayer-2.2.1/pianoplayer/hand.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,30 +191,33 @@
                 if an.measure > start_measure + nmeasures : break
 
             if i > N-11:
                 self.autodepth = False
                 self.depth = 9
 
             best_finger = 0
+            ninenotes = None
             if i > N-10:
-                if len(out)>1: best_finger = out.pop(1)
+                if len(out)>1: 
+                    best_finger = out.pop(1)
+                ninenotes = self.noteseq[N-9 : N]
             else:
                 ninenotes = self.noteseq[i : i+9]
                 out, vel  = self.optimize_seq(ninenotes, start_finger)
                 best_finger  = out[0]
                 start_finger = out[1]
 
             an.fingering = best_finger
             self.set_fingers_positions(out, ninenotes, 0)
             self.fingerseq.append(list(self.cfps))
 
             if best_finger>0 and i < N-3:
                 fng = Fingering(best_finger)
                 if an.isChord:
-                    if len(an.chord21.pitches) < 3:
+                    if len(an.chord21.pitches) < 4:
                         # dont show fingering in the lyrics line for >3 note-chords
                         if self.lyrics:
                             nl = len(an.chord21.pitches) - an.chordnr
                             an.chord21.addLyric(best_finger, nl)
                         else:
                             an.chord21.articulations.append(fng)
                 else:
```

### Comparing `pianoplayer-2.2.0/pianoplayer/scorereader.py` & `pianoplayer-2.2.1/pianoplayer/scorereader.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 def reader(sf, beam=0):
 
     noteseq = []
 
     if hasattr(sf, 'parts'):
         if len(sf.parts) <= beam:
             return []
-        strm = sf.parts[beam].flat
+        strm = sf.parts[beam].flatten()
     elif hasattr(sf, 'elements'):
         if len(sf.elements)==1 and beam==1:
             strm = sf[0]
         else:
             if len(sf) <= beam:
                 return []
             strm = sf[beam]
```

### Comparing `pianoplayer-2.2.0/pianoplayer/utils.py` & `pianoplayer-2.2.1/pianoplayer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,32 +40,32 @@
         return b
     else:
         return a
 
 
 def fpress(f, color):
     f.rotate(-20, axis=(1, 0, 0), point=f.pos())
-    f.addPos([0, 0, -1])
+    f.shift([0, 0, -1])
     f.color(color)
 
 
 def frelease(f):
-    f.addPos([0, 0, 1])
+    f.shift([0, 0, 1])
     f.rotate(20, axis=(1, 0, 0), point=f.pos())
     f.color((0.7, 0.3, 0.3))
 
 
 def kpress(f, color):
     f.rotate(4, axis=(1, 0, 0), point=f.pos())
-    f.addPos([0, 0, -0.4])
+    f.shift([0, 0, -0.4])
     f.color(color)
 
 
 def krelease(f):
-    f.addPos([0, 0, 0.4])
+    f.shift([0, 0, 0.4])
     p = f.pos()
     f.rotate(-4, axis=(1, 0, 0), point=p)
     if p[2] > 0.5:
         f.color("k")
     else:
         f.color("w")
```

### Comparing `pianoplayer-2.2.0/pianoplayer/vkeyboard.py` & `pianoplayer-2.2.1/pianoplayer/vkeyboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,210 +1,260 @@
 #!/usr/bin/env python3
-#-------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------
 # Name:         VirtualKeyboard
 # Purpose:      Find optimal fingering for piano scores
 # URL:          https://github.com/marcomusy/pianoplayer
 # Author:       Marco Musy
-#-------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------
 try:
     from vedo import Plotter, Assembly, printc
-    from vedo import Ellipsoid, Box, Cylinder, Text
+    from vedo import Ellipsoid, Box, Cylinder, Text3D
 except:
     pass
 
 from pianoplayer import __version__
 from pianoplayer.utils import fpress, frelease, kpress, krelease, nameof
 from pianoplayer.wavegenerator import playSound
 import pianoplayer.utils as utils
 
 
 ###########################################################
 class VirtualKeyboard:
-
-    def __init__(self, songname=''):
+    def __init__(self, songname=""):
 
         self.KB = dict()
         self.vp = None
         self.rightHand = None
-        self.leftHand  = None
+        self.leftHand = None
         self.vpRH = None
         self.vpLH = None
         self.playsounds = True
         self.verbose = True
         self.songname = songname
-        self.t0 = 0 # keep track of how many seconds to play
+        self.t0 = 0  # keep track of how many seconds to play
         self.dt = 0.1
         self.speedfactor = 1
-        self.engagedfingersR = [False]*6 # element 0 is dummy
-        self.engagedfingersL = [False]*6
-        self.engagedkeysR    = []
-        self.engagedkeysL    = []
+        self.engagedfingersR = [False] * 6  # element 0 is dummy
+        self.engagedfingersL = [False] * 6
+        self.engagedkeysR = []
+        self.engagedkeysL = []
         self.build_keyboard()
 
     ################################################################################
     def makeHandActor(self, f=1):
-        a1, a2, a3, c = (10*f,0,0), (0,7*f,0), (0,0,3*f), (.7,0.3,0.3)
-        palm = Ellipsoid(pos=(0,-3,0), axis1=a1, axis2=a2, axis3=a3, alpha=0.6, c=c)
-        wrist= Box(pos=(0,-9,0), length=6*f, width=5, height=2, alpha=0.4, c=c)
-        arm  = Assembly([palm,wrist])
-        f1 = Cylinder((-2, 1.5,0), axis=(0,1,0), height=5, r=.8*f, c=c)
-        f2 = Cylinder((-1, 3  ,0), axis=(0,1,0), height=6, r=.7*f, c=c)
-        f3 = Cylinder(( 0, 4  ,0), axis=(0,1,0), height=6.2, r=.75*f, c=c)
-        f4 = Cylinder(( 1, 3.5,0), axis=(0,1,0), height=6.1, r=.7*f, c=c)
-        f5 = Cylinder(( 2, 2  ,0), axis=(0,1,0), height=5, r=.6*f, c=c)
-        self.vp += [arm, f1,f2,f3,f4,f5] # add actors to internal list
-        return [arm, f1,f2,f3,f4,f5]
+        a1, a2, a3, c = (10 * f, 0, 0), (0, 7 * f, 0), (0, 0, 3 * f), (0.7, 0.3, 0.3)
+        palm = Ellipsoid(pos=(0, -3, 0), axis1=a1, axis2=a2, axis3=a3, alpha=0.6, c=c)
+        wrist = Box(pos=(0, -9, 0), length=6 * f, width=5, height=2, alpha=0.4, c=c)
+        arm = Assembly([palm, wrist])
+        f1 = Cylinder((-2, 1.5, 0), axis=(0, 1, 0), height=5, r=0.8 * f, c=c)
+        f2 = Cylinder((-1, 3, 0), axis=(0, 1, 0), height=6, r=0.7 * f, c=c)
+        f3 = Cylinder((0, 4, 0), axis=(0, 1, 0), height=6.2, r=0.75 * f, c=c)
+        f4 = Cylinder((1, 3.5, 0), axis=(0, 1, 0), height=6.1, r=0.7 * f, c=c)
+        f5 = Cylinder((2, 2, 0), axis=(0, 1, 0), height=5, r=0.6 * f, c=c)
+        self.vp += [arm, f1, f2, f3, f4, f5]  # add actors to internal list
+        return [arm, f1, f2, f3, f4, f5]
 
-    def build_RH(self, hand): #########################Build Right Hand
+    def build_RH(self, hand):  #########################Build Right Hand
         self.rightHand = hand
         f = utils.handSizeFactor(hand.size)
         self.vpRH = self.makeHandActor(f)
-        for limb in self.vpRH: # initial x positions are superseded later
-            limb.x( limb.x()* 2.5 )
-            limb.addPos([16.5*5+1, -7.5, 3] )
+        for limb in self.vpRH:  # initial x positions are superseded later
+            limb.x(limb.x() * 2.5)
+            limb.shift([16.5 * 5 + 1, -7.5, 3])
 
-    def build_LH(self, hand): ########################Build Left Hand
+    def build_LH(self, hand):  ########################Build Left Hand
         self.leftHand = hand
         f = utils.handSizeFactor(hand.size)
         self.vpLH = self.makeHandActor(f)
         for limb in self.vpLH:
-            limb.x( limb.x()* 2.5 )
-            limb.addPos([16.5*3+1, -7.5, 3] )
-
+            limb.x(limb.x() * 2.5)
+            limb.shift([16.5 * 3 + 1, -7.5, 3])
 
     #######################################################Build Keyboard
     def build_keyboard(self):
-        nts = ("C","D","E","F","G","A","B")
+        nts = ("C", "D", "E", "F", "G", "A", "B")
         tol = 0.12
-        keybsize = 16.5 # in cm, span of one octave
-        wb = keybsize/7
+        keybsize = 16.5  # in cm, span of one octave
+        wb = keybsize / 7
         nr_octaves = 7
-        span = nr_octaves*wb*7
+        span = nr_octaves * wb * 7
 
-        self.vp = Plotter(title='PianoPlayer '+__version__,
-                          axes=0, size=(1400,700), bg='cornsilk', bg2='lb')
-
-        #wooden top and base
-        self.vp += Box(pos=(span/2+keybsize, 6, 1),
-                       length=span+1, height=3, width= 5).texture('wood1')
-        self.vp += Box(pos=(span/2+keybsize, 0, -1),
-                       length=span+1, height=1, width=17).texture('wood1')
-        self.vp += Text('PianoPlayer ^'+__version__+" ",
-                        pos=(18, 5., 2.3), depth=.5, c='silver', italic=0.8)
-        leggio = Box(pos=(span/1.55,8,10),
-                     length=span/2, height=span/8, width=0.08, c=(1,1,0.9)).rotateX(-20)
-        self.vp += leggio.texture('paper1')
-        self.vp += Text('Playing:\n'+self.songname[-30:].replace('_',"\\_"), font="Theemim",
-                        vspacing=3, depth=0.04, s=1.35, c='k', italic=0.5
-                       ).rotateX(70).pos([55,10,6])
+        self.vp = Plotter(
+            title="PianoPlayer " + __version__,
+            axes=0,
+            size=(1400, 700),
+            bg="cornsilk",
+            bg2="lb",
+        )
+
+        # wooden top and base
+        self.vp += Box(
+            pos=(span / 2 + keybsize, 6, 1),
+            length=span + 1,
+            height=3,
+            width=5,
+            c="orange1",
+        )
+
+        self.vp += Box(
+            pos=(span / 2 + keybsize, 0, -1),
+            length=span + 1,
+            height=1,
+            width=17,
+            c="orange1",
+        )
+
+        self.vp += Text3D(
+            "PianoPlayer ^" + __version__ + " ",
+            pos=(18, 5.0, 2.3),
+            depth=0.5,
+            c="silver",
+            italic=0.8,
+        )
+
+        leggio = Box(
+            pos=(span / 1.55, 8, 10),
+            length=span / 2,
+            height=span / 8,
+            width=0.08,
+            c=(1, 1, 0.9),
+        ).rotate_x(-20)
+        self.vp += leggio
+
+        self.vp += (
+            Text3D(
+                "Playing:\n" + self.songname[-30:].replace("_", "\\_"),
+                font="Theemim",
+                vspacing=3,
+                depth=0.04,
+                s=1.35,
+                c="k",
+                italic=0.5,
+            )
+            .rotate_x(70)
+            .pos([55, 10, 6])
+        )
 
         for ioct in range(nr_octaves):
-            for ik in range(7):              #white keys
-                x  = ik * wb + (ioct+1)*keybsize +wb/2
-                tb = Box(pos=(x,-2,0), length=wb-tol, height=1, width=12, c='white')
-                self.KB.update({nts[ik]+str(ioct+1) : tb})
+            for ik in range(7):  # white keys
+                x = ik * wb + (ioct + 1) * keybsize + wb / 2
+                tb = Box(pos=(x, -2, 0), length=wb - tol, height=1, width=12, c="white")
+                self.KB.update({nts[ik] + str(ioct + 1): tb})
                 self.vp += tb
-                if not nts[ik] in ("E","B"): #black keys
-                    tn = Box(pos=(x+wb/2,0,1), length=wb*.6, height=1, width=8, c='black')
-                    self.KB.update({nts[ik]+"#"+str(ioct+1) : tn})
+                if not nts[ik] in ("E", "B"):  # black keys
+                    tn = Box(
+                        pos=(x + wb / 2, 0, 1),
+                        length=wb * 0.6,
+                        height=1,
+                        width=8,
+                        c="black",
+                    )
+                    self.KB.update({nts[ik] + "#" + str(ioct + 1): tn})
                     self.vp += tn
-        cam = dict(pos=(110, -51.1, 89.1),
-                   focalPoint=(81.5, 0.531, 2.82),
-                   viewup=(-0.163, 0.822, 0.546),
-                   distance=105, clippingRange=(41.4, 179))
+        cam = dict(
+            pos=(110, -51.1, 89.1),
+            focal_point=(81.5, 0.531, 2.82),
+            viewup=(-0.163, 0.822, 0.546),
+            distance=105,
+            clipping_range=(41.4, 179),
+        )
         self.vp.show(interactive=0, camera=cam, resetcam=0)
 
-
     #####################################################################
     def play(self):
 
-        printc('Press space to proceed by one note', c=1)
-        printc('Press Esc to exit.', c=1)
+        printc("Press space to proceed by one note", c=1)
+        printc("Press Esc to exit.", c=1)
 
         if self.rightHand:
-            self.engagedkeysR    = [False]*len(self.rightHand.noteseq)
-            self.engagedfingersR = [False]*6  # element 0 is dummy
+            self.engagedkeysR = [False] * len(self.rightHand.noteseq)
+            self.engagedfingersR = [False] * 6  # element 0 is dummy
         if self.leftHand:
-            self.engagedkeysL    = [False]*len(self.leftHand.noteseq)
-            self.engagedfingersL = [False]*6
+            self.engagedkeysL = [False] * len(self.leftHand.noteseq)
+            self.engagedfingersL = [False] * 6
 
-        t=0.0
+        t = 0.0
         while True:
-            if self.rightHand: self._moveHand( 1, t)
-            if self.leftHand:  self._moveHand(-1, t)
-            if t > 1000: break
-            t += self.dt                      # absolute time flows
+            if self.rightHand:
+                self._moveHand(1, t)
+            if self.leftHand:
+                self._moveHand(-1, t)
+            if t > 1000:
+                break
+            t += self.dt  # absolute time flows
 
-        if self.verbose: printc('End of note sequence reached.')
-        self.vp.keyPressFunction = None       # disable observer
+        if self.verbose:
+            printc("End of note sequence reached.")
 
     ###################################################################
-    def _moveHand(self, side, t):############# runs inside play() loop
+    def _moveHand(self, side, t):  ############# runs inside play() loop
 
         if side == 1:
-            c1, c2         = 'tomato', 'orange'
-            engagedkeys    = self.engagedkeysR
+            c1, c2 = "tomato", "orange"
+            engagedkeys = self.engagedkeysR
             engagedfingers = self.engagedfingersR
-            H              = self.rightHand
-            vpH            = self.vpRH
+            H = self.rightHand
+            vpH = self.vpRH
         else:
-            c1, c2         = 'purple', 'mediumpurple'
-            engagedkeys    = self.engagedkeysL
+            c1, c2 = "purple", "mediumpurple"
+            engagedkeys = self.engagedkeysL
             engagedfingers = self.engagedfingersL
-            H              = self.leftHand
-            vpH            = self.vpLH
+            H = self.leftHand
+            vpH = self.vpLH
 
-        for i, n in enumerate(H.noteseq):#####################
-            start, stop, f = n.time, n.time+n.duration, n.fingering
-            if isinstance(f, str): continue
-            if f and stop <= t <= stop+self.dt and engagedkeys[i]: #release key
-                engagedkeys[i]    = False
+        for i, n in enumerate(H.noteseq):  #####################
+            start, stop, f = n.time, n.time + n.duration, n.fingering
+            if isinstance(f, str):
+                continue
+            if f and stop <= t <= stop + self.dt and engagedkeys[i]:  # release key
+                engagedkeys[i] = False
                 engagedfingers[f] = False
                 name = nameof(n)
                 krelease(self.KB[name])
                 frelease(vpH[f])
-                if hasattr(self.vp, 'interactor'):
+                if hasattr(self.vp, "interactor"):
                     self.vp.render()
 
-        for i, n in enumerate(H.noteseq):#####################
-            start, stop, f = n.time, n.time+n.duration, n.fingering
+        for i, n in enumerate(H.noteseq):  #####################
+            start, stop, f = n.time, n.time + n.duration, n.fingering
             if isinstance(f, str):
-                print('Warning: cannot understand lyrics:',f, 'skip note',i)
+                print("Warning: cannot understand lyrics:", f, "skip note", i)
                 continue
             if f and start <= t < stop and not engagedkeys[i] and not engagedfingers[f]:
                 # press key
-                if i >= len(H.fingerseq): return
-                engagedkeys[i]    = True
+                if i >= len(H.fingerseq):
+                    return
+                engagedkeys[i] = True
                 engagedfingers[f] = True
                 name = nameof(n)
 
-                if t> self.t0 + self.vp.clock:
+                if t > self.t0 + self.vp.clock:
                     self.t0 = t
                     self.vp.show(interactive=False, resetcam=False)
 
-                for g in [1,2,3,4,5]:
-                    vpH[g].x( side * H.fingerseq[i][g] )
-                vpH[0].x(vpH[3].x()) # index 0 is arm, put it where middle finger is
+                for g in [1, 2, 3, 4, 5]:
+                    vpH[g].x(side * H.fingerseq[i][g])
+                vpH[0].x(vpH[3].x())  # index 0 is arm, put it where middle finger is
 
-                fpress(vpH[f],  c1)
+                fpress(vpH[f], c1)
                 kpress(self.KB[name], c2)
 
                 if self.verbose:
-                    msg = 'meas.'+str(n.measure)+' t='+str(round(t,2))
-                    if side==1: printc(msg,'\t\t\t\tRH.finger', f, 'hit', name, c='b')
-                    else:       printc(msg,      '\tLH.finger', f, 'hit', name, c='m')
+                    msg = "meas." + str(n.measure) + " t=" + str(round(t, 2))
+                    if side == 1:
+                        printc(msg, "\t\t\t\tRH.finger", f, "hit", name, c="b")
+                    else:
+                        printc(msg, "\tLH.finger", f, "hit", name, c="m")
 
                 if self.playsounds:
                     self.vp.show(interactive=False, resetcam=False)
                     playSound(n, self.speedfactor, wait=True)
-                    if hasattr(self.vp, 'interactor'):
+                    if hasattr(self.vp, "interactor"):
                         self.vp.interactor.Start()
                 else:
                     self.vp.show(interactive=1, resetcam=0)
 
 
 ############################ test
 if __name__ == "__main__":
-    vk = VirtualKeyboard('Chopin Valse in A minor')
-    vk.vp.show(interactive=1, resetcam=0)
-
-
+    vk = VirtualKeyboard("Chopin Valse in A minor")
+    vk.vp.show(interactive=True, resetcam=False)
```

### Comparing `pianoplayer-2.2.0/pianoplayer/wavegenerator.py` & `pianoplayer-2.2.1/pianoplayer/wavegenerator.py`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/pianoplayer.egg-info/PKG-INFO` & `pianoplayer-2.2.1/pianoplayer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pianoplayer
-Version: 2.2.0
+Version: 2.2.1
 Summary: Automatic piano fingering generator. Finds and shows in 3D the best fingering combination to play a score.
 Home-page: https://github.com/marcomusy/pianoplayer
 Author: Marco Musy
 Author-email: marco.musy@gmail.com
 License: MIT
-Description: Automatic piano fingering generator.
-            Finds and shows in a 3D visualization the best fingering combination to play a score.
-        
-            Check out https://github.com/marcomusy/pianoplayer for documentation.
 Keywords: piano fingering
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE
+
+Automatic piano fingering generator.
+    Finds and shows in a 3D visualization the best fingering combination to play a score.
+
+    Check out https://github.com/marcomusy/pianoplayer for documentation.
```

### Comparing `pianoplayer-2.2.0/pianoplayer.egg-info/SOURCES.txt` & `pianoplayer-2.2.1/pianoplayer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 bin/pianoplayer
 pianoplayer/__init__.py
 pianoplayer/hand.py
 pianoplayer/scorereader.py
```

### Comparing `pianoplayer-2.2.0/scores/bach_airgstring.xml` & `pianoplayer-2.2.1/scores/bach_airgstring.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/bach_invention4.xml` & `pianoplayer-2.2.1/scores/bach_invention4.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/bach_joy.xml` & `pianoplayer-2.2.1/scores/bach_joy.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/bach_prelude.xml` & `pianoplayer-2.2.1/scores/bach_prelude.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/clayderman_ladyd.xml` & `pianoplayer-2.2.1/scores/clayderman_ladyd.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/couperin_baricades.xml` & `pianoplayer-2.2.1/scores/couperin_baricades.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/mozart_sonfacile.xml` & `pianoplayer-2.2.1/scores/mozart_sonfacile.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/pachelbel_canon.xml` & `pianoplayer-2.2.1/scores/pachelbel_canon.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/test_chords.xml` & `pianoplayer-2.2.1/scores/test_chords.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/test_octaves.xml` & `pianoplayer-2.2.1/scores/test_octaves.xml`

 * *Files identical despite different names*

### Comparing `pianoplayer-2.2.0/scores/test_scales.xml` & `pianoplayer-2.2.1/scores/test_scales.xml`

 * *Files identical despite different names*

