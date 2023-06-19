# Comparing `tmp/amqp-mqtt-transport-0.1.2.tar.gz` & `tmp/amqp-mqtt-transport-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mqtt-transport-0.1.2.tar", last modified: Mon Jun 19 13:45:15 2023, max compression
+gzip compressed data, was "amqp-mqtt-transport-0.1.3.tar", last modified: Mon Jun 19 13:51:56 2023, max compression
```

## Comparing `amqp-mqtt-transport-0.1.2.tar` & `amqp-mqtt-transport-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:45:15.763514 amqp-mqtt-transport-0.1.2/
--rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp-mqtt-transport-0.1.2/.gitattributes
--rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp-mqtt-transport-0.1.2/.gitignore
--rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp-mqtt-transport-0.1.2/LICENSE
--rw-rw-r--   0 igor      (1001) igor      (1001)     1012 2023-06-19 13:15:40.000000 amqp-mqtt-transport-0.1.2/Makefile
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:45:15.763514 amqp-mqtt-transport-0.1.2/PKG-INFO
--rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp-mqtt-transport-0.1.2/README.md
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:45:15.719513 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:45:15.000000 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      588 2023-06-19 13:45:15.000000 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-19 13:45:15.000000 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       92 2023-06-19 13:45:15.000000 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/requires.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       10 2023-06-19 13:45:15.000000 amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)      799 2023-06-19 13:44:24.000000 amqp-mqtt-transport-0.1.2/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-19 13:45:15.763514 amqp-mqtt-transport-0.1.2/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp-mqtt-transport-0.1.2/setup.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:45:15.735513 amqp-mqtt-transport-0.1.2/transport/
--rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp-mqtt-transport-0.1.2/transport/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.2/transport/abc.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:45:15.751514 amqp-mqtt-transport-0.1.2/transport/amqp/
--rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.2/transport/amqp/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.2/transport/amqp/consumer.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp-mqtt-transport-0.1.2/transport/amqp/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.2/transport/amqp/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.2/transport/message_scheduler.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:45:15.759514 amqp-mqtt-transport-0.1.2/transport/mqtt/
--rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.2/transport/mqtt/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp-mqtt-transport-0.1.2/transport/mqtt/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp-mqtt-transport-0.1.2/transport/mqtt/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.2/transport/scheduled_publisher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:51:56.679990 amqp-mqtt-transport-0.1.3/
+-rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp-mqtt-transport-0.1.3/.gitattributes
+-rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp-mqtt-transport-0.1.3/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp-mqtt-transport-0.1.3/LICENSE
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp-mqtt-transport-0.1.3/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:51:56.679990 amqp-mqtt-transport-0.1.3/PKG-INFO
+-rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp-mqtt-transport-0.1.3/README.md
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:51:56.671990 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-19 13:51:56.000000 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      588 2023-06-19 13:51:56.000000 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-19 13:51:56.000000 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       65 2023-06-19 13:51:56.000000 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       10 2023-06-19 13:51:56.000000 amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/top_level.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)      758 2023-06-19 13:49:57.000000 amqp-mqtt-transport-0.1.3/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-19 13:51:56.679990 amqp-mqtt-transport-0.1.3/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp-mqtt-transport-0.1.3/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:51:56.675990 amqp-mqtt-transport-0.1.3/transport/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp-mqtt-transport-0.1.3/transport/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.3/transport/abc.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:51:56.675990 amqp-mqtt-transport-0.1.3/transport/amqp/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.3/transport/amqp/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.3/transport/amqp/consumer.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp-mqtt-transport-0.1.3/transport/amqp/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.3/transport/amqp/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp-mqtt-transport-0.1.3/transport/message_scheduler.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-19 13:51:56.675990 amqp-mqtt-transport-0.1.3/transport/mqtt/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp-mqtt-transport-0.1.3/transport/mqtt/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp-mqtt-transport-0.1.3/transport/mqtt/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp-mqtt-transport-0.1.3/transport/mqtt/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp-mqtt-transport-0.1.3/transport/scheduled_publisher.py
```

### Comparing `amqp-mqtt-transport-0.1.2/LICENSE` & `amqp-mqtt-transport-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/Makefile` & `amqp-mqtt-transport-0.1.3/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 run: venv
 	@echo "This is import only package, can't run"
 
 install: venv
 	. venv/bin/activate && python3.10 -m pip install -e .
 
 build: install
-	. venv/bin/activate && python3.10 -m build
+	. venv/bin/activate && pip install build && python3.10 -m build
 
 upload_to_pypi: build
-	. venv/bin/activate && python3.10 -m twine upload --repository pypi dist/*
+	. venv/bin/activate && pip install twine && python3.10 -m twine upload --repository pypi dist/*
 
 autopep8: install
 	. venv/bin/activate && autopep8 --in-place --exclude "./venv/**" --recursive .
 
 clean:
 	rm -rf venv dist *.egg-info
 	find -iname "*.pyc" -delete
```

### Comparing `amqp-mqtt-transport-0.1.2/PKG-INFO` & `amqp-mqtt-transport-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.2/README.md` & `amqp-mqtt-transport-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/PKG-INFO` & `amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.2
+Version: 0.1.3
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.2/amqp_mqtt_transport.egg-info/SOURCES.txt` & `amqp-mqtt-transport-0.1.3/amqp_mqtt_transport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/pyproject.toml` & `amqp-mqtt-transport-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqp-mqtt-transport"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
@@ -17,17 +17,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "tenacity<=8.2.2",
     "aio-pika<=9.0.5",
     "autopep8==2.0.2",
-    "paho-mqtt==1.5.1",
-    "build==0.10.0",
-    "twine==4.0.2"
+    "paho-mqtt==1.5.1"
 ]
 
 [tool.autopep8]
 max_line_length = 120
 ignore = []
 recursive = true
 aggressive = 5
```

### Comparing `amqp-mqtt-transport-0.1.2/transport/abc.py` & `amqp-mqtt-transport-0.1.3/transport/abc.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/amqp/consumer.py` & `amqp-mqtt-transport-0.1.3/transport/amqp/consumer.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/amqp/controller.py` & `amqp-mqtt-transport-0.1.3/transport/amqp/controller.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/amqp/publisher.py` & `amqp-mqtt-transport-0.1.3/transport/amqp/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/message_scheduler.py` & `amqp-mqtt-transport-0.1.3/transport/message_scheduler.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/mqtt/controller.py` & `amqp-mqtt-transport-0.1.3/transport/mqtt/controller.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/mqtt/publisher.py` & `amqp-mqtt-transport-0.1.3/transport/mqtt/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.2/transport/scheduled_publisher.py` & `amqp-mqtt-transport-0.1.3/transport/scheduled_publisher.py`

 * *Files identical despite different names*

