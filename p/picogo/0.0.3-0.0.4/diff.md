# Comparing `tmp/picogo-0.0.3.tar.gz` & `tmp/picogo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picogo-0.0.3.tar", last modified: Mon Jun 19 01:57:06 2023, max compression
+gzip compressed data, was "picogo-0.0.4.tar", last modified: Mon Jun 19 02:04:18 2023, max compression
```

## Comparing `picogo-0.0.3.tar` & `picogo-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:57:06.043927 picogo-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      799 2023-06-19 01:57:06.042929 picogo-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 01:57:06.030929 picogo-0.0.3/picogo/
--rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.3/picogo/ATemplate.py
--rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.3/picogo/Battery.py
--rw-rw-rw-   0        0        0     1323 2023-04-30 08:44:21.000000 picogo-0.0.3/picogo/BatteryTest.py
--rw-rw-rw-   0        0        0     9465 2023-06-17 12:04:45.000000 picogo-0.0.3/picogo/BlueTooth.py
--rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.3/picogo/BootselButton.py
--rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.3/picogo/BuzzerTest.py
--rw-rw-rw-   0        0        0       73 2023-04-29 03:34:10.000000 picogo-0.0.3/picogo/FirmwareVersion.py
--rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.3/picogo/HelloWorld.py
--rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.3/picogo/I2CScan.py
--rw-rw-rw-   0        0        0     1139 2023-05-02 01:21:04.000000 picogo-0.0.3/picogo/IRObstacleAvoidance.py
--rw-rw-rw-   0        0        0      301 2023-05-02 01:13:40.000000 picogo-0.0.3/picogo/IRSensor.py
--rw-rw-rw-   0        0        0    19928 2023-06-14 13:45:08.000000 picogo-0.0.3/picogo/LCD.py
--rw-rw-rw-   0        0        0      350 2023-05-01 06:37:44.000000 picogo-0.0.3/picogo/LCDBatteryTest.py
--rw-rw-rw-   0        0        0      672 2023-04-28 09:20:44.000000 picogo-0.0.3/picogo/LCDGraphicTest.py
--rw-rw-rw-   0        0        0     1878 2023-06-10 00:49:58.000000 picogo-0.0.3/picogo/LCDImageTest.py
--rw-rw-rw-   0        0        0      430 2023-04-28 11:47:42.000000 picogo-0.0.3/picogo/LCDPrintTest.py
--rw-rw-rw-   0        0        0      283 2023-06-12 11:01:04.000000 picogo-0.0.3/picogo/LCDTextTest.py
--rw-rw-rw-   0        0        0      417 2023-05-01 06:38:27.000000 picogo-0.0.3/picogo/LCDUltraSonicTest.py
--rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.3/picogo/LEDBlink.py
--rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.3/picogo/LEDBlinkTimer.py
--rw-rw-rw-   0        0        0     1716 2023-04-26 13:16:58.000000 picogo-0.0.3/picogo/LineTracking.py
--rw-rw-rw-   0        0        0     2603 2023-04-24 07:36:11.000000 picogo-0.0.3/picogo/LineTracking2.py
--rw-rw-rw-   0        0        0     2047 2023-04-25 06:06:56.000000 picogo-0.0.3/picogo/LineTrackingPID.py
--rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.3/picogo/LogoText.py
--rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.3/picogo/LogoText_01.py
--rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.3/picogo/Motor.py
--rw-rw-rw-   0        0        0      104 2023-05-09 03:06:41.000000 picogo-0.0.3/picogo/MotorStop.py
--rw-rw-rw-   0        0        0      370 2023-06-14 13:29:40.000000 picogo-0.0.3/picogo/MotorTest.py
--rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.3/picogo/Motor_org.py
--rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.3/picogo/RGBLed.py
--rw-rw-rw-   0        0        0     2438 2023-06-09 23:56:17.000000 picogo-0.0.3/picogo/RemoteController.py
--rw-rw-rw-   0        0        0     1827 2023-06-17 12:27:54.000000 picogo-0.0.3/picogo/Robot.py
--rw-rw-rw-   0        0        0     6671 2023-05-06 11:53:13.000000 picogo-0.0.3/picogo/TRSensor.py
--rw-rw-rw-   0        0        0     1208 2023-05-02 04:02:25.000000 picogo-0.0.3/picogo/TRSensorTest.py
--rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.3/picogo/TextNumber.py
--rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.3/picogo/UltraSonic.py
--rw-rw-rw-   0        0        0     2762 2023-04-27 02:21:32.000000 picogo-0.0.3/picogo/UltraSonicInfraredFollow.py
--rw-rw-rw-   0        0        0     1549 2023-04-30 09:34:14.000000 picogo-0.0.3/picogo/UltraSonicInfraredObstacleAvoidance.py
--rw-rw-rw-   0        0        0      819 2023-04-30 09:31:55.000000 picogo-0.0.3/picogo/UltraSonicObstacleAvoidance.py
--rw-rw-rw-   0        0        0      273 2023-04-30 09:31:06.000000 picogo-0.0.3/picogo/UltraSonicTest.py
--rw-rw-rw-   0        0        0      184 2023-06-19 01:52:00.000000 picogo-0.0.3/picogo/__init__.py
--rw-rw-rw-   0        0        0      190 2023-06-15 03:10:09.000000 picogo-0.0.3/picogo/main.py
--rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.3/picogo/picozero.py
-drwxrwxrwx   0        0        0        0 2023-06-19 01:57:06.039927 picogo-0.0.3/picogo.egg-info/
--rw-rw-rw-   0        0        0      799 2023-06-19 01:57:05.000000 picogo-0.0.3/picogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-06-19 01:57:05.000000 picogo-0.0.3/picogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:57:05.000000 picogo-0.0.3/picogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 01:57:05.000000 picogo-0.0.3/picogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 01:57:06.043927 picogo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-06-19 01:32:53.000000 picogo-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.679485 picogo-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      799 2023-06-19 02:04:18.678482 picogo-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.661484 picogo-0.0.4/picogo/
+-rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.4/picogo/ATemplate.py
+-rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.4/picogo/Battery.py
+-rw-rw-rw-   0        0        0     1323 2023-04-30 08:44:21.000000 picogo-0.0.4/picogo/BatteryTest.py
+-rw-rw-rw-   0        0        0     9466 2023-06-19 02:03:56.000000 picogo-0.0.4/picogo/BlueTooth.py
+-rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.4/picogo/BootselButton.py
+-rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.4/picogo/BuzzerTest.py
+-rw-rw-rw-   0        0        0       73 2023-04-29 03:34:10.000000 picogo-0.0.4/picogo/FirmwareVersion.py
+-rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.4/picogo/HelloWorld.py
+-rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.4/picogo/I2CScan.py
+-rw-rw-rw-   0        0        0     1139 2023-05-02 01:21:04.000000 picogo-0.0.4/picogo/IRObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      301 2023-05-02 01:13:40.000000 picogo-0.0.4/picogo/IRSensor.py
+-rw-rw-rw-   0        0        0    19928 2023-06-14 13:45:08.000000 picogo-0.0.4/picogo/LCD.py
+-rw-rw-rw-   0        0        0      350 2023-05-01 06:37:44.000000 picogo-0.0.4/picogo/LCDBatteryTest.py
+-rw-rw-rw-   0        0        0      672 2023-04-28 09:20:44.000000 picogo-0.0.4/picogo/LCDGraphicTest.py
+-rw-rw-rw-   0        0        0     1878 2023-06-10 00:49:58.000000 picogo-0.0.4/picogo/LCDImageTest.py
+-rw-rw-rw-   0        0        0      430 2023-04-28 11:47:42.000000 picogo-0.0.4/picogo/LCDPrintTest.py
+-rw-rw-rw-   0        0        0      283 2023-06-12 11:01:04.000000 picogo-0.0.4/picogo/LCDTextTest.py
+-rw-rw-rw-   0        0        0      417 2023-05-01 06:38:27.000000 picogo-0.0.4/picogo/LCDUltraSonicTest.py
+-rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.4/picogo/LEDBlink.py
+-rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.4/picogo/LEDBlinkTimer.py
+-rw-rw-rw-   0        0        0     1716 2023-04-26 13:16:58.000000 picogo-0.0.4/picogo/LineTracking.py
+-rw-rw-rw-   0        0        0     2603 2023-04-24 07:36:11.000000 picogo-0.0.4/picogo/LineTracking2.py
+-rw-rw-rw-   0        0        0     2047 2023-04-25 06:06:56.000000 picogo-0.0.4/picogo/LineTrackingPID.py
+-rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.4/picogo/LogoText.py
+-rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.4/picogo/LogoText_01.py
+-rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.4/picogo/Motor.py
+-rw-rw-rw-   0        0        0      104 2023-05-09 03:06:41.000000 picogo-0.0.4/picogo/MotorStop.py
+-rw-rw-rw-   0        0        0      370 2023-06-14 13:29:40.000000 picogo-0.0.4/picogo/MotorTest.py
+-rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.4/picogo/Motor_org.py
+-rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.4/picogo/RGBLed.py
+-rw-rw-rw-   0        0        0     2438 2023-06-09 23:56:17.000000 picogo-0.0.4/picogo/RemoteController.py
+-rw-rw-rw-   0        0        0     1828 2023-06-19 02:03:44.000000 picogo-0.0.4/picogo/Robot.py
+-rw-rw-rw-   0        0        0     6671 2023-05-06 11:53:13.000000 picogo-0.0.4/picogo/TRSensor.py
+-rw-rw-rw-   0        0        0     1208 2023-05-02 04:02:25.000000 picogo-0.0.4/picogo/TRSensorTest.py
+-rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.4/picogo/TextNumber.py
+-rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.4/picogo/UltraSonic.py
+-rw-rw-rw-   0        0        0     2762 2023-04-27 02:21:32.000000 picogo-0.0.4/picogo/UltraSonicInfraredFollow.py
+-rw-rw-rw-   0        0        0     1549 2023-04-30 09:34:14.000000 picogo-0.0.4/picogo/UltraSonicInfraredObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      819 2023-04-30 09:31:55.000000 picogo-0.0.4/picogo/UltraSonicObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      273 2023-04-30 09:31:06.000000 picogo-0.0.4/picogo/UltraSonicTest.py
+-rw-rw-rw-   0        0        0      184 2023-06-19 01:52:00.000000 picogo-0.0.4/picogo/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-06-15 03:10:09.000000 picogo-0.0.4/picogo/main.py
+-rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.4/picogo/picozero.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.676486 picogo-0.0.4/picogo.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1112 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:04:18.680487 picogo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-06-19 02:04:09.000000 picogo-0.0.4/setup.py
```

### Comparing `picogo-0.0.3/LICENSE.md` & `picogo-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/PKG-INFO` & `picogo-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.3/picogo/Battery.py` & `picogo-0.0.4/picogo/Battery.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/BatteryTest.py` & `picogo-0.0.4/picogo/BatteryTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/BlueTooth.py` & `picogo-0.0.4/picogo/BlueTooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import machine
 import ujson, utime
 
