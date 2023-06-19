# Comparing `tmp/roboid-1.6.3.tar.gz` & `tmp/roboid-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\roboid-1.6.3.tar", last modified: Mon May  8 03:06:55 2023, max compression
+gzip compressed data, was "dist\roboid-1.6.4.tar", last modified: Mon Jun 19 15:28:43 2023, max compression
```

## Comparing `roboid-1.6.3.tar` & `roboid-1.6.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.547230 roboid-1.6.3/
--rw-rw-rw-   0        0        0      802 2020-08-22 18:46:06.000000 roboid-1.6.3/LICENSE
--rw-rw-rw-   0        0        0      118 2020-08-27 07:49:02.000000 roboid-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0      583 2023-05-08 03:06:55.547230 roboid-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      196 2021-07-16 15:38:12.000000 roboid-1.6.3/README.md
--rw-rw-rw-   0        0        0       13 2022-08-16 21:06:30.000000 roboid-1.6.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.517352 roboid-1.6.3/roboid/
--rw-rw-rw-   0        0        0     2489 2022-09-10 13:00:51.000000 roboid-1.6.3/roboid/__init__.py
--rw-rw-rw-   0        0        0    43482 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/albert_ai.py
--rw-rw-rw-   0        0        0    39296 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/albert_ai_roboid.py
--rw-rw-rw-   0        0        0    33110 2023-05-08 02:43:56.000000 roboid-1.6.3/roboid/beagle.py
--rw-rw-rw-   0        0        0    52299 2023-05-08 02:55:25.000000 roboid-1.6.3/roboid/beagle_roboid.py
--rw-rw-rw-   0        0        0     1054 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/connector.py
--rw-rw-rw-   0        0        0    25181 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/grid.py
--rw-rw-rw-   0        0        0    25768 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster.py
--rw-rw-rw-   0        0        0    26191 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster_roboid.py
--rw-rw-rw-   0        0        0    65291 2022-09-10 12:35:40.000000 roboid-1.6.3/roboid/hamster_s.py
--rw-rw-rw-   0        0        0    34484 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster_s_roboid.py
--rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/keyboard.py
--rw-rw-rw-   0        0        0    17970 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/model.py
--rw-rw-rw-   0        0        0     9409 2022-09-06 12:48:38.000000 roboid-1.6.3/roboid/runner.py
--rw-rw-rw-   0        0        0     1270 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/scanner.py
--rw-rw-rw-   0        0        0    13718 2022-09-06 13:10:19.000000 roboid-1.6.3/roboid/serial_connector.py
--rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/serial_queue.py
--rw-rw-rw-   0        0        0    36958 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/turtle.py
--rw-rw-rw-   0        0        0    28613 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/turtle_roboid.py
--rw-rw-rw-   0        0        0     1132 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/util.py
--rw-rw-rw-   0        0        0    36730 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/zerone.py
--rw-rw-rw-   0        0        0    24208 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/zerone_roboid.py
-drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.545245 roboid-1.6.3/roboid.egg-info/
--rw-rw-rw-   0        0        0      583 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-08 03:06:55.549224 roboid-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      582 2023-05-08 03:04:03.000000 roboid-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:28:43.882023 roboid-1.6.4/
+-rw-rw-rw-   0        0        0      802 2020-08-22 18:46:06.000000 roboid-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0      118 2020-08-27 07:49:02.000000 roboid-1.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      583 2023-06-19 15:28:43.883022 roboid-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2021-07-16 15:38:12.000000 roboid-1.6.4/README.md
+-rw-rw-rw-   0        0        0       13 2022-08-16 21:06:30.000000 roboid-1.6.4/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 15:28:43.849064 roboid-1.6.4/roboid/
+-rw-rw-rw-   0        0        0     2489 2023-06-19 15:18:12.000000 roboid-1.6.4/roboid/__init__.py
+-rw-rw-rw-   0        0        0    43482 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/albert_ai.py
+-rw-rw-rw-   0        0        0    39296 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/albert_ai_roboid.py
+-rw-rw-rw-   0        0        0    33110 2023-05-08 02:43:56.000000 roboid-1.6.4/roboid/beagle.py
+-rw-rw-rw-   0        0        0    52299 2023-05-08 02:55:25.000000 roboid-1.6.4/roboid/beagle_roboid.py
+-rw-rw-rw-   0        0        0     1054 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/connector.py
+-rw-rw-rw-   0        0        0    25181 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/grid.py
+-rw-rw-rw-   0        0        0    25768 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/hamster.py
+-rw-rw-rw-   0        0        0    26191 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/hamster_roboid.py
+-rw-rw-rw-   0        0        0    65291 2022-09-10 12:35:40.000000 roboid-1.6.4/roboid/hamster_s.py
+-rw-rw-rw-   0        0        0    34484 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/hamster_s_roboid.py
+-rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/keyboard.py
+-rw-rw-rw-   0        0        0    18230 2023-06-19 15:24:25.000000 roboid-1.6.4/roboid/model.py
+-rw-rw-rw-   0        0        0     9409 2022-09-06 12:48:38.000000 roboid-1.6.4/roboid/runner.py
+-rw-rw-rw-   0        0        0     1270 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/scanner.py
+-rw-rw-rw-   0        0        0    13718 2022-09-06 13:10:19.000000 roboid-1.6.4/roboid/serial_connector.py
+-rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/serial_queue.py
+-rw-rw-rw-   0        0        0    36958 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/turtle.py
+-rw-rw-rw-   0        0        0    28613 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/turtle_roboid.py
+-rw-rw-rw-   0        0        0     1132 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/util.py
+-rw-rw-rw-   0        0        0    36730 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/zerone.py
+-rw-rw-rw-   0        0        0    24208 2022-09-06 12:45:31.000000 roboid-1.6.4/roboid/zerone_roboid.py
+drwxrwxrwx   0        0        0        0 2023-06-19 15:28:43.881032 roboid-1.6.4/roboid.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 15:28:43.000000 roboid-1.6.4/roboid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-19 15:28:43.884036 roboid-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-06-19 15:17:26.000000 roboid-1.6.4/setup.py
```

### Comparing `roboid-1.6.3/LICENSE` & `roboid-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/PKG-INFO` & `roboid-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboid
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `roboid-1.6.3/roboid/__init__.py` & `roboid-1.6.4/roboid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from roboid.beagle import Beagle
 from roboid.grid import GridHamster
 from roboid.grid import GridHamsterS
 from roboid.grid import GridTurtle
 from roboid.grid import GridAlbertAi
 from roboid.grid import GridZerone
 
-__version__ = "1.6.2"
+__version__ = "1.6.4"
 
 __all__ = ["DeviceType", "DataType", "Hamster", "GridHamster", "HamsterS", "GridHamsterS", "Turtle", "GridTurtle", "AlbertAi", "GridAlbertAi", "Zerone", "GridZerone", "Beagle", "Keyboard", "scan", "dispose", "set_executable", "wait", "wait_until_ready", "wait_until", "when_do", "while_do", "parallel"]
 
 def scan():
     Scanner.scan()
 
 def dispose():
```

