# Comparing `tmp/CKAstroTools-0.0.2.tar.gz` & `tmp/CKAstroTools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/koenig/PycharmProjects/ckastrotools/dist/.tmp-sby0dqam/CKAstroTools-0.0.2.tar", last modified: Sun Jun 18 09:39:16 2023, max compression
+gzip compressed data, was "CKAstroTools-0.0.3.tar", last modified: Mon Jun 19 09:22:16 2023, max compression
```

## Comparing `CKAstroTools-0.0.2.tar` & `CKAstroTools-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      750 2023-06-18 09:30:05.000000 CKAstroTools-0.0.2/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/ckastrotools/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/ckastrotools/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.2/ckastrotools/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.2/ckastrotools/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    16547 2023-06-16 04:26:53.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-18 09:37:37.000000 CKAstroTools-0.0.2/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.039456 CKAstroTools-0.0.3/CKAstroTools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-19 09:22:16.000000 CKAstroTools-0.0.3/CKAstroTools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      750 2023-06-18 09:30:05.000000 CKAstroTools-0.0.3/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.039456 CKAstroTools-0.0.3/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.3/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.3/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.3/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    17474 2023-06-19 09:19:24.000000 CKAstroTools-0.0.3/ckastrotools/milkyway/spiralarms.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-19 09:20:37.000000 CKAstroTools-0.0.3/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-19 09:22:16.043457 CKAstroTools-0.0.3/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.3/tests/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `CKAstroTools-0.0.2/CKAstroTools.egg-info/PKG-INFO` & `CKAstroTools-0.0.3/CKAstroTools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.2
+Version: 0.0.3
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.2/LICENSE` & `CKAstroTools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.2/PKG-INFO` & `CKAstroTools-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.2
+Version: 0.0.3
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.2/README.md` & `CKAstroTools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.2/ckastrotools/io/subcube.py` & `CKAstroTools-0.0.3/ckastrotools/io/subcube.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.2/ckastrotools/milkyway/spiralarms.py` & `CKAstroTools-0.0.3/ckastrotools/milkyway/spiralarms.py`

 * *Files 14% similar despite different names*

