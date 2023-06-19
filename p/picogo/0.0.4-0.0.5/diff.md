# Comparing `tmp/picogo-0.0.4.tar.gz` & `tmp/picogo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picogo-0.0.4.tar", last modified: Mon Jun 19 02:04:18 2023, max compression
+gzip compressed data, was "picogo-0.0.5.tar", last modified: Mon Jun 19 02:39:21 2023, max compression
```

## Comparing `picogo-0.0.4.tar` & `picogo-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.679485 picogo-0.0.4/
--rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.4/LICENSE.md
--rw-rw-rw-   0        0        0      799 2023-06-19 02:04:18.678482 picogo-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.661484 picogo-0.0.4/picogo/
--rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.4/picogo/ATemplate.py
--rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.4/picogo/Battery.py
--rw-rw-rw-   0        0        0     1323 2023-04-30 08:44:21.000000 picogo-0.0.4/picogo/BatteryTest.py
--rw-rw-rw-   0        0        0     9466 2023-06-19 02:03:56.000000 picogo-0.0.4/picogo/BlueTooth.py
--rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.4/picogo/BootselButton.py
--rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.4/picogo/BuzzerTest.py
--rw-rw-rw-   0        0        0       73 2023-04-29 03:34:10.000000 picogo-0.0.4/picogo/FirmwareVersion.py
--rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.4/picogo/HelloWorld.py
--rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.4/picogo/I2CScan.py
--rw-rw-rw-   0        0        0     1139 2023-05-02 01:21:04.000000 picogo-0.0.4/picogo/IRObstacleAvoidance.py
--rw-rw-rw-   0        0        0      301 2023-05-02 01:13:40.000000 picogo-0.0.4/picogo/IRSensor.py
--rw-rw-rw-   0        0        0    19928 2023-06-14 13:45:08.000000 picogo-0.0.4/picogo/LCD.py
--rw-rw-rw-   0        0        0      350 2023-05-01 06:37:44.000000 picogo-0.0.4/picogo/LCDBatteryTest.py
--rw-rw-rw-   0        0        0      672 2023-04-28 09:20:44.000000 picogo-0.0.4/picogo/LCDGraphicTest.py
--rw-rw-rw-   0        0        0     1878 2023-06-10 00:49:58.000000 picogo-0.0.4/picogo/LCDImageTest.py
--rw-rw-rw-   0        0        0      430 2023-04-28 11:47:42.000000 picogo-0.0.4/picogo/LCDPrintTest.py
--rw-rw-rw-   0        0        0      283 2023-06-12 11:01:04.000000 picogo-0.0.4/picogo/LCDTextTest.py
--rw-rw-rw-   0        0        0      417 2023-05-01 06:38:27.000000 picogo-0.0.4/picogo/LCDUltraSonicTest.py
--rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.4/picogo/LEDBlink.py
--rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.4/picogo/LEDBlinkTimer.py
--rw-rw-rw-   0        0        0     1716 2023-04-26 13:16:58.000000 picogo-0.0.4/picogo/LineTracking.py
--rw-rw-rw-   0        0        0     2603 2023-04-24 07:36:11.000000 picogo-0.0.4/picogo/LineTracking2.py
--rw-rw-rw-   0        0        0     2047 2023-04-25 06:06:56.000000 picogo-0.0.4/picogo/LineTrackingPID.py
--rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.4/picogo/LogoText.py
--rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.4/picogo/LogoText_01.py
--rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.4/picogo/Motor.py
--rw-rw-rw-   0        0        0      104 2023-05-09 03:06:41.000000 picogo-0.0.4/picogo/MotorStop.py
--rw-rw-rw-   0        0        0      370 2023-06-14 13:29:40.000000 picogo-0.0.4/picogo/MotorTest.py
--rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.4/picogo/Motor_org.py
--rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.4/picogo/RGBLed.py
--rw-rw-rw-   0        0        0     2438 2023-06-09 23:56:17.000000 picogo-0.0.4/picogo/RemoteController.py
--rw-rw-rw-   0        0        0     1828 2023-06-19 02:03:44.000000 picogo-0.0.4/picogo/Robot.py
--rw-rw-rw-   0        0        0     6671 2023-05-06 11:53:13.000000 picogo-0.0.4/picogo/TRSensor.py
--rw-rw-rw-   0        0        0     1208 2023-05-02 04:02:25.000000 picogo-0.0.4/picogo/TRSensorTest.py
--rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.4/picogo/TextNumber.py
--rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.4/picogo/UltraSonic.py
--rw-rw-rw-   0        0        0     2762 2023-04-27 02:21:32.000000 picogo-0.0.4/picogo/UltraSonicInfraredFollow.py
--rw-rw-rw-   0        0        0     1549 2023-04-30 09:34:14.000000 picogo-0.0.4/picogo/UltraSonicInfraredObstacleAvoidance.py
--rw-rw-rw-   0        0        0      819 2023-04-30 09:31:55.000000 picogo-0.0.4/picogo/UltraSonicObstacleAvoidance.py
--rw-rw-rw-   0        0        0      273 2023-04-30 09:31:06.000000 picogo-0.0.4/picogo/UltraSonicTest.py
--rw-rw-rw-   0        0        0      184 2023-06-19 01:52:00.000000 picogo-0.0.4/picogo/__init__.py
--rw-rw-rw-   0        0        0      190 2023-06-15 03:10:09.000000 picogo-0.0.4/picogo/main.py
--rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.4/picogo/picozero.py
-drwxrwxrwx   0        0        0        0 2023-06-19 02:04:18.676486 picogo-0.0.4/picogo.egg-info/
--rw-rw-rw-   0        0        0      799 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 02:04:18.000000 picogo-0.0.4/picogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 02:04:18.680487 picogo-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-06-19 02:04:09.000000 picogo-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:39:21.669444 picogo-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-06-19 00:42:56.000000 picogo-0.0.5/LICENSE.md
+-rw-rw-rw-   0        0        0      799 2023-06-19 02:39:21.668438 picogo-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 02:39:21.646440 picogo-0.0.5/picogo/
+-rw-rw-rw-   0        0        0       61 2023-04-25 02:18:41.000000 picogo-0.0.5/picogo/ATemplate.py
+-rw-rw-rw-   0        0        0      608 2023-04-29 07:54:32.000000 picogo-0.0.5/picogo/Battery.py
+-rw-rw-rw-   0        0        0     1327 2023-06-19 02:24:52.000000 picogo-0.0.5/picogo/BatteryTest.py
+-rw-rw-rw-   0        0        0     9466 2023-06-19 02:03:56.000000 picogo-0.0.5/picogo/BlueTooth.py
+-rw-rw-rw-   0        0        0      338 2023-04-20 01:55:46.000000 picogo-0.0.5/picogo/BootselButton.py
+-rw-rw-rw-   0        0        0      190 2023-04-19 11:56:21.000000 picogo-0.0.5/picogo/BuzzerTest.py
+-rw-rw-rw-   0        0        0       75 2023-06-19 02:25:11.000000 picogo-0.0.5/picogo/FirmwareVersion.py
+-rw-rw-rw-   0        0        0       50 2023-05-02 07:09:50.000000 picogo-0.0.5/picogo/HelloWorld.py
+-rw-rw-rw-   0        0        0      327 2023-04-30 08:45:42.000000 picogo-0.0.5/picogo/I2CScan.py
+-rw-rw-rw-   0        0        0     1144 2023-06-19 02:25:42.000000 picogo-0.0.5/picogo/IRObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      301 2023-06-19 02:25:56.000000 picogo-0.0.5/picogo/IRSensor.py
+-rw-rw-rw-   0        0        0    19928 2023-06-19 02:35:34.000000 picogo-0.0.5/picogo/LCD.py
+-rw-rw-rw-   0        0        0      355 2023-06-19 02:27:03.000000 picogo-0.0.5/picogo/LCDBatteryTest.py
+-rw-rw-rw-   0        0        0      673 2023-06-19 02:27:11.000000 picogo-0.0.5/picogo/LCDGraphicTest.py
+-rw-rw-rw-   0        0        0     1879 2023-06-19 02:27:24.000000 picogo-0.0.5/picogo/LCDImageTest.py
+-rw-rw-rw-   0        0        0      431 2023-06-19 02:27:32.000000 picogo-0.0.5/picogo/LCDPrintTest.py
+-rw-rw-rw-   0        0        0      284 2023-06-19 02:27:45.000000 picogo-0.0.5/picogo/LCDTextTest.py
+-rw-rw-rw-   0        0        0      421 2023-06-19 02:28:04.000000 picogo-0.0.5/picogo/LCDUltraSonicTest.py
+-rw-rw-rw-   0        0        0      294 2023-05-01 03:38:35.000000 picogo-0.0.5/picogo/LEDBlink.py
+-rw-rw-rw-   0        0        0      235 2023-06-13 02:14:44.000000 picogo-0.0.5/picogo/LEDBlinkTimer.py
+-rw-rw-rw-   0        0        0     1721 2023-06-19 02:28:25.000000 picogo-0.0.5/picogo/LineTracking.py
+-rw-rw-rw-   0        0        0     2608 2023-06-19 02:28:41.000000 picogo-0.0.5/picogo/LineTracking2.py
+-rw-rw-rw-   0        0        0     2051 2023-06-19 02:28:56.000000 picogo-0.0.5/picogo/LineTrackingPID.py
+-rw-rw-rw-   0        0        0      182 2023-06-14 11:06:32.000000 picogo-0.0.5/picogo/LogoText.py
+-rw-rw-rw-   0        0        0      181 2023-06-13 01:11:25.000000 picogo-0.0.5/picogo/LogoText_01.py
+-rw-rw-rw-   0        0        0     2698 2023-06-10 00:30:57.000000 picogo-0.0.5/picogo/Motor.py
+-rw-rw-rw-   0        0        0      105 2023-06-19 02:29:14.000000 picogo-0.0.5/picogo/MotorStop.py
+-rw-rw-rw-   0        0        0      373 2023-06-19 02:29:25.000000 picogo-0.0.5/picogo/MotorTest.py
+-rw-rw-rw-   0        0        0     3410 2023-05-06 11:25:22.000000 picogo-0.0.5/picogo/Motor_org.py
+-rw-rw-rw-   0        0        0     3975 2023-06-15 03:21:58.000000 picogo-0.0.5/picogo/RGBLed.py
+-rw-rw-rw-   0        0        0     2441 2023-06-19 02:29:51.000000 picogo-0.0.5/picogo/RemoteController.py
+-rw-rw-rw-   0        0        0     1828 2023-06-19 02:03:44.000000 picogo-0.0.5/picogo/Robot.py
+-rw-rw-rw-   0        0        0     6663 2023-06-19 02:24:19.000000 picogo-0.0.5/picogo/TRSensor.py
+-rw-rw-rw-   0        0        0     1213 2023-06-19 02:30:35.000000 picogo-0.0.5/picogo/TRSensorTest.py
+-rw-rw-rw-   0        0        0     1151 2023-06-15 08:20:26.000000 picogo-0.0.5/picogo/TextNumber.py
+-rw-rw-rw-   0        0        0      747 2023-04-30 09:30:10.000000 picogo-0.0.5/picogo/UltraSonic.py
+-rw-rw-rw-   0        0        0     2748 2023-06-19 02:32:31.000000 picogo-0.0.5/picogo/UltraSonicInfraredFollow.py
+-rw-rw-rw-   0        0        0     1551 2023-06-19 02:33:34.000000 picogo-0.0.5/picogo/UltraSonicInfraredObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      823 2023-06-19 02:33:53.000000 picogo-0.0.5/picogo/UltraSonicObstacleAvoidance.py
+-rw-rw-rw-   0        0        0      276 2023-06-19 02:34:05.000000 picogo-0.0.5/picogo/UltraSonicTest.py
+-rw-rw-rw-   0        0        0      184 2023-06-19 02:08:06.000000 picogo-0.0.5/picogo/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-06-19 02:23:22.000000 picogo-0.0.5/picogo/main.py
+-rw-rw-rw-   0        0        0    67890 2023-05-03 04:35:20.000000 picogo-0.0.5/picogo/picozero.py
+drwxrwxrwx   0        0        0        0 2023-06-19 02:39:21.666438 picogo-0.0.5/picogo.egg-info/
+-rw-rw-rw-   0        0        0      799 2023-06-19 02:39:20.000000 picogo-0.0.5/picogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1112 2023-06-19 02:39:21.000000 picogo-0.0.5/picogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 02:39:20.000000 picogo-0.0.5/picogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 02:39:20.000000 picogo-0.0.5/picogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 02:39:21.670440 picogo-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-06-19 02:07:53.000000 picogo-0.0.5/setup.py
```

### Comparing `picogo-0.0.4/LICENSE.md` & `picogo-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/PKG-INFO` & `picogo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.4/picogo/Battery.py` & `picogo-0.0.5/picogo/Battery.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/BatteryTest.py` & `picogo-0.0.5/picogo/BatteryTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from Battery import Battery
-from LCD import LCD
 from time import sleep
 