### Comparing `roboid-1.6.3/roboid/albert_ai.py` & `roboid-1.6.4/roboid/albert_ai.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/albert_ai_roboid.py` & `roboid-1.6.4/roboid/albert_ai_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/beagle.py` & `roboid-1.6.4/roboid/beagle.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/beagle_roboid.py` & `roboid-1.6.4/roboid/beagle_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/connector.py` & `roboid-1.6.4/roboid/connector.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/grid.py` & `roboid-1.6.4/roboid/grid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/hamster.py` & `roboid-1.6.4/roboid/hamster.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/hamster_roboid.py` & `roboid-1.6.4/roboid/hamster_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/hamster_s.py` & `roboid-1.6.4/roboid/hamster_s.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/hamster_s_roboid.py` & `roboid-1.6.4/roboid/hamster_s_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/keyboard.py` & `roboid-1.6.4/roboid/keyboard.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/model.py` & `roboid-1.6.4/roboid/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,19 @@
 
     def _clear_written(self):
         for device in self._devices:
             device._clear_written()
         for roboid in self._roboids:
             roboid._clear_written()
 
+    def is_connected(self):
+        if self._connector:
+            return self._connector.is_connected()
+        return False
+
 
 class Robot(NamedElement):
     def __init__(self, id, name, index):
         super(Robot, self).__init__(name)
         self._id = id
         self._index = index
         self._roboids = []
@@ -516,7 +521,12 @@
     def _notify_sensory_device_data_changed(self):
         for roboid in self._roboids:
             roboid._notify_sensory_device_data_changed()
 
     def _notify_motoring_device_data_changed(self):
         for roboid in self._roboids:
             roboid._notify_motoring_device_data_changed()
+
+    def is_connected(self):
+        if self._roboid:
+            return self._roboid.is_connected()
+        return False
```

### Comparing `roboid-1.6.3/roboid/runner.py` & `roboid-1.6.4/roboid/runner.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/scanner.py` & `roboid-1.6.4/roboid/scanner.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/serial_connector.py` & `roboid-1.6.4/roboid/serial_connector.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/serial_queue.py` & `roboid-1.6.4/roboid/serial_queue.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/turtle.py` & `roboid-1.6.4/roboid/turtle.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/turtle_roboid.py` & `roboid-1.6.4/roboid/turtle_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/util.py` & `roboid-1.6.4/roboid/util.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/zerone.py` & `roboid-1.6.4/roboid/zerone.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid/zerone_roboid.py` & `roboid-1.6.4/roboid/zerone_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/roboid.egg-info/PKG-INFO` & `roboid-1.6.4/roboid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboid
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `roboid-1.6.3/roboid.egg-info/SOURCES.txt` & `roboid-1.6.4/roboid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboid-1.6.3/setup.py` & `roboid-1.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="roboid",
-	version="1.6.3",
+	version="1.6.4",
 	author="Kwang-Hyun Park",
 	author_email="akaii@kw.ac.kr",
 	description="Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
 	install_requires=["pyserial"],
 	packages=find_packages(exclude=["examples", "tests"]),
```