```diff
@@ -156,28 +156,28 @@
         'outer0': {'R_ref': 12.24,  # kpc
                    'beta_ref': 18.,  # deg (from Galactic center to sun =0)
                    'pitch': 9.4,  # deg
                    'width': 0.65}}  # kpc
 
     ck = {'perseus': {'R_ref': 10.9,  # kpc
                       'beta_ref': -16.6,  # deg (from Galactic center to sun =0)
-                      'beta_min': 180.0,  # deg
-                      'beta_max': 280.0,  # deg
+                      'beta_min': -91.415,  # deg (i.e. ~l=280)
+                      'beta_max': 0.0,  # deg (i.e. ~l=180)
                       'pitch': 5.7,  # deg
                       'width': 0.38},  # kpc
           'local': {'R_ref': 9.8,  # kpc
                     'beta_ref': -0.5,  # deg (from Galactic center to sun =0)
-                    'beta_min': 180.0,  # deg
-                    'beta_max': 280.0,  # deg
+                    'beta_min': -91.415,  # deg (i.e. ~l=280)
+                    'beta_max': 0.0,  # deg (i.e. ~l=180)
                     'pitch': -24,  # deg
                     'width': 0.33},  # kpc
           'outer': {'R_ref': 14.4,  # kpc
-                    'beta_ref': -23.5,  # deg (from Galactic center to sun =0)
-                    'beta_min': 180.0,  # deg
-                    'beta_max': 280.0,  # deg
+                    'beta_ref': 180.,  # deg (from Galactic center to sun =0)
+                    'beta_min': -91.415,  # deg (i.e. ~l=280)
+                    'beta_max': 0.0,  # deg (i.e. ~l=180)
                     'pitch': 15.8,  # deg
                     'width': 0.63}}  # kpc
 
     xinyu2016 = {'outer': {'R_ref': 13.6,  # kpc
                            'beta_ref': 26.9,  # deg (from Galactic center to sun =0)
                            'beta_min': -110.0,  # deg
                            'beta_max': 270.0,  # deg
@@ -219,26 +219,52 @@
         spiral_arm_params = vallee2015
     elif model == 'ck':
         spiral_arm_params = ck
 
     return spiral_arm_params
 
 
-def getSpiralArmXY(spiral_name, beta_min=-110, beta_max=270., model='reid2014',
-                   resolution=0.0001, R_0=8.34):
+def getSpiralArm(name, model='reid2014', beta_min=None, beta_max=None,
+                 resolution=0.0001, R_0=8.34):
+    """
+    Get the spiral arm model for a given arm name.
+
+    Parameters
+    ----------
+    name: str
+        Name of the spiral arm.
+    model: str
+        Name of the spiral arm model to be used.
+    beta_min: float
+        Minimum galactocentric angle in degrees (0=GC to sun, clockwise).
+        If None, the default value.
+    beta_max: float
+        Maximum galactocentric angle in degrees (0=GC to sun, clockwise).
+        If None, the default value.
+    resolution: float
+        Resolution of the spiral arm model in degrees.
+    R_0: float
+        Galactocentric distance of the sun in kpc.
+
+    Returns
+    -------
+    Coordinates of the spiral arm in the galactocentric frame.
+    """
     spiral_arm_params = _getSpiralParameters(model)
 
-    R_ref = spiral_arm_params[spiral_name]['R_ref']
-    beta_ref = spiral_arm_params[spiral_name]['beta_ref']
-    pitch = spiral_arm_params[spiral_name]['pitch']
+    R_ref = spiral_arm_params[name]['R_ref']
+    beta_ref = spiral_arm_params[name]['beta_ref']
+    pitch = spiral_arm_params[name]['pitch']
     if beta_min is None:
-        beta_min = spiral_arm_params[spiral_name]['beta_min']
+        beta_min = spiral_arm_params[name]['beta_min']
     if beta_max is None:
-        beta_max = spiral_arm_params[spiral_name]['beta_max']
-
+        beta_max = spiral_arm_params[name]['beta_max']
+    print(beta_min)
+    print(beta_max)
+    print(resolution)
     beta = np.arange(beta_max, beta_min, -1. * resolution)  # [deg]
 
     R_gal = R_ref * np.exp(-1 * (beta - beta_ref) * np.pi / 180. * np.tan(np.pi / 180. * pitch))  # kpc
 
     #     x = R_gal * -1. * np.cos(beta * np.pi/180.)
     #     y = R_gal * np.sin(beta * np.pi/180.)
     x = -1 * R_gal * np.sin((90 - beta) * np.pi / 180.)
@@ -252,74 +278,85 @@
     return arm
 
 
 def getSpiralArmsDetail(model='reid2019'):
 
     # if model=='optimized':
     #     # SAGITTARIUS arm
-    #     svx1, svy1 = getSpiralArmXY('sagittarius', beta_min=-245., beta_max=-2, model='vallee2015')
-    #     sx, sy = getSpiralArmXY('sagittarius', beta_min=-2, beta_max=68, model='reid2014')
-    #     svx2, svy2 = getSpiralArmXY('sagittarius', beta_min=68, beta_max=225, model='vallee2015')
+    #     svx1, svy1 = getSpiralArm('sagittarius', beta_min=-245., beta_max=-2, model='vallee2015')
+    #     sx, sy = getSpiralArm('sagittarius', beta_min=-2, beta_max=68, model='reid2014')
+    #     svx2, svy2 = getSpiralArm('sagittarius', beta_min=68, beta_max=225, model='vallee2015')
     #
     #     # SCUTUM arm
-    #     scx, scy = getSpiralArmXY('scutum', beta_min=3, beta_max=101)
-    #     scvx, scvy = getSpiralArmXY('scutum', beta_min=35, beta_max=363, model='vallee2015')
-    #     scvx2, scvy2 = getSpiralArmXY('scutum', beta_min=461, beta_max=560, model='vallee2015')
+    #     scx, scy = getSpiralArm('scutum', beta_min=3, beta_max=101)
+    #     scvx, scvy = getSpiralArm('scutum', beta_min=35, beta_max=363, model='vallee2015')
+    #     scvx2, scvy2 = getSpiralArm('scutum', beta_min=461, beta_max=560, model='vallee2015')
     #
     #     # OUTER arm
-    #     ox, oy = getSpiralArmXY('outer', beta_min=-6, beta_max=56)
-    #     ovx, ovy = getSpiralArmXY('outer', beta_min=56, beta_max=410, model='vallee2015')
-    #     ockx, ocky = getSpiralArmXY('outer', beta_min=-70, beta_max=-6, model='ck')
+    #     ox, oy = getSpiralArm('outer', beta_min=-6, beta_max=56)
+    #     ovx, ovy = getSpiralArm('outer', beta_min=56, beta_max=410, model='vallee2015')
+    #     ockx, ocky = getSpiralArm('outer', beta_min=-70, beta_max=-6, model='ck')
     #
     #     # PERSEUS spiral arm
-    #     px, py = getSpiralArmXY('perseus', beta_min=-21, beta_max=88)
-    #     pvx, pvy = getSpiralArmXY('perseus', beta_min=90, beta_max=390, model='vallee2015')
-    #     pckx, pcky = getSpiralArmXY('perseus', beta_min=-40, beta_max=-10, model='ck')
-    #     pvx2, pvy2 = getSpiralArmXY('perseus', beta_min=-160, beta_max=-40, model='vallee2015')
+    #     px, py = getSpiralArm('perseus', beta_min=-21, beta_max=88)
+    #     pvx, pvy = getSpiralArm('perseus', beta_min=90, beta_max=390, model='vallee2015')
+    #     pckx, pcky = getSpiralArm('perseus', beta_min=-40, beta_max=-10, model='ck')
+    #     pvx2, pvy2 = getSpiralArm('perseus', beta_min=-160, beta_max=-40, model='vallee2015')
     #
     #     return sy, sx, svy1, svx1, svy2, svx2, scy, scx, scvy, scvx, scvy2, scvx2, oy, ox, ovy, ovx, ocky, ockx, py, px, pvy, pvx, pvy2, pvx2, pcky, pckx
     # else:
 
     # SAGITTARIUS arm
-    # svx1, svy1 = getSpiralArmXY('sagittarius', beta_min=-245., beta_max=-2, model=model)
-    # sx, sy = getSpiralArmXY('sagittarius', beta_min=-2, beta_max=68, model=model)
-    # svx2, svy2 = getSpiralArmXY('sagittarius', beta_min=68, beta_max=225, model=model)
+    # svx1, svy1 = getSpiralArm('sagittarius', beta_min=-245., beta_max=-2, model=model)
+    # sx, sy = getSpiralArm('sagittarius', beta_min=-2, beta_max=68, model=model)
+    # svx2, svy2 = getSpiralArm('sagittarius', beta_min=68, beta_max=225, model=model)
     # sag_x = list(svx1)+list(sx)+list(svx2)
     # sag_y = list(svy1)+list(sy)+list(svy2)
-    sagittarius = getSpiralArmXY('sagittarius', beta_min=-245., beta_max=225, model=model)
+    sagittarius = getSpiralArm('sagittarius', model=model, beta_min=-245., beta_max=225)
 
     # SCUTUM arm
-    # scx, scy = getSpiralArmXY('scutum', beta_min=3, beta_max=101, model=model)
-    # scvx, scvy = getSpiralArmXY('scutum', beta_min=101, beta_max=363, model=model)
-    # scvx2, scvy2 = getSpiralArmXY('scutum', beta_min=363, beta_max=560, model=model)
+    # scx, scy = getSpiralArm('scutum', beta_min=3, beta_max=101, model=model)
+    # scvx, scvy = getSpiralArm('scutum', beta_min=101, beta_max=363, model=model)
+    # scvx2, scvy2 = getSpiralArm('scutum', beta_min=363, beta_max=560, model=model)
     # scutum_x = list(scx)+list(scvx)+list(scvx2)
     # scutum_y = list(scy)+list(scvy)+list(scvy2)
-    scutum = getSpiralArmXY('scutum', beta_min=3, beta_max=560, model=model)
+    scutum = getSpiralArm('scutum', beta_max=560, model=model, beta_min=3)
 
     # OUTER arm
-    # ockx, ocky = getSpiralArmXY('outer', beta_min=-70, beta_max=-6, model=model)
-    # ox, oy = getSpiralArmXY('outer', beta_min=-6, beta_max=56, model=model)
-    # ovx, ovy = getSpiralArmXY('outer', beta_min=56, beta_max=410, model=model)
+    # ockx, ocky = getSpiralArm('outer', beta_min=-70, beta_max=-6, model=model)
+    # ox, oy = getSpiralArm('outer', beta_min=-6, beta_max=56, model=model)
+    # ovx, ovy = getSpiralArm('outer', beta_min=56, beta_max=410, model=model)
     # outer_x = list(ockx) + list(ox) + list(ovx)
     # outer_y = list(ocky) + list(oy) + list(ovy)
-    outer = getSpiralArmXY('outer', beta_min=-70, beta_max=410, model=model)
+    outer = getSpiralArm('outer', model=model, beta_min=-70, beta_max=410)
 
     # PERSEUS spiral arm
-    # pvx2, pvy2 = getSpiralArmXY('perseus', beta_min=-160, beta_max=-40, model=model)
-    # pckx, pcky = getSpiralArmXY('perseus', beta_min=-40, beta_max=-10, model=model)
-    # px, py = getSpiralArmXY('perseus', beta_min=-10, beta_max=90, model=model)
-    # pvx, pvy = getSpiralArmXY('perseus', beta_min=90, beta_max=390, model=model)
+    # pvx2, pvy2 = getSpiralArm('perseus', beta_min=-160, beta_max=-40, model=model)
+    # pckx, pcky = getSpiralArm('perseus', beta_min=-40, beta_max=-10, model=model)
+    # px, py = getSpiralArm('perseus', beta_min=-10, beta_max=90, model=model)
+    # pvx, pvy = getSpiralArm('perseus', beta_min=90, beta_max=390, model=model)
     # per_x = list(pckx) + list(pvx2) + list(px) + list(pvx)
     # per_y = list(pcky) + list(pvy2) + list(py) + list(pvy)
-    perseus = getSpiralArmXY('perseus', beta_min=-160, beta_max=390, model=model)
+    perseus = getSpiralArm('perseus', model=model, beta_min=-160, beta_max=390)
 
     return sagittarius, scutum, outer, perseus
 
 
 def getSpiralArms(model='vallee2015'):
+    """
+    Returns the spiral arms in a dictionary.
+
+    Parameters
+    ----------
+    model: The model to use
+
+    Returns
+    -------
+    dict: A dictionary with the spiral arms.
+    """
     sagittarius, scutum, outer, perseus = getSpiralArmsDetail(model=model)
 
     return {'sagittarius': sagittarius,
             'scutum': scutum,
             'perseus': perseus,
             'outer': outer}
     #
```

### Comparing `CKAstroTools-0.0.2/pyproject.toml` & `CKAstroTools-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CKAstroTools"
 description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