-from Robot import Robot
+from .Robot import Robot
 
 class BlueTooth :
     def __init__( self ):
         print( "Hello ... Bluetooth!" )
         
         self.robot = Robot()
         self.uart = self.robot.uart
```

### Comparing `picogo-0.0.3/picogo/IRObstacleAvoidance.py` & `picogo-0.0.4/picogo/IRObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LCD.py` & `picogo-0.0.4/picogo/LCD.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LCDGraphicTest.py` & `picogo-0.0.4/picogo/LCDGraphicTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LCDImageTest.py` & `picogo-0.0.4/picogo/LCDImageTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LineTracking.py` & `picogo-0.0.4/picogo/LineTracking.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LineTracking2.py` & `picogo-0.0.4/picogo/LineTracking2.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/LineTrackingPID.py` & `picogo-0.0.4/picogo/LineTrackingPID.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/Motor.py` & `picogo-0.0.4/picogo/Motor.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/Motor_org.py` & `picogo-0.0.4/picogo/Motor_org.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/RGBLed.py` & `picogo-0.0.4/picogo/RGBLed.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/RemoteController.py` & `picogo-0.0.4/picogo/RemoteController.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/Robot.py` & `picogo-0.0.4/picogo/Robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import machine
+from machine import Pin, Timer
 import ujson, utime
