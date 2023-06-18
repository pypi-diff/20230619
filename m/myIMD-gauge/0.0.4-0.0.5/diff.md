# Comparing `tmp/myIMD_gauge-0.0.4-py3-none-any.whl.zip` & `tmp/myIMD_gauge-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2078 bytes, number of entries: 6
+Zip file size: 2171 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       37 b- defN 23-Feb-22 08:26 myIMD_gauge/__init__.py
--rw-rw-rw-  2.0 fat     1815 b- defN 23-Mar-24 04:57 myIMD_gauge/myIMD_gauge.py
--rw-rw-rw-  2.0 fat      228 b- defN 23-Mar-24 04:58 myIMD_gauge-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-24 04:58 myIMD_gauge-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Mar-24 04:58 myIMD_gauge-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      474 b- defN 23-Mar-24 04:58 myIMD_gauge-0.0.4.dist-info/RECORD
-6 files, 2658 bytes uncompressed, 1214 bytes compressed:  54.3%
+-rw-rw-rw-  2.0 fat     2331 b- defN 23-Jun-18 22:50 myIMD_gauge/myIMD_gauge.py
+-rw-rw-rw-  2.0 fat      228 b- defN 23-Jun-18 22:52 myIMD_gauge-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 22:52 myIMD_gauge-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-18 22:52 myIMD_gauge-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      474 b- defN 23-Jun-18 22:52 myIMD_gauge-0.0.5.dist-info/RECORD
+6 files, 3174 bytes uncompressed, 1307 bytes compressed:  58.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myIMD_gauge/__init__.py
 Comment: 
 
 Filename: myIMD_gauge/myIMD_gauge.py
 Comment: 
 
-Filename: myIMD_gauge-0.0.4.dist-info/METADATA
+Filename: myIMD_gauge-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: myIMD_gauge-0.0.4.dist-info/WHEEL
+Filename: myIMD_gauge-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: myIMD_gauge-0.0.4.dist-info/top_level.txt
+Filename: myIMD_gauge-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: myIMD_gauge-0.0.4.dist-info/RECORD
+Filename: myIMD_gauge-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myIMD_gauge/myIMD_gauge.py

```diff
@@ -1,34 +1,46 @@
-# 0.0.4
+# 0.0.5
 
 import serial
 import time
 
 class IMD_Gauge_communication:
     class Command:
         Get_start = b'XAG\r'
         Get_stop = b'XAS\r'
         Reset_Zero = b'Z\r'
         ShutDown = b'XQT\r'
 
+    class IMD_Gauge_error(Exception):
+        pass
+
     def __init__(self):
         self._ser: serial.serialwin32.Serial = None
         self._alldata = ''
         self._time = time.perf_counter()
 
     def __del__(self):
         self.exit()
 
     def init(self, COM):
         try:
             self._ser = serial.Serial(COM, baudrate=460800, bytesize=serial.EIGHTBITS, parity=serial.PARITY_NONE,
                                 stopbits=serial.STOPBITS_ONE, timeout=0.0001)
             time.sleep(0.001)
             self._ser.write(self.Command.Get_start)
-            time.sleep(0.001)
+            time.sleep(0.01)
+            self._alldata = self._alldata + self._ser.read_all().decode()
+            count = 0
+            while self._alldata == '':
+                self._alldata = self._alldata + self._ser.read_all().decode()
+                self._ser.write(self.Command.Get_start)
+                time.sleep(0.001)
+                count += 1
+                if count > 1000:
+                    raise self.IMD_Gauge_error('Initialize Error. Please restart Device')
             return 1
         except serial.serialutil.SerialException:
             return -1
 
     def read(self):
         self._alldata = self._alldata + self._ser.read_all().decode()
         while self._alldata == '':
```