+from .Battery import Battery
+from .LCD import LCD
+
 if __name__ == '__main__' :
     
     lcd = LCD()
     
     lcd.fill(0xF232)
     lcd.line(2,2,70,2,0xBB56)
     lcd.line(70,2,85,17,0xBB56)
```

### Comparing `picogo-0.0.4/picogo/BlueTooth.py` & `picogo-0.0.5/picogo/BlueTooth.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/IRObstacleAvoidance.py` & `picogo-0.0.5/picogo/IRObstacleAvoidance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from Motor import PicoGo
-from LCD import LCD
-from IRSensor import IRSensor
 from time import sleep
 
+from .Motor import PicoGo
+from .LCD import LCD
+from .IRSensor import IRSensor
+
 if __name__ == '__main__' :
     
     robot = PicoGo()
     lcd = LCD()
     irSensor = IRSensor()
     
     lcd.disp_init()
```

### Comparing `picogo-0.0.4/picogo/LCD.py` & `picogo-0.0.5/picogo/LCD.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from machine import Pin, SPI
 from time import sleep
-from Battery import Battery
-from UltraSonic import UltraSonic
-from IRSensor import IRSensor
-from TRSensor import TRSensor
-from Motor import Motor
 from random import randint
+import framebuf, builtins
 
-import framebuf
-import builtins
+from .Battery import Battery
+from .UltraSonic import UltraSonic
+from .IRSensor import IRSensor
+from .TRSensor import TRSensor
+from .Motor import Motor
     
 # ST7789
 class LCD(framebuf.FrameBuffer):
     
     # RGC 565 Color Definition
     WHITE  = white  = 0xFFFF
     BLACK  = black  = 0x0000
