# Comparing `tmp/KitronikPicoSmartAirQuality-1.0.0.tar.gz` & `tmp/KitronikPicoSmartAirQuality-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KitronikPicoSmartAirQuality-1.0.0.tar", last modified: Fri Jan  6 15:38:27 2023, max compression
+gzip compressed data, was "KitronikPicoSmartAirQuality-1.0.1.tar", last modified: Mon Jun 19 07:37:42 2023, max compression
```

## Comparing `KitronikPicoSmartAirQuality-1.0.0.tar` & `KitronikPicoSmartAirQuality-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-01-06 15:38:27.246814 KitronikPicoSmartAirQuality-1.0.0/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-01-06 15:38:27.246814 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-01-06 15:38:27.000000 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)      280 2023-01-06 15:38:27.000000 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-01-06 15:38:27.000000 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       15 2023-01-06 15:38:27.000000 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)      382 2023-01-06 15:37:32.000000 KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQualityWheelSetup.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-01-06 15:36:07.000000 KitronikPicoSmartAirQuality-1.0.0/LICENSE
--rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-01-06 15:38:27.246814 KitronikPicoSmartAirQuality-1.0.0/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)    54521 2023-01-06 15:36:07.000000 KitronikPicoSmartAirQuality-1.0.0/PicoAirQuality.py
--rw-r--r--   0 jack      (1000) jack      (1000)    12800 2023-01-06 15:36:07.000000 KitronikPicoSmartAirQuality-1.0.0/README.md
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-01-06 15:38:27.246814 KitronikPicoSmartAirQuality-1.0.0/setup.cfg
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)      280 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/SOURCES.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)        1 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/dependency_links.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)       15 2023-06-19 07:37:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/top_level.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)      382 2023-06-19 07:35:42.000000 KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQualityWheelSetup.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1070 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/LICENSE
+-rw-r--r--   0 jack      (1000) jack      (1000)    12991 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)    55785 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/PicoAirQuality.py
+-rw-r--r--   0 jack      (1000) jack      (1000)    12800 2023-06-19 07:34:18.000000 KitronikPicoSmartAirQuality-1.0.1/README.md
+-rw-r--r--   0 jack      (1000) jack      (1000)       38 2023-06-19 07:37:42.494702 KitronikPicoSmartAirQuality-1.0.1/setup.cfg
```

### Comparing `KitronikPicoSmartAirQuality-1.0.0/KitronikPicoSmartAirQuality.egg-info/PKG-INFO` & `KitronikPicoSmartAirQuality-1.0.1/KitronikPicoSmartAirQuality.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KitronikPicoSmartAirQuality
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kitronik Air Quality Datalogging Board for Pico
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Other Languages: [FRANCAIS](README_FR.md)
 
 # Kitronik-Pico-Smart-Air-Quality-Board-MicroPython
```

### Comparing `KitronikPicoSmartAirQuality-1.0.0/LICENSE` & `KitronikPicoSmartAirQuality-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `KitronikPicoSmartAirQuality-1.0.0/PKG-INFO` & `KitronikPicoSmartAirQuality-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KitronikPicoSmartAirQuality
-Version: 1.0.0
+Version: 1.0.1
 Summary: Kitronik Air Quality Datalogging Board for Pico
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Other Languages: [FRANCAIS](README_FR.md)
 
 # Kitronik-Pico-Smart-Air-Quality-Board-MicroPython
```

### Comparing `KitronikPicoSmartAirQuality-1.0.0/PicoAirQuality.py` & `KitronikPicoSmartAirQuality-1.0.1/PicoAirQuality.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 # Servo
 servo = Pin(2, Pin.OUT)
 servo.value(0)
 # Buzzer
 buzzer = PWM(Pin(4))
 buzzer.duty_u16(0)
 
+# List of which StateMachines we have used
+usedSM = [False, False, False, False, False, False, False, False]
+
 # The KitronikButton class enable the use of the 2 user input buttons on the board
 class KitronikButton:
     def __init__(self):
         self.buttonA = Pin(12, Pin.IN, Pin.PULL_DOWN)
         self.buttonB = Pin(13, Pin.IN, Pin.PULL_DOWN)
 
 # The KitronikOutputControl class enables control of the servo and high-power outputs on the board
@@ -54,19 +57,33 @@
         # 1us is freq of 1000000
         # Servo pulses range from 500 to 2500us and overall pulse train is 20000us repeat.
         # Servo is on GP2
         self.maxServoPulse = 2500
         self.minServoPulse = 500
         self.pulseTrain = 20000
         self.degreesToUS = 2000/180
+
         # Create and start the servo statemachine
