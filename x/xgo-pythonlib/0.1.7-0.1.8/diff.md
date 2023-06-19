# Comparing `tmp/xgo-pythonlib-0.1.7.tar.gz` & `tmp/xgo-pythonlib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.7.tar", last modified: Wed Jun 14 22:45:43 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.8.tar", last modified: Mon Jun 19 03:03:48 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.7.tar` & `xgo-pythonlib-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.528756 xgo-pythonlib-0.1.7/
--rw-rw-rw-   0        0        0     2111 2023-06-14 22:45:43.527756 xgo-pythonlib-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1484 2023-06-14 22:43:47.000000 xgo-pythonlib-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 22:45:43.528756 xgo-pythonlib-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-06-14 22:45:34.000000 xgo-pythonlib-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.519242 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2111 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-14 22:45:43.000000 xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.521242 xgo-pythonlib-0.1.7/xgoedu/
--rw-rw-rw-   0        0        0    37464 2023-06-14 02:34:21.000000 xgo-pythonlib-0.1.7/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.522242 xgo-pythonlib-0.1.7/xgolib/
--rw-rw-rw-   0        0        0    26394 2023-06-13 03:07:35.000000 xgo-pythonlib-0.1.7/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:45:43.526756 xgo-pythonlib-0.1.7/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.7/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.7/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.7/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/
+-rw-rw-rw-   0        0        0     2111 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1484 2023-06-14 22:43:47.000000 xgo-pythonlib-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-06-19 02:58:00.000000 xgo-pythonlib-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.491381 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2111 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.493380 xgo-pythonlib-0.1.8/xgoedu/
+-rw-rw-rw-   0        0        0    37464 2023-06-19 03:01:26.000000 xgo-pythonlib-0.1.8/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.495453 xgo-pythonlib-0.1.8/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.1.8/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.501506 xgo-pythonlib-0.1.8/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.8/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.8/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.8/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.7/PKG-INFO` & `xgo-pythonlib-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.1.7/README.md` & `xgo-pythonlib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.7/setup.py` & `xgo-pythonlib-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.7/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.7
+Version: 0.1.8
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.1.7/xgoedu/__init__.py` & `xgo-pythonlib-0.1.8/xgoedu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.3'
-__last_modified__ = '2023/6/12'
+__versinon__ = '1.2.4'
+__last_modified__ = '2023/6/19'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -204,23 +204,23 @@
     '''
     filename 文件名 字符串
     '''
     def xgoSpeaker(self,filename):
         path="/home/pi/xgoMusic/"
         os.system("mplayer"+" "+path+filename)
 
-    def xgovideoAudio(self,filename):
+    def xgoVideoAudio(self,filename):
         path="/home/pi/xgoVideos/"
         time.sleep(0.2)  #音画速度同步了 但是时间轴可能不同步 这里调试一下
         cmd="sudo mplayer "+path+filename+" -novideo"
         os.system(cmd)
 
-    def xgovideo(self,filename):
+    def xgoVideo(self,filename):
         path="/home/pi/xgoVideos/"
-        x=threading.Thread(target=self.xgovideoAudio,args=(filename,))
+        x=threading.Thread(target=self.xgoVideoAudio,args=(filename,))
         x.start()
         global counter
         video=cv2.VideoCapture(path+filename)
         fps = video.get(cv2.CAP_PROP_FPS) 
         print(fps)
         init_time=time.time()
         counter=0
@@ -275,15 +275,15 @@
             image = cv2.merge((r,g,b))
             image = cv2.flip(image,1)
             imgok = Image.fromarray(image)
             self.display.ShowImage(imgok)
             if not self.camera_still:
                 break
 
-    def xgovideoRecord(self,filename="record",seconds=5):
+    def xgoVideoRecord(self,filename="record",seconds=5):
         path="/home/pi/xgoVideos/"
         self.camera_still=False
         time.sleep(0.6)
         self.open_camera()
         FPS=15
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
```

### Comparing `xgo-pythonlib-0.1.7/xgolib/__init__.py` & `xgo-pythonlib-0.1.8/xgolib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import serial
 import struct
 import time
 import math