@@ -526,15 +525,15 @@
     def disp_logo(self, fg=None, bg=None, flush=True) : 
         print( "disp_logo" )
         
         self.disp_logo_text( fg=fg, bg=bg, flush=flush)
     pass
 
     def disp_logo_text(self, fg=None, bg=None, flush=True) :
-        from LogoText import logo_text
+        from .LogoText import logo_text
 
         self.disp_full_text( logo_text, fg=fg, bg=bg, flush=flush )
     
         del logo_text
     pass        
 
     def disp_logo_image(self, logo_image, flush=True) : 
@@ -576,15 +575,15 @@
     
         flush and self.flush() 
     pass
 
     def disp_full_number( self, number=0, fg=None, bg=None, flush=True) :
         debug = False
         
-        from TextNumber import numbers
+        from .TextNumber import numbers
         
         number = int(number)
         number = f"{number:d}"
         
         texts = numbers[0] 
         texts = texts.split( "\n" )
```

### Comparing `picogo-0.0.4/picogo/LCDGraphicTest.py` & `picogo-0.0.5/picogo/LCDGraphicTest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from LCD import LCD
+from .LCD import LCD
         
 if __name__=='__main__':
     lcd = LCD()
     
     width = lcd.width
     height = lcd.height
```

### Comparing `picogo-0.0.4/picogo/LCDImageTest.py` & `picogo-0.0.5/picogo/LCDImageTest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import sys
 
 from PIL import Image
