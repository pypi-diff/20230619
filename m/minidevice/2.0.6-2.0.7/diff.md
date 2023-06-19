# Comparing `tmp/minidevice-2.0.6.tar.gz` & `tmp/minidevice-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.6.tar", last modified: Sun Jun 18 05:31:15 2023, max compression
+gzip compressed data, was "minidevice-2.0.7.tar", last modified: Mon Jun 19 01:19:03 2023, max compression
```

## Comparing `minidevice-2.0.6.tar` & `minidevice-2.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.564545 minidevice-2.0.6/
--rw-rw-rw-   0        0        0     3077 2023-06-18 05:31:15.563538 minidevice-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2783 2023-06-18 05:30:28.000000 minidevice-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.530305 minidevice-2.0.6/minidevice/
--rw-rw-rw-   0        0        0     2758 2023-06-18 04:18:15.000000 minidevice-2.0.6/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.6/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      268 2023-06-18 05:20:44.000000 minidevice-2.0.6/minidevice/__init__.py
--rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.6/minidevice/adb.py
--rw-rw-rw-   0        0        0     1659 2023-06-18 05:27:30.000000 minidevice-2.0.6/minidevice/device.py
--rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.6/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.6/minidevice/logger.py
--rw-rw-rw-   0        0        0    12808 2023-06-18 04:22:01.000000 minidevice-2.0.6/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1720 2023-06-18 05:21:56.000000 minidevice-2.0.6/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      687 2023-06-18 04:29:14.000000 minidevice-2.0.6/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.6/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.559634 minidevice-2.0.6/minidevice.egg-info/
--rw-rw-rw-   0        0        0     3077 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 05:31:15.000000 minidevice-2.0.6/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 05:31:15.565550 minidevice-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-18 05:31:12.000000 minidevice-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.627362 minidevice-2.0.7/
+-rw-rw-rw-   0        0        0     3077 2023-06-19 01:19:03.627362 minidevice-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2023-06-18 05:30:28.000000 minidevice-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.608809 minidevice-2.0.7/minidevice/
+-rw-rw-rw-   0        0        0     2809 2023-06-19 01:16:20.000000 minidevice-2.0.7/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.7/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      268 2023-06-18 05:20:44.000000 minidevice-2.0.7/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    21023 2023-06-18 04:23:42.000000 minidevice-2.0.7/minidevice/adb.py
+-rw-rw-rw-   0        0        0     1659 2023-06-18 05:27:30.000000 minidevice-2.0.7/minidevice/device.py
+-rw-rw-rw-   0        0        0    20739 2023-06-18 02:48:13.000000 minidevice-2.0.7/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.7/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12881 2023-06-19 01:17:22.000000 minidevice-2.0.7/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1774 2023-06-19 01:14:32.000000 minidevice-2.0.7/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      687 2023-06-18 04:29:14.000000 minidevice-2.0.7/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.7/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-19 01:19:03.625410 minidevice-2.0.7/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     3077 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 01:19:03.000000 minidevice-2.0.7/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 01:19:03.628339 minidevice-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-19 01:18:33.000000 minidevice-2.0.7/setup.py
```

### Comparing `minidevice-2.0.6/PKG-INFO` & `minidevice-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.6
+Version: 2.0.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.6/README.md` & `minidevice-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice/DroidCast.py` & `minidevice-2.0.7/minidevice/DroidCast.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,7 +78,10 @@
 
     def screencap_raw(self) -> bytes:
         if self.droidcast_popen.poll() is not None:
             self.__stop()
             self.__start()
         return self.DroidCastSession.get(self.droidcast_url, timeout=3).content
 
+    def __del__(self):
+        self.__stop()
+
```

### Comparing `minidevice-2.0.6/minidevice/QueueUtils.py` & `minidevice-2.0.7/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice/adb.py` & `minidevice-2.0.7/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice/device.py` & `minidevice-2.0.7/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice/images.py` & `minidevice-2.0.7/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice/minicap.py` & `minidevice-2.0.7/minidevice/minicap.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,17 @@
 
     def __stop_minicap_by_stream(self):
         self.minicap_stream.stop()  # 停止stream
         self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
         if self.minicap_popen.poll() is None:  # 清理管道
             self.minicap_popen.kill()
 
-
+    def __del__(self):
+        self.__stop_minicap_by_stream()
+        
 if __name__ == "__main__":
     a = Minicap("127.0.0.1:16384")
     time.sleep(5)
     import cv2
 
     cv2.imshow("", a.screencap_opencv())
     cv2.waitKey()
```

### Comparing `minidevice-2.0.6/minidevice/minitouch.py` & `minidevice-2.0.7/minidevice/minitouch.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,11 +45,13 @@
             duration (int): 持续时间. Defaults to 300.
         """
         MNTDevice.swipe(self, points, duration=duration)
         logger.debug(
             f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
         )
 
+    def __del__(self):
+        MNTDevice.stop(self)
 
 if __name__ == "__main__":
     a = Minitouch("127.0.0.1:16384")
     a.stop()
```

### Comparing `minidevice-2.0.6/minidevice/screencap.py` & `minidevice-2.0.7/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.6/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.7/minidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.6
+Version: 2.0.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.6/setup.py` & `minidevice-2.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.6',
+      version='2.0.7',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

