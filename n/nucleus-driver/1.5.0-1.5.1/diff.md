# Comparing `tmp/nucleus_driver-1.5.0.tar.gz` & `tmp/nucleus_driver-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.0.tar", last modified: Fri Jun  9 06:15:00 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.1.tar", last modified: Mon Jun 19 08:18:55 2023, max compression
```

## Comparing `nucleus_driver-1.5.0.tar` & `nucleus_driver-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.306002 nucleus_driver-1.5.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.306002 nucleus_driver-1.5.0/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-01 06:58:05.000000 nucleus_driver-1.5.0/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16919 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16554 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.0/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19018 2023-04-14 09:56:26.000000 nucleus_driver-1.5.0/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.0/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-09 06:15:00.310002 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-09 06:15:00.000000 nucleus_driver-1.5.0/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.492737 nucleus_driver-1.5.1/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-06-19 08:02:36.000000 nucleus_driver-1.5.1/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16918 2023-06-09 12:27:05.000000 nucleus_driver-1.5.1/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-15 06:32:32.000000 nucleus_driver-1.5.1/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39751 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.1/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19319 2023-06-15 09:06:07.000000 nucleus_driver-1.5.1/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11259 2023-06-08 13:16:41.000000 nucleus_driver-1.5.1/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 08:18:55.496737 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-06-19 08:18:55.000000 nucleus_driver-1.5.1/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.0/LICENSE.txt` & `nucleus_driver-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/PKG-INFO` & `nucleus_driver-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.5.0
+Version: 1.5.1
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.0/README.md` & `nucleus_driver-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/setup.cfg` & `nucleus_driver-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.0
+version = 1.5.1
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,14 @@
 
             except UnicodeDecodeError:
                 self.messages.write_warning('Failed to decode GETALL message')
 
         else:
             self.messages.write_warning('Unable to obtain GETALL information')
 
-
     def disconnect(self) -> bool:
 
         if self.get_connection_status() is False:
             self.messages.write_message(message='Nucleus is already disconnected')
             return False
 
         def _disconnect_serial():
```

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_flash.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,16 +146,17 @@
                         firmware_name_version['BUILD'] = element
                         break
                     except ValueError:
                         firmware_name_version['EXTRA'] = '"{}"'.format(element)
 
         if self.dvl_firmware_name is not None:
             dvl_rematch = re.match(self.LDR_FILE_PATTERN, self.dvl_firmware_name)
-            firmware_name_version['DVLFW'] = dvl_rematch[2]
-            firmware_name_version['DVLMINOR'] = dvl_rematch[3]
+            if dvl_rematch is not None:
+                firmware_name_version['DVLFW'] = dvl_rematch[2]
+                firmware_name_version['DVLMINOR'] = dvl_rematch[3]
 
         if self.nucleus_firmware_name is not None and not nucleus_rematch:
             self.messages.write_warning(message='Nucleus firmware does not contain version number in its file name')
 
         elif self.nucleus_firmware_name is not None:
 
             for key in ['MAJOR', 'MINOR', 'PATCH', 'EXTRA', 'BUILD']:
```

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.1/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/app.py` & `nucleus_driver-1.5.1/src/nucleus_driver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,20 @@
             return
 
         response = self.nucleus_driver.clear_syslog()
 
         for message in response:
             self.nucleus_driver.messages.write_message(message)
 
+        if self.nucleus_driver.connection.get_connection_type() == 'tcp':
+            self.nucleus_driver.messages.write_warning('TCP connection has been lost due to device being restarted after clearing syslog. Reconnect to device!')
+            self.nucleus_driver.connection.disconnet()
+
+        
+
     ##########################################
     # Download
     ###########################################
 
     download_dvl_parser = Cmd2ArgumentParser(description='Download dvl diagnostics data')
     download_dvl_parser.add_argument('-f', '--fid', help='id of file to download')
     download_dvl_parser.add_argument('-s', '--sa', help='start byte address of file to download')
```

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.1/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.1/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.5.0
+Version: 1.5.1
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.0/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.1/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

