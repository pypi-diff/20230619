# Comparing `tmp/nucleus_driver-1.5.1.tar.gz` & `tmp/nucleus_driver-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.1.tar", last modified: Mon Jun 19 08:18:55 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.2.tar", last modified: Mon Jun 19 11:29:18 2023, max compression
```

## Comparing `nucleus_driver-1.5.1.tar` & `nucleus_driver-1.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.492737 nucleus_driver-1.5.1/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-19 08:02:36.000000 nucleus_driver-1.5.1/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16918 2023-06-09 12:27:05.000000 nucleus_driver-1.5.1/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-15 06:32:32.000000 nucleus_driver-1.5.1/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-15 09:06:07.000000 nucleus_driver-1.5.1/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-19 08:02:36.000000 nucleus_driver-1.5.2/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17554 2023-06-19 11:22:50.000000 nucleus_driver-1.5.2/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-19 11:22:47.000000 nucleus_driver-1.5.2/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-15 06:32:32.000000 nucleus_driver-1.5.2/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.2/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-15 09:06:07.000000 nucleus_driver-1.5.2/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.2/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 11:29:18.297179 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-19 11:29:18.000000 nucleus_driver-1.5.2/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.1/LICENSE.txt` & `nucleus_driver-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/PKG-INFO` & `nucleus_driver-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.5.1
+Version: 1.5.2
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.1/README.md` & `nucleus_driver-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/setup.cfg` & `nucleus_driver-1.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.1
+version = 1.5.2
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -351,15 +351,15 @@
                 self.messages.write_exception(message='Failed to disconnet from serial connection: {}'.format(exception))
 
                 return False
 
         def _disconnect_tcp():
 
             try:
-                #self.tcp.shutdown(socket.SHUT_RDWR)
+                self.tcp.shutdown(socket.SHUT_RDWR)
                 self.tcp.close()
 
                 time.sleep(0.01)
 
                 self._connection_type = None
                 self.tcp = socket.socket()
 
@@ -430,74 +430,81 @@
 
         read_data = b''
 
         def _serial_read() -> bytes:
             serial_data = b''
 
             try:
-
-                init_time = datetime.now()
-
-                while (datetime.now() - init_time).total_seconds() <= timeout:
-                    serial_data += self.serial.read(1)
-
-                    if terminator is not None:
+                if terminator is not None:
+                    init_time = datetime.now()
+                    while (datetime.now() - init_time).seconds < timeout:
+                        serial_data += self.serial.read_until(terminator, size)
                         if terminator in serial_data or b'ERROR\r\n' in serial_data:
                             break
 
-                    if size is not None:
+                elif size is not None:
+                    init_time = datetime.now()
+                    while (datetime.now() - init_time).seconds < timeout:
+                        serial_data += self.serial.read(size=max(0, size - len(serial_data)))
                         if len(serial_data) >= size:
                             break
 
+                else:
+                    if self.serial.in_waiting:
+                        serial_data += self.serial.read(self.serial.in_waiting)
+
             except Exception as exception:
                 self.messages.write_exception(message='Failed to read serial data from Nucleus: {}'.format(exception))
 
             return serial_data
 
         def _tcp_read() -> bytes:
 
             def _read() -> bool:
                 try:
                     self.tcp_buffer += self.tcp.recv(4096)
                     return True
                 except socket.timeout:
                     return True
                 except Exception as exception:
-                    self.messages.write_exception(message='Failed to read tcp data from Nucleus: {}'.format(exception))
-                    return False
-
-            def _get_byte_from_tcp_buffer() -> bytes:
+                    if self.get_connection_status():
+                        self.messages.write_exception(message='Failed to read tcp data from Nucleus: {}'.format(exception))
 
-                if len(self.tcp_buffer) == 0:
-                    return b''
-
-                byte = self.tcp_buffer[0:1]
-                self.tcp_buffer = self.tcp_buffer[1:]
+                    return False
 
-                return byte
+            if terminator is not None:
 
-            tcp_data = b''
+                init_time = datetime.now()
+                while (datetime.now() - init_time).seconds < timeout:
+                    if terminator in self.tcp_buffer:
+                        break
+                    else:
+                        if not _read():
+                            break
 
-            init_time = datetime.now()
+                line, separator, self.tcp_buffer = self.tcp_buffer.partition(terminator)
+                tcp_data = line + separator
 
-            while (datetime.now() - init_time).total_seconds() <= timeout:
+            elif size is not None:
 
-                if len(self.tcp_buffer) == 0:
-                    if not _read():
+                init_time = datetime.now()
+                while (datetime.now() - init_time).seconds < timeout:
+                    if len(self.tcp_buffer) >= size:
                         break
+                    else:
+                        if not _read():
+                            break
 
-                tcp_data += _get_byte_from_tcp_buffer()
-
-                if terminator is not None:
-                    if terminator in tcp_data or b'ERROR\r\n' in tcp_data:
-                        break
+                tcp_data = self.tcp_buffer[:size]
+                self.tcp_buffer = self.tcp_buffer[size:]
 
-                if size is not None:
-                    if len(tcp_data) >= size:
-                        break
+            else:
+                _read()
+                tcp_data = self.tcp_buffer
+                self.tcp_buffer = b''
 
             return tcp_data
 
         if self.get_connection_type() == 'serial':
             read_data = _serial_read()
 
         if self.get_connection_type() == 'tcp':
```

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.2/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/app.py` & `nucleus_driver-1.5.2/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.2/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.2/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.5.1
+Version: 1.5.2
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.1/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.2/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

