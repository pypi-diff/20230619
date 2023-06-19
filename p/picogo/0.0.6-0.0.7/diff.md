# Comparing `tmp/picogo-0.0.6.tar.gz` & `tmp/picogo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picogo-0.0.6.tar", last modified: Mon Jun 19 03:17:18 2023, max compression
+gzip compressed data, was "picogo-0.0.7.tar", last modified: Mon Jun 19 03:22:04 2023, max compression
```

## Comparing `picogo-0.0.6.tar` & `picogo-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:17:18.141291 picogo-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0      799 2023-06-19 03:17:18.139292 picogo-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 03:17:18.121290 picogo-0.0.6/picogo/
--rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.6/picogo/ATemplate.py
--rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.6/picogo/Battery.py
--rw-rw-rw-   0        0        0     1327 2023-06-19 02:24:52.000000 picogo-0.0.6/picogo/BatteryTest.py
--rw-rw-rw-   0        0        0     9466 2023-06-19 02:03:56.000000 picogo-0.0.6/picogo/BlueTooth.py
--rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.6/picogo/BootselButton.py
--rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.6/picogo/BuzzerTest.py
--rw-rw-rw-   0        0        0       75 2023-06-19 02:25:11.000000 picogo-0.0.6/picogo/FirmwareVersion.py
--rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.6/picogo/HelloWorld.py
--rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.6/picogo/I2CScan.py
--rw-rw-rw-   0        0        0     1144 2023-06-19 02:25:42.000000 picogo-0.0.6/picogo/IRObstacleAvoidance.py
--rw-rw-rw-   0        0        0      301 2023-06-19 02:25:56.000000 picogo-0.0.6/picogo/IRSensor.py
--rw-rw-rw-   0        0        0    19928 2023-06-19 02:35:34.000000 picogo-0.0.6/picogo/LCD.py
--rw-rw-rw-   0        0        0      355 2023-06-19 02:27:03.000000 picogo-0.0.6/picogo/LCDBatteryTest.py
--rw-rw-rw-   0        0        0      673 2023-06-19 02:27:11.000000 picogo-0.0.6/picogo/LCDGraphicTest.py
--rw-rw-rw-   0        0        0     1879 2023-06-19 02:27:24.000000 picogo-0.0.6/picogo/LCDImageTest.py
--rw-rw-rw-   0        0        0      431 2023-06-19 02:27:32.000000 picogo-0.0.6/picogo/LCDPrintTest.py
--rw-rw-rw-   0        0        0      284 2023-06-19 02:27:45.000000 picogo-0.0.6/picogo/LCDTextTest.py
--rw-rw-rw-   0        0        0      421 2023-06-19 02:28:04.000000 picogo-0.0.6/picogo/LCDUltraSonicTest.py
--rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.6/picogo/LEDBlink.py
--rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.6/picogo/LEDBlinkTimer.py
--rw-rw-rw-   0        0        0     1721 2023-06-19 02:28:25.000000 picogo-0.0.6/picogo/LineTracking.py
--rw-rw-rw-   0        0        0     2608 2023-06-19 02:28:41.000000 picogo-0.0.6/picogo/LineTracking2.py
--rw-rw-rw-   0        0        0     2051 2023-06-19 02:28:56.000000 picogo-0.0.6/picogo/LineTrackingPID.py
--rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.6/picogo/LogoText.py
--rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.6/picogo/LogoText_01.py
--rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.6/picogo/Motor.py
--rw-rw-rw-   0        0        0      105 2023-06-19 02:29:14.000000 picogo-0.0.6/picogo/MotorStop.py
--rw-rw-rw-   0        0        0      373 2023-06-19 02:29:25.000000 picogo-0.0.6/picogo/MotorTest.py
--rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.6/picogo/Motor_org.py
--rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.6/picogo/RGBLed.py
--rw-rw-rw-   0        0        0     2441 2023-06-19 02:29:51.000000 picogo-0.0.6/picogo/RemoteController.py
--rw-rw-rw-   0        0        0     1828 2023-06-19 02:03:44.000000 picogo-0.0.6/picogo/Robot.py
--rw-rw-rw-   0        0        0     6663 2023-06-19 02:24:19.000000 picogo-0.0.6/picogo/TRSensor.py
--rw-rw-rw-   0        0        0     1213 2023-06-19 02:30:35.000000 picogo-0.0.6/picogo/TRSensorTest.py
--rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.6/picogo/TextNumber.py
--rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.6/picogo/UltraSonic.py
--rw-rw-rw-   0        0        0     2748 2023-06-19 02:32:31.000000 picogo-0.0.6/picogo/UltraSonicInfraredFollow.py
--rw-rw-rw-   0        0        0     1551 2023-06-19 02:33:34.000000 picogo-0.0.6/picogo/UltraSonicInfraredObstacleAvoidance.py
--rw-rw-rw-   0        0        0      823 2023-06-19 02:33:53.000000 picogo-0.0.6/picogo/UltraSonicObstacleAvoidance.py
--rw-rw-rw-   0        0        0      276 2023-06-19 02:34:05.000000 picogo-0.0.6/picogo/UltraSonicTest.py
--rw-rw-rw-   0        0        0      184 2023-06-19 02:08:06.000000 picogo-0.0.6/picogo/__init__.py
--rw-rw-rw-   0        0        0      191 2023-06-19 02:23:22.000000 picogo-0.0.6/picogo/main.py
--rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.6/picogo/picozero.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:17:18.135293 picogo-0.0.6/picogo.egg-info/
--rw-rw-rw-   0        0        0      799 2023-06-19 03:17:18.000000 picogo-0.0.6/picogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-06-19 03:17:18.000000 picogo-0.0.6/picogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:17:18.000000 picogo-0.0.6/picogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 03:17:18.000000 picogo-0.0.6/picogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 03:17:18.141291 picogo-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-06-19 03:16:57.000000 picogo-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:22:04.963479 picogo-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0      799 2023-06-19 03:22:04.962481 picogo-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 03:22:04.954520 picogo-0.0.7/picogo/
+-rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.7/picogo/ATemplate.py
+-rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.7/picogo/Battery.py
+-rw-rw-rw-   0        0        0     1327 2023-06-19 02:24:52.000000 picogo-0.0.7/picogo/BatteryTest.py
+-rw-rw-rw-   0        0        0     9466 2023-06-19 02:03:56.000000 picogo-0.0.7/picogo/BlueTooth.py
+-rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.7/picogo/BootselButton.py
+-rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.7/picogo/BuzzerTest.py
+-rw-rw-rw-   0        0        0       75 2023-06-19 02:25:11.000000 picogo-0.0.7/picogo/FirmwareVersion.py
+-rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.7/picogo/HelloWorld.py
+-rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.7/picogo/I2CScan.py
+-rw-rw-rw-   0        0        0     1144 2023-06-19 02:25:42.000000 picogo-0.0.7/picogo/IRObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      301 2023-06-19 02:25:56.000000 picogo-0.0.7/picogo/IRSensor.py
+-rw-rw-rw-   0        0        0    19928 2023-06-19 02:35:34.000000 picogo-0.0.7/picogo/LCD.py
+-rw-rw-rw-   0        0        0      355 2023-06-19 02:27:03.000000 picogo-0.0.7/picogo/LCDBatteryTest.py
+-rw-rw-rw-   0        0        0      673 2023-06-19 02:27:11.000000 picogo-0.0.7/picogo/LCDGraphicTest.py
+-rw-rw-rw-   0        0        0     1879 2023-06-19 02:27:24.000000 picogo-0.0.7/picogo/LCDImageTest.py
+-rw-rw-rw-   0        0        0      431 2023-06-19 02:27:32.000000 picogo-0.0.7/picogo/LCDPrintTest.py
+-rw-rw-rw-   0        0        0      284 2023-06-19 02:27:45.000000 picogo-0.0.7/picogo/LCDTextTest.py
+-rw-rw-rw-   0        0        0      421 2023-06-19 02:28:04.000000 picogo-0.0.7/picogo/LCDUltraSonicTest.py
+-rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.7/picogo/LEDBlink.py
+-rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.7/picogo/LEDBlinkTimer.py
+-rw-rw-rw-   0        0        0     1721 2023-06-19 02:28:25.000000 picogo-0.0.7/picogo/LineTracking.py
+-rw-rw-rw-   0        0        0     2608 2023-06-19 02:28:41.000000 picogo-0.0.7/picogo/LineTracking2.py
+-rw-rw-rw-   0        0        0     2051 2023-06-19 02:28:56.000000 picogo-0.0.7/picogo/LineTrackingPID.py
+-rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.7/picogo/LogoText.py
+-rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.7/picogo/LogoText_01.py
+-rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.7/picogo/Motor.py
+-rw-rw-rw-   0        0        0      105 2023-06-19 02:29:14.000000 picogo-0.0.7/picogo/MotorStop.py
+-rw-rw-rw-   0        0        0      373 2023-06-19 02:29:25.000000 picogo-0.0.7/picogo/MotorTest.py
+-rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.7/picogo/Motor_org.py
+-rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.7/picogo/RGBLed.py
+-rw-rw-rw-   0        0        0     2441 2023-06-19 02:29:51.000000 picogo-0.0.7/picogo/RemoteController.py
+-rw-rw-rw-   0        0        0     1828 2023-06-19 02:03:44.000000 picogo-0.0.7/picogo/Robot.py
+-rw-rw-rw-   0        0        0     6663 2023-06-19 02:24:19.000000 picogo-0.0.7/picogo/TRSensor.py
+-rw-rw-rw-   0        0        0     1213 2023-06-19 02:30:35.000000 picogo-0.0.7/picogo/TRSensorTest.py
+-rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.7/picogo/TextNumber.py
+-rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.7/picogo/UltraSonic.py
+-rw-rw-rw-   0        0        0     2748 2023-06-19 02:32:31.000000 picogo-0.0.7/picogo/UltraSonicInfraredFollow.py
+-rw-rw-rw-   0        0        0     1551 2023-06-19 02:33:34.000000 picogo-0.0.7/picogo/UltraSonicInfraredObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      823 2023-06-19 02:33:53.000000 picogo-0.0.7/picogo/UltraSonicObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      276 2023-06-19 02:34:05.000000 picogo-0.0.7/picogo/UltraSonicTest.py
+-rw-rw-rw-   0        0        0      184 2023-06-19 02:08:06.000000 picogo-0.0.7/picogo/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-06-19 02:23:22.000000 picogo-0.0.7/picogo/main.py
+-rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.7/picogo/picozero.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:22:04.961480 picogo-0.0.7/picogo.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-06-19 03:22:04.000000 picogo-0.0.7/picogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1112 2023-06-19 03:22:04.000000 picogo-0.0.7/picogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:22:04.000000 picogo-0.0.7/picogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 03:22:04.000000 picogo-0.0.7/picogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:22:04.963479 picogo-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-06-19 03:17:46.000000 picogo-0.0.7/setup.py
```

### Comparing `picogo-0.0.6/LICENSE.md` & `picogo-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/PKG-INFO` & `picogo-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.6
+Version: 0.0.7
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.6/picogo/Battery.py` & `picogo-0.0.7/picogo/Battery.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/BatteryTest.py` & `picogo-0.0.7/picogo/BatteryTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/BlueTooth.py` & `picogo-0.0.7/picogo/BlueTooth.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/IRObstacleAvoidance.py` & `picogo-0.0.7/picogo/IRObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LCD.py` & `picogo-0.0.7/picogo/LCD.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LCDGraphicTest.py` & `picogo-0.0.7/picogo/LCDGraphicTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LCDImageTest.py` & `picogo-0.0.7/picogo/LCDImageTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LineTracking.py` & `picogo-0.0.7/picogo/LineTracking.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LineTracking2.py` & `picogo-0.0.7/picogo/LineTracking2.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/LineTrackingPID.py` & `picogo-0.0.7/picogo/LineTrackingPID.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/Motor.py` & `picogo-0.0.7/picogo/Motor.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/Motor_org.py` & `picogo-0.0.7/picogo/Motor_org.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/RGBLed.py` & `picogo-0.0.7/picogo/RGBLed.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/RemoteController.py` & `picogo-0.0.7/picogo/RemoteController.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/Robot.py` & `picogo-0.0.7/picogo/Robot.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/TRSensor.py` & `picogo-0.0.7/picogo/TRSensor.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/TRSensorTest.py` & `picogo-0.0.7/picogo/TRSensorTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/TextNumber.py` & `picogo-0.0.7/picogo/TextNumber.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/UltraSonic.py` & `picogo-0.0.7/picogo/UltraSonic.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/UltraSonicInfraredFollow.py` & `picogo-0.0.7/picogo/UltraSonicInfraredFollow.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/UltraSonicInfraredObstacleAvoidance.py` & `picogo-0.0.7/picogo/UltraSonicInfraredObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/UltraSonicObstacleAvoidance.py` & `picogo-0.0.7/picogo/UltraSonicObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo/picozero.py` & `picogo-0.0.7/picogo/picozero.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/picogo.egg-info/PKG-INFO` & `picogo-0.0.7/picogo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.6
+Version: 0.0.7
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.6/picogo.egg-info/SOURCES.txt` & `picogo-0.0.7/picogo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picogo-0.0.6/setup.py` & `picogo-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 __project__ = 'picogo'
 __packages__ = ['picogo']
 __desc__ = 'A beginner-friendly library for using picogo with the Raspberry Pi Pico. '
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 __author__ = "SkySLAM Co., Ltd."
 __author_email__ = 'terabuilder@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/sunabove/PicoGo'
 __keywords__ = [
     'picogo',
     'pico',
```