-from LCD import LCD
+from .LCD import LCD
 
 print("""
 image.py - Display an image on the LCD.
 
 If you're using Breakout Garden, plug the 1.3" LCD (SPI)
 breakout into the front slot.
```

### Comparing `picogo-0.0.4/picogo/LineTracking.py` & `picogo-0.0.5/picogo/LineTracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from TRSensor import TRSensor
-from Motor import PicoGo
 from time import sleep
-from LCD import LCD
+
+from .TRSensor import TRSensor
+from .Motor import PicoGo
+from .LCD import LCD
 
 if __name__ == '__main__' :
     
     print("TRSensor Test Program ...")
     
     lcd = LCD() 
     lcd.disp_text( f"LineTracking", 50, 60 )
```

### Comparing `picogo-0.0.4/picogo/LineTracking2.py` & `picogo-0.0.5/picogo/LineTracking2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from machine import Pin
-from TRSensor import TRSensor
-from Motor import PicoGo
-from RGBLed import RGBLed
 import time
 
+from .TRSensor import TRSensor
+from .Motor import PicoGo
+from .RGBLed import RGBLed
+
 
 M = PicoGo()
 Buzzer = Pin(4, Pin.OUT)
 DSR = Pin(2, Pin.IN)
 DSL = Pin(3, Pin.IN)
 
 strip = RGBLed()
```

### Comparing `picogo-0.0.4/picogo/LineTrackingPID.py` & `picogo-0.0.5/picogo/LineTrackingPID.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from TRSensor import TRSensor
-from Motor import PicoGo
 from time import sleep
 
+from .TRSensor import TRSensor
+from .Motor import PicoGo
+
 if __name__ == '__main__' :
     print("TRSensor Test Program ...")
     sleep(3)
     robot = PicoGo()
 
     trs = TRSensor()
     for i in range(100):
```

### Comparing `picogo-0.0.4/picogo/Motor.py` & `picogo-0.0.5/picogo/Motor.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/Motor_org.py` & `picogo-0.0.5/picogo/Motor_org.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/RGBLed.py` & `picogo-0.0.5/picogo/RGBLed.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/RemoteController.py` & `picogo-0.0.5/picogo/RemoteController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from machine import Pin
-from Motor import Motor
 from time import sleep_us
 
+from .Motor import Motor
+
 def getkey( irRemoteCon ):
         
     if irRemoteCon.value() == 0 :
         count = 0
         
         while (irRemoteCon.value() == 0) and (count < 100) : #9ms
             count += 1
```

### Comparing `picogo-0.0.4/picogo/Robot.py` & `picogo-0.0.5/picogo/Robot.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/TRSensor.py` & `picogo-0.0.5/picogo/TRSensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from machine import Pin
+import machine, rp2
 from time import sleep, sleep_ms
-import machine 
-import rp2
 
 @rp2.asm_pio(out_shiftdir=0, autopull=True, pull_thresh=12, autopush=True, push_thresh=12, sideset_init=(rp2.PIO.OUT_LOW), out_init=rp2.PIO.OUT_LOW)
 def spi_cpha0():
     out(pins, 1).side(0x0)[1]
     in_(pins, 1).side(0x1)[1]
 pass
```

### Comparing `picogo-0.0.4/picogo/TRSensorTest.py` & `picogo-0.0.5/picogo/TRSensorTest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from Motor import PicoGo
-from TRSensor import TRSensor
 from time import sleep, sleep_ms
-from LCD import LCD
+
+from .Motor import PicoGo
+from .TRSensor import TRSensor
+from .LCD import LCD
 
 if __name__ == '__main__':
 
     print( "TRSensor Test ... \n" )
     
     lcd = LCD()
     lcd.disp_init(flush=1)
```

### Comparing `picogo-0.0.4/picogo/TextNumber.py` & `picogo-0.0.5/picogo/TextNumber.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/UltraSonic.py` & `picogo-0.0.5/picogo/UltraSonic.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo/UltraSonicInfraredFollow.py` & `picogo-0.0.5/picogo/UltraSonicInfraredFollow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from machine import UART, Pin
-from TRSensor import TRSensor
-from Motor import PicoGo
-from ws2812 import NeoPixel
-from ST7789 import ST7789
-import ujson
-import utime
+import ujson, utime
+
+from .TRSensor import TRSensor
+from .Motor import PicoGo
+from .RGBLed import RGBLed
+from .LCD import LCD
 
 
 bat = machine.ADC(Pin(26))
 temp = machine.ADC(4)
 
-lcd = ST7789()
+lcd = LCD()
 lcd.fill(0xF232)
 lcd.line(2,2,70,2,0xBB56)
 lcd.line(70,2,85,17,0xBB56)
 lcd.line(85,17,222,17,0xBB56)
 lcd.line(222,17,237,32,0xBB56)
 lcd.line(2,2,2,118,0xBB56)
 lcd.line(2,118,16,132,0xBB56)
@@ -38,15 +38,15 @@
 DSR = Pin(2, Pin.IN)
 DSL = Pin(3, Pin.IN)
 Echo = Pin(15, Pin.IN)
 Trig = Pin(14, Pin.OUT)
 Trig.value(0)
 Echo.value(0)
 
-strip = NeoPixel()
+strip = RGBLed()
 strip.pixels_set(0, strip.BLACK)
 strip.pixels_set(1, strip.BLACK)
 strip.pixels_set(2, strip.BLACK)
 strip.pixels_set(3, strip.BLACK)
 strip.pixels_show()
 
 LOW_SPEED    =  30
```

### Comparing `picogo-0.0.4/picogo/UltraSonicInfraredObstacleAvoidance.py` & `picogo-0.0.5/picogo/UltraSonicInfraredObstacleAvoidance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from machine import Pin
-from Motor import PicoGo
-from UltraSonic import UltraSonic
 from time import sleep
 
+from .Motor import Motor
+from .UltraSonic import UltraSonic
+
 if __name__ == '__main__' :
 
-    robot = PicoGo()
+    motor = Motor()
     ultraSonic = UltraSonic()
     
     dsr = Pin(2, Pin.IN)
     dsl = Pin(3, Pin.IN)
     
     duration = 0.02
     speed = 20
@@ -26,31 +27,31 @@
         right_block = ( dsl.value()== 0 )
         
         if dist < max_dist or left_block or right_block == 0 :
             obstacle_cnt += 1
         pass
     
         if obstacle_cnt == 1 :
-            robot.stop()
+            motor.stop()
             sleep( duration)
         pass
     
         if left_block and right_block : # 양쪽에 장애물이 있을 때, 좌회전
-            robot.left( speed )
+            motor.left( speed )
             sleep( 5*duration )
         elif left_block :   # 좌측 장애물시, 우회전
-            robot.right( speed )
+            motor.right( speed )
             sleep( 5*duration )
         elif right_block :  # 우측 장애물시, 좌회전
-            robot.left( speed )
+            motor.left( speed )
             sleep( 5*duration )
         if dist < max_dist : # 전방 장애물 있을 경우, 좌회전 
-            robot.left( speed )
+            motor.left( speed )
             sleep( 5*duration )        
         else :              # 장매물이 없으면, 전진
             obstacle_cnt = 0 
-            robot.forward( speed )
+            motor.forward( speed )
             sleep( duration )
         pass
     pass
 
 pass
```

### Comparing `picogo-0.0.4/picogo/UltraSonicObstacleAvoidance.py` & `picogo-0.0.5/picogo/UltraSonicObstacleAvoidance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from Motor import PicoGo
-from UltraSonic import UltraSonic
 from time import sleep
 
+from .Motor import PicoGo
+from .UltraSonic import UltraSonic
+
 if __name__ == '__main__' :
     print( "Hello" )
 
     robot = PicoGo()
     ultraSonic = UltraSonic()
     
     duration = 0.02
```

### Comparing `picogo-0.0.4/picogo/picozero.py` & `picogo-0.0.5/picogo/picozero.py`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/picogo.egg-info/PKG-INFO` & `picogo-0.0.5/picogo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picogo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A beginner-friendly library for using picogo with the Raspberry Pi Pico. 
 Home-page: https://github.com/sunabove/PicoGo
 Author: SkySLAM Co., Ltd.
 Author-email: terabuilder@gmail.com
 License: MIT
 Keywords: picogo,pico,raspberry,raspberry pi,picorun,skyslam
 Classifier: Intended Audience :: Developers
```

### Comparing `picogo-0.0.4/picogo.egg-info/SOURCES.txt` & `picogo-0.0.5/picogo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picogo-0.0.4/setup.py` & `picogo-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 __project__ = 'picogo'
 __packages__ = ['picogo']
 __desc__ = 'A beginner-friendly library for using picogo with the Raspberry Pi Pico. '
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __author__ = "SkySLAM Co., Ltd."
 __author_email__ = 'terabuilder@gmail.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/sunabove/PicoGo'
 __keywords__ = [
     'picogo',
     'pico',
```