-
 from time import sleep
 
-from Motor import Motor
-from machine import Pin, Timer
-from RGBLed import RGBLed
-from LCD import LCD
+from .Motor import Motor
+from .RGBLed import RGBLed
+from .LCD import LCD
 
 class Robot :
     
     VERSION = 1000
     
     low_speed  = 30
     med_speed  = 50
```

### Comparing `picogo-0.0.3/picogo/TRSensor.py` & `picogo-0.0.4/picogo/TRSensor.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/TRSensorTest.py` & `picogo-0.0.4/picogo/TRSensorTest.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/TextNumber.py` & `picogo-0.0.4/picogo/TextNumber.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/UltraSonic.py` & `picogo-0.0.4/picogo/UltraSonic.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/UltraSonicInfraredFollow.py` & `picogo-0.0.4/picogo/UltraSonicInfraredFollow.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/UltraSonicInfraredObstacleAvoidance.py` & `picogo-0.0.4/picogo/UltraSonicInfraredObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/UltraSonicObstacleAvoidance.py` & `picogo-0.0.4/picogo/UltraSonicObstacleAvoidance.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo/picozero.py` & `picogo-0.0.4/picogo/picozero.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/picogo.egg-info/PKG-INFO` & `picogo-0.0.4/picogo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.3/picogo.egg-info/SOURCES.txt` & `picogo-0.0.4/picogo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picogo-0.0.3/setup.py` & `picogo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 __project__ = 'picogo'
 __packages__ = ['picogo']
 __desc__ = 'A beginner-friendly library for using picogo with the Raspberry Pi Pico. '
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __author__ = "SkySLAM Co., Ltd."
 __author_email__ = 'terabuilder@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/sunabove/PicoGo'
 __keywords__ = [
     'picogo',
     'pico',
```