-        self.servo.append (StateMachine(1, self._servo_pwm, freq=2000000, sideset_base=Pin(2)))
+        for i in range(8): # StateMachine range from 0 to 7
+            if usedSM[i]:
+                continue # Ignore this index if already used
+            try:
+                self.servo.append(StateMachine(i, self._servo_pwm, freq=2000000, sideset_base=Pin(2)))
+                usedSM[i] = True # Set this index to used
+                break # Have claimed the SM, can leave now
+            except ValueError:
+                pass # External resouce has SM, move on
+            if i == 7:
+                # Cannot find an unused SM
+                raise ValueError("Could not claim a StateMachine, all in use")
+        
         self.servo[0].put(self.pulseTrain)
         self.servo[0].exec("pull()")
         self.servo[0].exec("mov(isr, osr)")
+        self.servo[0].put(self.minServoPulse)
         self.registerServo()
 
     # Doesn't actually register/unregister, just stops and starts the servo PIO
     # The servo is registered by default in the __init__() function - these are only required if you want to use Pin 2 for something else, and then register the servo again
     def registerServo(self):
         if(not self.servo[0].active()):
             self.servo[0].active(1)
@@ -294,16 +311,29 @@
         jmp("bitloop")          .side(1)    [T2 - 1]
         label("do_zero")
         nop()                   .side(0)    [T2 - 1]
         wrap()
 
     def __init__(self, num_zip_leds):
         self.num_zip_leds = num_zip_leds
+        
         # Create  and start the StateMachine for the ZIPLeds
-        self.ZIPLEDs = StateMachine(4, self._ZIPLEDOutput, freq=8_000_000, sideset_base=Pin(20))
+        for i in range(8): # StateMachine range from 0 to 7
+            if usedSM[i]:
+                continue # Ignore this index if already used
+            try:
+                self.ZIPLEDs = StateMachine(i, self._ZIPLEDOutput, freq=8_000_000, sideset_base=Pin(20))
+                usedSM[i] = True # Set this index to used
+                break # Have claimed the SM, can leave now
+            except ValueError:
+                pass # External resouce has SM, move on
+            if i == 7:
+                # Cannot find an unused SM
+                raise ValueError("Could not claim a StateMachine, all in use")
+        
         self.theLEDs = array.array("I", [0 for _ in range(self.num_zip_leds)]) #an array for the LED colours.
         self.brightness = 0.5 #20% initially 
         self.ZIPLEDs.active(1)
             
         # Define some colour tuples for people to use.    
         self.BLACK = (0, 0, 0)
         self.RED = (255, 0, 0)
@@ -518,15 +548,15 @@
         mappedVal = toMin + ((value - frMin) * ((toMax - toMin) / (frMax - frMin)))
         return mappedVal
 
     def __init__(self, i2cAddr=0x77, sda=6, scl=7):
         self.CHIP_ADDRESS = i2cAddr    # I2C address as determined by hardware configuration
         sda = Pin(sda)
         scl = Pin(scl)
-        self.i2c = I2C(1,sda=sda, scl=scl, freq=100000)
+        self.i2c = I2C(1, sda=sda, scl=scl, freq=100_000, timeout=100_000)
 
         # Useful BME688 Register Addresses
         # Control
         self.CTRL_MEAS = 0x74       # Bit position <7:5>: Temperature oversampling   Bit position <4:2>: Pressure oversampling   Bit position <1:0>: Sensor power mode
         self.RESET = 0xE0           # Write 0xB6 to initiate soft-reset (same effect as power-on reset)
         self.CHIP_ID = 0xD0         # Read this to return the chip ID: 0x61 - good way to check communication is occurring
         self.CTRL_HUM = 0x72        # Bit position <2:0>: Humidity oversampling settings
@@ -1059,15 +1089,15 @@
         self.SET_DISP_CLK_DIV = const(0xD5)
         self.SET_PRECHARGE = const(0xD9)
         self.SET_VCOM_DESEL = const(0xDB)
         self.SET_CHARGE_PUMP = const(0x8D)
 
         sda = Pin(sda)
         scl = Pin(scl)
-        self.i2c = I2C(1,sda=sda, scl=scl, freq=100000)
+        self.i2c = I2C(1, sda=sda, scl=scl, freq=100_000, timeout=100_000)
 
         self.plotArray = []
         self.plotYMin = 0
         self.plotYMax = 100
         self.yPixelMin = 63
         self.yPixelMax = 12
 
@@ -1219,7 +1249,8 @@
     # Can be filled (True) or just an outline (False)
     # Need to call 'show()' to make the rectangle actually display
     def drawRect(self, start_x, start_y, width, height, fill=False):
         if (fill == False):
             super().rect(start_x, start_y, width, height, 1)
         elif (fill == True):
             super().fill_rect(start_x, start_y, width, height, 1)
+
```

### Comparing `KitronikPicoSmartAirQuality-1.0.0/README.md` & `KitronikPicoSmartAirQuality-1.0.1/README.md`

 * *Files identical despite different names*