-__version__ = '1.3.1'
-__last_modified__ = '2023/6/13'
+__version__ = '1.3.3'
+__last_modified__ = '2023/6/19'
 
 """
 XGOorder 用来存放命令地址和对应数据
 XGOorder is used to store the command address and corresponding data
 """
 
 XGOorder = {
@@ -135,20 +135,22 @@
         self.ser.flushInput()
         self.port = port
         self.rx_FLAG = 0
         self.rx_COUNT = 0
         self.rx_ADDR = 0
         self.rx_LEN = 0
         self.rx_data = bytearray(50)
+        time.sleep(1)
         self.version = self.read_firmware()
         if self.version[0] == 'M':
             changePara('xgomini')
         elif self.version[0] == 'L':
             changePara('xgolite')
         else:
+            changePara('xgomini')
             print("ERROR!Can't read firmware version!")
         self.mintime = 0.65
         self.reset()
         time.sleep(0.5)
         self.init_yaw = self.read_yaw()
         pass
 
@@ -361,17 +363,14 @@
 
     def motor(self, motor_id, data):
         """
         控制机器狗单个舵机转动
         Control the rotation of a single steering gear of the robot
         """
         MOTOR_ID = [11, 12, 13, 21, 22, 23, 31, 32, 33, 41, 42, 43, 51, 52, 53]
-        if motor_id == 51:
-            self.claw(data)
-            return
 
         if isinstance(motor_id, list):
             if len(motor_id) != len(data):
                 print("Error!Length Mismatching!")
                 return
             index = []
             for i in range(len(motor_id)):
@@ -412,15 +411,15 @@
         index = search(direction, ['r', 'p', 'y'])
         if index == -1:
             print("ERROR!Direction must be 'r', 'p' or 'y'")
             return
         if period == 0:
             XGOorder["PERIODIC_ROT"][index] = 0
         else:
-            XGOorder["PERIODIC_ROT"][index] = conver2u8(period, XGOparam["PERIOD_LIMIT"][0], mode=1)
+            XGOorder["PERIODIC_ROT"][index] = conver2u8(period, XGOparam["PERIOD_LIMIT"][0], min_value=1)
         self.__send("PERIODIC_ROT", index)
 
     def periodic_rot(self, direction, period):
         """
         使机器狗周期性转动
         Make the robot rotate periodically
         """
@@ -437,15 +436,15 @@
         index = search(direction, ['x', 'y', 'z'])
         if index == -1:
             print("ERROR!Direction must be 'x', 'y' or 'z'")
             return
         if period == 0:
             XGOorder["PERIODIC_TRAN"][index] = 0
         else:
-            XGOorder["PERIODIC_TRAN"][index] = conver2u8(period, XGOparam["PERIOD_LIMIT"][0], mode=1)
+            XGOorder["PERIODIC_TRAN"][index] = conver2u8(period, XGOparam["PERIOD_LIMIT"][0], min_value=1)
         self.__send("PERIODIC_TRAN", index)
 
     def periodic_tran(self, direction, period):
         """
         使机器狗周期性平动
         Make the robot translate periodically
         """
@@ -462,15 +461,15 @@
         """
         使机器狗原地踏步
         Make the robot marks time
         """
         if data == 0:
             XGOorder["MarkTime"][1] = 0
         else:
-            XGOorder["MarkTime"][1] = conver2u8(data, XGOparam["MARK_TIME_LIMIT"], mode=1)
+            XGOorder["MarkTime"][1] = conver2u8(data, XGOparam["MARK_TIME_LIMIT"], min_value=1)
         self.__send("MarkTime")
 
     def pace(self, mode):
         """
         改变机器狗的踏步频率
         Change the step frequency of the robot
         """
@@ -571,15 +570,15 @@
 
     def read_firmware(self):
         self.__read(XGOorder["FIRMWARE_VERSION"][0], 10)
         self.ser.read_all()
         firmware_version = 'Null'
         if self.__unpack():
             data = self.rx_data[0:10]
-            firmware_version = data.decode("utf-8").strip('\0')
+            firmware_version = data.decode("ascii").strip('\0')
         return firmware_version
 
     def read_roll(self):
         self.__read(XGOorder["ROLL"][0], 4)
         self.ser.read_all()
         roll = 0
         if self.__unpack():
```

### Comparing `xgo-pythonlib-0.1.7/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.8/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.7/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.8/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

